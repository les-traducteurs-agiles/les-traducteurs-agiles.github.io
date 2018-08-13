---
layout: post
title:  "Ne devez-vous pas vous CONNECTER d'abord ?"
date:   2011-12-06 00:01
published: true
tags:
- user story
---

Dans mon précédent article, []Éviter l'itération zéro](http://www.les-traducteurs-agiles.org/2011/12/06/evitez-l-iteration-zero.html), je proposais de commencer avec “la **première chose évidente** ayant besoin d'être réalisée. (_Indice: ce n'est pas ‘se connecter’)_” Comme [Jon Kern l'a mentionné récemment](http://technicaldebt.com/?p=957), ce sujet est apparu ailleurs, j'étais également présent dans cette liste de discussion.

Jon a, bien entendu, raison dans un certain sens. Vous pouvez commencer par la connexion si vous voulez. Vous pouvez aussi commencer par une Itération Zéro. (Ou, une Itération Moins Une, comme j'ai pu le voir dans une organisation lorsque leur liste de pré-planification a dépassé une itération.) J'ai observé que vous pouvez généralement obtenir **plus rapidement de meilleurs logiciels** si vous commencez par un autre élément.

Il y a plusieurs très bonnes raisons pour cela. D'une part, il est improbable que vous génériez beaucoup de valeur métier en livrant un système permettant aux personnes de se connecter et rien d'autre. A moins que vous écriviez une librairie de connexion intégrable par d’autres dans leur code, ce quelque chose d'autre est l'idée centrale du système. Il y a sûrement certaines choses à propos de cette idée centrale que nous ne connaissons pas encore en détail. A l’inverse, “la connexion” est largement connue et comprise (même si quelques fois, elle est mal implémentée). Même si nous décidons que nous ne pouvons livrer le système sans "connexion", nous pouvons apprendre des choses importantes plus tôt si nous travaillons d'abord sur l'idée centrale. (Et je peux imaginer, si nécessaire, avoir un système utilisable où l'accès sera contrôlé en plaçant l'ordinateur dans une pièce sécurisée et où seules les personnes habilitées pourront y toucher).

Apprendre des informations importantes au plus tôt est l'un des avantages les plus subtils et puissants lorsqu’on travaille en mode agile. Cela peut aider le métier à prendre de meilleures décisions pour arbitrer, ou même sur l'orientation à donner. C'est l'un des principes fondateurs pour démarrer en Lean, mais cela fonctionne pour des organisations qui y sont également déjà accoutumées. Il y a presque toujours quelque chose de nouveau dans ce que nous faisons, sinon nous ne dépenserions pas d'argent pour le faire.

Ce modèle d'apprentissage accéléré est performant pour les métiers qui l’utilisent. Cela l'est également pour les développeurs travaillant sur du code. Au fur et à mesure que nous construisons notre application, nous pouvons apprendre de meilleures manières de structurer le code, et nous pouvons utiliser cette information lorsque nous écrivons du code supplémentaire. Je constate que cela me permet de faire un meilleur boulot lorsque je développe du code d'une manière itérative et incrémentale que lorsque je crée une conception en amont et que je l'implémente.

Examinons comment Jon nous propose de commencer :

> Par exemple, pour commencer, vous pouvez simplement vérifier que la réponse est "connexion réussie" (ou "échec de connexion" pour tester qu'une tentative de connexion erronée a bien échoué)... simplement :

~~~
Scénario : Connexion réussie
Lorsque je me connecte en tant qu'admin
Alors je devrais être connecté
~~~

~~~
Scénario : Échec de connexion
Lorsque je me connecte en tant que asdf56ghasdkfh
Alors je ne devrais pas être connecté
~~~

> Et vos étapes devraient cacher la logique pour remplir le formulaire de connexion et en vérifier sa réussite :

~~~
Given /^Je me connecte comme "([^"]*)"$/ do |login|
@login_name = login
visit login_path
fill_in "login", :with => login
fill_in "password", :with => "password"
click_button "login_button"
end

Then /^Je devrais être connecté$/ do
response.should contain "Connexion réussie"
end

Then /^Je ne devrais pas être connecté$/ do
response.should contain "Échec de connexion. Veuillez essayer à nouveau."
end
~~~

En commençant aussi simplement, où allons nous mettre notre logique de contrôle d'accès ? De préférence dans notre contrôleur MVC ou notre présentateur MVP. Puis nous déciderons vers quelle page nous dirigerons l'utilisateur. En effet, nous protégeons la page "Connexion réussie" de la personne non-authentifiée. Est-ce que cette page est l'élément pour lequel nous voulons contrôler l'accès ?

Une fois, j'ai travaillé pour un client ayant une application permettant aux utilisateurs habilités d’accéder à des documents pour lesquels ils étaient autorisés. Ce n'était pas une boîte agile, et ils ne travaillaient pas en itérations courtes et en utilisant de petites stories. Néanmoins, pendant un certain nombres d'années, ils avaient livré de nouvelles fonctionnalités à chaque lot. Et ils étaient des programmeurs consciencieux, vérifiant minutieusement qu'ils ne livraient pas de bogues. Ayant commencé à implémenter leur idée de contrôle d'accès, ils ont fini par mettre leur vérification d'autorisation dans la classe Action de leur application Struts. Avec le temps, il y a eu besoin d’avoir des autorisations supplémentaires concernant certains documents. Seuls des utilisateurs autorisés pouvaient voir n'importe quel document, mais certains documents devaient être disponibles uniquement à un sous-ensemble d'utilisateurs. La classe Action vérifiait que l'utilisateur identifié, récupérait la liste des documents, et filtrait ceux pour lesquels cet utilisateur n'avait pas de droit de consultation.

Voyez-vous un problème avec cette façon de faire ?

Cela fonctionne assez bien, mais cela cause certains maux de tête en cas de maintenance. Même s’il n'y avait pas de liens vers les documents non autorisés, il n'y avait rien empêchant un utilisateur astucieux de deviner l'url et de les récupérer de cette façon : il aurait dû y avoir une vérification d'autorisation à ce niveau là aussi. Et il y avait de multiples listes de documents, chacune devant faire cette vérification. Quelques fois lorsque la logique d'autorisations changeait, l'une des classes Actions devait être ignorée. Extraire le code qui filtre les autorisations et le mettre dans une méthode devrait grandement réduire cette duplication et rendre cette erreur particulière moins épineuse, mais certaines listes avaient des règles de filtrage différentes. Ainsi, les classes Actions conserveraient la duplication dans l'ordre des étapes que chacune doit appliquer pour protéger correctement les éléments. (C’est un mode de duplication plus subtil et que beaucoup ignore.) Et il y avait un pré-requis pour montrer certains documents de la liste aux personnes non encore autorisées à les récupérer.

C'était très complexe et sujet à erreurs. Imposer la sécurité sur la couche externe, au lieu de le faire directement autour des éléments protégés, entraîna beaucoup de modifications et de variantes dans l'implémentation. Je suis sûr que Jon Kern, vous et moi n'aurions pas fini avec une telle conception sujette aux erreurs. Jon est un excellent concepteur de logiciel, beaucoup plus que moi. Il peut expliquer pourquoi vous voudriez concevoir d'une certaine manière et en décrire les raisons. Moi, d'un autre côté, je me suis entraîné à être sensible à la duplication. Du code piloté par les tests avec une aversion à la duplication m'aurait conduit vers une conception différente.

J'ai aidé ces programmeurs à implémenter une nouvelle fonctionnalité, en l’occurrence offrir des accès de niveau gouvernemental à certains documents même si l’utilisateur concerné n'était pas connecté du tout. Étant donné que ceci requérait une modification de tous les contrôles d'accès, cela nous motiva pour modifier la conception. Pendant que j’ajoutais cette nouvelle exigence en utilisant une Conception Pilotée par les Tests, j'en ai profité pour remanier le code et supprimer la duplication. En le faisant, j'ai repoussé les vérifications d'accès plus profond dans le code, en passant par un objet “AuthenticationToken” pouvant être traité comme une boîte noire par les couches d'accès. Finalement, le contrôle fut réalisé dans les requêtes de la base de données, s'assurant par simple inspection qu'aucun chemin dans l'interface utilisateur ne pourrait conduire à une condition qui aurait permis un accès non autorisé.

Vous êtes probablement un bon développeur également. Je suis certain que vous n'auriez pas fait l'erreur. [Linda Rising m'a dit récemment](http://www.youtube.com/watch?v=QvhOXU72OL4) que 80% des gens pensaient qu'ils étaient au-dessus de la moyenne, vous devez être très bon. Comme cela peut se passer, les développeurs qui avaient bâti ce système étaient très bon, mais ils n'étaient pas expérimentés avec la technologie. Ce système J2EE était le premier code Java qu'ils aient écrits. Généralement, ces développeurs réussissaient à être très consciencieux pour vérifier tous les chemins. Ce fut très rare lorsqu’ils en loupèrent un et que le bogue échappa aux tests d'intégration liés aux utilisateurs.

Je soutiens qu’en implémentant la fonctionnalité principale d'abord, dans cet exemple la détermination et la récupération des documents, nous serions davantage en mesure d’ajouter de façon naturelle les contrôles d'accès autour des éléments importants. En d'autres situations, il y aurait pu y avoir d'autres considérations pour le contrôle d'accès qui auraient été différentes pour l'application que je décris. Dans n'importe quel cas, si notre story principale est :

~~~
Quand je fais quoi que ce soit que mon application sait faire
Alors j'obtiens le résultat en le faisant
~~~

Avec toutes ces variations de "faire", l'endroit approprié pour le contrôle d'accès sera évidemment, pour plus de 80% d'entre nous, la story test :

~~~
Étant donné que je ne suis pas un utilisateur autorisé
Quand je fais quoi que ce soit que mon application sait faire
Alors je me vois refuser le résultat en le faisant
~~~

Même s’il est certainement vrai que nous pouvons obtenir la conception désirée dans tous les cas, comme le blog de Jon et mon récit l'illustrent, il est plus facile, plus directe et plus communément admis que nous l’obtiendrons ainsi si nous commençons par notre fonctionnalité métier principale, donc avant la story de connexion.

Ce n'est pas une loi de l'univers, mais c'est une bonne heuristique : **ne commencez _pas_ par la story de connexion**.


---
Auteur : [George Dinwiddie](http://blog.gdinwiddie.com/about/)  
Source : [Don’t You Have to LOGIN first?](http://blog.gdinwiddie.com/2011/06/11/dont-you-have-to-login-first/)  
Date de parution originale : 11 Juin 2011  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Relecteurs : [Sylvain Fraïssé](http://www.les-traducteurs-agiles.org/traducteurs/), [Fabrice Aimetti](http://www.fabrice-aimetti.fr/)  
Date de traduction : 06/12/2011  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

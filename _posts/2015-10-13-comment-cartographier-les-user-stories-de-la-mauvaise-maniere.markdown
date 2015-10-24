---
layout: post
title:  "Comment cartographier les user stories de la mauvaise manière"
date:   2015-10-13 21:00:55
published: true
categories: 
- user-stories
- pratique
---

**Résumé :**

_Lorsque l'équipe de Lisa Crispin a eu l'opportunité de mettre en pratique l'idée de cartographie des user stories qu'elle avait apprise de Jeff Patton, l'équipe s'est ruée dessus avec enthousiasme et elle a loupé quelques étapes. Vous allez découvrir ce qui s'est passé, ce qui ne s'est pas passé, et les enseignements que l'équipe en a tiré._

Lors de ces dernières années, j'ai participé à quelques ateliers et conférences de Jeff Patton où j'ai pu découvrir la [cartographie des user stories](http://www.agileproductdesign.com/blog/the new backlog.html). Il s'agit d'une manière pratique pour modéliser un thème ou un projet et le découper en user stories. La première fois où Jeff a écrit à ce sujet fut dans un article de _Better Software_ intitulé ["Tout est dans la manière dont vous le découpez"](https://dl.dropboxusercontent.com/u/50968566/Cartographie_user_stories/Tout_est_dans_la_mani%C3%A8re_dont_vous_d%C3%A9coupez.pdf).

De ce que j'ai appris de Jeff, il faut commencer par rassembler votre équipe de développement et les parties prenantes. Ensuite créer des personas pour représenter vos différents genres et rôles d'utilisateurs, puis penser à comment chaque persona devrait utiliser votre système ou votre fonctionnalité. Qu'est-ce qu'ils feraient d'abord ? Qu'est-ce qu'ils feraient ensuite ? Faire après une frise temporelle des activités utilisateurs sur un mur, une table ou sur le sol. Puis, prendre du recul et examiner chaque tâche utilisateur en détail et créer les tâches utilisateur et les détails concernant ces tâches, qui deviendront éventuellement des user stories. Ecrire celles-ci sur des cartes aussi, et les empiler verticalement en-dessous l'activité utilisateur correspondante.

Une fois que la cartographie des user stories est en place, vous pouvez la découper en user stories et planifier lesquelles iront dans chaque itération et dans chaque version. Vous devriez parcourir la cartographie des user stories avec les parties prenantes et voir si vous pouvez pensez à d'autres détails ou à d'autres problèmes. La cartographie des user stories vous aide à réfléchir à propos de la valeur que le système délivre.

**Impatient d'essayer**  
Comme la plupart des équipes que je connais, notre équipe se débat pour obtenir le bon niveau de détails sur les exigences de chaque user story avant que de commencer à tester et à coder. Nous ne voulons pas faire de conception préalable, mais nous ne voulons pas perdre du temps à faire du va-et-vient avec le _product owner_ et les autres experts métiers pour définir avec précisions les spécifications pendant le développement. Des techniques de _brainstorming_ telles que les cartes heuristiques nous y ont aidé, mais nous avons  toujours le sentiment que nous perdons trop de temps avec l'accouchement des exigences.

J'avais envie depuis quelques temps d'essayer la cartographie des user stories et de voir si elle pouvait nous aider à matérialiser les détails d'un thème et les user stories avant le développement. J'étais donc contente lorsqu'un après-midi notre _ScrumMaster_ vint me dire : "Nous voulons essayer la cartographie des user stories pour le thème de demain 'Nous vous aidons à choisir'."

J'étais ravi que finalement mon voeu soit exaucé, mais j'étais aussi embêtée. Je devais partir pour les Agile Testing Days [^1] à Postdam dans quelques jours, et nous étions en plein milieu d'un sprint difficile et assez animé. Je n'avais pas le temps de rentrer pour étudier attentivement comment faire précisément une cartographie de stories. Je pensais que je pourrais survoler le sujet. (petite musique d'attaque de requins bien connue).

[^1]: conférénce dédiée aux tests logiciels en approche agile

Une chose que j'avais compris à propos de la cartographie des user stories était que toutes les parties prenantes doivent participer. Très souvent, il nous manquait des parties prenantes essentielles dans nos réunions d'estimations et de _brainstorming_, aussi ai-je insisté pour que toutes les parties prenantes de ce thème soient présentes pour notre session de cartographie des user stories. Dans ce cas, il s'agissait d'une seule personne, mais beaucoup des thèmes dont nous nous occupons impliquent plusieurs parties prenantes.

**Mal le faire**  
Nous nous sommes rassemblés dans notre salle de conférence avec des grandes notes adhésives, des marqueurs, et un tableau blanc. Mais tout d'abord, quelques informations pour comprendre le contexte de notre domaine : notre application automatise tous les aspects de la vente, de la création et de la gestion de plans de retraites 401(k)[^1]. Le thème "Nous vous aidons à choisir" que nous devions planifier reposait sur une tierce partie commerciale aidant les épargnants 401(k) à décider comment investir leurs fonds de pensions. Si un employeur qui propose ce plan 401(k) à ses employés veut offrir ce service, cet employeur doit payer un extra.

[^1]: Système de retraite défini dans le droit fiscal américain - NdT

Nous étions dix personnes dans la pièce. La première chose que j'ai oublié était de devoir les répartir en petits groupes de trois à cinq personnes et que chaque groupe devait cartographier le thème. Oh oh.

J'ai commencé par poser des questions à nos experts métiers au sujet des personas pour le thème. Qui devrait l'utiliser ? La réponse fût les commerciaux. Malheureusement, nos parties prenantes ne connaissaient quasiment rien au sujet des commerciaux, donc nous ne pourrions pas vraiment donner vie à la personnalité de ce persona. Ce n'était pas un bon début ! Tous ce que nous pourrions faire serait de l'appeler "Sammy le commercial" et dire qu'il était seulement intéressé par réaliser une vente.

Ensuite, j'ai demandé pour ce thème à chacun de se lever, de prendre un marqueur et quelques notes adhésives et de commencer à mettre des tâches utilisateurs sur une frise temporelle. Qu'est-ce que Sammy le commercial ferait d'abord ? Qu'est-ce qu'il ferait ensuite ? Nous savions que le thème tournait autour de la mise en place d'un nouveau plan 401(k), et donc que nous devrions organiser les tâches utilisateurs autour de ça.

Personne ne s'est levé de sa chaise. Si seulement j'avais pu me rappeler de faire la répartition en petits groupes ! J'ai répété ma requête de manière plus assertive. Le _ScrumMaster_ s'est levé et est venu se joindre à moi. Personne d'autre ne s'est levé. Après coup, je pense que j'aurais dû faire la cartographie des stories sur la table de conférence à la place de la faire sur le tableau, mais sur le moment je n'y ai pas pensé. 

Ayant abandonné le fait que les personnes se déplacent physiquement, j'ai posé la question, "Quelle est la première chose que Sammy le commercial ferait ?". Il va créer un plan 401(k) pour un employeur. C'était une accroche en plusieurs étapes afin que la frise temporelle paraisse assez évidente. J'ai écris "Étape 1" sur une note adhésive et je l'ai mise sur le tableau blanc. Le commercial saisirait les informations concernant l'entreprise, puis sélectionnerait les options de contributions du plan, puis sélectionnerait les fonds communs de placement ou les options "Aidez-moi à choisir", et ainsi de suite.

Une fois que nous avons eu une frise temporelle pour ces tâches, nous avons pris du recul et nous sommes entrés dans les détails. Qu'est-ce qui changerait à chaque étape par rapport à ce que font aujourd'hui les commerciaux lorsqu'ils créent un plan 401(k). Nous avons noté alors les détails nécessaires pour chaque page d'IHM ainsi que quelques exigences concernant l'implémentation.

Malheureusement, nous avions commencé à un niveau trop détaillé. D'abord, nous aurions dû identifier les "activités utilisateurs" - les éléments haut niveau que font les utilisateurs pour accomplir un objectif donné. Établir un plan 401(k) est une activité de l'utilisateur Commercial. Gérer les fonds communs de placement est une activité utilisateur. Nous avons commencé avec les étapes spécifiques des "tâches utilisateurs" existantes au sein d'une activité utilisateur. "Sélectionner un regroupement de fonds" est une tâche utilisateur au sein de l'activité d'établir un plan 401(k).

Malgré tout, nous avons parcouru la frise temporelle de ce que Sammy le commercial ferait. Nous avons aussi pensé au besoin pour l'interface utilisateur de pouvoir gérer le programme "Nous vous aidons à choisir" ainsi qu'à un rapport de synthèse de gestion. Nous avons aussi écrit des notes adhésives pour le système de gestion du "regroupement des fonds communs de placement" qui serait offert et pour les quelques rapports permettant le suivi des plans 401(k) ayant choisis une "gamme de fonds". Nous avons ajouté beaucoup d'éléments détaillés pour chaque étape de la frise temporelle, à la fois d'une perspective utilisateur que d'une perspective d'implémentation technique.  

J'ai aussi oublié que nous aurions dû parcourir la cartographie des user stories avec les parties prenantes. C'est une manière de tester la cartographie et de trouver des détails supplémentaires. Bien sûr, maintenant que nous avions la cartographie, nous pourrions le faire plus tard.

**Qu'est-ce que nous avons fait pour nous sortir de là ?**  
En fin de la réunion, je savais que j'avais fait plusieurs erreurs sur la cartographies des user stories. J'ai présenté mes excuses à l'équipe, j'ai levé mes bras en l'air en signe de reconnaissance de mes erreurs, et j'ai dit : "Comme c'est fascinant !". Je leur ai demandé d'applaudir mon échec. J'ai espéré que aurions encore appris quelque chose.

Lorsque la réunion a pris fin, je suis revenu sur mes notes sur la cartographie des user stories et j'ai trouvé ce que j'avais raté. Je suis revenu vers le tableau blanc et j'ai ajouté les notes adhésives pour la ligne "activité utilisateur" manquante. (Nous avions des activités utilisateur implicites, mais nous ne les avions pas spécifié sur le tableau blanc). J'ai colorié certains détails selon un code couleur en dessous de chaque tâche utilisateur pour indiquer lesquelles étaient des implémentations techniques, lesquelles étaient des questions importantes, et lesquelles étaient des tâches connues. Et maintenant, cela ressemblait plus à une cartographie de stories (voir figure 1).

![story mapping]({{ site.url }}assets/comment_cartographier/Crispin_Lisa_Story_Mapping_01.jpg)

J'ai demandé à mes co-équipiers leur _feedback_ sur notre tentative quelque peu raté de "cartographie des user stories". Étant donné que nous ne savions pas comment la cartographie des user stories était censé fonctionner, ils étaient OK avec ça. Ils avaient senti que nous avions mis en lumière certains détails sur les stories de ce thème que nous n'aurions pas pu voir autrement qu'à partir du moment où nous aurions commencer à coder.

Un programmeur a fait remarquer qu'il pensait que la cartographie des user stories avait de la valeur en raison de la présence à la réunion de la partie prenante (je l'appellerai "Z"). Le plus souvent, nous avions seulement le product owner pour représenter les parties prenantes. Z s'avéra plus réceptif à des solutions plus simples que notre product owner, et étant donné qu'elle était la véritable partie prenante, elle devait prendre les décisions. Nous avons donc eu plus d'informations par la seule présence de Z à la réunion.

**La prochaine fois**  
Nous avons commencé à travailler sur les user stories de ce thème le sprint d'après. Nous avons senti que nous commencions avec une meilleure compréhension commune que nous ne le faisons certaines fois pour un nouveau thème. Nous avons découpé le thème en user stories de taille appropriée et nous avons compris les dépendances entre elles. Toutefois, une certaine confusion est survenue, à propos de relations sous-jacentes sur une partie du modèle, et a provoqué plusieurs heures de perte en temps et en discussion.  C'est justement ce que nous avions tenter d'éviter avec la cartographie des user stories, et cela arrivait encore. C'était très frustrant.

En dépit d'avoir toujours certains "accouchements d'exigences", mes co-équipiers sentent que la cartographie des user stories vaut le coup d'être essayer. Ils pensent qu'elle a autant de potentiel qu'une technique de _brainstorming_. La prochaine fois, nous nous répartirons en deux petits groupes, chacun produisant une carte, que nous consoliderons ensuite. Nous saurons commencer par les activités utilisateurs pour ensuite les approfondir en tâches utilisateurs et en détails. Nous essayerons la cartographie sur la table de conférence, afin que je ne sois pas la seule personne à écrire les activités, tâches et détails utilisateurs.

Même les échecs nous permettent d'apprendre, je suis heureuse d'avoir vu mes erreurs et de les avoir reconnues plutôt que de m'être découragée. Nous nous améliorons en essayant des expériences, et l'équipe est d'accord pour continuer celle-la. Je vous tiendrai au courant !

---  
Auteur : [Lisa Crispin](http://lisacrispin.com/about/)  
Source : [Story Mapping The Wrong Way](http://www.stickyminds.com/article/story-mapping-wrong-way)  
Date de parution originale : 12 Décembre 2011  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 13/10/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

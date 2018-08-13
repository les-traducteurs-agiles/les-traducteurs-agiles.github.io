---
layout: post
title:  "Le modèle INVEST - S comme stories Suffisamment petites, extenSibles "
date:   2017-10-16 00:00:01
published: true
tags:
- user story
---

Le **S** du modèle [INVEST](http://www.les-traducteurs-agiles.org/story/2015/02/23/investissez-dans-de-bonnes-stories-et-dans-des-taches-smart.html) est pour “Suffisamment petites”. J’utilise désormais ce **S** pour quelque chose d’autre qui je pense capture cette idée encore mieux : extenSible.

Extensible signifie “pouvoir changer de taille ou d’échelle”, ce qui est plutôt pratique dans une _storie_. Nous voulons des _stories_ taillées selon ce que nous essayons de faire.

Envisager les _stories_ sur trois niveaux différents - haut, intermédiaire et bas - s’avère plutôt pratique.

## Les _stories_ de haut niveau : Thèmes et activités

Le niveau le plus haut nous permet d’appréhender la forme et la portée du système dont nous avons besoin.

Ce type d’élément est si gros que la plupart des gens ne les appellent pas des _stories_. Vous les connaissez peut-être sous le nom de “Thèmes” (Kent Beck), d’“activités” (Jeff Patton), d’“épiques” (SaFE), ou de “niveau cerf-volant” (Alistair Cockburn). (Nous n’irons pas plus loin dans les détails).

Par exemple, supposons que nous voulons créer un nouveau système de location de voiture. Nous pourrions envisager de parler de :

* Réservation de véhicules
* Location de véhicules
* Retour de véhicules
* Statistiques

En regardant cette liste, nous pourrions réaliser tout d’un coup que nous n’avions pas pensé aux “Vols et accidents” : que se passe t’il si un véhicule est volé ou endommagé ? Peut-être que le concept devrait être “Gestion de flotte” et qu’il devrait inclure la préparation des véhicules.

Je ne suis pas un expert en location de véhicules, mais il y a sûrement d’autres domaines importants à envisager pour ce système. À ce niveau de vision, ce nombre est sans doute plus proche de la douzaine que de la centaine.

Il ne s’agit donc pas du type de _stories_ que quelqu’un peut implémenter directement. Nous utilisons ce type de _stories_ pour répondre à la question “Avons-nous oublier quelque chose d’important ?”

## Les _stories_ de de niveau intermédiaire : les gros titres

Le niveau intermédiaire correspond aux gros titres des _stories_. Plus précisément au niveau de la cartographie des _stories_ et des plannings de livraison.

Pour qu’un gros titre ait du sens, nous devons parler d’un type particulier de _story_ : Externe et [ayant de la valeur](http://www.les-traducteurs-agiles.org/2017/04/25/le-modele-invest-pour-des-stories-de-valeur.html). De telles _stories_ démarrent à l’extérieur d’un système, et décrivent l’action d’un utilisateur ou d’un système qui accomplit quelque chose d’important pour une partie prenante.

Il n’est pas nécessaire que les gros titres suivent un modèle en particulier ; par défaut, j’utilise le modèle proposé par _Industrial Logic_ : **Rôle - Action - Contexte** :

* Rôle - l’utilisateur ou le système déclenchant la story
* Action - ce qu’il se passe
* Contexte [optionnel] - quand, où, et/ou comment

_Exemple_ : un client achète un article  
_Exemple_ : un client achète un article avec une carte bancaire

Certaines équipes écrivent des gros titres et des _stories_ super détaillés, mais  qui couvrent une partie d’une action du système seulement. Ne procédez pas de cette manière - vos _stories_ doivent décrire une interaction complète (tout en restant si possible concise) et qui apporte quelque chose. Gardez pour plus tard les détails.

De manière assez ironique, les gens créés parfois des “stories techniques” (sic) partielles au prétexte qu’ainsi les _stories_ restent de petite taille. Elles sont peut être de petite taille, mais il ne s’agit pas de _**user** stories_. Un _Product Owner_ ne peut pas travailler avec efficacement.

> Les “_stories_ techniques” (sic) sont peut être de petite taille, mais il ne s’agit pas de _**user** stories_

Les _stories_ qui ont de l’importance aux yeux des utilisateurs et sur lesquelles il est possible d’avoir plusieurs niveaux de détails offrent beaucoup de plus souplesse dans un modèle de livraison agile. Si nous pouvons rassembler les _stories_ les plus critiques et les livrer d’une manière minimaliste, nous pourrons ainsi avoir rapidement une version opérationnelle du système (cf. le concept d’Alistair Cockburn du [Squelette qui marche](http://alistair.cockburn.us/Walking+skeleton).)

Une fois que le système est opérationnel même s’il n’est pas parfait, nous pouvons commencer à l’utiliser, tout en l’améliorant simultanément au fur et mesure des usages. Cela peut nous permettre de commencer à en tirer quelques revenus (eh ouais !) mais cela nous apportera en tout cas des retours d’informations bien plus vite.

Nous avons besoin de ces retours d’informations … car, que nous le voulions ou non, nous sommes ignorants. Nous avons sans doute des théories sur ce qui est valable, mais nous n’avons pas pu les vérifier jusqu’à présent. Nous avons construit un château de cartes basé sur nos propres suppositions. (Lisez donc [ceci](https://www.amazon.fr/Lean-Startup-Adoptez-linnovation-continue/dp/2744066400) si vous voulez approfondir le sujet des produits minimum viables.)

Je suis sûr et certain qu’il y a des domaines où les _Product Owners_ savent pertinemment la valeur des choses qu’ils demandent, mais j’avoue que je n’en rencontre pas souvent. Dans les endroits où j’interviens, souvent les gens n’ont que peu de données sur l’utilisation des applications, les ventes, etc. Et même lorsqu’ils ont des données sur ce que les utilisateurs et les clients font, ils ont tendance à essayer de prédire l’avenir et ce qui pourrait plaire aux personnes qui ne sont pas (encore) des utilisateurs ou pas (encore) des clients.

## Les _stories_ de bas niveau : les détails

Tout en bas, nous nous occupons de savoir comment nous allons réaliser les choses.

Par exemple : _**Un client achète un article**_

Cette _story_ peut être faite de plusieurs manières.

Par exemple, j’ai l’habitude d’acheter des cartouches de gaz pour soda sur un site web sur lequel il est possible d’envoyer sa commande simplement par courriel en indiquant votre numéro de téléphone. Ensuite Joe vous rappelle pour récupérer vos informations de paiement et de livraisons.

Cette _story_ pourrait fonctionner aussi de l’une des manières suivante :

* Dans un magasin physique, un client pourrait demander à un vendeur un certain article. Le vendeur l’attrape sur une étagère derrière lui, écrit un reçu avec un papier carbone, vous donne l’article et l’original du reçu et met la copie carbone sur une pique.

* Dans un supermarché, un client pourrait déambuler dans le magasin, prendre les articles qu’il souhaite dans un chariot, puis les payer à une caisse à la sortie du magasin. Certaines magasins ont des caisses en libre-service où vous pouvez passer vous-mêmes les articles en caisse.

* Quand vous achetez quelque chose sur Amazon.com, votre carte de crédit est déjà enregistré (suite à un achat précédent), et Amazon essaye de vous vendre des produits connexes ou des produits de gamme supérieure lors de la finalisation de votre commande. (Votre achat d’ailleurs viendra alimenter différente tableaux et statistiques, quis sont décrits peut-être dans d’autres _stories_.)

De nombreuses variations peuvent naître d’un seul gros titre. C’est ça des _stories_ extensibles.

Nous allons dans différents types de magasins pour pouvoir faire les choses de manière différentes, mais nous oublions quelque fois que nos implémentations peuvent évoluer elles-aussi.

> Différentes variations peuvent naître d’un seul gros titre. _C’est_ ça des _stories_ extensibles.

Vous avez reconnu peut-être la nature [itérative](http://jpattonassociates.com/dont_know_what_i_want/) de cette approche. Ce qui est itératif ce n’est pas seulement l’implémentation logicielle mais aussi les détails de la _story_

## Extensibilité et décomposition

Un gros titre peut couvrir plusieurs _stories_ potentielles.

Vous êtes peut-être déjà familier avec l’idée de la [décomposition des _stories_](http://xp123.com/articles/twenty-ways-to-split-stories/). Par exemple, sur une _story_ quelconque, l’équipe peut venir vous voir et vous dire “Cette _story_ est trop grosse, un plus petit morceau nous irait amplement.”

Mais la décomposition peut s’avérer traumatisante : vous avez bâti une description complète d’une _story_ avec toutes les possibilités et toutes les idées possibles que vous ayez pu imaginer. Puis l’équipe prend un scalpel, un couteau, ou une massue, et la met en charpie.

Ce processus peut amener un _product owner_ au bord des larmes.

C’est là où l’extensibilité entre en jeu. Pensez à l’[intensité](http://xp123.com/articles/intensifying-stories-running-with-the-winners/) d’une story comme d’un cadran : squelettique, minimale, naturelle, élaborée, excessive. (Ce sont des niveaux d’intensité dont les contours ne sont pas complètement définis)

![échelle d’intensité]({{ site.url }}assets/bill_wake/intensityScale-fr.png)

Passez de la _décomposition_ des _stories_ à l’__**intensification**___ des _stories_.

> Passez de la _décomposition_ des _stories_ à l’__**intensification**___ des _stories_.

En tant que _product owner_, travailler graduellement. Démarrez petit - encore plus petit que vous ne pourriez l’imaginer - et faites grandir vos _stories_  -

## Quelle taille ?

Les grosses _stories_ c’est compliqué.

* Il est assez difficile de savoir si nous avons les bonnes fonctionnalités (étant donné que nous ajoutons beaucoup de choses sans avoir beaucoup de recul)

* Les grosses _stories_ sont souvent le résultat du mélange d’un ensemble de choses ayant plus ou moins de valeur, il est donc plutôt difficile de faire la part de la contribution de chacune.

* Les grosses _stories_ obligent l’équipe de livraison à digérer et à livrer des grosses portions de travail.

> Les grosses _stories_ c’est compliqué

Vous avez peut être appris à faire des _stories_ qui soient des FMV : Fonctionnalités Minimales Vendables. Mais même ce genre de _stories_, c’est trop gros dans un monde de livraison continue. À la place, pensez au Minimum de Fonctionnalités Utiles - un ensemble de petites choses qui rendent la vie d’une personne un peu plus facile (et qui peuvent se transformer en choses plus imposantes).

Prenons par exemple, l’évolution d’un moteur de recherche : l’interface utilisateur demeure inchangée, mais les résultats de la recherche sont un peu plus pertinents. Cette évolution vaut le coup d’être livrer même si elle ne mérite pas de figurer dans les journaux.

J’encourage souvent les gens à faire des _stories_ plus petites - allant de quelques heures à quelques jours d’effort, et non de quelques semaines à quelques mois.

Est-ce que des _stories_ peuvent devenir trop petites ? Tout à fait. J’aime bien l’analogie de Jeff Patton, du [sac de feuilles mortes](http://jpattonassociates.com/the-new-backlog/), dépourvues de structure et qui vous submergent sous une tonne de détails, pour parler des _stories_ trop atomisées.

Comment pouvez-vous gérer des _stories_ trop petites ? Fusionnez-les. (C’est l’une des raisons pour lesquelles j’aime bien voir les _stories_ sous la perspective des “gros” titres - vous pouvez avoir des _stories_ couvrant différents niveaux de détails, en les généralisant et en les fusionnant par la suite, elles seront à même de parler des gros titres et de l’état actuel de l’implémentation.)

Malheureusement, un certain nombre d’outils “agiles” de planification prennent une vue hiérarchique, atomisée, et n’aide pas beaucoup à penser en terme de _stories_ extensibles. Cela fait du boulot de maintenir une vision d’ensemble.

## Conclusion

John Gall a dit “Tout système complexe opérationnel est à l’origine un système simple opérationnel qui a évolué. Un système complexe créé ex-nihilo ne fonctionnera jamais et ne pourra jamais être corrigé. Vous devrez recommencer avec système opérationnel simple.” C’est un bon rappel pour les _stories_.

Rappelez-vous les trois niveaux vus précédemment :

1. **Thème - Haut niveau** : Abordons-nous les bonnes choses ?
2. **Gros titre - Niveau intermédiaire** : Est-ce que l’utilisateur obtient quelque chose qui soit important à ses yeux ?
3. **Détails - Bas niveau** : Avons-nous besoin de quelque chose de nouveau, ou pouvons-nous améliorer quelque chose d’existant ?

Plutôt que de décomposer des _stories_ trop grosses, entraînez-vous à démarrer avec des versions plus petites, puis à les étendre et à les intensifier. Si vous devez les décomposer, faites-le d’un point de vue utilisateur et non d’un point de vue technique.

Vous trouverez que des _stories_ extensibles vont vous :

* Aider à rendre l’avancement visible
* Donner une utilité immédiate
* Donner du retour pour vous aider à aller vers un résultat ayant plus de valeur
* Aider à réduire le risque commercial et technique

---
Auteur : [Bill Wake](http://xp123.com/about/)  
Source : [Small – Scalable – Stories in the INVEST Model](http://xp123.com/articles/small-scalable-stories-in-the-invest-model/)  
Date de parution originale : 02 Novembre 2016  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 16/10/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

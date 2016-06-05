---
layout: post
title:  "Soyez bienveillant avec votre code"
date:   2016-06-05 21:00:55
published: true
categories: 
- developpement
---

En tant que programmeur, je passe beaucoup de temps en face d'un ordinateur. Mais en dépit des apparences, je ne suis pas là, je ne suis pas devant un ordinateur 8 heures par jour m'abîmant les yeux et affaiblissant mes muscles. Je suis quelque part ailleurs.

Je suis dans un monde spectaculaire remplis d'idées exécutables, manipulant des artéfacts abstraits faits de concepts. Je les assemble pour générer une structure significative dans laquelle un programme d'ordinateur peut évoluer. Ce monde est comme une cité qui grossit au fur et à mesure que nous y ajoutons de nouveaux comportements. Il y des quartiers de dépôts, des marchés de paniers d'achats, des concours de mode de vues, la circulation gérée par des contrôleurs, etc.

Mais cette cité n'est pas à moi tout seul. Elle est construite par toutes les personnes de mon équipe. C'est un endroit partagé avec d'autres, dans lequel nos créations grandissent ensemble. Au début, il est simple et petite comme un village avec juste quelques petites classes, mais avec le temps, il évolue en une cité peuplée où abonde les composants. Une partie des quartiers est bien propre et délicatement ouvragée avec des grattes-ciels bien découplés, alors que d'autres se détériorent, sous la pression du "Livrez maintenant !"

## La théorie de la fenêtre brisée

La théorie de la fenêtre brisée repose sur une série d'expériences sur des voitures abandonnées. Une voiture avait été laissée à Palo Alto en Californie par des chercheurs, elle y resta intacte pendant plus d'une semaine. Une semaine après, un chercheur retourna à la voiture et cassa une vitre. Maintenant que la voiture semblait abandonnée, plutôt que simplement garée, il se passa peu de temps avant qu’elle soit vandalisée et détruite. Il avait suffit d'une vitre brisée pour démarrer ce processus.

En quelques mots, la théorie précise que la perception sociale du degré de préoccupation que les gens autour de vous montre à propos de quelque chose est un facteur important de votre propre degré de préoccupation pour cette même chose. Lorsque vous voyez des détritus dans la rue, jeter un papier sale de plus par terre ne fait pas beaucoup de différence. Lorsque les rues autour de vous sont propres, vous vous arrêtez et vous réfléchissez. 

L'autre partie de la théorie est que les problèmes sont plus faciles à corriger lorsqu'ils sont petits. Ce qui commence avec une seule fenêtre cassée conduit à davantage de fenêtres cassées, et éventuellement à des bâtiments abandonnés ou infestés de vermines. Les petits problèmes peuvent devenir facilement de gros problèmes si nous ne les corrigeons pas rapidement.

## Contribuez-vous à l'effet de la fenêtre cassée ?

En tant que bon développeur, il y a de fortes chances que vous soyez vraiment bon à trouver des erreurs, ou que vous trouviez de meilleures façons d'implémenter le code d'un autre développeur. Quelques fois je m'aperçois que je m'interroge sur ce à quoi était en train de penser le développeur qui a écrit ce code, ou même s'il l'appelait "tas de merde" à voix haute. Mais que se passe t'il si je ne le change pas ?

Quel est l'effet de pointer du doigt quelque chose de vraiment mauvais dans le code, et de ne rien faire dessus ? C'est comme montrer une fenêtre cassée et laisser savoir à tout le monde que vandaliser le quartier est acceptable.

Avoir un code dégradé n'est pas génial, mais le danger réel repose sur ce qui se passe lorsque vous et votre équipe l'acceptez en tant que réalité et que personne ne le corrige. Imaginez l'effet que cela peut avoir sur de nouveaux arrivants dans l'équipe si tout le monde agit de cette manière. C'est comme une invitation à vivre dans l'une des pires parties de la cité. Aimeriez-vous vivre là ? Auriez-vous le courage d'améliorer les choses si personne d'autre ne le fait ?

Si les fenêtres cassées s'accumulent, alors au bout d'un certain temps la dégradation progressive de la qualité de votre projet sera hors de contrôle. C’est comme avec la théorie de la fenêtre cassée, au début le coût du _refactoring_ d'un code merdique est réduit, mais si vous trainez, il deviendra rapidement inabordable.

Ce qui marque le plus cette différence vis-à-vis de la qualité d'un projet est l'attitude de l'équipe quant à l'amélioration des choses.

## Le règle des scouts

Les bonnes équipes suivent la règle des scouts : "Toujours laissé le terrain du campement plus propre que vous ne l'avez trouvé." Les bonnes équipes améliorent l'environnement, rendant les choses plus faciles pour les autres pour ajouter du nouveau code. Rendez votre cité plus belle lentement en réparant une fenêtre à la fois. Faites-le pendant que vous êtes en train d'ajouter une nouvelle fonctionnalité dans le coin. Il n'y a pas de quartier en sale état avec la règle des scouts.  

L'une des premières étapes pour appliquer cette règle est d'arrêter d'ignorer le code difficile. En désignant un code comme mauvais, vous êtes en train de le mettre à l’index comme étant un code ne valant pas le coup d'être sauvé. Quand vous faites ça, vous êtes en train de renforcer l'idée que votre quartier est un quartier malfamé. Le "bordel" devient alors une part essentielle de votre code, et il n'y a rien que vous puissiez faire pour empêcher ça.

Traitez-le plutôt comme "laissé sans surveillance". Cela ne veut pas dire que le code est bon, mais cela exprime votre volonté de l'améliorer. C'est un morceau de logiciel qui fonctionne vraiment, mais qui attend d'avoir (et qui mérite) un peu d'attention et de soin.

## Et, maintenant quoi ?

Si vous sentez que vous ne savez pas par où commencer pour améliorer votre cité… Si vous voyez beaucoup de vitres brisées… Si vous savez que votre ville a besoin d'aller mieux… Alors commencez à agir maintenant.

Vous pouvez encouragez les personnes à agir simplement en changeant les mots que vous utilisez. Commencez en parlant de l'état du code par rapport à un calendrier précis (par exemple "c'est sans surveillance pour l'instant".) et bannissez l'idée que le code est un "tas de merde". En faisant cela, vous générez un environnement propice à l'application de la règle des scouts. Commencez par _refactorer_ des petits morceaux de logiciels lorsque vous en verrez l'occasion et encouragez votre équipe à faire de même.

Références :

"Is the Broken Windows Theory Effective?" - SiOWfa13: Science in Our World: Certainty and Controversy. N.p., n.d. Web. 01 Oct. 2015.

---  
Auteur : [alexandru codreanu, dario garcia, lucas giudice](http://www.8thlight.com/team/)  
Source : [Caring about coding](https://blog.8thlight.com/alexandru-codreanu/dario-garcia/lucas-giudice/2015/10/30/caring-coding.html)  
Date de parution originale : 30 Octobre 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 05/06/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



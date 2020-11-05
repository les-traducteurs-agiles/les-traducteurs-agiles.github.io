---
layout: post
title:  "Testabilité et bonne conception"
date:   2014-08-28 23:24:55
tags: test
---
La plupart du temps, le groupe de discussion Yahoo sur le développement piloté par les tests est plutôt calme, mais récemment, il a été réveillé de son sommeil hivernal. La question "Est-il correct d'ajouter du code à une classe uniquement pour améliorer sa testabilité ?" a provoqué une discussion tous azimut ayant abouti à la discussion de ce qui constitue une bonne conception. Avec le commentaire suivant, "Oncle Bob" Martin a tracé dans le sable une ligne jaune à ne pas franchir :


> Une définition raisonnable d'une bonne conception est la testabilité. Il est difficile d'imaginer un système logiciel qui soit à la fois testable et mal conçu. Il est aussi difficile d'imaginer un système logiciel qui soit bien conçu mais également intestable.


Je suis foncièrement d'accord avec cette affirmation, bien que je n'irai pas aussi loin. Je ne pense pas qu'il soit difficile d'imaginer un code qui soit testable, mais mal conçu. Un contre-exemple trivial serait une duplication endémique de code testable. Bien que cela n'affecte pas sa testabilité, j'appellerai cela une mauvaise conception. Aussi, je modèrerai la définition d'Oncle Bob ainsi "Une composante raisonnable de la définition d'une bonne conception est la testabilité.".


Pour moi, la notion de "code testable" est la même chose qu'un "circuit testable" lorsque je travaillais sur un circuit imprimé sur-mesure. En gros, cela dépend de la capacité à mettre le circuit ou le code dans un état connu, à le faire travailler, et voir les interactions avec ses collaborateurs et son état résultant.


Pour les circuits imprimés, la première chose pour rendre un circuit testable était l'état interne prédictif et discernable. Quelques fois, cela peut être accomplit simplement, en ayant au départ un état démarré connu, plutôt qu'aléatoire, et par être capable d'enregistrer les nœuds internes dans un registre à décalage pour être lu ensuite sur un port de sortie dans un mode spécial de test. Cela était suffisant pour le rendre testable, mais généralement pas assez pour le rendre facile à tester.


Être capable de contrôler les nœuds internes dans divers états connus donnait beaucoup plus de possibilités, permettant ainsi de "tester unitairement" différents blocs de circuits. Cela demandait généralement l'ajout de composants supplémentaires uniquement pour la testabilité (un point pertinent par rapport à la question originelle), mais les efforts étaient récompensés par la réduction des temps de tests des unités en production.


Avec les circuits imprimés, une grosse partie de la dépense est dans l'assemblage, et cette dépense est liée significativement au nombre de connecteurs. L'équipement de test évolua pour faire l'équivalent des "lits de clous" utilisés sur les cartes de circuits imprimés, mais appliqué aux zones de contact des matrices de circuits qui ne sont jamais reliés aux connecteurs. Cela permet un accès plus facile aux nœuds internes, à la fois pour contrôler l'état et pour le lire, ceci avant même de découper la plaque de silicium en puces individuelles. Les têtes qui sondent le circuit ont une petite buse qui permettent de faire des pulvérisations sur les circuits défectueux afin qu'ils soient écartés avant l'assemblage.


Avec les logiciels, la capacité à contrôler et à accéder aux nœuds internes est beaucoup plus facile - et souvent sans requérir à aucun circuit logique supplémentaire. Malheureusement, beaucoup de programmes font en sorte de rendre ces nœuds internes inaccessibles, ceci malgré l'absence de coût que pourrait engendrer le fait de les rendre accessibles.


C'est donc de cela dont je veux parler lorsque je parle de la testabilité. Et c'est pourquoi je chicane un peu avec l'affirmation d'Oncle Bob disant que le code testable est nécessairement bien conçu. Le contraire est plutôt facile à croire, mais il y a des cas où, pour des raisons inconnues, la conception est toujours craignos.


Du code bien conçu, comme des circuits bien conçus, porte mieux la complexité et ainsi est plus facile à tester de manière adéquate. Ceci est pour moi, un point important. Nous sommes très susceptibles de rater le coche. Faisons-en sorte de le rater le plus difficilement possible. Et faisons-en sorte qu'il soit de le savoir le plus facilement possible lorsque nous le ratons.


Pour citer C. A. R. Hoare,


> Il y a deux manières d'élaborer la conception d'un logiciel : La première est de la faire si simple qu'il est visible qu'il n'y a pas de défauts, et l'autre est de la faire si compliqué qu'il n'y a pas défauts visibles.


Adam Sroka exprime son inconfort d'appeler un code testable à moins qu'il n'ait été, en effet, testé. À nouveau, je me réjouis de mettre la barre un peu moins haute. Il peut être visible qu'un code est testable même s'il n'a pas été testé. Généralement, ce code doit être assez simple afin que sa testabilité soit évidente. Dans la plupart des cas, néanmoins, le code qui n'est pas testé, est aussi, clairement intestable. De prime abord, les affirmations d'Oncle Bob et d'Adam sonnent justes. Je ne me sens pas vraiment concerné avec la vérité absolue d'aucune d'entre elles. Je préfère toutefois l'affirmation de Michael Feather indiquant qu'il y a une forte synergie entre la testabilité et une bonne conception.


---
Auteur : [George Dinwiddie](http://blog.gdinwiddie.com/about/)  
Source : [Testability & Good Design](http://blog.gdinwiddie.com/2010/02/14/testability-good-design/)  
Date de parution originale : 14 Février 2010  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 28/08/2014  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

---
layout: post
title:  "Les tests continus dans DevOps …"
date:   2018-07-08 00:01
published: true
tags:
- tests
- devops
---

J'ai assisté récemment à des conférences, certaines sur les tests, d'autres sur l'agilité et d'autres encore sur le développement. Même si certaines des sessions étaient agaçantes en raison de quelques embrouillaminis sur un ou deux trucs (que ce soit sur les tests, l'automatisation, agile, BDD,TDD), de manière générale je pense que ces conférences étaient plutôt d'un bon niveau, j'ai pu rencontrer et échanger avec de nouvelles personnes.

Et s'il y a bien une chose dont j'ai entendu parlé avec insistance, c'est DevOps. Beaucoup de gens en parlaient. C'est un sujet majeur ! Toutefois, beaucoup de personnes semblent complètement perdues quant à savoir où se situent les tests dans ce monde merveilleux de DevOps. Certaines suggèrent que DevOps ce n'est que de l'automatisation, mais lorsque vous leur demandez d'expliquer, leurs arguments tombent à plat. D'autres personnes refusent catégoriquement de savoir comment ils pourraient essayer de faire des tests et de les implémenter dans le cadre de DevOps.
Une personne a même dit que désormias plus aucun tests n'étaient nécessaires, tout en montrant sur écran une représentation du modèle DevOps sur laquelle ne figurait aucune mention sur les tests.

J'ai tenté de reproduire de mémoire ce modèle avec le dessin ci-dessous :

![1er modèle]({{ site.url }}assets/dan_ashby/Dev-Ops1.png)

Il s'avère que ce modèle est présenté assez fréquemment dans les différentes conférences (ou du moins avec quelques variations) et vous pouvez aisément comprendre pourquoi les gens s'épuisent à comprendre la place des tests dans un modèle qui ne les mentionne même pas.

Pour moi, les tests sont présents à chacun des points de ce modèle. Laissez-moi donc vous montrez ce que cela veut dire avec une version modifiée de ce modèle

![2ème modèle]({{ site.url }}assets/janet_gregory/Dev-Ops1.png)

Nous pouvons tester le plan. Si, dans ce monde devops, avoir un plan signifie avoir une conception, alors nous pouvons tester la conception. Les tests de la conception d'un logiciel sont exploratoires par nature. Les tests peuvent bien sûr toujours reposer sur la notion de risque car nous utilisons les risques comme d'heuristiques pour focaliser notre investigation. Nos idées que nous explorons à travers nos questions nous aideront à découvrir davantage d'informations. Informations qui nous aideront à remanier la conception (ou le plan) pour le rendre meilleur !

Nous pouvons tester une branche (pas une branche physique d'un arbre, même si je pense que cela pourrait faire l'objet d'un défi de test intéressant à faire pour une certaine personne …). Nous pouvons tester les différentes branches de développement, ou nous pourrions tester les différentes stratégies de branches. Réfléchissez donc à toutes les conversations que vous avez à propos des stratégies de branches, vous vous poser des questions, vous investiguez sur ces différentes idées et remanier vos stratégies … C'est ça faire du test.

Et bien sûr, nous pouvons investiguez notre code ! Nous pouvons vérifier notre code face aux exigences dont nous avons pu discuter lors de notre planification ! Les revues de code - les tests exploratoires pour investiguez sur les erreurs et vérifier si le code est écrit de la meilleure manière possible ou s'il existe une meilleure manière. … Les tests unitaires — grâce à des contrôles automatisés performants qui permettent de s'assurer qu'une exigence est bien prise en compte par le code … Et si vous êtes un développeur qui écrit du code, alors vous pouvez même vous mettre en binôme avec un testeur qui partagera avec vous des idées de tests vraiment cool au sujet des différents risques, des différentes interactions, des différentes perspectives, des différentes variables et des différentes combinaisons de toutes ces choses qui vous aideront tout de suite pendant que vous codez le logiciel ! (Ouais !! C'est super cool !!)

Les fusions doivent être testées et vérifiées aussi ! Faites donc attention aux risques cachés avec les intégrations (et sur les niveaux d'intégrations), et faites attention aussi aux fusions d'erreurs !

Nous pouvons à tous les coups tester la compilation aussi ! Pourquoi ne pas tester le processus de compilation et l'améliorer ? Et en plus de cela, pour quoi ne pas faire tourner un environnement quel qu'il soit et faire quelque tests du produit aussi ? Le test exploratoire est l'approche la plus efficace pour tester et nous aider à voir le niveau de qualité perçu.

Lorsqu'il s'agit de la livraison, nous pouvons là aussi à coup sûr tester ce processus. Et nous pouvons tester notre déploiement (sur un environnement de test et sur un environnement de production aussi). Certaines personnes aiment faire un test "de la fumée" ou un contrôle "sanitaire". Explorez donc à vous en donner à cœur-joie. Assurez-vous juste que votre test (ou les données de votre test) ne vient pas perturber les utilisateurs.

Et une fois que le produit sera disponible, il ne fait aucun doute que vos utilisateurs verront ces fabuleux champs de saisies, ces boutons étincelants ; ils cliqueront à qui mieux-mieux pour satisfaire cette curiosité qui existe en chacun de nous et ainsi tenter de répondre à cette mystérieuse question "et que va t'il se passer si je fais ça …".

Et finalement, vient la supervision … Mais en aucune manière, ce n'est pas parce qu'elle vient en dernier qu'elle n'est pas importante. La supervision est très utile pour nous fournir les informations sur ce que nous lui avons dit de surveiller. Et c'est là que nous pouvons venir tester ! Est-ce que nous lui demandons de regarder les bonnes choses ? Que devrait-elle examiner pour nous envoyer ces petits paquets d'informations pertinentes ? Explorons ces idées ! Et gardons un œil sur cette information et investiguons sur ce qu'elle peut nous raconter aussi.

Mais que manque t'il dans ce diagramme … ? Je ne peux m'empêcher de penser qu'il y a quelque chose qui manque … Ah oui ! Ça saute aux yeux désormais ! Nous ne pouvons pas commencer à planifier à moins d'avoir une idée n'est-ce-pas ?

Ce modèle n'indique pas du tout le travail qui se déroule avant de planifier quoi que ce soit. Voici une image gif sous la forme d'un nuage explosif qui me permettra de préciser ma pensée sur ce point :

![Commencer avec une idée]({{ site.url }}assets/dan_ashby/starts-with-an-idea-fr.gif)

Tester une idée est bien une chose pour laquelle certaines personnes passent complètement à côté … Tout comme le diagramme. Tester une idée est vitale ; investiguer pour découvrir une information, remanier une idée pour l'améliorer et la rendre plus solide. Cela nous permet de contrôler un paquet d'artéfacts, nous pouvons tester ces artéfacts et les remanier aussi. Et nous pouvons alors utiliser ces artéfacts pour contrôler les différentes activités que nous menons, que ce soit la conception et la planification, le développement, le test et la vérification … Et toutes ces activités produisent aussi tout un tas de choses utiles — De la qualité logicielle à tous les niveaux !

Chouette, cet article a été intéressant et nous a permis de franchir une étape dans la compréhension où sont les tests dans le monde de DevOps.

---
Auteur : [Dan Ashby](https://danashby.co.uk/about-me/)  
Source : [Continuous Testing in DevOps…](https://danashby.co.uk/2016/10/19/continuous-testing-in-devops/)  
Date de parution originale : 19 Octobre 2016  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 08/07/2018  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

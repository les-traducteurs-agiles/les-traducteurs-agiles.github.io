---
layout: post
title:  "Les tests continus dans DevOps…"
date:   2018-06-28 00:01
published: true
tags:
- tag1
- tag2
---

I’ve recently attended a number of conferences, some testing ones, some agile ones and some dev ones too. Although some of the talks were painful due to misunderstandings of one thing or another (be it testing, automation, agile, BDD, TDD, etc…), overall, I thought the conferences were pretty good and I met some new people too and got to share some stories with them.

J'ai assisté récemment à quelques conférences, certaines sur les tests, d'autres sur l'agilité et d'autres encore sur les dév. Même si certaines des sessions étaient pénibles à écouter en raison d'une mauvaise compréhension sur un ou deux trucs (que ce soit sur les tests, l'automatisation, agile, BDD,TDD), de manière générale je pense que ces conférences étaient plutôt bonnes, j'ai rencontré de nouvelles personnes et j'ai pu discuter avec elles sur différents sujets.

One thing I heard a fair amount was about DevOps. Many people were talking about it. It’s a big topic! But too many people seemed hugely confused about where testing fits in this wonderful world of DevOps. Some suggested that you only need automation in DevOps, but when asked to explain, their arguments fell floppily by the waist-side. Some people blatently refused to guess at how they’d try and implement testing in DevOps.
And one person even said that no testing was required at all, as he pointed to a DevOps model on a slide, which had no mention of testing on it whatsoever.

Et s'il y a bien une chose dont j'ai entendu parlé avec insistance, c'est DevOps. Beaucoup de gens en parlaient. C'est un sujet majeur ! Toutefois, trop de personnes semblent complètement perdues quant à savoir où se situent les tests dans ce monde merveilleux de DevOps. Certaines suggèrent que DevOps ce n'est que de l'automatisation, mais lorsque vous leur demandez d'expliquer, leurs arguments tombent à plat. Certaines personnes refusent catégoriquement de savoir comment ils pourraient essayer de faire des tests et de les implémenter dans le cadre de DevOps.
Une personne a même dit que plus aucun tests n'étaient nécessaire, tout en montrant sur une diapo une représentation du modèle DevOps sur laquelle ne figurait aucune mention sur les tests.

Here’s my hand-drawn attempt at replicating that model:

J'ai tenté de reproduire de mémoire ce modèle avec le dessin ci-dessous :

[model-1](https://danashby04.files.wordpress.com/2016/10/model-1.jpg?w=820)

![1er modèle]({{ site.url }}assets/dan_ashby/Dev-Ops1.png)

It transpired that this model was presented quite a lot throughout the conferences (or extremely similar ones were presented) and you can see why people struggle to understand where testing fits in a model that doesn’t mention it at all.

Il s'avère que ce modèle est présenté assez fréquemment dans les différentes conférences (ou du moins avec quelques variations) et vous pouvez donc tout à fait comprendre pourquoi les gens luttent pour essayer de comprendre où les tests se situent dans un modèle qui ne les mentionne même pas.

For me, testing fits at each and every single point in this model. Let me break this down for you in an updated version of that model to show you what I mean:

Pour moi, les tests sont présents à chacun des points de ce modèle. Laissez-moi donc vous montrez ce que cela veut dire avec une version modifiée de ce modèle

[model-2](https://danashby04.files.wordpress.com/2016/10/model-2.jpg?w=820)

![2ème modèle]({{ site.url }}assets/janet_gregory/Dev-Ops1.png)

We can test the plan. If, in this devops world, plan comes to mean design, then we can test the design. Testing the design of the software is exploratory in nature. It can still be risk based, as we use the risks as heuristics to focus our investigation. Our ideas that we explore through questions will help us incover more information. Information that will help us refactor the design (or plan) to make it better!

Nous pouvons tester le plan. Si, dans ce monde devops, avoir un plan signifie avoir une conception, alors nous pouvons tester la conception. Les tests de la conception d'un logiciel sont exploratoires par nature. Les tests peuvent bien sûr toujours reposer sur la notion de risque car nous utilisons les risques comme d'heuristiques pour focaliser notre investigation. Nos idées que nous explorons à travers nos questions nous aideront à découvrir davantage d'informations. Informations qui nous aideront à refactorer la conception (ou le plan) et ainsi à le rendre meilleur !

We can test a branch (not a physical branch on a tree, although I’m sure that would make an interesting testing challenge for someone…). We can test individual development branches, or we could test our branching strategies. See all the conversations that you have about your branching strategy, and you ask questions and investigate ideas and refactor your strategies… That’s testing.

Nous pouvons tester une branche (pas une branche physique d'un arbre, même si je pense que cela pourrait faire l'objet d'un défi de test intéressant à faire pour quelqu'un …). Nous pouvons tester les différentes branches de développement, ou nous pourrions tester les différentes stratégies de branches. Réfléchissez donc à toutes les conversations que vous avez à propos des stratégies de branches ; vous pourriez donc vouloir vous poser des questions et investiguez sur ces différentes idées et refactorer vos stratégies … C'est ça le test.

And of course we can investigate our code! We can also check our code too against any expectations that were discussed as part of our planning! Code reviews – exploratory testing to investigate for mistakes and to see if the code is written is a really great way or to investigate if there is a better way… Unit checks – awesome automated checks at code level to ensure that an expectation is met by the code… And if you are a developer writing some code, then you can even pair up with the tester who will share some really cool test ideas about different risks, different interactions, different perspectives, different variables and different combinations of all these things to help you right there while you code the software! (Yey!! How cool!!)

Et bien sûr, nous pouvons investiguez notre code ! Nous pouvons aussi vérifier notre code par rapport aux attentes dont nous avons pu discuter lors de notre planification ! Les revues de code - les tests exploratoires pour investiguez sur les erreurs et pour voir si le code est écrit de la meilleure manière ou s'il existe une meilleure manière. … Les tests unitaires — avec des contrôles automatisés performants au niveau du code pour s'assurer qu'une exigence est bien prise en compte par le code … Et si vous êtes un développeur qui écrit du code, alors vous pouvez même vous mettre en binôme avec un testeur qui partagera avec ce dernier des idées de tests vraiment cool au sujet des différents risques, des différentes interactions, des différentes perspectives, des différentes variables et des différentes combinaisons de toutes ces choses qui vous aideront tout de suite pendant que vous codez le logiciel ! (Ouais !! C'est super cool !!)

Merges need to be tested and checked too! Watch out for the hidden risks of different integrations (and different levels of integrations), and also watch out for merge clashes too!

Les fusions doivent être testées et vérifiées aussi ! Faites donc attention aux risques cachées sur les différentes intégrations (et sur les différents niveaux d'intégrations), et faites attention également aux fusions d'erreurs !

We can certainly test the build too! Why not test your build process and enhance it?
On top of that, Why not spin up an env and do some exploratory testing of the product too? ET is the most effective approach to testing and helps us see a perceived level of quality.

Nous pouvons à tous les coups tester la compilation aussi ! Pourquoi ne pas tester le processus de compilation et l'améliorer ? Et en plus de cela, pour quoi ne pas faire tourner un environnement et faire quelque tests du produit aussi ? Le test exploratoire est l'approche la plus efficace pour tester et ainsi pour nous aider à voir le niveau de qualité perçu.

When it comes to the release, we can certainly test that process too. And we can test our deployment (on a test env & on production too). Some people like to do “sanity” or “smoke” testing and checking. Explore your heart out! Just make sure that your testing (or your test data) isn’t disruptive to the users.

Lorsqu'il s'agit de la livraison, nous pouvons là aussi à coup sûr tester ce processus. Et nous pouvons tester notre déploiement (sur un environnement de test et sur un environnement de production aussi). Certains personnes aiment faire un test "de la fumée" ou un contrôle "sanitaire". Explorer à vous en donner à cœur-joie. Assurez-vous juste que votre test (ou les données de votre test) ne vient pas perturber les utilisateurs.

And once its live, no doubt that your users will see the shiny fields and buttons and will be clicking away to appease their curiosity of solving the “what if I do this…” mysteries that live inside us all.

Et une fois que le produit sera disponible, il ne fait aucun doute que vos utilisateurs verront ces fabuleux champs de saisies et ces boutons étincelants et cliqueront à qui mieux-mieux pour satisfaire cette curiosité qui est en chacun de nous et répondre aux questions "et si je fais ça …"

And finally, here comes the monitoring… But in no way is it least by being last. Monitoring is powerful in supplying us information on what we tell it to look for. And that’s where we can test it! Are we telling it to look at the right things? What should it be looking for to automatically send us those informative little bundles of information? Lets explore these ideas! And lets keep an eye out for that information and investigate what its telling us too.

Et finalement, vient la supervision … Mais en aucune manière, ce n'est pas parce qu'elle vient en dernier qu'elle n'est pas importante. La supervision est très utile pour nous fournir les informations sur ce que nous lui avons dit de surveiller. Et c'est là que nous pouvons venir tester ! Est-ce que nous lui demandons de regarder les bonnes choses ? Que devrait-elle regarder pour nous envoyer ces petits paquets d'informations ? Explorons ces idées ! Et gardons un œil sur cette information et investiguons sur ce qu'elle nous raconte aussi.

But what is missing in the diagram…? I can’t help but feel there is something missing…..
Oh yeah! It’s so obvious now! We can’t start planning unless we have the idea, right??

Mais que manque t'il dans ce diagramme … ? Je ne peux m'empêcher de penser qu'il y a quelque chose qui manque … Ah oui ! Ça saute aux yeux désormais ! Nous ne pouvons commencer à planifier à moins d'avoir une idée n'est-ce-pas ?

The model doesn’t mention all that work that happens before that planning bit. Here’s an explosive fluffy-clouded gif to help explain my thinking on this:

Ce modèle n'indique pas du tout le travail qui se déroule avant de planifier quoi que ce soit. Voici une image gif sous la forme d'un nuage explosif qui me permettra de préciser ma pensée sur ce point :

![starts-with-an-idea](https://danashby04.files.wordpress.com/2016/10/starts-with-an-idea.gif?w=820)

![Commencer avec une idée]({{ site.url }}assets/dan_ashby/starts-with-an-idea-fr.gif)

Testing the idea is something that some people completely miss the boat with… Just like the model did. Testing the idea is vital; investigating to uncover information, refactoring the idea to enhance and solidify it. It allows us to stem lots of different artifacts and we can test those artifacts them to refactor them too. And we can then use those artifacts to stem all of the activities that we conduct, from; designing and planning, development, testing and checking… And those activities produce lots of useful outputs too – Quality software for one!

Tester une idée est bien quelque chose où certaines personnes passent complètement à côté … Tout comme le diagramme. Tester une idée est vitale ; investiguer pour découvrir une information, refactorer une idée pour l'améliorer et la rendre plus solide. Cela nous permet de juguler un paquet d'artéfacts, nous pouvons tester ces artéfacts et les refactorer aussi. Et nous pouvons alors utiliser ces artéfacts pour juguler les différentes activités que nous menons, que ce soit ; la conception et la planification, le développement, le test et la vérification … Et toutes ces activités produisent aussi tout un tas de choses utiles — Tout pour un logiciel qualité !

So hopefully this blog post has been entertaining and has enabled us to take one step further forward in helping to solve that puzzle of where testing fits within the world of DevOps.

Chouette, cet article a été intéressant et nous a permis de franchir une étape pour résoudre cette énigme de savoir où sont les tests dans le monde de DevOps.

---
Auteur : [Dan Ashby](https://danashby.co.uk/about-me/)  
Source : [Continuous Testing in DevOps…](https://danashby.co.uk/2016/10/19/continuous-testing-in-devops/)  
Date de parution originale : 19 Octobre 2016  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : jj/mm/yyyy  nbsp

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

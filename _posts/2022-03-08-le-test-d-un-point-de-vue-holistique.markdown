---
layout: post
title:  "Le test d'un point de vue holistique"
date:   2022-03-08 08:08
published: false
tags:
- test
---

# Holistic testing is a term that I have been thinking about for a while now. There are many different types of testing that need to included in our support for better quality.

# Le test holistique est une expression à laquelle je réfléchis depuis quelques temps. Il existe différents types de test à prendre en compte dans nos efforts d'amélioration de la qualité.

In January 2021, I wrote a blog post called “[Testing And Coding, Not Coding ‘Then’ Testing”](https://janetgregory.ca/testing-and-coding-not-coding-then-testing/) to emphasize that testing and coding are part of the same process. In that post, I introduced a diagram (Figure 1) to show continuous testing.

En janvier 2021, j'ai écrit un article de blog intitulé [« Tester et coder, et non coder « puis » tester »](http://www.les-traducteurs-agiles.org/2022/03/07/tester-et-coder-et-non-coder-puis-tester.html) pour mettre l'accent sur le test et le codage comme faisant partie du même processus. Dans cet article, j'avais présenté le schéma ci-dessous pour illustrer le test continu

![Continuous testing](https://janetgregory.ca/wp-content/uploads/sites/16/2021/04/Continuous-testing-500x281.jpg)

![Test continu]({{ site.url }}assets/janet_gregory/shift-diagram-fr.png)

**Figure 1: Continuous testing**

**Schéma 1 : test continu**

I was ok with the diagram but not completely happy with it, and it seemed to confuse some people, so I’ve been tweaking it and considering what message I really wanted to get across and have settled on this diagram / model (Figure 2) to show how I view a development life cycle.

J'étais plutôt en phase avec ce schéma sans en être complètement satisfaite, mais il m'a semblé qu'il a semé la confusion chez certaines personnes, je l'ai donc un peu modifié et j'ai réfléchi au message que je voulais vraiment faire passer et j'en suis arrivé à ce nouveau schéma / modèle afin de montrer la manière dont j'envisage le cycle de vie du développement.

![Dev cycle1](https://janetgregory.ca/wp-content/uploads/sites/16/2021/04/Dev-cycle1-500x258.jpg)

![Dev cycle1](https://janetgregory.ca/wp-content/uploads/sites/16/2021/04/Dev-cycle1-500x258.jpg)

**Figure 2: Development lifecycle**

**Schéma 2 : Cycle de vie du développement**

It is similar to the DevOps cycle, but you’ll notice it does not have coding, build or test as separate stages within the cycle. To me, the building stage includes coding, and testing is performed in each and every stage.

Il est similaire au cycle DevOps, mais vous remarquerez qu'il n'y a pas comme étape à part entière dans ce cycle ni le codage, ni la construction ni le test. En ce qui me concerne l'étape de construction inclue le codage, et le test quant à lui est réalisé à chaque et à toutes les étapes.

It is hard to include feedback cycles in a diagram without complicating it too much, but this cycle is not meant to be framed by time. Some of the stages will go very quickly or maybe very slowly depending on how many knowns or unknowns exist. Sometimes a team will need to pause and go back a stage or two.

Il est difficile d'inclure des boucles de rétroaction dans un schéma sans compliquer celui-ci outre mesure, mais ce cycle ne s'inscrit pas dans un cadre temporel donné. Certaines des étapes se dérouleront très vites ou peut être très lentement en fonction du nombre d'éléments connus ou inconnus qui existent. Certaines fois une équipe aura besoin de marquer une pause et de reculer d'une étape ou deux.

![Dev cycle2 with pauses](https://janetgregory.ca/wp-content/uploads/sites/16/2021/04/Dev-cycle2-with-pauses-500x261.jpg)

![Dev cycle2 with pauses](https://janetgregory.ca/wp-content/uploads/sites/16/2021/04/Dev-cycle2-with-pauses-500x261.jpg)

**Figure 3: Development cycle with pauses**

**Schéma 3: Cycle de développement avec des pauses**

In Figure 3, I added possible pauses, allowing time for the team to reflect when necessary. For example, perhaps when you are trying to understand more about the feature, you realize that you don’t have enough information and need to go back to planning or discovery? Does this feature even make sense?  Or maybe you’ve deployed to the test environment and you have found some serious issues and need to go back to build, or maybe even back further to understand the behavior or technical implementation a bit more.

Dans le schéma n°3, j'ai ajouté les pauses possibles, afin de permettre à l'équipe de réfléchir si cela est nécessaire. Par exemple, peut être que lorsque vous êtes en train d'essayer de comprendre davantage de choses sur une fonctionnalité, vous réalisez soudainement que vous n'avez pas assez d'information et que vous avez besoin de retourner à l'étape de la planification ou à celle de l'exploration ? Mais cette fonctionnalité a t'elle même un sens ? Ou peut être que vous étiez en train de déployer en environnement de test et vous avez trouvé de grosses anomalies qui ont nécessité que vous retourniez à l'étape de construction voire même plus loin pour mieux comprendre le comportement observé ou l'implémentation technique.

I’ve labeled this model “**holistic testing**”, but so far, I haven’t even mentioned testing. So where does the testing come into play in this model? Taking the idea of Dan Ashby’s “[we test here and here and here](https://danashby.co.uk/2016/10/19/continuous-testing-in-devops/)”, diagram, I’ve tried to list some of the types of testing team might be doing throughout the cycle (Figure 4). _Note:_ this is not meant to be an exhaustive list.

J'ai nommé ce modèle « le test holistique », mais jusqu'à présent, je n'ai même pas mentionné le test. Alors où le test entre t'il en scène dans ce modèle ? En reprenant l'idée du schéma de Dan Ashby « [nous testons ici et ici et ici](http://www.les-traducteurs-agiles.org/2018/07/08/les-tests-continus-dans-devops.html) », j'ai essayé de lister certains types de test que l'équipe pourrait faire tout au long du cycle (Schéma 4).  
_Remarque_ : il ne s'agit pas d'une liste exhaustive

![Dev cycle3 with tests](https://janetgregory.ca/wp-content/uploads/sites/16/2021/04/Dev-cycle3-with-tests-500x281.jpg)

![Dev cycle3 with tests](https://janetgregory.ca/wp-content/uploads/sites/16/2021/04/Dev-cycle3-with-tests-500x281.jpg)


**Figure 4: Holistic testing**

**Schéma 4: le test holistique**

The left side of the loop shows the testing we can be done early. The right side of the loop is about testing to find bugs and learn. There is no start or end of an infinite loop, but I’ll start at discovery – the beginning of an idea.

La partie gauche de la boucle montre les tests que nous pouvons faire au plus tôt. La partie droite de la boucle traite des tests en vue de trouver des anomalies et d'apprendre. Il n'existe pas de commencement ou de fin dans une boucle infinie, mais je vais commencer par la découverte — le commencement d'une idée.

**Discovery:** We are looking for business value. This is often product managers working with customers to decide if the feature is worth while pursuing. They are testing the idea.

**Découverte** : La valeur métier est ce que nous recherchons ici. Le plus souvent ce sont les responsables produits, qui travaillant avec les clients, décident si une fonctionnalité vaut le coût d'être poursuivie. Ils sont en train de tester une idée.

**Planning:** Identify the risks to determine which quality attributes will be important to the feature. Features are sliced into smaller stories and this is time to advocate for testable stories. Teams may start looking at high level acceptance tests and start to get a better understanding of the stories.

**Planification** : Ici, nous identifions les risques pour déterminer quels sont les critères qualités qui seront importants pour une fonctionnalité donnée. Les fonctionnalités sont découpées en _stories_ plus petites, c'est le moment de plaider pour des _stories_ testables. Les équipes peuvent commencer à réfléchir à des tests d'acceptation de haut niveau et à avoir une meilleure compréhension des _stories_.

**Understanding:** Practices like acceptance test-driven development or behaviour-driven development are part of understanding the stories. Teams may use user experience experts to learn about the customer experience. Matt Wynne’s [example mapping](https://medium.com/@mattwynne/introducing-example-mapping-42ccd15f8adf) is a great framework to help map business rules to examples, or perhaps teams can use the 7 Product Dimensions from Ellen Gottesdiener and Mary Gorman’s [_Discover to Deliver_](https://www.discovertodeliver.com/) for structured conversations. Programmers may help by creating low-fidelity prototypes for fast, iterative feedback to reduce some of the risk around unknowns. Conversations around the different quality attributes let teams determine the ‘what and how’ to instrument the code for testing or monitoring or what events to tag for observing later.

**Compréhension** : Des pratiques comme le développement piloté par les tests ou le développement piloté par le comportement font partie de la compréhension des _stories_. Les équipes peuvent faire appel à des experts en expérience utilisateur pour apprendre qu'est ce que l'expérience client. La [cartographie des exemples (example mapping)[VF]](http://www.les-traducteurs-agiles.org/2017/03/21/presentation-cartographie-des-exemples.html) de Matt Wynne est un cadre de travail génial pour aider à cartographie des règles métiers sous la forme d'exemples ; les équipes peuvent aussi utiliser les 7 dimensions du produit et les discussions structurées d'Ellen Gottesdiener et de Mary Gorman’s [_Discover to Deliver_](https://www.discovertodeliver.com/). Les développeurs peuvent aider à créer des prototypes frugaux pour avoir des retours d'informations rapides, itératifs et réduire ainsi une partie des risques liés à la part d'inconnu dans le projet. Les conversations liées aux différents critères qualités permettent aux équipes de déterminer « le quoi et le comment » qui permettront à leur tour d'instrumenter le code pour le test, la surveillance ou les événements à retenir en vue de les observer plus tard.

#RELECTURE

**Building:** This is where the team implement user stories and features – perhaps practicing test-driven development (TDD) and using fast feedback principles to test as soon as possible. Small testable stories make these practices easier to apply. Ensemble work, pairing, code reviews and test reviews take place. The examples created earlier can be used to create executable tests that guide development. These automated tests can become part of your regression suit to give fast feedback to detect regression failures. Teams will perform exploratory testing to uncover what they didn’t think about when they were developing. Understanding the version control system and workflows help determine what testing needs to be done to manage technical risk.

**Construction** : C'est le moment où l'équipe implémente les _user stories_ et les fonctionnalités — des pratiques comme le développement piloté par les tests (TDD) et des principes de rétroactions rapides peuvent permettre peut être de tester dès que possible. De petites _stories_ testables rendent ces pratiques plus faciles à appliquer. Du travail de groupe, du binomage, des revues de codes et des revues de tests, tout ceci se passe pendant la construction. Les exemples créés précédemment peuvent être utilisés pour créer des tests exécutables qui guideront le développement. Ces tests automatisés peuvent faire partie intégrante de votre suite de tests de régression pour que vous ayez des retours d'informations rapides et ainsi détecter des régressions.

**Deploying**: “Build once, deploy many.” I remember when I first heard this idea and how it helped the testing effort. Deploying the same build to multiple environments in the deployment pipeline, enables different testing activities to be performed on different environments, knowing the code will always be the same. For example, the differences might be the configuration, or the amount of data used. Many teams still struggle to have stable test environments, but as organizations adopt virtual and cloud infrastructures, teams can spin up test environments on demand. This may make testing some of the quality attributes simpler like load or performance testing. Deploying to a production like environment if you are not yet doing continuous delivery or deployment enables you to test the system as a whole.

**Déploiement** : « Construire une fois, déployer de nombreuses fois ». Je me rappelle de la première fois où j'ai entendu cette idée et de la manière dont elle a permis d'aider l'effort de test. Déployer le même artefact sur différents environnement à l'aide d'une chaîne de déploiement, permets aux différentes activités de tests d'être accomplis sur différents environnements tout en sacahtn que le code (testé - NdT) sera toujours le même. Par exemple, les différences (observées - NdT) pourraient être dues à la configuration, ou à la quantité de données utilisées. beaucoup d'équipes luttent pour avoir des environnements de test stables, mais au fur et à mesure que les entreprises adoptent des infrastructures virtuelles ou dans les nuages, les équipes peuvent avoir des environnements de test à la demande. Cela rend le test de certains critères qualité comme le test de charge ou de performance plus simple. Déployer dans un environnement identique à la production si vous ne faites pas encore le livraison continu ou de déploiement continu vous permet de tester le système dans sa globalité.

![](https://janetgregory.ca/wp-content/uploads/sites/16/2021/04/Simple-deployment-pipeline.jpg)

![](https://janetgregory.ca/wp-content/uploads/sites/16/2021/04/Simple-deployment-pipeline.jpg)



**Figure 5: Simple deployment pipeline**

**Schéma 5 : chaîne de déploiement simple**

**Releasing:** There are many different mechanisms for releasing to the customer these days. If you are practicing continuous delivery or deployment, you may be using a blue / green deployment strategy. Both environments are the same configuration, but the delivery is to the idle one so testing can happen safely. When ready, the switch is flipped, and the new feature is now on the active production site. More and more teams are using release feature toggles which enable a team to put the feature in production but only make it visible to customers when they feel ready.

**Livraison** : Il existe plusieurs mécanismes différents pour livrer au client désormais. Si vous pratiquez la livraison continu ou le déploiement continu, vous pouvez être amené peut être à utiliser une stratégie de déploiement bleu / vert. Ces deux types d'environnements possède la même configuration, mais la livraison se fait sur le serveur passif afin que les tests puissent se faire de manière sécurisée. Lorsque cette opération est faite, on fait la bascule, et la nouvelle fonctionnalité est désormais présent sur le site actif de production. De plus en plus d'équipe font des livraisons de fonctionnalités activables qui permettent à une équipe de mettre une fonctionnalité en production mais qu'elle ne rendra visible aux clients que lorsqu'elle se sentira prête.

**Observability**: The team captures events they hope will enable them to find problems very quickly if they occur. It’s a way to watch how the customers use the product and allow the team to respond accordingly. Teams can also monitor the system for warnings and errors (if the code has been instrumented to do that).

**Observabilité** : L'équipe capture les évènements qui, elle l'espère, lui permettront de trouver les problèmes très vite si jamais ils viennent à se produire. C'est une manière, pour l'équipe, de regarder comment les clients utilisent le produit et de réagir en fonction de cela. Les équipes peuvent aussi surveiller la survenue d'alertes et d'erreurs dans le système (si le code a bien été instrumenté pour faire cela).

**Learning:** People have questioned me about testing as part of learning. As teams observe how their product is used by their customers, they can hypothesize about how to improve. They are testing our assumptions.

**Apprentissage** : Des personnes m'ont posé des questions au sujet de la place du test dans le cadre de l'apprentissage. Au fur et à mesure que les équipes observent la manière dont leur produit est utilisé par les clients, elles peuvent émettre des hypothèses sur la manière de l'améliorer. Elles sont en train de tester nos postulats.

**Summary**

**En résumé**

The term [continuous testing](https://www.mabl.com/blog/what-does-continuous-testing-actually-mean) has been used and abused, so I’m staying away from that particular term, and I hope that the term “holistic testing” resonates with people. When we test, we need to consider all types of testing, not only the ones we think a tester is responsible for. It includes automation, exploratory testing, or any other type of human-centric testing. It involves the whole team, the product organization, and even the customer. We need to consider testing from a holistic point of view, and I’m hoping this diagram will help people to understand the ‘when’ the different types of testing might take place.

Le terme [test continu (VO)](https://www.mabl.com/blog/what-does-continuous-testing-actually-mean) a été utilisé jusqu'à la corde et détourné de sa signification première, je vais par conséquent me détourner de ce terme et j'espère que le terme « terme holistique » résonera chez les gens. Lorsque nous testons, nous devons considérer tous les types de tests, pas seulement celles dont nous pensons que le testeur est reponsable. Cela inclus l'automatisation, le test exploratoire, ou n'importe quel autre test centré sur l'humain. Cela implique que toute l'équipe, toute l'organisation du produit, et même le client. Nous devons considérer le test d'un point de vue holistique, et j'espère que ce schéma aidera les personne à comprendre « à quel moment » les différents types de test devraient prendre place.

The highest performing teams and organizations that I have worked with, have taken a holistic point of view to the quality of their product, and understand how testing can support that vision.

Les équipes et les organisations les plus performantes avec lesquelles j'ai pu travailler, ont adopté un point de vue holistique sur la qualité de leur produit, et ont compris la manière dont le test permet de soutenir cette vision.

---
Auteur : [Janet Gregory](https://janetgregory.ca/about/)  
Source : [Testing from a holistic point of view](https://janetgregory.ca/testing-from-a-holistic-point-of-view/)  
Date de parution originale : 30 Avril 2021  

---
Traducteur : [[Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : jj/mm/yyyy  nbsp

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

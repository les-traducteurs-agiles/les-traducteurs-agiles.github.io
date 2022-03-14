---
layout: post
title:  "Le test d'un point de vue holistique"
date:   2022-03-14 00:01
published: true
tags:
- test
---

**Le _test holistique_ est un terme auquel je réfléchis depuis quelques temps. Il existe différents types de test à prendre en compte dans nos efforts en vue d'améliorer de la qualité.**

En janvier 2021, j'ai écrit un article de blog intitulé [« Tester et coder, et non coder « puis » tester » (VF)](http://www.les-traducteurs-agiles.org/2022/03/07/tester-et-coder-et-non-coder-puis-tester.html) pour mettre l'accent sur le test et le codage comme faisant partie du même processus. Dans cet article, j'avais présenté le schéma ci-dessous pour illustrer le test continu

![Test continu]({{ site.url }}assets/janet_gregory/shift-diagram-fr.png)

**Schéma 1 : Test continu**

J'étais plutôt en phase avec ce schéma sans en être complètement satisfaite, mais il semble qu'il ait semé la confusion chez certaines personnes, je l'ai donc un peu modifié et j'ai réfléchi au message que je voulais vraiment faire passer et j'en suis arrivé à ce nouveau schéma / modèle (cf. schéma 2) afin de montrer la manière dont j'envisage le cycle de vie du développement.

![Cycle de dev 1]({{ site.url }}assets/janet_gregory/Dev-cycle1-fr.png)

**Schéma 2 : Cycle de vie du développement**

Il est similaire au cycle DevOps, mais vous remarquerez qu'il n'y a pas dans ce cycle d'étape à part entière concernant le codage, la construction et le test. En ce qui me concerne l'étape de construction inclue le codage ; le test quant à lui est réalisé à chaque et à toutes les étapes.

Il est difficile d'inclure des boucles de rétroaction dans un schéma sans compliquer celui-ci outre mesure, et de plus ce cycle ne s'inscrit pas dans un cadre temporel donné. Certaines des étapes se dérouleront très vites et d'autres peut être très lentement en fonction du nombre d'éléments connus ou inconnus. Certaines fois une équipe aura besoin de marquer une pause et de reculer d'une étape ou deux.

![Cycle de dev 2 avec des pauses]({{ site.url }}assets/janet_gregory/Dev-cycle2-with-pauses-fr.png)

**Schéma 3: Cycle de développement avec des pauses**

Dans le schéma n°3, j'ai ajouté les pauses possibles, afin de permettre à l'équipe de réfléchir lorsque cela s'avère nécessaire. Par exemple, peut être que lorsque vous êtes en train d'essayer de comprendre davantage de choses sur une fonctionnalité, vous réalisez soudainement que vous n'avez pas assez d'information et que vous avez besoin de retourner à l'étape de la planification ou à celle de l'exploration ? Mais cette fonctionnalité a t'elle même un sens ? Ou peut être que vous étiez en train de déployer en environnement de test et vous avez trouvé de grosses anomalies qui ont nécessité que vous retourniez à l'étape de construction voire même plus loin pour mieux comprendre le comportement observé ou l'implémentation technique.

J'ai nommé ce modèle « **le test holistique** », mais jusqu'à présent, je n'ai même pas mentionné le test. Alors où le test entre t'il en scène dans ce modèle ? En reprenant l'idée du schéma de Dan Ashby « [nous testons ici et ici et ici (VF)](http://www.les-traducteurs-agiles.org/2018/07/08/les-tests-continus-dans-devops.html) », j'ai essayé de lister certains types de test que l'équipe pourrait faire tout au long du cycle (Schéma 4).  
_Remarque_ : il ne s'agit pas d'une liste exhaustive

![Dev cycle3 with tests]({{ site.url }}assets/janet_gregory/Dev-cycle3-with-tests-1024x576-fr.png)

**Schéma 4: le test holistique**

La partie gauche de la boucle montre les tests que nous pouvons faire au plus tôt. La partie droite de la boucle traite des tests en vue de trouver des anomalies et d'apprendre. Il n'existe pas de commencement ou de fin dans une boucle infinie, mais je vais commencer par la découverte — le commencement d'une idée.

**Découverte** : La valeur métier est ce que nous recherchons ici. Le plus souvent ce sont les responsables produits, qui travaillant avec les clients, décident si une fonctionnalité vaut le coût d'être poursuivie. Ils sont en train de tester une idée.

**Planification** : Ici, nous identifions les risques pour déterminer quels sont les critères qualités qui seront importants pour une fonctionnalité donnée. Les fonctionnalités sont découpées en _stories_ plus petites, c'est le moment de plaider pour des _stories_ testables. Les équipes peuvent commencer à réfléchir à des tests d'acceptation de haut niveau et à avoir une meilleure compréhension des _stories_.

**Compréhension** : Des pratiques comme le développement piloté par les tests ou le développement piloté par le comportement font partie de la compréhension des _stories_. Les équipes peuvent faire appel à des experts en expérience utilisateur pour apprendre qu'est ce que l'expérience client. La [cartographie des exemples (VF)](http://www.les-traducteurs-agiles.org/2017/03/21/presentation-cartographie-des-exemples.html) de Matt Wynne est un cadre de travail génial pour aider à cartographie des règles métiers sous la forme d'exemples. Les équipes peuvent aussi utiliser les 7 dimensions du produit et les discussions structurées d'Ellen Gottesdiener et de Mary Gorman pour [découvrir ce qu'il faut livrer (VO)](https://www.discovertodeliver.com/). Les développeurs peuvent aider à créer des prototypes frugaux pour avoir des retours d'informations rapides, itératifs et réduire ainsi une partie des risques liés à la part d'inconnu dans le projet. Les conversations liées aux différents critères qualités permettent aux équipes de déterminer « le quoi et le comment » qui permettront à leur tour d'instrumenter le code pour le test, la surveillance ou les événements à retenir en vue de les observer plus tard.

**Construction** : C'est le moment où l'équipe implémente les _user stories_ et les fonctionnalités — il se peut que l'utilisation de pratiques comme le développement piloté par les tests (TDD) et des principes de rétroactions rapides permettent à l'équipe de tester dès que possible. D'ailleurs des _stories_ petites et testables rendent ces pratiques plus faciles à appliquer. Le travail de groupe, le travail en binome, les revues de codes et les revues de tests, tout ceci se passe pendant la construction. Les exemples créés précédemment peuvent être utilisés pour créer des tests exécutables qui guideront le développement. Ces tests automatisés peuvent devenir une partie de votre suite de tests de régression pour que vous ayez des retours d'informations rapides et ainsi détecter des régressions. L'équipe réalisera aussi des tests exploratoires pour découvrir ce à quoi elle n'a pas pensé lors du développement. Comprendre les systèmes de contrôle de version et les flux de travails associés vont l'aider à déterminer quels tests doivent être effectués pour gérer les risques techniques.

**Déploiement** : « Construire une fois, déployer de nombreuses fois ». Je me rappelle de la première fois où j'ai entendu cette idée et de la manière dont elle a permis de faire avancer les tests. Déployer le même artefact sur différents environnement à l'aide d'une chaîne de déploiement, permet aux différentes activités de tests d'être réalisées sur différents environnements tout en sachant que le code sera toujours le même. Par exemple, les disparités pourraient être dues à la configuration, ou à la quantité de données utilisées. beaucoup d'équipes luttent pour avoir des environnements de test stables, mais au fur et à mesure que les entreprises adoptent des infrastructures virtuelles ou dans les nuages, les équipes peuvent désormais avoir des environnements de test à la demande. Cela rend le test de certains critères qualité comme le test de charge ou de performance plus simple. Déployer dans un environnement identique à la production si vous ne faites pas encore de livraison continu ou de déploiement continu vous permet de tester le système dans sa globalité.

![Chaîne de déploiement simple]({{ site.url }}assets/janet_gregory/Simple-deployment-pipeline-fr.png)

**Schéma 5 : chaîne de déploiement simple**

**Livraison** : Il existe plusieurs mécanismes différents pour livrer au client désormais. Si vous pratiquez la livraison continue ou le déploiement continu, vous pouvez être amené peut être à utiliser une stratégie de déploiement bleu / vert. Ces deux types d'environnements possède la même configuration, mais la livraison se fait sur le serveur passif afin que les tests puissent se faire de manière sécurisée. Lorsque cette opération est faite, on fait la bascule, et la nouvelle fonctionnalité se retrouve ensuite sur le site actif de production. De plus en plus d'équipe font des livraisons de fonctionnalités activables, ce qui permet à une équipe de mettre une fonctionnalité en production mais qu'elle ne rendra visible aux clients que lorsqu'elle se sentira prête.

**Observabilité** : L'équipe enregistre les évènements qui se passent dans le système, ce qui elle l'espère, lui permettront de trouver les problèmes très vite si jamais ils viennent à se produire. C'est une manière, pour l'équipe, de regarder comment les clients utilisent le produit et de réagir en fonction de cela. Les équipes peuvent aussi surveiller la survenue d'alertes et d'erreurs dans le système (si le code a bien été instrumenté pour faire cela).

**Apprentissage** : Des personnes m'ont posé des questions au sujet de la place du test dans le cadre de l'apprentissage. Au fur et à mesure que les équipes observent la manière dont leur produit est utilisé par les clients, elles peuvent émettre des hypothèses sur la manière de l'améliorer. Elles sont en train de tester nos postulats.

## En résumé

Le terme [test continu (VO)](https://www.mabl.com/blog/what-does-continuous-testing-actually-mean) a été utilisé jusqu'à la corde et détourné de sa signification première, je vais par conséquent me détourner de ce terme et j'espère que le terme « terme holistique » résonnera chez les gens. Lorsque nous testons, nous devons considérer tous les types de tests, pas seulement ceux dont nous pensons que le testeur est responsable. Cela inclus l'automatisation, le test exploratoire, ou n'importe quel autre test centré sur l'humain. Cela implique toute l'équipe, toute l'organisation du produit, et même le client. Nous devons considérer le test d'un point de vue holistique, et j'espère que ce schéma aidera les personne à comprendre « à quel moment » les différents types de test devraient prendre place.

Les équipes et les organisations les plus performantes avec lesquelles j'ai pu travailler, ont adopté un point de vue holistique sur la qualité de leur produit, et ont compris la manière dont le test permet de soutenir cette vision.

---
Auteur : [Janet Gregory](https://janetgregory.ca/about/)  
Source : [Testing from a holistic point of view](https://janetgregory.ca/testing-from-a-holistic-point-of-view/)  
Date de parution originale : 30 Avril 2021  

---
Traducteur : [[Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 14/03/2022  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

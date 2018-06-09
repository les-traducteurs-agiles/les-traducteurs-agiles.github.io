---
layout: post
title:  "LeSS - Spécifications par l'exemple"
date:   2018-02-10 00:01
published: true
tags:
- LeSS
---


[<< Portail LeSS < Portail Excellence Technique](http://www.les-traducteurs-agiles.org/2016/12/26/less-portail-excellence-technique.html)

> Deux choses sont infinies : l’univers et la stupidité humaine ; même si je n’en suis pas certain en ce qui concerne l’univers. -- Albert Einstein


Les spécifications par l’exemple ou le développement piloté par les tests d’acceptation (A-TDD) est une approche collaborative de découverte des exigences dans laquelle les exemples et les tests automatisables sont utilisés afin de spécifier les exigences - par la création de spécifications exécutables. Celles-ci sont crées par l’équipe, le Product Owner, ainsi que par d’autres parties prenantes lors d’ateliers sur les exigences.

Remarque concernant la terminologie : nous utiliserons indifféremment A-TDD et Spécifications par l’Exemple.

Le développement piloté par les tests d’acceptation intègre un certain nombre d’idées majeures :

* les tests en tant qu'exigences, les exigences en tant que tests
* les ateliers pour clarifier les exigences
* l’ingénierie concurrente
* plutôt prévenir que détecter


**Les tests en tant qu'exigences, les exigences en tant que tests** : Dans l'ouvrage [Exploring Requirements: Quality before Design](http://www.amazon.fr/Exploring-Requirements-Quality-Before-Design/dp/0932633137), les auteurs Gause et Weinberg creusent le lien entre exigences et tests, “l’une des manières les plus efficaces pour tester les exigences est d’avoir des cas de tests ressemblant à ceux servant à tester un système complet”. [Melnik et Martin](http://gmelnik.com/papers/Melnik-Martin-Tests-and-Requirements-The-Moebius-Strip-IEEE-Software-2008.pdf) étendent cette théorie plus loin en proclamant : “Au fur et à mesure de la montée en puissance du formalisme, les tests et les exigences deviennent impossible à distinguer l’un de l’autre. À la limite, les tests et les exigences sont équivalents”. Les tests doivent être précis afin d’être automatisables. Le développement piloté par les tests d’acceptation exploite ce formalisme et reformule les exigences à travers l’écriture de tests automatisables.

**Les ateliers pour clarifier les exigences** : Le sixième principe agile nous rappelle que “La méthode la plus simple et la plus efficace pour transmettre de l’information à l'équipe de développement et à l’intérieur de celle-ci est le dialogue en face à face.” Les ateliers de clarifications des exigences en face-à-face sont utilisés depuis l’invention du [Joint Application Design (JAD)](http://www.amazon.fr/Joint-Application-Development-Jane-Wood/dp/0471042994). Ils sont aussi utilisés en [Rapid Application Development (RAD)](http://www.amazon.fr/Rapid-Application-Development-James-Martin/dp/0023767758) ainsi que dans la méthode agile [DSDM](http://www.amazon.fr/DSDM-Dynamic-Systems-Development-Practice/dp/0201178893). Le développement piloté par les tests d’acceptation exploite de manière similaire les conversations en face-à-face dans les ateliers pour formaliser les exigences sous la forme de tests.

**L’ingénierie concurrente** : Les auteurs de [Concurrent Engineering Effectiveness](http://www.amazon.com/Concurrent-Engineering-Effectiveness-Integrating-Organizations/dp/1569902313) définissent l’ingénierie concurrente ainsi : “Il existe un tel lien étroit entre les participants lors du processus de développement d’un produit, qu’ils accomplissent leur travail à peu près en même temps.” Le moteur principal de l’ingénierie concurrente est le raccourcissement du temps de développement. Avoir des itérations de deux semaines c’est court, l’équipe doit trouver par conséquent une manière de travailler de façon concurrente - développer de façon séquentielle sur une itération aussi courte ne marche pas. Nous avons vu des équipes inventer des spécifications par l’exemple encore et encore, simplement parce qu’elles devaient répondre à la question “Comment pouvons-nous accomplir notre travail en même temps.”

**Plutôt prévenir que détecter** : Dans l’une des toutes premières études sur Toyota, [A Study of the Toyota Production System](http://www.amazon.fr/Study-Toyota-Production-System-Engineering/dp/0915299178), Singeo Shingo écrit : “L’objectif de l’inspection doit être la prévention ; toutefois, pour que l’inspection puisse avoir ce rôle, nous devons changer notre manière de penser.” De manière similaire, dans [“The Growth of Software Testing,”](http://www.clearspecs.com/downloads/ClearSpecs16V01_GrowthOfSoftwareTest.pdf), les auteurs identifient cinq périodes distinctes dans l’évolution du test logiciel. Ils nomment la dernière période “La période orientée prévention” et affirme “Poser des questions relatives aux tests … le plus tôt possible est souvent plus important pour la qualité logicielle et la réduction des coûts de développement que le passage des tests proprement dit.” C’est exactement ce que s’efforce de faire les spécifications par l’exemple. Lorsque des testeurs sont présents lors d’ateliers sur les exigences, ils peuvent poser des questions relatives aux tests, et de cette manière améliorer les exigences et prévenir les anomalies. Le mouvement Qualité Totale - influencé par Toyota et le développement du lean - promeut aussi la prévention plutôt que la détection.

Comment fonctionne l’A-TDD ? L’illustration ci-dessous permet d’en avoir un aperçu :

![Vue générale a-tdd]({{ site.url }}assets/less/a-tdd overview-fr.png)


## Aperçu du développement piloté par les tests d’acceptation

Le développement piloté par les tests d’acceptation se déroule en trois étapes :

1. Discuter des exigences au cours d’un atelier.
2. Développer ces exigences de façon concurrente au cours d’une itération.
3. Livrer les résultats aux parties prenantes pour acceptation


**Discuter** : La découverte des exigences est faite à travers de discussions lors des ateliers sur les exigences. Les participants d’un atelier sont les membres de l’équipe pluridisciplinaire, le Product Owner ou leurs représentants, ainsi que toute autre partie-prenante ayant potentiellement des informations sur les exigences. Une question type à poser lors de ce genre d’ateliers est “Imaginez le système à réaliser. Comment voudriez-vous l’utiliser et qu’est-ce que vous en attendriez ?”. Ce type de question donne comme résultats des exemples d’utilisation, et ces exemples peuvent être écrits sous la forme de tests d’exigences. L’objectif de l’atelier devrait être la discussion et la découverte des exigences plutôt que les tests en eux-mêmes.

**Développer** : À la fin de l’atelier, les exemples sont distillés en tests et l’ensemble des activités nécessaires à l’implémentation des exigences est fait de manière concurrente. Cela inclut :

* faire du code liant les tests et le système à tester (les “bibliothèques de tests” et les “tables bas-niveaux” dans Robot Framework ou les “fixtures” dans Fit)
* implémenter l’exigence de telle manière que le test passe
* mettre à jour l’architecture et toute documentation interne selon les conventions de travail propres à l’équipe
* écrire la documentation client des exigences
* faire des tests exploratoires complémentaires


La liste exacte dépend du produit, du contexte, des conventions de travail et de la [Définition du Fini (fr)](http://www.les-traducteurs-agiles.org/2017/10/29/less-la-definition-du-fini.html).

**Livrer** : Lors du passage des tests, les exigences sont revues avec le Product Owner et d’autres parties prenantes. De nouvelles exigences peuvent ainsi naître ou amener à des changements au niveau des tests existants.

L’illustration ci-dessous décrit plus en détails le développement piloté par les tests d’acceptation

![Vue détaillée a-tdd]({{ site.url }}assets/less/a-tdd in more details-fr.png)


Les étapes pour que les développements pilotés par les tests d’acceptation s’intègrent harmonieusement dans le cycle LeSS :

![Les étapes a-tdd]({{ site.url }}assets/less/a-tdd steps-fr.png)

Intégration des étapes du développement piloté par les tests d’acceptation dans le cycle itératif Scrum.

_Discuter en atelier_ : Avant de faire une Planification du Sprint détaillée, l’équipe, le Product Owner, et les autres parties prenantes clarifient les exigences de manière collaborative lors d’un atelier.

_Développer de manière concurrente_ : Les tâches permettant d’implémenter les tests/exigences sont créées lors de la Planification du Sprint détaillée et implémentées lors de l’itération. Toutes les activités se déroulent “à peu près en même temps”.

_Livrer pour acceptation_ : L’incrément opérationnel du produit — les tests d’acceptation passants — sont livrés pour acceptation aux parties prenantes et discutés avec tous lors de la Revue de Sprint.

## Discuter en atelier

Les expériences de ces ateliers sont profondément liées à celles citées dans le chapitre Exigences. Cette section couvre les sujets en rapport avec le développement piloté par les tests d’acceptation ; le chapitre Exigences couvre les ateliers sur les exigences plus en détails.

### Discuter en atelier lors de l’Affinage du Backlog de Produit

L’équipe et le Product Owner ‘inspecte’ le Backlog du Produit pendant l’[Affinage du Backlog Produit (fr)](http://www.les-traducteurs-agiles.org/2018/01/26/less-l-affinage-du-backlog-produit.html) pour s’assurer que ce dernier semble correct. Cette activité comprend les éléments suivants :

* Estimer et clarifier les nouveaux items ajoutés dans le Backlog du Produit
* Découper les gros items en plus petits en vue de les sélectionner pour implémentation.
* Clarifier les items imminents afin que l’équipe soit en mesure de les comprendre suffisamment pour les implémenter.


La clarification des items imminents peut être faite lors d’ateliers sur les exigences orientées A-TDD. Juste pour être clair, l’affinage du Backlog du Produit c’est non seulement des ateliers A-TDD sur les exigences mais cela peut aussi faire partie de l’activité d’affinage. D’autres activités possibles incluent l’estimation et le découpage.

### Clarifier plutôt qu’écrire des tests

L’A-TDD permet de clarifier collaborativement les exigences. L’emphase est mise sur la communication, la collaboration, et l’apprentissage à travers des exemples et des tests. L’approfondissement de la compréhension est l’objectif, les tests sont les moyens d’y arriver. Le livre intitulé de manière tout à fait approprié [Bridging the Communication Gap](http://www.amazon.fr/Bridging-Communication-Gap-Specification-Acceptance/dp/0955683610) met en avant :

> [le développement piloté par les tests d’acceptation] n’est pas une technique de programmation : il s’agit d’une technique de communication rapprochant les personnes impliquées dans un projet informatique.


Les gens sont souvent préoccupés par avoir des livrables tangibles lors d’un atelier - les tests - et ils oublient les effets intangibles - la connaissance. La compréhension et la clarté des exigences sont les livrables clés d’un atelier sur les exigences ; les tests en sont l’expression.

Il ne s’agit pas d’une fausse dichotomie. Les tests sont importants et cette technique s’appelle le développement piloté par les tests d’acceptations. Sans tests, il s’agirait juste d’un atelier sur les exigences - mais cela permet d’éviter de confondre la fin avec les moyens.

### Exemples d’utilisation


> “Pouvez-vous me donner un exemple ?”


Cette question peut soudainement transformer une discussion vague et abstraite en une question claire et concrète. Lors de la discussion sur de nouveaux produits, les gens ont tendance à parler en termes abstraits et conceptuels. Ils débattent les uns avec les autres sans se comprendre - ils restent bloqués. Demander des exemples ramène la discussion à la réalité.

Par exemple, nous entendons des affirmations telles que “Le système doit se remettre des situations d’erreurs”. C’est plutôt vague, nous demandons donc des exemples qui vont modifier la discussion. Cela pourrait être “Lorsque nous débranchons le câble, le système ne devrait pas tomber en panne” - ce qui est plus concret et plus compréhensible. Les exemples sont aussi utilisés pour avoir davantage de clarifications, tels que, “Comment le système devra t’il se remettre si nous enlevons une unité du système lorsque celui-ci est en train de marcher ?”.

Les exemples ne sont pas seulement utiles pour clarifier les exigences mais aussi pour clarifier les manières de travailler. “Nous ne pourrons jamais automatiser tous nos tests !” est une phrase à laquelle nous devrions répondre par “Pouvez-vous me donner un exemple d’un test non-automatisable ?” et ainsi progressivement déplacer le sujet de la discussion du principe vers la pratique.

![Les exemples en a-tdd]({{ site.url }}assets/less/a-tdd examples-fr.png)

L’illustration ci-dessus montre les relations entre les exemples, les exigences et les tests. Lors des ateliers sur les exigences, l’utilisation des exemples pour élaborer les exigences et les transformer en tests.

### "N'optimisez" pas l’atelier sur les exigences

Alors que nous étions en train de discuter d’A-TDD avec un groupe produit important, ce dernier a noté, “Nous avons amélioré l’atelier d’A-TDD. Seules trois personnes y participent : le Product Owner, le Scrum Master, et un spécialiste de l’équipe”. Nous leur avons demandé comment les autres membres de l’équipe pourraient être en mesure comprendre les exigences afin de pouvoir les implémenter et la réponse fut “Le spécialiste leur dira”. Ils ont ‘optimisé’ l’atelier en réintroduisant le traditionnel transfert de connaissance analyste-équipe comme avant.

### Éviter d’utiliser des ordinateurs et des projecteurs lors d’un atelier

Les ordinateurs pompent l’énergie vitale des ateliers. Ils deviennent le centre de la discussion. À part pour vérifier certaines informations, éviter donc d’avoir le besoin d’‘optimiser l’atelier en travaillant directement sur ordinateur. À la place …

### Condenser le flux de travail en règles métiers

La clarification des exigences lors des ateliers commence souvent avec des concepts abstraits, et puis lorsque des exemples sont mis sur la table, la focale de la discussion se déplace vers des discussions sur le flux de travail - “Lorsque j’utilise le système, je fais l’étape un, puis l’étape deux, et je m’attends à obtenir comme résultat X.”.

Il peut arriver que ces exemples de flux de travail soient similaires à l’exception de quelques variations sur une ou deux étapes. Les tests des flux de travail contiennent des règles métiers cachées, qui peuvent être extraites et insérées dans un test orienté données. Cela recentre la discussion sur la clarification du domaine et permet de réduire la complexité en supprimant des détails superflus.

### Des tests sur les murs

L’endroit idéal pour les tests c’est sur le mur - euh, du moins avec un tableau blanc entre les tests et le mur. Ce qui est écrit ou dessiné sur le tableau blanc sont enregistrés à l’aide de photos. Après l’atelier, les tests peuvent être distillés et retranscrits dans un outil.

![Des tests sur les murs 1]({{ site.url }}assets/less/a-tdd testwall1.jpg)

&nbsp;  

![Des tests sur les murs 2]({{ site.url }}assets/less/a-tdd test-wall2.jpg)

### De l’utilisation du format table

Exprimer des règles métiers sous la forme de tables permet de les rendre plus compréhensibles et aident à trouver des cas manquants. Les tables encouragent la clarté de la réflexion. [David Parnas, expert en informatique est un promoteur de longue date](http://link.springer.com/chapter/10.1007/978-3-7091-6510-2_12#page-1) de l’utilisation des tables dans la documentation des exigences.


> [Lors de la documentation des exigences,] l’écriture, la compréhension et la découverte se déroulent en même temps … Les notations tabulaires sont d’une grande aide dans ce genre de situations. Tout d’abord nous déterminons la structure de la table, et nous nous assurons que les en-têtes de colonne couvrent tous les cas possibles, puis nous nous concentrons ensuite à compléter les différentes entrées de la table.


### De l’utilisation des tests de flux de travail

Récupérer les règles métiers et faire des tests pilotés par les données ne peut pas toujours se faire ni même s’avérer souhaitable. Certaines exigences s’avèrent tout simplement bien mieux exprimées sous la forme de l’exemple d’un flux de travail (un scénario comportant plusieurs étapes). Les tests des règles métiers pilotés par les données peuvent souvent être complétés par des exemples de flux de travail qui, en un certain sens, permettent de les relier.

Attention : lorsque la plupart de vos tests sont des tests de flux de travail, alors il est très probable que vous ayez manqué certaines règles métiers

### Agenda type d’atelier

Comment se structure un atelier A-TDD sur les exigences ? Nous suivons fréquemment l’agenda suivant :

1. _Introduction_ : le Product Owner accueille l’ensemble des participants et explique l’objectif de l’atelier.
2. _Sélection_ : l’équipe et le Product Owner sélectionnent les items du Backlog de Produit sur lesquels ils vont travailler.
3. _Tour d’horizon_ : le Product Owner ou un représentant fait un bref tour d’horizon des exigences sélectionnées
4. _Divergence_ : l’équipe se scinde en deux ou trois sous-groupes prenant chacun un item et qui chacun commence à écrire des exemples sur tableau blanc. Le Product Owner et les représentants tournent entre les sous-groupes.
5. _Fusion_ : les sous-groupes se réunissent et l’un après l’autre font part de leurs travaux à l’ensemble du groupe.
6. _Répétition_ : les cycles de divergences-fusion durent généralement de 30 à 45 minutes. Plusieurs cycles peuvent se dérouler lors d’un atelier.
7. _Conclusion_ : le Product Owner résume le travail. Puis, s’ensuit un court débriefing sur l’atelier.
8. _Distillation_ : les participants prennent des photos de l’ensemble des travaux et les posent dans un wiki. Ils peuvent également diffuser certains tests et les documenter sur leur outil d’A-TDD.

## Développer de manière concurrente

Après que les exigences aient été éclaircies, elles doivent être implémentées. Les différentes activités nécessaires à l’implémentation sont faites de manière concurrente. En même temps, l’équipe étoffe les tests tout en implémentant le code, en écrivant la documentation, en mettant à jour la description de la conception, et ainsi de suite.

### Distiller les tests

De nombreux exemples sont créés pendant l’atelier sur les exigences. Tous les exemples ne deviennent pas des tests - seuls les éléments essentiels des exigences sont distillés sous la forme de tests. Les éléments non essentiels ou en doublons sont écartés - ils ont rempli leurs rôles pendant l’atelier d’accroissement des connaissances.

Comment à partir des exemples en distiller des tests ? Voici quelques techniques :

* **Duplication** : Enlever tout élément en double au niveau des exemples en écrivant des tests sous différentes formes. Par exemple, un jeu de tests de flux de travail peut être fusionné en un test de règle métier. La plupart de ces opérations devraient se faire durant l’atelier.
* **Classe d’équivalence** — Certains exemples font partie de la même classe d’équivalence et donc un seul test peut s’avérer suffisant. La présence de testeurs spécialisés est tout spécialement bienvenue, étant donné que le partitionnement par classe d’équivalence est une technique de tests classique.
* **Acceptation** - Étant donné que tous les exemples ne sont pas d’égale importance, il convient de demander au Product Owner “Quels sont les exemples que vous voulez voir fonctionner à la fin de l’itération ?”

### Faites-vous accompagner de facilitateurs et de coachs spécialisées en A-TDD

L’A-TDD est facile à faire, et difficile à adopter. Cela exige de remettre en question des postulats ancrés profondément et des changements d’habitudes. Un coach (externe) ayant de l’expérience en A-TDD et en changements organisationnels s’avèrent souvent nécessaire pour l’adopter. Trouvez un coach.

Il est important de réaliser que les compétences d’un bon coach en A-TDD sont différentes de celles d’un bon coach en TDD. Le coaching en TDD est davantage technique, et davantage focalisé sur les développeurs, alors que l’A-TDD concerne toute l’équipe. En plus d’avoir des compétences techniques, un bon coach en A-TDD possède aussi d’excellentes compétences en facilitation d’ateliers.

### Utiliser un outil d’A-TDD

* FIT est sans doute le premier outil d’A-TDD. Il a été développé par Ward Cunningham en 2002. Les tests FIT consistent l’utilisation de tables HTML avec un morceau de code liant - appelé “fixture”. Micah et Bob Martin ont créé une extension à FIT appelée FitNesse permettant d’écrire les tables dans un wiki. FitNesse contient également Slim - un modèle d’exécution moins gourmand offrant une meilleure portabilité et une meilleure flexibilité pour explorer de nouvelles syntaxes de tests. Vous trouverez plus d’informations dans les ouvrages que nous vous recommandons à la fin de ce chapitre.
* Robot Framework vient à l’origine de Nokia Siemens Networks et a été développé par Pekka Klärck. Le code a été libéré en 2008. Robot partage certaines caractéristiques avec FIT, tel que les tests structures sous forme tabulaire et la présence de code permettant de lier les tables au système testé. Toutefois, il possède certaines fonctionnalités uniques comme les tables en couche (mots-clé utilisateur).
* Inspiré par les travaux de Dan North, Cucumber a été développé par Aslak Hellesøy. Il suit le format given/when/then (NdT : étant donné <un contexte>/lorsque <se produit un évènement/une action>/alors <il arrive telle ou telle chose/résultat>) pour décrire les exemples. Les tests Cucumber sont des phrases lisibles en texte brut.


### N’utilisez pas les outils conventionnels pour faire du développement piloté par les tests d’acceptation

Some product groups we worked with try to use their conventional test tools such as Lisp-based scripts or TTCN for A-TDD. This invariably fails. Why? A-TDD-style tests are created so that the Product Owner or user can read and understand the tests. But the test format—scripts—of these conventional tools are created for testers and are thus unsuitable for documenting requirements. It is nearly impossible to involve the Product Owner in writing examples using such tools.

Certains des groupes de produits avec lesquels nous travaillons essayent d’utiliser des outils de tests conventionnels tels que des scripts en Lisp ou des notations de tests et de contrôle de tests (NdT : pour plus d’informations sur ces notations consultez [https://fr.wikipedia.org/wiki/TTCN](https://fr.wikipedia.org/wiki/TTCN)) adapté à l’A-TDD. Tout cela échoue invariablement. Pourquoi ? Le style des tests pour l’A-TDD est fait afin que le Product Owner ou que l’utilisateur puisse lire et comprendre les tests. Mais le format de type des scripts des tests de ces outils conventionnels sont faits pour un testeur professionnel et s’avère donc inapproprié pour la documentation d’exigences. Il est presque impossible d’impliquer le Product Owner dans la rédaction d’exemples avec de tels outils.

### Mais à la place utilisez un outil dédié à l’A-TDD qui servira d’intermédiaire aux outils de tests conventionnels

Devez-vous abandonner tous les outils conventionnels de tests lorsque vous adoptez l’A-TDD ? Peut-être pas.

Un groupe de produits, dédié aux graphismes, avec lequel nous avons travaillé avait passé plusieurs années à mettre en place un langage de scripts afin d’automatiser leurs tests. Cela devrait leur prendre quelques années de plus pour développer du code permettant de faire le liant (bibliothèques de tests ou fixtures) entre le framework A-TDD et leur système en tests - d’ailleurs la majeure partie de ce code sera du même acabit que ce qu’ils ont pu faire avec leur langage de scripts.

Une alternative est de laisser le code faisant le liant d’englober leur langage de scripts et ainsi de réutiliser le travail déjà fait. Les outils conventionnels de tests ne sont pas nécessairement de mauvais outils, mais simplement ils fournissent le mauvais format - le mauvais langage - permettant d’avoir des spécifications exécutables.

## Livrer pour acceptation

Le code est implémenté et tous les tests passent. Et ensuite ? Le cycle d’A-TDD, comme celui de Scrum, renferme un cycle d’inspection-adaptation dans lequel les résultats sont livrés aux parties prenantes, qui en inspectent les effets à travers les tests et qui décident comment procéder - quelles exigences seront implémentées par la suite.

### Montrer les tests lors de la Revue de Sprint

Lors d’une Revue de Sprint, l’équipe démontre des progrès visibles au Product Owner en montrant ce qui a été produit lors de l’itération.

Nous avons travaillé avec certains groupes pour définir les étapes de la démo pendant la Planification du Sprint. Une équipe passait un temps disproportionné en préparation de démo. Un gaspillage total.

Lors de la Planification du Sprint, une alternative possible est de définir les exemples qui doivent passer et montrer les progrès en utilisant les tests lors de la Revue de Sprint.

## Ouvrages recommandés

* [Specification by Example](https://www.amazon.fr/Specification-Example-Gojko-Adzic/dp/1617290084) de Gojko Adzic. Ce livre aborde plusieurs études de cas de “spécifications par l’exemple”. Gojko a inventé ce terme afin de remplacer tous les précédents termes comme l’A-TDD.
* [Bridging the Communication Gap](https://www.amazon.fr/Bridging-Communication-Gap-Specification-Acceptance/dp/0955683610/) de Gojko Adzic. Ce livre précède l’ouvrage Specification by Example et se concentre plus particulièrement sur la clarification des exigences et sur les ateliers.
* [Acceptance Test Driven Development: An Overview](http://testobsessed.com/2008/12/acceptance-test-driven-development-atdd-an-overview/) par Elisabeth Hendrickson. Il s’agit ici d’un article de blog et d’un papier donnant une vue d’ensemble sur l’A-TDD avec un exemple détaillé de l’utilisation de Robot Framework.
* [Fit for Developing Software](https://www.amazon.fr/Fit-Developing-Software-Framework-Integrated/dp/0321269349) par Rick Mugridge et Ward Cunningham. Ce livre aborde plus particulièrement comment améliorer la communication des exigences à travers l’utilisation des tables Fit.
* [Robot Framework User Guide](http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html). Ce guide n’aborde pas en tant que tel l’A-TDD mais donne une excellent introduction sur l’outil Robot Framework.
* [Test-Driven .NET Development with FitNesse](https://www.amazon.fr/Test-Driven-NET-Development-FitNesse/dp/0955683602) de Gojko Adzic. Ce livre met moins l’emphase sur l’A-TDD et davantage sur FitNesse. Il offre néanmoins une bonne description de l’outil.


---
Auteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Source : [Titre_article_en_vo](url_article_en_vo)  
Date de parution originale : jj_MMMM_yyyy  

---
Traducteur : [Prénom_Nom](url_bio)  
Date de traduction : jj/mm/yyyy  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

---
layout: post
title:  "LeSS - Tests d'Acceptation"
date:   2019-01-08 00:01
published: true
tags:
- less
---

## Don’t confusing acceptance and user-acceptance test

## Ne confondez pas tests d'acceptation et tests d'acceptation utilisateur

In the ideal situation, acceptance test and user-acceptance test are the same, but… Agile development literature uses the term “acceptance tests,” where we use the term “customer-facing tests.” However, in traditional development, “acceptance test” often means “user-acceptance test,” which might be different. Avoid misunderstandings.

Dans l'idéal, les tests d'acceptation et les tests d'acceptation utilisateur sont identiques, mais … la littérature du développement Agile utilise le terme de « tests d'acceptation » là où nous utilisons le terme de « tests orientés utilisateur ». Toutefois, en développement traditionnel, les « tests d'acceptation » veulent souvent dire « tests d'acceptation utilisateur » ce qui pourrait s'avérer différents. Évitons donc les malentendus.

acceptance_vs_uat.png



UAT is a subset of acceptance tests

Illustration 1 : Les tests d'acceptation utilisateur sont un sous-ensemble des tests d'acceptation

The above figure expresses the relationship in a diagram. User-acceptance test (UAT) is a part of acceptance testing in agile development. But acceptance test might also include non-UAT tests such as traditional functional or system test created by the team.

L'illustration ci-dessus montre ce qui relie ces 2 types de tests. Les tests d'acceptation utilisateur (TAU) ne sont qu'une partie des tests d'acceptation en développement agile. Mais les tests d'acceptation peuvent aussi inclure des tests qui ne soient pas des tests d'acceptations utilisateur tel que les traditionnels tests fonctionnels ou les tests systèmes faits par l'équipe.

Ideally, all the acceptance testing—including UAT—is done within the iteration. However, getting the UAT in the iteration may be difficult because it requires active end-user involvement and not all customers are ready for that. In that case, UAT is excluded from the Definition of Done until the product group improves their relationship with the customer so that they can expand their Definition of Done.

Idéalement, tous les tests d'acceptation - y compris les tests d'acceptation utilisateurs - sont faits dans l'itération. Toutefois, faire les tests d'acceptation utilisateur dans l'itération peut s'avérer difficile parce que cela demande une implication active de l'utilisateur final et tous les utilisateurs finaux ne sont pas prêts à ça. Dans ce cas, les tests d'acceptation utilisateur sont exclus de la Définition du Fini jusqu'à ce que le groupe produit améliore sa relation avec l'utilisateur final afin qu'il puisse étendre sa Définition du Fini.

## Show tests in Sprint Review

## Montrer les tests en Revue de Sprint

In a [Sprint Review](https://less.works/less/framework/sprint-review.html), the team demonstrates visible progress to the Product Owner by showing the output of the iteration.

Lors d'une [Revue de Sprint](http://www.les-traducteurs-agiles.org/2017/08/30/less-la-revue-de-sprint.html), l'équipe montre des avancées visibles au Product Owner en montrant ce qui a été produit pendant l'itération.

We worked with some groups that defined the demo steps during the Sprint planning. The team would spend an inordinate amount of time in demo preparation. A complete waste.

Certains des groupes avec lesquels nous avons travaillé préparaient à l'avance les différentes étapes pendant la Planification de Sprint. Dans ces cas-là, l'équipe passe un temps démesuré en préparation de démo. Un véritable gâchis.

During [Sprint Planning](https://less.works/less/framework/sprint-planning-one.html), an alternative is to define the examples that need to pass and show the progress by using these tests in the Sprint Review.

Lors de la [Planification du Sprint](http://www.les-traducteurs-agiles.org/2017/03/09/less-la-planification-du-sprint-1ere-partie.html), une alternative possible est de définir les exemples passants et montrer l'avancement des travaux en utilisant ces tests lors de la Revue du Sprint.

## Use acceptance test-driven development

## Utiliser le développement piloté par les tests d'acceptation

[Acceptance test-driven development (A-TDD) or Specification by Example](https://less.works/less/technical-excellence/specification-by-example.html) is a collaborative requirements discovery approach where examples and automatable tests are used for specifying requirements—creating executable specifications. These are created with the team, Product Owner, and other stakeholders in requirements workshops.

[Le développment piloté par les tests d'acceptation (A-TDD) ou Spécifications par l'exemple](http://www.les-traducteurs-agiles.org/2018/02/10/less-specifications-par-l-exemple.html) est une approche collaborative de découverte des exigences dans laquelle des exemples et des tests automatisés sont utilisés pour spécifier les exigences, créant ainsi des spécifications exécutables. Elles sont créées conjointement par l'équipe, le Product Owner, et les autres parties prenantes lors d'ateliers d'exigences.  

---
Auteur : The LeSS Company B.V.  
Source : [Acceptance Testing](https://less.works/less/technical-excellence/acceptance-testing.html)  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Relecteur : [Fabrice Aimetti](http://www.fabrice-aimetti.fr/)  
Date de traduction : 09/01/2019  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

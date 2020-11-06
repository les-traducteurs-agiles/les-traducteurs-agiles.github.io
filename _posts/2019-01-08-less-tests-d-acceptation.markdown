---
layout: post
title:  "LeSS - Tests d'Acceptation"
date:   2019-01-09 00:01
published: true
tags:
- less
---

« [Portail LeSS](http://www.les-traducteurs-agiles.org/2016/12/26/portail-less.html) < [Portail Excellence Technique](http://www.les-traducteurs-agiles.org/2016/12/26/less-portail-excellence-technique.html)

## Ne confondez pas tests d'acceptation et tests d'acceptation utilisateur

Dans l'idéal, les tests d'acceptation et les tests d'acceptation utilisateur sont identiques, mais … la littérature du développement Agile utilise le terme de « tests d'acceptation » là où nous utilisons le terme de « tests avec les utilisateurs ». Toutefois, en développement traditionnel, les « tests d'acceptation » veulent souvent dire « tests d'acceptation utilisateur » ce qui pourrait s'avérer différents. Évitons donc les malentendus.

![Les tests d'acceptation utilisateur sont un sous-ensemble des tests d'acceptation]({{ site.url }}assets/less/Less-xacceptance_vs_uat-fr.png)

Illustration 1 : Les tests d'acceptation utilisateur sont un sous-ensemble des tests d'acceptation

L'illustration ci-dessus montre ce qui relie ces 2 types de tests. Les tests d'acceptation utilisateur (TAU) ne sont qu'une partie des tests d'acceptation en développement agile. Mais les tests d'acceptation peuvent aussi inclure des tests qui ne soient pas des tests d'acceptations utilisateur tel que les traditionnels tests fonctionnels ou les tests systèmes faits par l'équipe.

Idéalement, tous les tests d'acceptation - y compris les tests d'acceptation utilisateurs - sont faits dans l'itération. Toutefois, faire les tests d'acceptation utilisateur dans l'itération peut s'avérer difficile parce que cela demande une implication active de l'utilisateur final et tous les utilisateurs finaux ne sont pas prêts à ça. Dans ce cas, les tests d'acceptation utilisateur sont exclus de la Définition du Fini jusqu'à ce que le groupe produit améliore sa relation avec l'utilisateur final afin qu'il puisse étendre sa Définition du Fini.

## Montrer les tests en Revue de Sprint

Lors d'une [Revue de Sprint](http://www.les-traducteurs-agiles.org/2017/08/30/less-la-revue-de-sprint.html), l'équipe montre des avancées visibles au Product Owner en montrant ce qui a été produit pendant l'itération.

Certains des groupes avec lesquels nous avons travaillé préparaient à l'avance les différentes étapes de la démo pendant la Planification de Sprint. Dans ces cas-là, l'équipe passe un temps démesuré en préparation de démo. Un véritable gâchis.

Lors de la [Planification du Sprint](http://www.les-traducteurs-agiles.org/2017/03/09/less-la-planification-du-sprint-1ere-partie.html), une alternative possible est de définir les exemples passants et montrer l'avancement des travaux en utilisant ces tests lors de la Revue du Sprint.

## Utiliser le développement piloté par les tests d'acceptation

[Le développement piloté par les tests d'acceptation (A-TDD) ou Spécifications par l'exemple](http://www.les-traducteurs-agiles.org/2018/02/10/less-specifications-par-l-exemple.html) est une approche collaborative de découverte des exigences dans laquelle des exemples et des tests automatisés sont utilisés pour spécifier les exigences, créant ainsi des spécifications exécutables. Elles sont créées conjointement par l'équipe, le Product Owner, et les autres parties prenantes lors d'ateliers d'exigences.

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

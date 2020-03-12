---
layout: post
title:  "LeSS - Développement piloté par les tests (TDD)"
date:   2020-03-08 00:01
published: true
tags:
- less
---

<< [Portail LeSS](http://www.les-traducteurs-agiles.org/2016/12/26/portail-less.html) < [Portail Excellence Technique](http://www.les-traducteurs-agiles.org/2016/12/26/less-portail-excellence-technique.html)

## Qu'est-ce que le développement piloté par les tests ?

Le développement piloté par les tests est un style de développement qui guide la conception par l’introduction de tests développés sur des cycles courts :

1. Écrire un test.
2. Implémenter juste ce qu'il faut de code pour passer le test.
3. Refactorer le code afin qu'il soit propre

![Cycle TDD]({{ site.url }}assets/less/tdd-cycle-fr.png)

Dans un langage comme Java, ce cycle ne prend pas plus de 5 minutes. Dans des langages plus anciens, ayant des temps de compilation plus longs et moins d’outils de refactoring automatisés, ce cycle est plus long - 20 minutes probablement.

Est-ce que le développement piloté par les tests est différent dans le cadre du développement de produits de taille importante ? Non, car il s’agit d’une pratique individuelle de développeur, peu importe le nombre de personnes impliquées dans le développement. La quantité de code patrimonial/historique, les anciennes technologies et les développements dans l’embarqué ont un impact sur les tests unitaires et sur le développement piloté par les tests. En conséquence, la plupart des expérimentations de cet article sont en lien avec ces sujets.

### Un cycle TDD type devrait être …

**Court** : Le temps de traitement pour passer chaque test est court. Cela pourrait prendre 5 minutes par cycle.
**Rhythmique** : vous sentirez le rythme très distinctement - « rouge, vert, refactorer … rouge, vert, refactorer … »
**Incrémental** : vous saurez au fur et à mesure que vous écrirez et ferez passer de plus en plus de tests, que des fonctionnalités sont construites de manière incrémentale.
**Focalisé sur la conception** : avec une bonne connaissance des principes de conception logicielle, vous découvrirez que le développement piloté par les tests n’est pas une technique de tests mais une méthode pour concevoir du logiciel.
**Discipliné** : le TDD est une autre façon de développer du logiciel. Casser les vieilles habitudes « coder et corriger » pour adopter une nouvelle habitude exigera de la discipline et de la persévérance.


## Pourquoi le TDD ?

## Accompagner le TDD

### Recourir à des coachs en TDD

À la relecture du projet de livret d’accompagnement, l’un de nos clients a énoncé que nous devrions insister davantage sur l’aspect coaching. "L’une de nos erreurs a été de ne pas avoir fourni suffisamment de coaching" a-t-il dit. Bien que nous ayons été d’accord avec lui, nous lui avons fait remarquer que nous étions tous les deux des consultants et que nous offrions ce type d’accompagnement, ce conseil n’était donc pas très crédible. Nous aurions aussi bien pu mettre une pancarte "Essayez... Engagez-nous...". Par conséquent, nous minimisons le conseil d’avoir recours à des coachs.

Toutefois en ce qui concerne le développement piloté par les tests, nous ne pouvons que trop insister : engagez des coachs ! Adopter le TDD signifie désapprendre le développement traditionnel et réapprendre comment concevoir et coder. Nous rencontrons rarement des gens qui soient en capacité de l’adopter en autodidacte. La plupart des développeurs ont besoin d’un coach pour programmer avec eux en binôme pendant quelques jours ou quelques semaines. Le coach leurs rappelle constamment d’écrire les tests d’abord et de mettre de l’ordre dans le code, y compris le code des tests. Il les aide à appliquer le TDD et à refactorer leur véritable code.

Le développement piloté par les tests pourrait bien être la pratique agile la plus difficile à adopter, mais il s’agit aussi de l’une des plus grosses opportunités pour améliorer la qualité de la conception et du code. Engagez des coachs !

### Coachs internes et externes

Des coachs externes sont nécessaires lors de l’adoption de TDD car la compétence n’existe pas encore dans l’entreprise. Mais, avec le temps, la montée en compétence de coachs internes diminuent la dépendance vis-à-vis de coachs externes et en réduit le coût.

Ceci dit, nous avons assisté à plusieurs échecs quant à la mise en place de coachs internes. Voici quelques raisons de ces échecs :

Ceci dit, nous avons assisté à plusieurs échecs quant à la mise en place de coachs internes. Voici quelques raisons de ces échecs :

* Aucune structure n’était en place pour décider avec quelle équipe travailler et quand le faire.
* Aucun temps n’était accordé pour du coaching. Au lieu de cela il était demandé aux coachs internes de faire du développement « traditionnel ».
* Les développeurs étaient moins enthousiastes d’apprendre de coachs internes... vous n’êtes jamais prophète dans votre propre pays.
* Les compétences de coach n’étaient ni appréciées ni encouragées à être davantage développées. En conséquence de quoi, les coachs internes compétents partaient souvent pour devenir coach externe.

Choisissez les deux, du coaching interne et du coaching externe. Dépendre de l’un des deux uniquement est risqué mais les combiner peut conduire à de bons résultats.

## Développement piloté par les tests pour une meilleure architecture

Le TDD peut aider à améliorer l’architecture d’un système. Comment ?

Quand nous faisons de l’accompagnement, une demande d’assistante fréquente qui nous est adressée est d’aider à assouplir « l’architecture rigide » de notre client. Cela se réduit le plus souvent à des problèmes de couplages très étroits entre les composants, un problème assez répandu dans du code patrimonial/historique écrit sans TDD parce que le développeur d’origine n’avait pas essayé de tester le composant de manière isolé.

D’un autre côté, lorsqu’un développeur créé un nouveau composant (comme une classe) avec le TDD, ou refactore un composant patrimonial/historique pour être testable unitairement, il doit casser les dépendances de ce composant afin qu’il soit testable de manière isolé. Cela exige de faire une conception (ou un refacoring) orientée injection de dépendances et d’augmenter l’utilisation de mécanismes pour plus de flexibilité : interfaces, polymorphisme, schéma de conceptions, frameworks d’injection de dépendances, pointeurs de fonctions, etc.

De cette manière, le TDD encourage un couplage plus lâche, plus simple, une configuration plus simple, en somme, les qualités d’une bonne architecture.

---
Auteur : The LeSS Company B.V.  
Source : [Test-Driven Development](https://less.works/less/technical-excellence/test-driven-development.html)  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Relecteur : [Fabrice Aimetti](http://www.fabrice-aimetti.fr/)  
Date de traduction : 08/03/2020  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

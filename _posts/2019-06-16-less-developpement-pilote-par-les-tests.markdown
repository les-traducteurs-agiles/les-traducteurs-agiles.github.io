---
layout: post
title:  "LeSS - Développement piloté par les tests (TDD)"
date:   2019-06-16 00:01
published: false
tags:
- less
---

# Test-Driven Development

# Développement piloté par les tests (TDD)

## What Is Test-Driven Development

## Qu'est-ce que le développement piloté par les tests ?

Test-driven development is a development style that drives the design by tests developed in short cycles of:

Le développement piloté par les tests est un style de développement qui guide la conception par l'introduction de tests développés sur des cycles courts :

1.  Write one test.
2.  Implement just enough code to make it pass.
3.  Refactor the code so it is clean.

1. Écrire un test.
2. Implémenter juste ce qu'il faut de code pour passer le test.
3. Refactorer le code afin qu'il soit tout propre

![TDD Cycle](https://less.works/img/technical-excellence/xtdd.png.pagespeed.ic.T3VU6bNkTY.png)



In a language such as Java, this cycle is as short as five minutes. In older languages, with slower compilation and less automated refactoring support, this cycle is longer—perhaps twenty minutes.

Dans un langage comme Java, ce cycle ne prend pas plus de 5 minutes. Dans des langages plus anciens, ayant des temps de compilation plus longs et moins d'outils de refactoring automatisés, ce cycle est plus long - 20 minutes environ.

Is test-driven development different in large product development? No. It is an individual developer practice and the number of people in the development does not matter.  
The amount of legacy code, old technology, and embedded develop- ment does have an impact on unit testing and test-driven development. Therefore, most experiments in this section are related to these.

Est-ce que le développement piloté par les tests est différent dans le cadre du développement de produits de taille importante ? Non, car il s'agit d'une pratique individuelle de développeur peu importe le nombre de personnes impliquées dans le développement.
La quantité de code historique, les anciennes technologies et les développements dans l'embarqué ont un impact sur le test unitaire et sur le développement piloté par les tests.
En conséquence, la plupart des expérimentations de la présente section sont en lien avec ces sujets.

### A TDD cycle Should Be …

### Un cycle TDD type devrait être …

**Short**
The turnaround time for passing each test is short. It could take 5 mins per cycle.
**Rhythmic**
You’ll feel the rhythm distinctly - “red, green, refactor... red, green refactor...”
**Incremental**
You’ll know that as you write and pass more tests, working functionalities are being build up incrementally.
**Design-focused**
With good knowledge of software design principles, you’ll discover TDD is not a testing technique but a method of designing software.
**Disciplined**
TDD is a different way of developing software. To break the old habit of "code and fix" and to adopt a new habit will require discipline and persistence.

**Court**
Le temps de traitement pour passer chaque test est court. Cela devrait prendre 5 minutes par cycle.
**Rhythmique**
Vous sentirez le rythme très distinctement - « rouge, vert, refactorer … rouge, vert, refactorer … »
**Incrémental**
Vous saurez au fur et à mesure que vous écrirez et ferez passer de plus en plus de tests, que des fonctionnalités sont construites de manière incrémentale
**Focalisé sur la conception**
Avec une bonne connaissance des principes de conception logicielle, vous découvrirez que le développement piloté par les tests n'est pas une technique de tests mais une méthode pour concevoir du logiciel.
**Discipliné**
Le TDD est une autre façon de développer du logiciel. Casser les vieilles habitudes « coder et corriger » pour adopter une nouvelle habitude exigera de la discipline et de la persévérance


## Why TDD?

## Pourquoi le TDD ?

## Coaching TDD

## Coacher le TDD

### Use TDD Coaches

### Recourir à des coachs en TDD

When a client of ours reviewed a draft of the companion book, he mentioned that we ought to stress coaching more. “One of our mistakes is that we didn’t provide enough coaching,” he said. Though we agreed with him, we pointed out that since we are both consultants and provide such coaching, this advice would not be very credible. We might as well add an experiment “Try…Hire us.” Thus, we minimized the advice related to hiring coaches.

À la relecture du brouillon du livret d'accompagnement, l'un de nos clients a énoncé que nous devrions insister davantage sur l'aspect coaching. « L'une de nos erreurs a été de ne pas avoir fourni suffisamment de coaching » a-t-il dit. Bien que nous ayons été d'accord avec lui, nous lui avons fait remarquer que nous étions tous les deux des consultants et que nous offrions ce type d'accompagnement, ce conseil n'était donc pas très crédible. Nous aurions bien pu aussi bien mettre une pancarte « Essayez … Engagez-nous ». Par conséquent, nous minimisons le conseil d'avoir recours à des coachs.

But related to test-driven development, we cannot stress strongly enough: Hire coaches! Adopting TDD means unlearning traditional programming and relearning how to design and code. We rarely meet people who were able to adopt this by self-education. Most developers need a coach to pair-program with them for days or weeks. The coach constantly reminds them to write the tests first and to really clean up the code—including the test code. He helps them apply TDD and refactoring to their real code.

Toutefois en ce qui concerne le développement piloté par les tests, nous ne pouvons que trop insister : engagez des coachs ! Adopter le TDD signifie désapprendre le développement traditionnel et réapprendre comment concevoir et coder. Nous rencontrons rarement des gens qui soient en capacité de l'adopter en autodidacte. La plupart des développeurs ont besoin d'un coach pour programmer avec eux en binome pendant quelques jours ou quelques semaines. Le coach leurs rappelle constamment d'écrire les tests d'abord et de mettre de l'ordre dans le code - y compris le code de tests. Il les aide à appliquer le TDD et à refactorer leur véritable code.

Test-driven development might be the hardest agile practice to adopt, but it is also one of the biggest opportunities for improving the quality of the design and code. Hire coaches!

Le développement piloté par les tests pourrait bien être la pratique agile la plus difficile à adopter, mais il s'agit aussi de l'une des plus grosses opportunités pour améliorer la qualité de la conception et du code. Engagez des coachs !

### Internal and external coaches

### Coachs internes et externes

External coaches are needed when adopting TDD because the com- petence does not yet exist inside the company. But, over time, growing internal coaches reduces the dependence on externals and the cost of coaching.

Des coachs externes sont nécessaires quant à l'adoption de TDD car la compétence n'existe pas encore dans l'entreprise. Mais, avec le temps, la montée en compétence de coachs internes diminuent la dépendance vis-à-vis de coachs externes et en réduit le coût.

That said, we have seen several attempts fail to develop internal coaches. Some reasons:

Ceci dit, nous avons assisté à plusieurs échecs quant à la mise en place de coachs internes. Voici quelques raisons de ces échecs :

* No structure was in place to decide when and with which teams to work.
* No time was reserved for coaching. Instead the internal coaches were asked to do normal development.
* Developers were less eager to learn from internal coaches…you are never a prophet in your own land.
* Coaching skills were not appreciated and further developed. The result is that skilled internal coaches often leave to be an external coach.

* Aucune structure n'était en place pour décider avec quelle équipe travailler et quand le faire.
* Aucun temps n'était accordé pour du coaching. Au lieu de cela il était demandé aux coachs internes de faire du développement « traditionnel ».
* Les développeurs étaient moins enthousiastes d'apprendre de coachs internes … vous n'êtes jamais prophète dans votre propre pays.
* Les compétences de coach n'étaient ni appréciées ni encouragées à être davantage développées. En conséquence de quoi, les coachs internes compétents partaient souvent pour devenir coach externe.

Choose both internal and external coaching. Depending on either of them alone is risky but combining them can lead to good results.

Choisissez les deux, du coaching interne et du coaching externe. Dépendre de l'un des deux uniquement est risqué mais les combiner peut conduire à de bons résultats.

## Test-driven development for a better architecture

## Développement piloté par les tests pour une meilleure architecture

TDD can help improve the architecture of a system. How?

Le TDD peut aider à améliorer l'architecture d'un système. Comment ?

When we are coaching, a frequent request is help for dealing with our client’s “inflexible architecture.” This most often boils down to problems in high coupling between components—a common problem in legacy code written without TDD because the original developer did not try to test the component in isolation.

Quand nous faisons de l'accompagnement, une demande d'assistante fréquente qui nous est adressée est d'aider à assouplir « l'architecture inflexible» de notre client. Cela se réduit le plus souvent à des problèmes de couplages très étroits entre les composants - un problème assez répandu dans du code ancien écrit sans TDD parce que le développeur d'origine n'avait pas essayé de tester le composant de manière isolé.

On the other hand, when a developer creates a new component (such as a class) with TDD, or refactors a legacy component to be unit-testable, they must break the dependencies of that component so that it is testable in isolation. That requires designing (or refactoring) for dependency injection and increased use of mechanisms for flexibility: interfaces, polymorphism, design patterns, dependency injection frameworks, function pointers, and more.

D'un autre côté, lorsqu'un développeur créé un nouveau composant (comme une classe) avec le TDD, ou refactore un composant historique pour être testable unitairement, il doit casser les dépendances de ce composant afin qu'il soit testable de manière isolé. Cela exige de faire une conception orientée injection de dépendances et d'augmenter l'utilisation de mécanismes pour plus de flexibilité : interfaces, polymorphisme, schéma de conceptions, _framework_ d'injection de dépendances, pointeurs de fonctions, etc

In this way, TDD encourages lower coupling and simple, flexible configuration—qualities of a good architecture.

De cette manière, le TDD encourage un couplage plus lâche, plus simple, une configuration plus simple - en somme, les qualités d'une bonne architecture.

---
Auteur : The LeSS Company B.V.  
Source : [Test-Driven Development](https://less.works/less/technical-excellence/test-driven-development.html)  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 06/03/2020  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

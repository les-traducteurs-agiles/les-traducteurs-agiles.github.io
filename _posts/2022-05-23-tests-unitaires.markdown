---
layout: post
title:  "Tests unitaires"
date:   2022-05-23 20:52
published: false
tags:
- less
---

## What Is Unit Test?

## Qu'est-ce que les tests unitaires ?

**Unit Test**s are software programs written to exercise other software programs (called **Code Under Test**, or **Production Code**) with **specific** preconditions and verify the **expected behaviour**s of the CUT.

**Les tests unitaires** sont des programmes informatiques écrits pour exercer d'autres programmes (que l'on peut appeler **Code en test**, ou **Code en Production**) à l'aide de pré conditions **spécifiées** et ainsi vérifier le comportement attendu du code testé.

Unit tests are usually written in the same programming language as their code under test.

Les tests unitaires sont généralement écrits dans le même langage de programmation que le code testé.

Each **unit test** should be small and test only limited piece of code functionality. Test cases are often grouped into **Test Groups** or **Test Suites**. There are many open source **unit test framework**s. The popular ones usually follow an **xUnit** pattern invented by [Kent Beck](http://c2.com/cgi/wiki?KentBeck "Kent Beck"), for example, JUnit for Java and CppUTest for C/C++.

Chaque **test unitaire** devrait être de taille réduite et ne devrait tester qu'une fraction limitée du code de la fonctionnalité. Les cas de tests sont souvent regroupés en **Groupes de tests** ou en **Suites de tests**. Il existe de nombreux **_frameworks_ de tests unitaires**. Les plus populaires, comme par exemple JUnit pour le langage Java et CppUTest pour les langages C/C++, suivent un schéma dénommé **xUnit** inventé par [Kent Beck](http://c2.com/cgi/wiki?KentBeck "Kent Beck").

Unit tests should also run very fast. Usually, we expect to **run hundreds of unit test cases within a few seconds**.

Les tests unitaires devraient aussi s'exécuter très rapidement. Généralement, on s'attend à ce qu'**une centaine de cas de tests unitaires s'exécute en quelques secondes**.

## Why Unit Test

## Pourquoi des tests unitaires

The purpose of unit testing is not for finding bugs. It’s a **specification** for the expected behaviours of the code under test. The code under test is the implementation for those expected behaviours. So unit test and the code under test are used to check the correctness of each other, and protect each other. Later when someone changed the code under test, and it changed the behaviour that is expected by the original author, the test will fail. If you code is covered by reasonable unit test, you can maintain the code without breaking the existing feature. That’s why Michael Feathers define **legacy code** as _code without unit test_.

L'objectif du test unitaire n'est pas de trouver des anomalies. Le test unitaire est une **spécification** des comportements attendus du code en test. Le code testé est l'implémentation de ces comportements attendus. Donc les tests unitaires et le code testé sont utilisés pour vérifier l'exactitude de l'un par rapport à l'autre et se protègent ainsi mutuellement. Si quelqu'un change le code en test, et que cela change le comportement attendu par l'auteur originel, le test échouera. Si votre code est couvert par un test unitaire cohérent, vous pouvez maintenir le code sans casser la fonctionnalité existante. C'est pourquoi Michael Feathers définit le **code hérité** comme du _code sans test unitaire_.

![](https://less.works/img/technical-excellence/xunit_test.png.pagespeed.ic.U9rHA2rtat.webp)

The purpose for unit testing is rather protect what we have implemented than to find any defects, just like the anchors set by a rock climber along his way up the rock. These anchors help him to protect what he has achieved.

Le but du test unitaire est plutôt de protéger ce que nous avons implémenté que de trouver des anomalies, tout comme les pitons mis par un grimpeur le long de son ascension. Ces pitons sont là pour l'aider à sécuriser le parcours qu'il a déjà accompli.

### Purpose of Unit Test

### Objectif du test unitaire

The purpose of unit test can be summarised as:

L'objectif du test unitaire peut être résumé ainsi :

- Facilitates changes
    - It protects the behaviours decided by the previous programmers. So that people can change the code without breaking the existing features.

- Faciliter les changements
  - Le test unitaire fait en sorte de protéger les comportements décidés par développeurs qui ont précédés afin qu'il soit possible de changer le code sans casser les fonctionnalités existantes.

- Simplifies integration
    - Unit test tests the basic units of the program, the functions and the classes. It makes sure the basic units are functioning as expected. When these units are integrated together, we can separate the integration problems (the coupling problems) from the unit internal problems (the cohesion problems).

- Simplifier l'intégration
  - Le test unitaire teste les unités de base du programme, autrement dit les fonctions et les classes. Le test unitaire fait en sorte de sécuriser les briques élémentaires pour qu'elles fonctionnent comme prévu. Lorsque ces unités de base sont intégrées ensemble, nous pouvons séparer les problèmes d'intégration (les problèmes de couplage) des problèmes internes des unités de base (les problèmes de cohésion).

- Documentation
    - Well-written unit test can be used as documentation for the functionality of the code under test. Unit test contains information typically you cannot find from the code under test, for example, the design purpose of the original programming who wrote the code, and how the code is expected to be used. Unit test as documentation, unlike other traditional documentation, it doesn’t “lie”. Because if it lies, the test would fail. And that indicates either the test or the code is wrong.

- Documentation
  - Des tests unitaires bien écrits peuvent être utilisés comme documentation vis-à-vis de la fonctionnalité du code en test. Le test unitaire contient une information que vous ne pouvez pas trouver dans le code testé, comme par exemple, quel est l'objectif de la conception du développeur originel de ce code, et comment le code est censé se comporter lors qu'il est utilisé. Le test unitaire, à la différence de la documentation traditionnelle, ne « ment » pas. Car si le test unitaire ment, le test viendrait à échouer. Et dans ce cas, cela indique que soit le test soit le code est erroné.

- Design tool
    - Unit test is also an important design tool. Unit test requires testability from the code understand. Easy-to-test usually means easy-to-use. So unit test could be used to make sure the design has consideration from the perspective of use, rather than only from the perspective of implementation. Testable code needs better modularity and fewer dependencies. So that the unit test can easily take a small part of the code under test (a “unit”) without taking care of the overwhelming amount of dependencies. So unit test could be used to make sure the design has “high cohesion, low coupling”.

- Outil de conception
  - Le test unitaire est aussi un outil de conception. Pour que le test unitaire remplisse son rôle, il est nécessaire d'appréhender la testabilité du code. Facile à tester veut généralement dire facile à utiliser. Cela veut dire que le test unitaire peut être utilisé pour que la conception se fasse du point de vue de l'utilisation et non seulement du point de vue de l'implémentation. Un code testable a besoin d'une plus grande modularité et de moins de dépendances. Le test unitaire peut donc facilement prendre une petite partie du code testé (un « unitaire ») sans avoir à se soucier de la quantité impressionnante de dépendances qu'il pourrait y avoir. Par conséquent, le test unitaire peut être utilisé pour s'assurer que la conception ait comme caractéristique « une forte cohésion, un faible couplage ».

### Why on “Unit” Level?

### Pourquoi à un niveau « unitaire » ?

“Yes, it’s important to use automated test to protect the existing functionalities. But why does it need to be on the unit level?”

« Oui, c'est important d'utiliser les tests automatisés pour de protéger les fonctionnalités existantes. Mais pourquoi cela doit-il être fait au niveau des tests unitaires ? »

You might wonder. Why don’t we just use thorough automated functional or system tests to protect the program?

Vous pourriez vous interroger. Pourquoi n'utilisons-nous tout simplement des tests fonctionnels automatisés ou des tests systèmes automatisés tout le temps pour protéger le programme ?

**Total cost of ownership** – Unit test is based on the abstraction level of the programming language. It’s just some code exercising other code. It doesn’t need to run in the same environment as the production. For compiled programming language, it doesn’t even need to use the same compiler as the production. The creating and running cost of unit test is very low. If designed properly, the cost of maintaining is also very low. You may not get the same level of confidence from one successful unit test case as you can get from a functional test. You will need many small unit test cases to get approximately the same level of confidence. But the cost of these small unit test cases is still much lower than owning a few functional test cases.

**Le coût total de possession** — Le test unitaire se base sur le niveau d'abstraction du langage de programmation utilisé. Il s'agit juste d'un bout de code qui va s'exécuter sur un autre bout de code. Il n'a pas besoin de s'exécuter sur le même environnement que celui en production. Pour un langage compilé, il n'est même pas nécessaire d'utiliser le même compilateur que celui en production. Le coût de la création et l'exécution est très faible. S'il est conçu correctement, le coût de maintenance est aussi très faible. Vous pouvez ne pas avoir le même niveau de confiance d'un cas de test unitaire qui s'est exécuté avec succès que pour un cas de test fonctionnel. Vous pourriez  avoir besoin de plusieurs cas de test unitaire pour avoir le même niveau de confiance. Mais le coût de tous ces petits cas de test unitaire restent tout de même plus faible que celeui de quelques cas de test fonctionnel.

If a software code base hasn’t got any unit test for the past 2 years, there will be extra cost for applying unit test to this code base. The cost comes mostly from two sources:

Si la base de code n'a pas eu de test unitaire dans les deux dernières années, il y aura un coût supplémentaire pour appliquer un test unitaire à cette base de code. Ce coût a deux sources principales :

1. The cost of applying a test framework to the code project. This is relatively easier for dynamic programming languages like Python, Ruby or Javascript. Usually, it’s also trivial for Java and C# project. It can be quite tricky for C/C++ project. No matter easy or hard, this is just one-time investment.

1. Le coût d'application d'un cadre de test sur le code du projet. Cela est relativement plus facile pour les langages de programmation dynamique comme Python, Ruby ou Javascript. De manière générale, c'est également trivial dans des projets Java ou C#. Cela peut être assez compliqué dans un projet C/C++. Que ce soit facile ou difficile, c'est un investissement à ne faire qu'une seule fois.

2. The existing code base is not testable. The code was designed without considering the testability. Applying unit test to this kind of code base often involves improving the current design. Doing so doesn’t only increase the cost of creating test, but also has potential cost of introducing new bugs by changing the design. So applying unit test to existing code base should be combined with other works that need the change from the code under test – when you have to change that piece of code regardless.

2. La base de code existante n'est pas testable. Le code a été conçu sans prendre en compte la testabilité. Appliquer des tests unitaires à ce type de base de code implique souvent d'améliorer la conception existante. Faire cette amélioration implique non seulement une augmentation du coût de la création des tests, mais a aussi un coût potentiel d'introduire de nouvelles anomalies en changeant cette conception. Aussi l'introduction de tests unitaires à une base de code existante devrait être combinée avec d'autres travaux qui nécessiteront le changement du code testé — lorsque vous devez changer ce morceau de code de toute façon.

**Internal Quality vs. External Quality** – High level automated test like functional test and system test checks the external quality of the software. External quality means how well the software is functioning according to the requirement. Unit test is not as effective as the functional test in protecting the external quality. On the other hand, unit test ensures some of the internal qualities of the software. Internal quality here means the testability of the code and how well the code is protected. A testable design is in general a good design. Other levels of automated test cannot serve this purpose as well as unit test.

**Qualité interne vs. qualité externe** — Les tests automatisés de haut niveau comme les tests fonctionnels et les tests systèmes permettent de vérifier la qualité externe du logiciel. La qualité externe signifie à quel point fonctionne le logiciel par rapport aux exigences. Les tests unitaires ne sont pas aussi efficients que les tests fonctionnels pour protéger la qualité externe. D'un autre côté, les tests unitaires s'assurent des qualités internes du logiciel. La qualité interne ici veut dire la testabilité du code et à quel point le code est protégé. Une conception testable reflète en général une bonne conception. D'autres types de tests automatisés ne permettent pas de remplir ce rôle aussi bien que les tests unitaires.

**Quality of feedback** When you passed a functional test, you could be very confident about the functionality you just tested. But when you found it fail, usually you need to do some debugging to see what is wrong. Unit test might be able to give you more precise information about what is working and what is broken.

**Qualité du _feedback_** Après avoir passé un test fonctionnel, vous pourriez être très confiant

Unit test is on the abstraction level of the programming language. When running unit test, everything should happen just within the CPU and memory. And each test case should be small. Therefore, it should run very fast. Typically, you should be able to run hundreds of unit tests within a few seconds. Including the compiling or other preparation time, the whole process of running unit test should take less than 1 minute.



Unit test should also be repeatable. If nothing changes, unit test runs should always return the same result.



If the unit test is very fast and repeatable, programmers can run it as often as they want, e.g. every a few minutes. The unit test will continuously provide quality feedback to the programmer. So that the programmer can go with a steady progress and focus on more important things rather than spending too much energy on trivial issues.



![](https://less.works/img/technical-excellence/xtest_levels.png.pagespeed.ic.-xbOy_tP-P.png)



A reasonable automated test structure should be like a pyramid. At the bottom are a lot of unit test cases. In the middle are much fewer integration level test cases. On the top, there are even fewer functional/system level tests.



## Common Misconceptions of Unit Test



### Unit test is not as important as the production code



It is true that in the end, it’s production code that makes the product. But most software products have evolutionary life cycles. The code is not static. It changes over time. Code without unit test does not have the necessary protection when being changed. Unit test also contains important information that is not included in the production code.



So unit test is just as important as the production code. They should be **in the same SCM repository**. They should follow the same coding standard as the production code.



### Unit Test is done by testing engineers



The purpose of unit test is not for finding bugs. Technically, it _checks_ rather than _tests_ if the code under test has implemented the behaviour intended by the programmer who designed it. So the reasonable choice is just let the same programmer writes both the test and the code under test.



It’s also encouraged to have two or more people pair up to do the programming together. They write the unit test and the code under test together. There are many fun ways of _pair-programming_. You may find more information in the Test-Driven Development section.



### You can write unit test without changing the code under test



This is often not true. If the code doesn’t have good testability, you might still be able to write unit test for it technically. But the unit test written for non-testable code is usually very hard to maintain and understand. Therefore, it doesn’t make much sense to have it.



**The secret of unit test is not about writing test, but writing testable code under test.** We want testable code and easy test, which is a win-win. We don’t want non-testable code and hard-to-maintain code, which is a lose-lose.



### I can add unit test later



Well, try asking the rock climbers to set their anchors later.



![](https://less.works/img/technical-excellence/xunit_test.png.pagespeed.ic.U9rHA2rtat.webp)

## Good Unit Test Patterns



### No news is good news



If the test passes, it should just print OK (and perhaps some dots to show the progress). No other information.



![](https://less.works/img/technical-excellence/500xNxunit_test_success.png.pagespeed.ic.W3mg1FIwIC.png)

Rule of thumb:



> No human intervention should be needed to get ready for the test, running the test cases or checking the result.



And when it fails, it should provide precise information. The goal is to limit the amount of time you spend on debugging when the test fails.  
![](https://less.works/img/technical-excellence/342xNxunit_test_fail.png.pagespeed.ic.eM-9actgRz.png)



### Arrange, Act, Assert



A good pattern to follow in a unit test is “**AAA**”: **Arrange**, **Act** and **Assert**.



If you can easily find this pattern in each of your test cases, your tests should be easy to understand, and they should be fairly specific and to the point. One unit test case should test only one thing. Therefore, there should be only one set of AAA in one test case. A test case shouldn’t be very long (longer than 10 lines of code) if it follows the AAA pattern.



import unittest
class TestGroupForTextWrapping(unittest.TestCase):

    def test\_should\_have\_no\_wrapping\_when\_string\_length\_is\_5\_and\_line\_width\_is\_10(self):
        \# Arrange:  Arrange all necessary preconditions and inputs.
        wrapper = TextWrapper(width=10)

        \# Act:  Act on the object or method under test.
        wrapped = wrapper.wrap("a" * 5)

        \# Assert:  Assert that the expected results have occurred.
        self.assertEqual(\["a" * 5\], wrapped)



### Behaviour Driven Development (BDD) Style



Similar to the **AAA** pattern, the **BDD** style uses three other keywords to specify each test case: **Given**, **When** and **Then**. (You can also use **And** as another keyword.)



    Given The Text Wrapper's Width Defined As 10
    And Using '-' As Word Connector
    When The Wrapper Wrap Text Length is Less Than 10
    Then The Text Should Not Be Wrapped




As you can see, “given-when-then” maps to “arrange-act-assert” pretty well. They both simply define a state transition of a Finite State Machine (FSM). You can find more on this in the [Uncle Bob’s article](https://sites.google.com/site/unclebobconsultingllc/the-truth-about-bdd). Some differences:



- BDD is more “outside-in”, which means that it emphasises more the external behaviour
- With BDD, you need to define a **domain specific language** to write your test specifications. Because of this, usually you’ll need a different framework. One example for Python is [behave](http://pythonhosted.org/behave/).



### The Golden Rule Of a Unit Test



In general, a good rule for unit test case is:



> **Each unit test case should be very limited in scope.**



So that:



- When the test fails, no debugging is needed to locate the problem.
- Tests are stable because dependencies are simple.
- Less duplication, easier to maintain.



There is no secret to write good unit test. In order to write good unit test, you need to create easy-to-test design.




---
Auteur : [Prénom_Nom](url_bio)  nbsp
Source : [LeSS - Unit Testing](http://less.works/less/technical-excellence/unit-testing.html)  nbsp
Date de parution originale : jj_MMMM_yyyy  nbsp

---
Traducteur : [Prénom_Nom](url_bio)  nbsp
Date de traduction : jj/mm/yyyy  nbsp

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

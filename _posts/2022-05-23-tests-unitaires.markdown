---
layout: post
title:  "LeSS - Tests unitaires"
date:   2022-06-29 00:01
published: true
tags:
- less
---

« [Portail LeSS](http://www.les-traducteurs-agiles.org/2016/12/26/portail-less.html) < [Portail Excellence Technique](http://www.les-traducteurs-agiles.org/2016/12/26/less-portail-excellence-technique.html)

## Que sont les tests unitaires ?

**Les tests unitaires** sont des programmes informatiques écrits pour
éprouver d'autres programmes (qui peuvent être désignés sous
l'appellation **Code sous tests**, ou **Code en Production**) à l'aide
de pré-conditions **spécifiques** et ainsi en vérifier le comportement
attendu.

Les tests unitaires sont généralement écrits dans le même langage de
programmation que le code testé.

Chaque **test unitaire** devrait être de taille réduite et ne devrait
tester qu'une fraction du code de la fonctionnalité. Les cas de tests
sont souvent regroupés en **Groupes de tests** ou en **Suites de
tests**. Il existe de nombreux ***frameworks* de tests unitaires**. Les
plus populaires, comme par exemple JUnit pour le langage Java et
CppUTest pour les langages C/C++, suivent un schéma dénommé **xUnit**
inventé par [Kent Beck](http://c2.com/cgi/wiki?KentBeck).

Les tests unitaires devraient aussi s'exécuter très rapidement.
Généralement, on s'attend à ce qu'**une centaine de cas de tests
unitaires s'exécutent en quelques secondes**.

## Pourquoi faire des tests unitaires ?

L'objectif du test unitaire n'est pas de trouver des anomalies. Le test
unitaire est une **spécification** des comportements attendus du code
sous test. Le code sous test est l'implémentation de ces comportements
attendus. Donc les tests unitaires et le code sous test sont utilisés
pour vérifier l'exactitude de l'un par rapport à l'autre, ils se
protègent ainsi mutuellement. Si quelqu'un change le code sous test, et
que cela change le comportement attendu par l'auteur originel, le test
échouera. Si votre code est couvert par un test unitaire cohérent, vous
pouvez maintenir le code sans casser la fonctionnalité existante. C'est
la raison pour laquelle Michael Feathers définit le **code
hérité/patrimonial** comme étant du *code sans test unitaire*.

![Test XUnit]({{ site.url }}assets/less/xunit_test_fr.png)

Le but du test unitaire est donc avant tout de protéger ce que nous
avons implémenté plutôt que de trouver des anomalies, tout comme les
pitons posés par un grimpeur le long de son ascension. Ces pitons sont
là pour l'aider à sécuriser le parcours qu'il a déjà accompli.

### Objectif du test unitaire

L'objectif du test unitaire peut être résumé ainsi :

-   Faciliter les changements
    -   Le test unitaire fait en sorte de protéger les comportements
        décidés par les développeurs qui se sont succédé afin qu'il
        soit possible de changer le code sans casser les fonctionnalités
        existantes.
-   Simplifier l'intégration
    -   Le test unitaire teste les unités de base du programme,
        autrement dit les fonctions et les classes. Le test unitaire
        fait en sorte de sécuriser les briques élémentaires pour
        qu'elles fonctionnent comme prévu. Lorsque ces unités de base
        sont intégrées ensemble, nous pouvons séparer ainsi les
        problèmes d'intégration (les problèmes de couplage) des
        problèmes internes des unités de base (les problèmes de
        cohésion).
-   Documentation
    -   Des tests unitaires bien écrits peuvent servir de documentation
        de la fonctionnalité du code sous test. Le test unitaire
        contient des informations que vous ne pouvez pas trouver dans le
        code testé, comme par exemple, l'objectif de la conception du
        développeur à l'origine du code, et de quelle manière le code
        est censé se comporter à l'exécution. Le test unitaire, à la
        différence de la documentation traditionnelle, ne \"ment\" pas.
        Parce que si le test unitaire ment, le test viendrait à échouer.
        Et dans ce cas, cela indique que le test ou le code est erroné.
-   Outil de conception
    -   Le test unitaire est aussi un outil de conception. Le test
        unitaire exige que le code soit testable dès sa conception.
        \"Facile à tester\" veut généralement dire \"facile à
        utiliser\". Cela signifie que le test unitaire peut être utilisé
        pour que la conception soit faite du point de vue de
        l'utilisation et non uniquement du point de vue de
        l'implémentation. Un code testable doit être davantage modulaire
        et avoir moins de dépendances. Ainsi, le test unitaire peut
        facilement ne concerner qu'une petite partie du code testé (un
        \"unitaire\") sans avoir à se soucier de la quantité
        impressionnante de dépendances qu'il pourrait y avoir. Par
        conséquent, le test unitaire peut être utilisé pour s'assurer
        que la conception ait comme caractéristique \"une forte
        cohésion, un faible couplage\".

### Pourquoi à un niveau « unitaire » ?

\"Oui, il est important d'utiliser des tests automatisés pour protéger
les fonctionnalités existantes. Mais pourquoi cela doit-il être fait au
niveau unitaire ?\"

Il est légitime de vous poser cette question. Pourquoi n'utilisons-nous
tout simplement pas de manière rigoureuse des tests fonctionnels
automatisés ou des tests systèmes automatisés pour protéger le programme
?

**Le coût total de possession** --- Le test unitaire se base sur le
niveau d'abstraction du langage de programmation utilisé. Il s'agit
juste d'un bout de code qui va tester un autre bout de code. Il n'a pas
besoin de s'exécuter sur le même environnement que celui en production.
Pour un langage compilé, il n'est même pas nécessaire d'utiliser le même
compilateur que celui en production. Le coût de la création et
l'exécution est très faible. S'il est conçu correctement, le coût de
maintenance est aussi très faible. Vous pouvez ne pas avoir le même
niveau de confiance pour un cas de test unitaire qui s'est exécuté avec
succès que pour un cas de test fonctionnel. Vous pourriez avoir besoin
de plusieurs cas de test unitaire pour avoir le même niveau de
confiance. Mais le coût de tous ces petits cas de test unitaire reste
malgré tout plus faible que celui de plusieurs cas de test fonctionnel.

Si le code source n\'a bénéficié d\'aucun test unitaire depuis les deux
dernières années, il y aura un coût supplémentaire pour lui en appliquer
un. Ce coût a deux origines principales :

1.  Le coût d'application d'un *framework* de test sur le code du
    projet. C\'est relativement plus facile pour des langages de
    programmation dynamique comme Python, Ruby ou Javascript. De manière
    générale, c'est aussi relativement trivial pour des projets Java ou
    C\#. Cela peut être toutefois assez compliqué pour un projet C/C++.
    Que ce soit facile ou difficile, c'est un investissement à ne faire
    qu'une seule fois.
2.  Le code source existant n'est pas testable car le code a été conçu
    au départ sans prendre en compte l'aspect testabilité. Appliquer des
    tests unitaires à ce type de code source implique souvent de devoir
    améliorer la conception existante. Mener cette amélioration implique
    non seulement une augmentation du coût concernant la création des
    tests, mais a potentiellement un autre coût qui est lié à
    l\'introduction de nouvelles anomalies en changeant ladite
    conception. Par conséquent, l'introduction de tests unitaires pour
    un code source existant se doit d'être combinée avec d'autres types
    de travaux qui nécessiteront des modifications dans le code sous
    test --- autrement dit lorsque le moment sera venu de changer ce
    morceau de code.

**Qualité interne vs. Qualité Externe** --- Les tests automatisés de
haut niveau comme les tests fonctionnels et les tests systèmes
contrôlent la qualité externe du logiciel. La qualité externe permet de
connaître le niveau de fonctionnement du logiciel par rapport aux
exigences. En effet, les tests unitaires ne sont pas aussi efficaces que
les tests fonctionnels pour protéger la qualité externe. Par contre, les
tests unitaires s'assurent de la qualité interne du logiciel. La qualité
interne veut dire ici la testabilité du code et permet de savoir jusqu'à
quel niveau le code est protégé. Une conception testable est synonyme en
général de bonne conception. D'autres types de tests automatisés ne
remplissent pas ce rôle aussi bien que les tests unitaires.

**Qualité du *feedback*** --- Après avoir passé un test fonctionnel,
vous pouvez être confiant vis-à-vis de la fonctionnalité testée. Mais
lorsque vous vous apercevez que le test échoue, vous devez généralement
faire du déboggage pour trouver ce qui est erroné. Les tests unitaires
peuvent vous donner une information plus précise sur ce qui fonctionne
ou ne fonctionne pas.

Les tests unitaires étant sur le même niveau d'abstraction que le
langage de programmation employé, tout devrait s'exécuter au niveau du
micro-processeur et de la mémoire lors de l'exécution du test unitaire.
Et comme chaque cas de test devrait être de petite taille, il devrait
donc s'exécuter très rapidement. Ainsi, vous devriez être en mesure
d'exécuter plusieurs centaines de tests unitaires en quelques secondes.
En prenant en compte le temps de compilation ou de préparation,
l'ensemble du processus d'exécution d'un test unitaire devrait prendre
moins d'une minute.

Les tests unitaires devraient aussi être répétables. Si rien ne change
d'une fois sur l'autre, l'exécution d'un test unitaire devrait toujours
retourner le même résultat.

Si un test unitaire est très rapide et répétable, les développeurs
peuvent l'exécuter aussi souvent qu'ils le veulent, par exemple toutes
les deux minutes. Le test unitaire fournira en permanence aux
développeurs des retours d'informations liés à la qualité. Cela
permettra ainsi aux développeurs d'avancer à un rythme régulier et de se
focaliser sur des choses plus importantes plutôt que de passer trop
d'énergie sur des choses triviales.

![Niveaux de test]({{ site.url }}assets/less/xtest_levels_fr.png)

Une structure de test automatisé acceptable devrait ressembler à une
pyramide. À la base de la pyramide, il y a un grand nombre de cas de
tests unitaires. Au milieu, des cas de tests d'intégration en moins
grand nombre. En haut, seulement quelques cas de tests fonctionnels ou
systèmes.

## Idées fausses à propos du test unitaire

### Le test unitaire n'est pas aussi vital que le code en production

Il est vrai qu'en fin de compte, c'est le code en production qui donne
vraiment vie au produit. Mais la plupart des produits logiciels ont des
cycles de vie évolutif. Le code n'est pas statique. Il change avec le
temps. Un code sans test unitaire n'est pas suffisamment protégé
lorsqu'une modification est faite. Le test unitaire contient aussi des
informations importantes qui ne sont pas présentes dans le code en
production.

Par conséquent le test unitaire est tout aussi important que le code en
production. Il devrait être stocké **dans le même dépôt de gestion du
code source**. Le test unitaire devrait d'ailleurs suivre les mêmes
conventions de codage que le code en production.

### Le test unitaire est fait par des ingénieurs tests

L'objectif du test unitaire n'est pas de trouver des anomalies.
Techniquement, il *vérifie* plutôt que *teste* si le code sous test a
implémenté le comportement voulu par le développeur qui l'a conçu. Donc
le choix logique est de simplement laisser la même personne écrire à la
fois le test et le code sous test.

Il est aussi encouragé d'avoir deux ou plusieurs personnes travaillant
de concert pour programmer à la fois le test et le code sous test. Il
existe plusieurs manières sympas pour programmer en binôme. Vous
trouverez davantage d'informations à ce sujet dans la section
développement piloté par les tests.

### Vous pouvez écrire des tests unitaires sans changer le code sous test

Ce n'est pas toujours le cas. Si le code n'a pas une bonne testabilité,
vous pourriez tout de même être capable techniquement d'écrire le test
unitaire qui va avec. Mais un test unitaire qui a été écrit pour un code
non-testable est généralement très difficile à maintenir et à
comprendre. Par conséquent, il n'y a pas vraiment de raison d'en avoir
un.

**Le secret du test unitaire n'est pas d'écrire du test, mais d'écrire
un code testable sous test.** Nous voulons du code testable et facile à
tester, ce qui s'avère une démarche gagnant-gagnant. Nous ne voulons pas
de code non-testable et difficile à maintenir, ce qui serait une
démarche perdant-perdant.

### Je peux ajouter les tests unitaires plus tard

Eh bien, essayez donc de demander à des grimpeurs de mettre leurs pitons
plus tard.

![Test XUnit]({{ site.url }}assets/less/xunit_test_fr.png)


## Schéma pour de bons tests unitaires

### Pas de nouvelles, bonnes nouvelles

Si le test passe, il devrait afficher seulement OK (voire quelques
points pour afficher son avancement). Aucune autre information n\'est
nécessaire.

![Test unitaire réussi]({{ site.url }}assets/less/unit_test_success.png)

Règle empirique :

> Aucune intervention humaine ne devrait être nécessaire pour préparer l’exécution du test, exécuter les cas de tests ou en vérifier les résultats.

Et lorsqu'un test unitaire échoue, il devrait nous fournir toutes les
informations nécessaires. L'objectif est de limiter la durée pendant
laquelle vous êtes occupé à débogguer le code concerné.

![Test unitaire échec]({{ site.url }}assets/less/342xNxunit_test_fail.png)

### Arranger, Agir, Auditer (*Arrange*, *Act*, *Assert*)

Un bon schéma à suivre en ce qui concerne les tests unitaires est
\"**AAA**\" : **Arrange (dans le sens de mettre en place)**, **Act (dans
le sens d'une action faite sur quelque chose)** et **Assert (dans le
sens de contrôler)**.

Si vous pouvez repérer ce schéma dans chacun de vos cas de tests, vos
tests devraient être facile à comprendre, et ils devraient s'avérer
suffisamment spécifiques et aller droit au but. Un cas de test unitaire
devrait tester une seule et unique chose. Par conséquent, il devrait y
avoir un seul AAA dans un cas de test. Un cas de test ne devrait pas
être très prolixe (c'est-à-dire plus de 10 lignes de code) s'il suit le
schéma AAA.

    import unittest class TestGroupForTextWrapping(unittest.TestCase):

    def test\_pas\_de\_retour\_à\_la\_ligne\_lorsque\_longueur\_de\_la\_chaîne\_de\_caractères\_de\_5\_et\_largeur\_de\_la\_ligne\_de\_10(self):
         \# Arrange :  Mettre en place toutes les préconditions nécessaires ainsi que les entrées.
         wrapper = TextWrapper(width=10)

         \# Act :  Agir sur l'objet ou sur la méthode sous test.
         wrapped = wrapper.wrap(&quot;a&quot; * 5)

         \# Assert :  Contrôle que le résultat attendu s'est bien produit.
         self.assertEqual(\[&quot;a&quot; * 5\], wrapped)

### Développement piloté par le comportement (BDD)

Identique au schéma **AAA**, le **BDD** utilise trois mots-clés
différents pour spécifier chaque cas de test : **Étant donné**,
**Lorsque** et **Alors**. (Vous pouvez aussi utiliser **Et** comme
mot-clé supplémentaire)

~~~~~~~~
Given / Étant donné que la longueur du texte pour le retour à la ligne
est défini à 10  

And / Et que le caractère \'-\' est utilisé comme
connecteur entre deux mots

When / Lorsque la longueur du texte est
inférieure à 10

Then / Alors le texte ne devrait pas être retourné à la
ligne`
~~~~~~~~

Comme vous pouvez le constater, le triptyque \"étant donné - lorsque -
alors\" s\'allie plutôt bien avec le triptyque \"Arrange - Act -
Assert\". Ils définissent tous les deux un état transition d'une machine
à état finie. Vous pouvez en savoir plus en consultant cet article
d'[Oncle
Bob](https://sites.google.com/site/unclebobconsultingllc/the-truth-about-bdd).
Voici quelques différences entre les deux :

-   Le BDD est davantage orienté \"dehors vers dedans\", cela veut dire
    qu'il met davantage l'accent sur le comportement externe
-   Avec le BDD, vous devez définir un **langage spécifique au domaine**
    pour écrire vos spécifications de tests. À cause de cela, vous aurez
    besoin généralement d'un *framework* supplémentaire. Par exemple,
    pour Python vous pourrez utiliser
    [behave](https://pypi.org/project/behave/).

### La règle d'or du test unitaire

De manière générale, une bonne règle d'or pour des tests unitaires
serait :

> **Chaque cas de test unitaire devrait comporter un périmètre très restreint.**

De telle manière que … :

-   Lorsque le test échoue, qu'il ne soit pas nécessaire de faire du
    déboggage pour localiser le problème.
-   Les tests soient stables car les dépendances sont limitées.
-   Il y ait moins de duplications, que ce soit plus facile à maintenir.

Il n'existe pas de secrets pour écrire un bon test unitaire. Afin
d'écrire un bon test unitaire, vous devez créer une conception qui soit
facile à tester.



---
Auteur : The LeSS Company B.V.  
Source : [LeSS - Unit Testing](http://less.works/less/technical-excellence/unit-testing.html)  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Relecteur : [Fabrice Aimetti](http://www.les-traducteurs-agiles.org/traducteurs/)
Date de traduction : 29/06/2022  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

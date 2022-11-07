---
layout: post
title:  "LeSS - Automatisation des tests"
date:   2022-11-06 00:01
published: true
tags:
- less
---

« [Portail LeSS](http://www.les-traducteurs-agiles.org/2016/12/26/portail-less.html) < [Portail Excellence Technique](http://www.les-traducteurs-agiles.org/2016/12/26/less-portail-excellence-technique.html)

## Tests manuels

Les développeurs agiles mettent en avant l'importance des tests
automatisés. En effet, avec des cycles courts, l'exécution manuelle des
tests de régression s'avère quasiment impossible. Cela signifie t-il
qu'il n'y a pas du tout de tests manuels ? Non. Certains tests manuels
sont toujours recommandés, même si ces tests diffèrent quelque peu des
tests manuels faits à l'aide de scripts.

### Automatiser les tests manuels

Les affirmations « Il est impossible d'automatiser des tests de pertes
de connexion réseau » ou « Il est impossible d'automatiser des tests
portant sur un problème matériel » reviennent souvent de la part des
groupes produits. Notre réponse est généralement « Non ce n'est pas
vrai » ou « Oui, vous pouvez faire ces types de tests. »

Elisabeth Hendrickson, l'auteur du mini-livre (vo) [*Exploratory Testing
in an Agile Context*](https://less.works/papers/et.pdf) ose d'ailleurs
dire

> Je pense que si vous êtes en mesure d'écrire un script de test manuel,
> c'est que vous êtes aussi en mesure de l'automatiser.

Il peut s'avérer difficile d'automatiser un test *exactement de la même
manière* que s'il était fait manuellement. Par exemple, il est quasiment
impossible de débrancher automatiquement un câble réseau pour un cas de
test de perte de connexion. Par conséquent, un test automatisé se fait
généralement de manière différente. À la place de débrancher
physiquement un câble, le test automatisé va instruire le pilote réseau
de répondre *comme si* le câble réseau avait été débranché.

Est-ce que ça vaut le coup d'automatiser tous les tests ? Selon
Elisabeth Hendrickson :

> Si un test est suffisamment important pour être scripté, et exécuté,
> il est alors suffisamment important pour être automatisé.

Pourquoi cela ? Le développement itératif et incrémental implique que le
code ne soit pas figé en fin d'itération mais qu'il ait, à la place de
cela, le potentiel d'être changé à chaque itération. Par conséquent,
faire du test de régression manuel signifierait ré-exécuter la majorité
des tests manuels à chaque itération. Il va sans dire que
l'automatisation s'avère rentable rapidement.

Cela s'avère être particulièrement vrai sur le développement à grande
échelle qui prône, entre autres, des équipes *features* et la propriété
collective du code, et pour lequel le filet de sécurité offert par les
tests automatisés est d'une importance capitale.

### Faire quelques tests manuels

Automatiser *tous* les tests pourrait ne pas valoir le coût voire même
ne pas être possible. Certains tests tels que ceux évoqués ci-dessous
devront alors être faits manuellement :

-   *Les tests nécessitant une appréciation et de la créativité de la
    part de quelqu'un*, c'est-à-dire d'une personne capable de juger si
    l'interface s'apprête bien à des tests d'utilisabilité. Les tests
    exploratoires, par définition, ont besoin de quelqu'un pour décider
    de la prochaine étape à explorer.
-   *Les tests nécessitant une action physique*, par exemple dans le cas
    de tests d'un système ayant des configurations matérielles
    différentes. Cela peut être automatisé par le biais de la
    simulation, mais la vraie configuration matérielle pourrait s'avérer
    nécessaire pour l'exécution du test final.
-   *Des tests coûteux par nature*. Par exemple, exécuter des tests de
    capacité en environnement de production peut s'avérer trop coûteux
    et par conséquent ne sont exécutés tout au plus qu'une ou deux fois
    au cours de la vie du produit. Toutefois, ces tests ne font que
    retarder le risque. Il est nécessaire de s'attaquer à ces risques le
    plus tôt possible avec des tests moins coûteux - par exemple, en
    exécutant des tests de capacité sur une simulation de
    l'environnement cible - cela permettra que l'exécution du vrai test,
    qui lui est coûteux, ne soit que la vérification finale.

Pas de fausse dichotomie : essayez d'automatiser tous les tests, mais
n'oubliez pas de faire des tests manuels lorsque c'est nécessaire.

### Faire des tests exploratoires {#faire_des_tests_exploratoires}

Dans son ouvrage *[Perfect Software and Other Illusions about
Testing](http://www.amazon.com/Perfect-Software-Other-Illusions-Testing/dp/0932633692)*,
Gérald Weinberg évoque : « l'idée reçue quant à l'exhaustivité des
tests, autrement dit il est possible de tout tester ! ». Ce n'est pas le
cas. Le nombre de scénarios possibles à tester est pour ainsi dire
infini et par conséquent automatiser tous les tests demanderait un
effort d'automatisation infini. Essayez donc plutôt d'automatiser les
tests déjà envisagés et consacrer du temps aussi efficacement que
possible sur les tests exploratoires pour trouver des cas de tests non
envisagés.

Vue globale du test exploratoire :

![Tests exploratoires]({{ site.url }}assets/less/et-fr.png)

Qu'est-ce que le test exploratoire ? Dans un de ses articles, James Bach
le définit comme étant « la combinaison de l'apprentissage, de la
conception de tests et de l'exécution de tests en simultané » --
[Bach03(vo)](http://www.satisfice.com/articles/what_is_et.shtml). Cela
vient en contraste avec le test scripté traditionnel dans lequel la
conception des cas de tests et l'exécution se font de manière séparée et
séquentielle avec d'abord la conception et après l'exécution. Le test
exploratoire a pour objectif d'utiliser le plus possible la créativité
humaine lors de l'exécution des tests, d'en tirer des informations et de
les utiliser pour prendre des décisions relatives à la conception des
tests. Cela sera plus clair à l'aide de l'exemple suivant :

Imaginons que Gina soit en train de tester une application de
modélisation 2D. Tout d'abord, elle commence par définir l'objectif de
sa session de test exploratoire que l'on appelle une mission ou une
charte. Sa charte est d' « Explorer les changements de formes en
déplaçant les points de contrôle ». Elle sélectionne une forme, la place
sur le canevas, et y ajoute deux points de contrôle. Elle déplace l'un
d'entre eux et observe ce qu'il se passe. En se basant sur ses
observations (apprentissage), elle détermine quelle sera la prochaine
étape (conception) et la réalise (exécution). La forme prend un nouvel
aspect même si elle remarque que lors du déplacement des points de
contrôle la forme a pris temporairement un nouvel aspect qu'elle
n'aurait probablement pas dû avoir. Aussi, elle continue à les déplacer
et à les déplacer jusqu'à ce qu'elle arrive à reproduire ce type de
transformation accidentelle.

Dans cet exemple, il n'y a pas de script détaillé préconçu ou de cas de
test mais plutôt un périmètre de test --- une charte. La première étape
est d'observer le système et à partir de cette observation de déterminer
l'action suivante à savoir la conception des tests. Toutes les
techniques traditionnelles de tests et toutes les heuristiques
traditionnelles de tests sont utilisées lors de cette phase de
conception.

Tests exploratoires
![Tests exploratoires]({{ site.url }}assets/less/et_scripted_difference-fr.png)

## Tests automatisés

### Créer des tests maintenables

« Les tests automatisés vont augmenter notre charge de maintenance des
tests » est une objection que nous entendons régulièrement. Il est
certain que la maintenance des tests vous coûtera un peu mais quelques
techniques simples peuvent minimiser ce coût :

-   supprimer toute duplication à l'intérieur et à l'extérieur des tests
-   supprimer les tests
-   ne pas tester à travers une IHM
-   exécuter les tests fréquemment

### Supprimer toute duplication à l'intérieur et à l'extérieur des tests

La duplication du code engendre un niveau de complexité, d'incertitude
et d'anomalies supplémentaires --- ayant pour conséquence un effort de
maintenance supplémentaire. C'est vrai tout autant pour le code de test
que pour le code en production. Vous pouvez vous éviter cela en
supprimant toute duplication de code qui serait présente.

Les flux de travail de tests sont une forme répandue de duplication. Ils
se présentent le plus souvent sous la forme d'un scénario parent avec
tout un ensemble de cas de tests dérivés avec par ici ou par là quelques
légères variations. Tous ces flux de travail de tests doivent être mis à
jour. Ce type de duplication peut être évité avec des tests pilotés par
les données qui se focalisent sur les règles métiers ou en séparant les
éléments dans des bibliothèques de tests ou des *fixtures*.

Nous avons accompagné une équipe qui avait fait une erreur assez
répandue au sein de beaucoup d'équipes --- elle avait repoussé
l'automatisation des tests à la fin de son itération. Il lui restait 4
jours avant la fin de l'itération et uniquement des tâches
d'automatisation à faire. Lors de son itération précédente, ces tâches
avaient été faites par un spécialiste des tests mais ces tâches devaient
être faites dorénavant par l'ensemble de l'équipe.

Nous avons fait démarrer l'équipe avec un atelier d'une journée au cours
duquel un spécialiste a formé et accompagné les différents membres de
l'équipe. Après cet atelier, l'équipe s'est scindée en plusieurs groupes
de deux personnes plus un groupe de trois personnes pour travailler sur
l'automatisation des tests. Quelque chose d'intéressant s'est produit :
les développeurs expérimentés de l'équipe se sont plaints du surcroit de
travail nécessaire à cause de la duplication présente dans les tests.
Avant ça, aucun d'entre eux ne l'avaient remarqué et le spécialiste des
tests --- qui n'avait pas beaucoup d'expérience en programmation --- ne
s'en était jamais soucié. Maintenant que toute l'équipe était impliquée,
tout le monde s'en souciait et la qualité des tests s'est alors
grandement améliorée.

### Supprimer des tests lorsqu'ils n'apportent aucune valeur

Les tests servent plusieurs objectifs. Ils servent d'exigences, de
vérifications et font aussi office de filet de sécurité pour prévenir la
régression du système.

Lorsqu'un test existant n'est plus nécessaire --- sachant qu'il n'est
qu'une sous-partie d'un autre test --- supprimez-le. Ne pas supprimer
les tests superflus n'apporte rien mais augmentent par contre le
travail de maintenance et diminuent la vitesse d'exécution des tests.

### Éviter de tester à travers une IHM

Les interfaces utilisateurs (ou IHM) ont tendance à changer fréquemment.
Exécuter vos tests à travers une IHM les rend vulnérables à ces
changements, même s'il n'y a aucun changement dans la logique du test,
cela augmente la charge de maintenance des tests.

Par conséquent, éviter de tester à travers une IHM et faites plutôt
appel directement à la logique applicative à travers une API. Un autre
avantage de faire cela est d'accélérer la vitesse d'exécution de vos
tests car tester à travers une IHM s'avère généralement toujours très
lent.

### Exécuter les tests fréquemment

Il y a longtemps, nous avons travaillé avec une grosse équipe
travaillant selon une approche en cascade. Le conseil habituel en
automatisation de test est de sélectionner et d'automatiser uniquement
les cas de tests les plus importants --- par une équipe dédiée à
l'automatisation des tests --- après la livraison. Ils ont donc fait ça.
À la fin de la livraison suivante, ils ont alors exécuté les tests et
\... ils ont tous échoués. Mettre à jour tous les tests aurait pris trop
de temps, alors ils ont décidé de tout tester manuellement.

Exécuter les tests une ou deux fois par livraison peut sembler efficace
--- car il y a moins de cycles CPU utilisés --- mais entre deux
livraisons beaucoup de choses auront changé, et par conséquent beaucoup
de tests échoueront, ce qui aura pour conséquence de générer un gros
travail de maintenance. Alternativement, exécuter les tests fréquemment
--- en utilisant un système d'intégration continue --- utilisera
davantage de cycles CPU mais il y aura moins de maintenance étant donné
que la charge de correction des tests sera moindre. Si vous avez une
forte charge de maintenance de tests, c'est probablement que vous ne les
exécutez pas assez fréquemment.

### Traiter les tests non fonctionnels comme des tests fonctionnels

Automatiser et exécuter de manière continue les tests non fonctionnels
est quelque chose d'essentiel. Les retarder jusqu'au dernier moment
signifie c'est prendre de très gros risques là où ça peut faire le plus
mal. Par exemple, s'il est exigé que le système doit avoir un certain
niveau de performance, il est nécessaire de le tester le plus tôt
possible pour déterminer s'il atteint le niveau exigé, et de le tester
de manière continue au fur et à mesure que de nouvelles fonctionnalités
sont ajoutées pour s'assurer que le système ne régresse pas par rapport
au niveau de performance exigé.

Les exigences non fonctionnelles sont souvent traitées de manière assez
exotique - les gens croient qu'elles ne peuvent être ni spécifiées ni
testées. C'est dramatique. Dans un atelier d'exigences, les exigences
non fonctionnelles sont considérées de la même manière que les tests
fonctionnels, et des tests d'exemples sont créés pour aider à la
compréhension.

### Exécuter de manière continue des tests qui prennent du temps à s'exécuter

Il est fréquent que les tests non fonctionnels ne puissent s'exécuter
dans un cycle normal d'intégration continue parce qu'ils prennent trop
de temps à s'exécuter - un test de stabilité peut prendre jusqu'à deux
semaines. Certains groupes produits les retardent pour ainsi dire juste
avant la livraison --- créant ainsi un cycle de boucle de rétroaction à
retardement. Ce n'est pas une bonne idée de procéder de cette manière.

Exécutez plutôt les tests qui prennent du temps de manière continue dans
un cycle d'intégration continue plus lent. Traitez-les comme n'importe
quel autre test. Lorsqu'ils échouent, informez les personnes ayant
implémenté le code. Après qu'ils aient fait le nécessaire, récupérez le
dernier exécutable et exécutez à nouveau les tests.

### Utiliser la virtualisation ou les conteneurs

Afin d'accélérer les tests et de maintenir l'investissement matériel à
un niveau raisonnable, maximiser l'utilisation de la virtualisation en
utilisant [VirtualBox](https://www.virtualbox.org/) ou
[VMWare](http://www.vmware.com/). Une alternative à l'utilisation d'une
machine virtuelle (qui n'est pas toujours très rapide à mettre en place
ou à maintenir) est l'utilisation d'un conteneur virtuel linux tel que
[Docker](http://www.docker.io/).

### Éviter d'utiliser des outils de tests commerciaux

Une fois nous avons accompagné une entreprise qui développait un outil
commercial d' « automatisation de tests » - et pour être plus précis un
outil de test IHM. Quel avait été l'accompagnement demandé ? D'apprendre
comment faire des tests automatisés pour l'aider à développer son outil
de tests automatisés\...

Une multitude d'outils commerciaux de tests existent. Nous avons
rarement rencontré des gens qui en aient été réellement satisfaits. La
plupart d'entre eux sont bien trop complexes, se focalisent davantage
sur la production de tableaux de bord et la gestion plutôt que sur une
automatisation robuste et satisfaisante des tests. Privilégiez plutôt
les outils libres et dont le code source est ouvert, faits par des
développeurs pour résoudre de vrais problèmes - plutôt que des outils
commerciaux.

Voici une liste d'outils d'automatisation de tests communément utilisés :

-   [Robot Framework](http://www.robotframework.org/)
-   [Cucumber](https://cucumber.io/)
-   [FitNesse](http://www.fitnesse.org/)
-   [Selenium](http://www.seleniumhq.org/)
-   [Capybara](https://github.com/jnicklas/capybara)

Il en existe bien plus encore. La liste ci-dessus porte uniquement sur
les outils les plus répandus, de nouveaux outils voient le jour
régulièrement.

---
Auteur : The LeSS Company B.V.  
Source : [Test Automation](https://less.works/less/technical-excellence/test-automation.html)  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Relecture : [Fabrice Aimetti](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 06/11/2022  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

---
layout: post
title:  "L'architecture hexagonale"
date:   2023-11-12 00:01
published: true
tags:
- architecture hexagonale
- agile
---

Note de relecture :
- à partir de  The Left-Right Asymmetry. le terme adapters est utilisé à la place de adaptateurs
- toujours à partir de ce point, les expressions anglophones ne sont plus entre « » mais simplement en _italique_


# Hexagonal architecture

# L'architecture hexagonale

Avant-propos du traducteur : certains mots ou certaines expressions ont été laissées en anglais dans la présente traduction de part leur usage plus répandu.  Toutefois pour satisfaire tous les lectorats possibles, des traductions françaises de ces mêmes mots ou expressions sont présentes en notes de bas de page.

mock == faux-semblant

_Create your application to work without either a UI or a database so you can run automated regression-tests against the application, work when the database becomes unavailable, and link applications together without any user involvement._

_Ou comment créer votre application de telle manière pour qu'elle puisse fonctionner sans interface utilisateur ou sans base de données vous donnant ainsi la possibilité d'exécuter des tests de régression sur celle-ci, de fonctionner même en cas d'indisponibilité de la base de données, et enfin de l'interconnecter avec d'autres applications sans que l'utilisateur ait à faire quoi que ce soit_

* * *

_Japanese translation of this article at_ [http://blog.tai2.net/hexagonal_architexture.html](http://blog.tai2.net/hexagonal_architexture.html)  
_Spanish translation of this article at_ [http://academyfor.us/posts/arquitectura-hexagonal](http://academyfor.us/posts/arquitectura-hexagonal) _courtesy of Arthur Mauricio Delgadillo_  
_original explanation w updates at_ [http://wiki.c2.com/?HexagonalArchitecture](http://wiki.c2.com/?HexagonalArchitecture) _and_ [http://wiki.c2.com/?PortsAndAdaptersArchitecture](http://wiki.c2.com/?PortsAndAdaptersArchitecture)

See also [Hexagonal Architecture FAQ](https://alistair.cockburn.us/Hexagonal+Architecture+FAQ) [(discussion: Re: Hexagonal Architecture FAQ)](https://alistair.cockburn.us/Re%3a+Hexagonal+Architecture+FAQ)

* * *

_Traduction japonaise de cet article_ [http://blog.tai2.net/hexagonal_architexture.html](http://blog.tai2.net/hexagonal_architexture.html)  
_Traduction espagnole de cet article_ [http://academyfor.us/posts/arquitectura-hexagonal](http://academyfor.us/posts/arquitectura-hexagonal) _par Arthur Mauricio Delgadillo_  
_Article d'origine mis à jour ici_ [http://wiki.c2.com/?HexagonalArchitecture](http://wiki.c2.com/?HexagonalArchitecture) _et là_ [http://wiki.c2.com/?PortsAndAdaptersArchitecture](http://wiki.c2.com/?PortsAndAdaptersArchitecture)

* * *
[Hexagonal architecture pic 1-to-4 socket.jpg](https://alistair.cockburn.us/Hexagonal+architecture+pic+1-to-4+socket.jpg)

![Hexagonal architecture pic 1-to-4 socket.jpg](https://alistair.cockburn.us/wp-content/uploads/2018/02/Hexagonal-architecture-pic-1-to-4-socket.jpg "Hexagonal architecture pic 1-to-4 socket.jpg")

[Hexagonal architecture pic 1-to-4 socket.jpg](https://alistair.cockburn.us/Hexagonal+architecture+pic+1-to-4+socket.jpg)

![Hexagonal architecture pic 1-to-4 socket.jpg](https://alistair.cockburn.us/wp-content/uploads/2018/02/Hexagonal-architecture-pic-1-to-4-socket.jpg "Représentation de l'architecture hexagonale 1-to-4 douille.jpg")


## The Pattern: Ports and Adapters (‘’Object Structural’’)

## Le modèle : Ports & Adapters (« Objet structurel »)

### Alternative name: ‘’Ports & Adapters’’

### Alternative name: ‘’Hexagonal Architecture’’

### Nom alternatif : « Ports & Adapters »[^1]

### Alternative name: « Architecture hexagonale »

### Intent

### But recherché

Allow an application to equally be driven by users, programs, automated test or batch scripts, and to be developed and tested in isolation from its eventual run-time devices and databases.

Permettre à une application de pouvoir être pilotée indifféremment par des utilisateurs, des programmes, des tests automatisés ou des batchs, de pouvoir être développée et testée de manière isolée de tout dispositif éventuel l'exécutant ou de toute base  de données qui y serait adossée.  

When any driver wants to use the application at a port, it sends a request that is converted by an adapter for the specific technology of the driver into an usable procedure call or message, which passes that to the application port. The application is blissfully ignorant of the driver’s technology. When the application has something to send out, it sends it out through a port to an adapter, which creates the appropriate signals needed by the receiving technology (human or automated). The application has a semantically sound interaction with the adapters on all sides of it, without actually knowing the nature of the things on the other side of the adapters.

Lorsqu'un pilote, quel qu'il soit, veut utiliser l'application sur un port donné, il envoie une requête qui est convertit par un adaptateur spécifique à la technologie utilisée par le pilote en procédure d'appel ou en message utilisable, qui à son tour est passé au port de l'application. L'application est complètement ignare de la technologie du pilote. Lorsque l'application a quelque chose à envoyer, elle le fait à travers le port vers l'adaptateur, qui à son tour créé le signal approprié attendu par la technologie réceptrice (humaine ou non). L'application a, sémantiquement parlant, des échanges avec les adaptateurs de tous côtés, sans connaître vraiment la nature des choses avec lesquelles elle communique de l'autre côté des adaptateurs.

Figure 1 : [Hexagonal architecture basic.gif](https://alistair.cockburn.us/Hexagonal+architecture+basic.gif)

![Hexagonal architecture basic.gif](https://alistair.cockburn.us/wp-content/uploads/2018/02/Hexagonal-architecture-basic-1.gif "Hexagonal architecture basic.gif")

Illustration 1 : [Architecture hexagonale.gif](https://alistair.cockburn.us/Hexagonal+architecture+basic.gif)

![Hexagonal architecture basic.gif](https://alistair.cockburn.us/wp-content/uploads/2018/02/Hexagonal-architecture-basic-1.gif "Hexagonal architecture basic.gif")


### Motivation

### Motivation

One of the great bugaboos of software applications over the years has been infiltration of business logic into the user interface code. The problem this causes is threefold:

L'un des plus grands épouvantails du monde informatique de ces dernières années a été l'immixtion de la logique métier au sein du code de l'interface utilisateur. Le problème que cela engendre est de trois ordres :

- First, the system can’t neatly be tested with automated test suites because part of the logic needing to be tested is dependent on oft-changing visual details such as field size and button placement;
- For the exact same reason, it becomes impossible to shift from a human-driven use of the system to a batch-run system;
- For still the same reason, it becomes difficult or impossible to allow the program to be driven by another program when that becomes attractive.

- Tout d'abord, il est impossible de tester le système de manière exhaustive avec des logiciels de tests automatisés car la partie de la logique qui doit être testée est dépendante de la partie visuelle dont les éléments sont amenés à changer régulièrement comme par exemple la taille d'un champ de saisie ou le placement d'un bouton ;
- Pour la même raison, il est impossible de remplacer une interaction humaine sur le système par des batchs ;
- Et toujours pour la même raison, il est difficile voire impossible de permettre au programme d'être piloté par un autre programme si cela devient intéressant.

The attempted solution, repeated in many organizations, is to create a new layer in the architecture, with the promise that this time, really and truly, no business logic will be put into the new layer. However, having no mechanism to detect when a violation of that promise occurs, the organization finds a few years later that the new layer is cluttered with business logic and the old problem has reappeared.

La solution tentée dans beaucoup d'organisations est de créer une nouvelle couche au niveau de l'architecture, avec la promesse que cette fois-ci, si si pour de vrai, qu'aucune logique métier ne viendra fourrer son nez dans la nouvelle couche. Toutefois, comme il n'existe aucun mécanisme permettant de détecter une violation de cette promesse, l'organisation découvre quelques années plus tard que cette nouvelle couche est parsemée de logique métier et le vieux problème refait surface. 

Imagine now that ‘’every’’ piece of functionality the application offers were available through an API (application programmed interface) or function call. In this situation, the test or QA department can run automated test scripts against the application to detect when any new coding breaks a previously working function. The business experts can create automated test cases, before the GUI details are finalized, that tells the programmers when they have done their work correctly (and these tests become the ones run by the test department). The application can be deployed in ‘’headless’’ mode, so only the API is available, and other programs can make use of its functionality — this simplifies the overall design of complex application suites and also permits business-to-business service applications to use each other without human intervention over the web. Finally, the automated function regression tests detect any violation of the promise to keep business logic out of the presentation layer. The organization can detect, and then correct, the logic leak.

Imaginez maintenant que « chaque » morceau de fonctionnalité que l'application offre soit rendue disponible à travers une API (interface d'application programmable) ou un appel de fonction. Dans cette situation, le département Test ou Assurance Qualité peut tout à fait exécuter des scripts de tests automatisés pour détecter que rien de nouveau n'est venu cassé une fonction qui fonctionnait auparavant. Les experts métiers peuvent créer des cas de test automatisés, avant que les détails de l'interface utilisateurs soient finalisés, ce qui permettra de dire aux développeurs qu'ils ont fait leur travail correctement (et ces tests deviennent ceux exécutés par le département Assurance Qualité). L'application peut être déployée en mode « headless »[^2], dans laquelle seule l'API est disponible. Dans ce cas de figure, seuls les autres programmes peuvent utiliser les fonctionnalités de l'application — cela simplifie la conception générale des suites d'applications complexes, et cela permet aussi aux applications offrant des services B2B de faire appels à leurs fonctionnalités réciproques à travers la Toile sans interventions humaines. Enfin, cela permet aux tests de régression automatisés de détecter les violations faites à cette promesse de garder en dehors de la couche de présentation la logique métier.
L'organisation peut alors détecter, puis corriger cette infiltration.       

An interesting similar problem exists on what is normally considered “the other side” of the application, where the application logic gets tied to an external database or other service. When the database server goes down or undergoes significant rework or replacement, the programmers can’t work because their work is tied to the presence of the database. This causes delay costs and often bad feelings between the people.

Un autre problème analogue et intéressant, existe dans ce que l'on appelle habituellement « l'autre côté » de l'application, lorsque la logique applicative se retrouve assujétie à une base de données ou à un autre service externe. Lorsque le serveur de la base de données tombe, est en cours de maintenance ou est remplacé par un autre, les développeurs se retrouvent dans l'impossibilité de travailler en raison de cet assujettissement. Ce qui entraîne des coûts liés au retard pris et souvent des ressentiments au sein des équipes. 

It is not obvious that the two problems are related, but there is a symmetry between them that shows up in the nature of the solution.

Il n'est pas sûr que les deux problèmes évoqués soient liés, mais il y a une certaine symétrie entre les deux qui apparaît quant à la nature de la solution.

### Nature of the Solution

### De la nature de la solution

Both the user-side and the server-side problems actually are caused by the same error in design and programming — the entanglement between the business logic and the interaction with external entities. The asymmetry to exploit is not that between ‘’left’’ and ‘’right’’ sides of the application but between ‘’inside’’ and ‘’outside’’ of the application. The rule to obey is that code pertaining to the ‘’inside’’ part should not leak into the ‘’outside’’ part.

En réalité, les problèmes du côté utilisateur et du côté serveur ont pour origine une même erreur de conception et de développement à savoir — l'enchevêtrement des logiques métier et interaction avec des entités externes. L'asymétrie à exploiter n'est pas entre le côté « gauche » ou « droite » de l'application mais entre l' « intérieur » et l' « extérieur » de l'application. La règle à laquelle se plier est que le code qui s'occupe de la partie « intérieure » ne devrait pas déborder sur la partie « extérieure ».

Removing any left-right or up-down asymmetry for a moment, we see that the application communicates over ‘’ports’’ to external agencies. The word “port” is supposed to evoke thoughts of ‘’ports’’ in an operating system, where any device that adheres to the protocols of a port can be plugged into it; and ‘’ports’’ on electronics gadgets, where again, any device that fits the mechanical and electrical protocols can be plugged in.

Mettons de côté pour l'instant l'asymétrie gauche-droite ou haut-bas, nous voyons alors que l'application communique avec des agents externes à travers des « ports ». Le mot « port » est supposé vous évoquer par analogie le concept de ports des systèmes d'exploitation, dans lesquels tout périphérique adhèrant aux protocoles d'un port peut y être branché ; il en est de même pour tout appareil électronique où là aussi tout périphérique compatible avec les protocoles mécaniques et électroniques d'un port peut y être branché.

- The protocol for a port is given by the _purpose of the conversation_ between the two devices.

- Le protocole d'un port est défini par le _but de la conversation_ entre deux appareils. 

The protocol takes the form of an application program interface (API).

Le protocole prend la forme d'une interface de programmation d'application (API).

For each external device there is an ‘’adapter’’ that converts the API definition to the signals needed by that device and vice versa. A graphical user interface or GUI is an example of an adapter that maps the movements of a person to the API of the port. Other adapters that fit the same port are automated test harnesses such as FIT or Fitnesse, batch drivers, and any code needed for communication between applications across the enterprise or net.

Pour chaque périphérique externe existe un « adaptateur » qui convertit la définition de l'API en signaux nécessaires à la bonne communication avec le périphérique et vice versa. Un interface homme-machine (IHM) est un exemple d'adaptateur qui convertit grâce à l'API du port les mouvements de la souris faits par un utilisateur. Parmi les autres adaptateurs qui peuvent se brancher sur le même port, citons les outils de tests automatisés tels que FIT ou Fitness, les outils de gestion de batchs, et bien sûr tout code permettant de faire communiquer différentes applications entre elles au sein ou à l'extérieur de l'entreprise.

On another side of the application, the application communicates with an external entity to get data. The protocol is typically a database protocol. From the application’s perspective, if the database is moved from a SQL database to a flat file or any other kind of database, the conversation across the API should not change. Additional adapters for the same port thus include an SQL adapter, a flat file adapter, and most importantly, an adapter to a “mock” database, one that sits in memory and doesn’t depend on the presence of the real database at all.

Passons à une autre partie de l'application, imaginons que celle-ci communique avec une entité externe pour obtenir des données. Le protocole utilisé est généralement un protocole de base de donnée. Du point de vue de l'application, si la source de données change d'une base de donnée SQL à un fichier plat ou à n'importe quelle autre type de base de données, la conversation qui se fait avec elle à travers l'API ne devrait pas changer. Des adaptateurs supplémentaires pour ce même port devrait donc inclure un adaptateur SQL, un adaptateur fichier plat et plus important encore un adaptateur vers une  base de données « mock [^3]» (comme par exemple une base de données résidente en mémoire) et qui ne devrait donc pas dépendre de l'existence d'une vraie base de donnée.

Many applications have only two ports: the user-side dialog and the database-side dialog. This gives them an asymmetric appearance, which makes it seem natural to build the application in a one-dimensional, three-, four-, or five-layer stacked architecture.

La plupart des applications possèdent seulement deux ports : le premier permettant de dialoguer du côté utilisateur, le second du côté base de donnée. Cela leurs donne une apparence asymétrique, ce qui rend naturelle, du moins en apparence, la mise en place d'une architecture à une, deux, trois, quatre voire cinq couches. 

There are two problems with these drawings. First and worst, people tend not to take the “lines” in the layered drawing seriously. They let the application logic leak across the layer boundaries, causing the problems mentioned above. Secondly, there may be more than two ports to the application, so that the architecture does not fit into the one-dimensional layer drawing.

Il existe deux problèmes avec ces représentations. Le premier et sans doute le pire est que les gens ont tendance à ne pas prendre au sérieux les « frontières » figurant sur la représentation des couches de l'architecture. Ils ont tendance à laisser la logique applicative empiéter au-delà de ses propres frontières, provoquant ainsi les problèmes mentionnés précédemment. Le deuxième, c'est qu'il y a peut être, en réalité, plus que deux ports pour l'application, de telle sorte que l'architecture telle qu'imaginée au départ ne tient pas dans une représentation à une dimension.

The hexagonal, or ports and adapters, architecture solves these problems by noting the symmetry in the situation: there is an application on the inside communicating over some number of ports with things on the outside. The items outside the application can be dealt with symmetrically.

L'architecture hexagonale, ou architecture ports et adaptateurs, résout ces problèmes simplement en faisant le constat de l'existence de cette symétrie pour ce genre de situation : à savoir que l'application à l'intérieure communique avec le monde extérieur à travers un certain nombre de ports. Les éléments figurant à l'extérieur de l'application peuvent être gérés de manière symétrique. 

The hexagon is intended to visually highlight

La forme de l'hexagone a été choisie car elle permet visuellement de mettre en avant 

(a) the inside-outside asymmetry and the similar nature of ports, to get away from the one-dimensional layered picture and all that evokes, and

(a) l'asymétrie intérieure-extérieure et la nature similaire des ports de telle manière que cela permet de s'affranchir des représentations en couche à une dimension et de ce que cela induit

(b) the presence of a defined number of different ports – two, three, or four (four is most I have encountered to date).

(b) la présence d'un nombre défini de ports - deux, trois, ou quatre (quatre étant le nombre le plus fréquent que j'ai pu observer jusqu'à présent)

The hexagon is not a hexagon because the number six is important, but rather to allow the people doing the drawing to have room to insert ports and adapters as they need, not being constrained by a one-dimensional layered drawing. The term ‘’hexagonal architecture’’ comes from this visual effect.

L'hexagone a été choisi non pas parce que le nombre six est important, mais plutôt parce qu'il permet aux gens de faire une représentation avec suffisamment d'espace pour y faire figurer les ports et les adapteurs dont ils ont besoin, de ne pas être restreint par une représentation à une dimension. L'expression « architecture hexagonale » provient du souhait d'avoir cet effet visuel. 

The term “port and adapters” picks up the ‘’purposes’’ of the parts of the drawing. A port identifies a purposeful conversation. There will typically be multiple adapters for any one port, for various technologies that may plug into that port. Typically, these might include a phone answering machine, a human voice, a touch-tone phone, a graphical human interface, a test harness, a batch driver, an http interface, a direct program-to-program interface, a mock (in-memory) database, a real database (perhaps different databases for development, test, and real use).

Le terme « ports et adapteurs » s'appuie sur ce que sont la nature des  « finalités » représentées sur le dessin. Un port représente une conversation définie. Il y a en général plusieurs adaptateurs pour un port donné, différentes technologies peuvent être branchées sur ce port. comme par exemple un répondeur téléphonique, une voix humaine, un téléphone fixe, une interface homme-machine, une suite de tests, un outil de gestion des traitements batchs, une interface http, une interface direct programme-à-programme,  une base de données « mock » (en mémoire), une « vraie » base de données (peut-être même plusieurs bases de données, l'une en environnement de développement, une autre pour l'environnement de test et une autre encore our l'environnement de production).

In the Application Notes, the left-right asymmetry will be brought up again. However, the primary purpose of this pattern is to focus on the inside-outside asymmetry, pretending briefly that all external items are identical from the perspective of the application.

Dans l'application Notes que nous verrons après, l'asymétrie gauche-droite sera remise en évidence. Toutefois, l'objectif premier de ce _pattern_ [^4] est de mettre en avant l'asymétrie interne-externe en évoquant brièvement que tous les éléments externes sont identiques du point de vue de l'application.

### Structure

### Structure

Figure 2 : [Hexagonal architecture with adapters.gif](https://alistair.cockburn.us/Hexagonal+architecture+with+adapters.gif)

Illustration 2 : [Architecture hexagonale avec adaptateurs.gif](https://alistair.cockburn.us/Hexagonal+architecture+with+adapters.gif)

![Hexagonal architecture with adapters.gif](https://alistair.cockburn.us/wp-content/uploads/2018/02/Hexagonal-architecture-with-adapters.gif "Hexagonal architecture with adapters.gif")

![Architecture hexagonale avec adaptateurs.gif](https://alistair.cockburn.us/wp-content/uploads/2018/02/Hexagonal-architecture-with-adapters.gif "Hexagonal architecture with adapters.gif")

Figure 2 shows an application having two active ports and several adapters for each port. The two ports are the application-controlling side and the data-retrieval side. This drawing shows that the application can be equally driven by an automated, system-level regression test suite, by a human user, by a remote http application, or by another local application. On the data side, the application can be configured to run decoupled from external databases using an in-memory oracle, or ‘’mock’’, database replacement; or it can run against the test- or run-time database. The functional specification of the application, perhaps in use cases, is made against the inner hexagon’s interface and not against any one of the external technologies that might be used.

L'illustration 2 représente une application avec deux ports actifs et plusieurs adaptateurs pour chaque port. Les deux ports représentés sont d'une part contrôle de l'application et d'autre part la récupération de données. Cette représentation illustre que l'application peut être pilotée indifféremment par un automate, par une suite de tests de non régression au niveau système, par un être humain, par une application à distance en mode http, ou par une autre application en local. Du côté données, l'application peut être configurée pour s'exécuter découplée de toute base de données externes en utilisant une base de données en mémoire (un « _mock_ »), ou encore une base de données de remplacement ; ou elle peut s'exécuter contre un test - ou un run-time de base de données. Les spécifications fonctionnelles de l'application, peuvent être sous la forme de cas d'utilisations, décrivent la partie interne de l'interface de l'hexagone et non les technologies externes qui pourraient être utilisées.

Figure 3 : [Hexagonal architecture barn door image.gif](https://alistair.cockburn.us/Hexagonal+architecture+barn+door+image.gif)

Illustration 3 : [Image de l'architecture hexagonale architecture dite de la porte de grange.gif](https://alistair.cockburn.us/Hexagonal+architecture+barn+door+image.gif)

![Hexagonal architecture barn door image.gif](https://alistair.cockburn.us/wp-content/uploads/2018/02/Hexagonal-architecture-barn-door-image-1.gif "Hexagonal architecture barn door image.gif")

![Image de l'architecture hexagonale architecture dite de la porte de grange.gif](https://alistair.cockburn.us/wp-content/uploads/2018/02/Hexagonal-architecture-barn-door-image-1.gif "Image de l'architecture hexagonale architecture dite de la porte de grange.gif")


Figure 3 shows the same application mapped to a three-layer architectural drawing. To simplify the drawing only two adapters are shown for each port. This drawing is intended to show how multiple adapters fit in the top and bottom layers, and the sequence in which the various adapters are used during system development. The numbered arrows show the order in which a team might develop and use the application:

L'illustration 3 représente la même application selon une architecture en 3 couches. Pour simplifier l'illustration, seuls deux adaptateurs sont montrés pour chacun des ports représentés. Cette représentation illustre comment un ensemble d'adaptateurs s'intègrent dans les couches hautes et basses de l'application ainsi que la séquence d'utilisation des adaptateurs lors du développement du système. Les flèches numérotées montrent l'ordre dans lequel une équipe pourrait développer et utiliser une telle application.

1. With a FIT test harness driving the application and using the mock (in-memory) database substituting for the real database;
2. Adding a GUI to the application, still running off the mock database;
3. In integration testing, with automated test scripts (e.g., from Cruise Control) driving the application against a real database containing test data;
4. In real use, with a person using the application to access a live database.

1. Une suite de tests FIT pilote l'application et utilise une base de données « mock » (c'est-à-dire en mémoire) qui se substitue à la vraie base de données ;
2. Ajouter une IHM à l'application tout en continuant d'utiliser la « fausse » base de données ;
3. Lors des tests d'intégration, des scripts de tests automatisés (à l'aide par exemple de Cruise Control) pilotent l'application connectée à la vraie base de données qui contient de données de tests ;
4. En condition d'utilisation réelle, avec une personne utilisant l'application connectée à la vraie base de données avec de vraies données

### Sample Code

### Exemple de code

The simplest application that demonstrates the ports & adapters fortunately comes with the FIT documentation. It is a simple discount computing application:

L'exemple d'application ci-dessous, une application de calcul de remise commerciale, illustre de la manière la plus simple possible ce qu'est concrètement l'architecture ports et adaptateurs. Il est fourni avec la documentation FIT qui va bien.


~~~ java
discount(amount) = amount * rate(amount);
~~~

In our adaptation, the amount will come from the user and the rate will come from a database, so there will be two ports. We implement them in stages:

Dans notre adaptation, le montant est fourni par l'utilisateur et le taux par une base de données, il y a donc deux ports. Nous les implémentons en plusieurs étapes :

- With tests but with a constant rate instead of a mock database,
- then with the GUI,
- then with a mock database that can be swapped out for a real database.

- D'abord avec des tests sur la base d'un taux constant à la place d'une base de données « _mock_ »,
- ensuite avec une IHM,
- ensuite avec une bases de données « _mock_ » qui pourra être remplacée par une véritable base de données. 

_Thanks to Gyan Sharma at IHC for providing the code for this example._

_Je tiens à remercier Gyan Sharma d'IHC de m'avoir fourni le code de cet exemple._

#### Stage 1: FIT App constant-as-mock-database

#### Étape 1: FIT App un-taux-constant-à-la-place-d'une-base-de-données


First we create the test cases as an HTML table (see the FIT documentation for this):

D'abord nous créons le cas de test sous la forme d'une table HTML (cf. documentation FIT pour plus d'informations à ce sujet)

| TestDiscounter | &nbsp;  |
| amount | discount() |
| 100  | 5 |
| 200 | 10 |

Note that the column names will become class and function names in our program. FIT contains ways to get rid of this “programmerese”, but for this article it is easier just to leave them in.

Il est intéressant de remarquer que les noms des colonnes deviendront les noms des classes et des fonctions dans notre programmes. Il existe différentes manières de faire dans FIT pour ne pas avoir à faire ces « programmeries », mais pour cet article nous mettrons cela de côté.

Knowing what the test data will be, we create the user-side adapter, the ColumnFixture that comes with FIT as shipped:

Sachant dorénavant ce que vont être les données de tests, nous allons créer l'adaptateur côté utilisateur et utiliser la fixture[^3] `ColumnFixture` disponible dans FIT :


~~~ java
import fit.ColumnFixture; 
public class TestDiscounter extends ColumnFixture 
{ 
   private Discounter app = new Discounter(); 
   public double amount;
   public double discount() 
   { return app.discount(amount); } 
}
~~~

That’s actually all there is to the adapter. So far, the tests run from the command line (see the FIT book for the path you’ll need). We used this one:

C'est tout ce qu'il y a à faire pour l'adapteur. Nous allons ensuite exécuter les tests à partir de la ligne de commande (consulter la documentation FIT pour adapter cette commande à votre environnement). Dans notre cas, voici ce que nous allons utiliser :

~~~
set FIT_HOME=/FIT/FitLibraryForFit15Feb2005
java -cp %FIT\_HOME%/lib/javaFit1.1b.jar;%FIT\_HOME%/dist/fitLibraryForFit.jar;src;bin
fit.FileRunner test/Discounter.html TestDiscount_Output.html
~~~

FIT produces an output file with colors showing us what passed (or failed, in case we made a typo somewhere along the way).

FIT produit un fichier comportant des codes couleurs nous montrant les tests ayant réussis (ou échoués au cas où nous aurions fait une erreur de frappe en cours de route.)

At this point the code is ready to check in, hook into Cruise Control or your automated build machine, and include in the build-and-test suite.

À ce stade, le code est prêt à être enregistré dans votre processus d'intégration continue (Cruise Control ou autre), et à être ajouté à votre chaîne _build-and-test_.

#### Stage 2: UI App constant-as-mock-database

#### Étape 2 : IHM App un-taux-constant-à-la-place-d'une-base-de-données

I’m going to let you create your own UI and have it drive the Discounter application, since the code is a bit long to include here. Some of the key lines in the code are these:

Le code étant un peu long à faire figurer ici dans son intégralité, je vais vous laisser créer votre propre IHM pour l'application `Discounter`.
Pour vous aider, voici quelques-unes de morceaux de code clés :

~~~ java
...
 Discounter app = new Discounter();
public void actionPerformed(ActionEvent event) 
{
    ...
   String amountStr = text1.getText();
   double amount = Double.parseDouble(amountStr);
   discount = app.discount(amount));
   text3.setText( "" + discount );
   ...
 }
~~~ 

At this point the application can be both demoed and regression tested. The user-side adapters are both running.

À ce stade, une démonstration de l'application peut être faite ainsi qu'un test de régression. Les adaptateurs du côté utilisateurs sont tous les deux opérationnels.

#### Stage 3: (FIT or UI) App mock database

#### Étape 3 (FIT ou IHM) APP fausse base de données

To create a replaceable adapter for the database side, we create an ‘’interface’’ to a repository, a ‘’RepositoryFactory’’ that will produce either the mock database or the real service object, and the in-memory mock for the database.

Pour créer un adaptateur remplaçable du côté base de données, nous créons une « interface » vers un dépôt,plus précisément  un générateur de dépôt (« _RepositoryFactory_ ») qui produira soit une base de données de type « _mock_ » soit une véritable base de données.

~~~ java
public interface RateRepository 
{
   double getRate(double amount);
 }
public class RepositoryFactory 
{
   public RepositoryFactory() {  super(); }
   public static RateRepository getMockRateRepository() 
   {
      return new MockRateRepository();
   }
}
public class MockRateRepository implements RateRepository 
{
   public double getRate(double amount) 
   {
      if(amount &lt;= 100) return 0.01;
      if(amount &lt;= 1000) return 0.02;
      return 0.05;
    }
 }
~~~

To hook this adapter into the Discounter application, we need to update the application itself to accept a repository adapter to use, and the have the (FIT or UI) user-side adapter pass the repository to use (real or mock) into the constructor of the application itself. Here is the updated application and a FIT adapter that passes in a mock repository (the FIT adapter code to choose whether to pass in the mock or real repository’s adapter is longer without adding much new information, so I omit that version here).

Pour insérer cet adaptateur dans l'application `Discounter`, nous devons mettre à jour l'application elle-même afin qu'elle puisse prendre en compte l'utilisation de l'adaptateur  _repository_ et avoir l'adaptateur côté utilisateur (que ce soit FIT ou une IHM) passer le dépôt (« _repository_ ») à utiliser (la vraie ou la fausse (« _mock_ ») base de données) au constructeur de l'application. Vous trouverez ci-dessous l'application mise à jour ainsi qu'un adaptateur FIT qui passe un faux dépôt (le code de l'adaptateur FIT permettant de choisir de passer l'adapteur vers le vrai ou le faux dépôt est lui aussi trop long tout en n'apportant pas grand chose en terme d'informations, je ne l'ai donc pas inclus dans la version ci-dessous).

~~~ java
import repository.RepositoryFactory;
import repository.RateRepository;
public class Discounter 
{
   private RateRepository rateRepository;
   public Discounter(RateRepository r) 
   {
      super();
      rateRepository = r;
    }
   public double discount(double amount) 
   {
      double rate = rateRepository.getRate( amount ); 
      return amount * rate;
    }
}
import app.Discounter;
import fit.ColumnFixture;
public class TestDiscounter extends ColumnFixture 
{
   private Discounter app = 
       new Discounter(RepositoryFactory.getMockRateRepository());
   public double amount;
   public double discount() 
   {
      return app.discount( amount );
   }
}
~~~

That concludes implementation of the simplest version of the hexagonal architecture.

Ceci conclut l'implémentation de la version la plus simple possible de l'architecture hexagonale.

For a different implementation, using Ruby and Rack for browser usage, see [https://github.com/totheralistair/SmallerWebHexagon](https://github.com/totheralistair/SmallerWebHexagon)

Vous pouvez consulter sur cette [page](https://github.com/totheralistair/SmallerWebHexagon) une implémentation différente de l'architecture hexagonale à base de Ruby et de Rack 

### Application Notes

### Notes de l'application

#### The Left-Right Asymmetry

#### L'asymétrie gauche

The ports and adapters pattern is deliberately written pretending that all ports are fundamentally similar. That pretense is useful at the architectural level. In implementation, ports and adapters show up in two flavors, which I’ll call ‘’primary’’ and ‘’secondary’’, for soon-to-be-obvious reasons. They could be also called ‘’driving’’ adapters and ‘’driven’’ adapters.

Le _pattern_ `ports & adapters` est écrit délibérément en partant du postulat que tous les ports sont foncièrement similaires. Ce postulat est utile à un niveau architecturale. En terme d'implémentation, les ports et les _adapters_ peuvent être de deux ordres, que j'appellerai respectivement « primaire » et « secondaire » pour des raisons qui vous paraîtront bientôt évidentes. Il est également possible de les appeler _adapters_ « pilote » et « piloté »

The alert reader will have noticed that in all the examples given, FIT fixtures are used on the left-side ports and mocks on the right. In the three-layer architecture, FIT sits in the top layer and the mock sits in the bottom layer.

Le lecteur avertit aura remarqué que dans tous les exemples données des _fixtures_ FIT sont utilisés pour les ports côté gauche et des _mocks_ côté droit. Dans une architecture en 3 couches, FIT se situe au niveau le plus haut alors que le _mock_ est au niveau le plus bas.

This is related to the idea from use cases of “primary actors” and “secondary actors”. A ‘’primary actor’’ is an actor that drives the application (takes it out of quiescent state to perform one of its advertised functions). A ‘’secondary actor’’ is one that the application drives, either to get answers from or to merely notify. The distinction between ‘’primary ‘’and’’ secondary ‘’lies in who triggers or is in charge of the conversation.

Ceci est à rapprocher de l'idée d'« acteurs primaires » et d'« acteurs secondaires » issues des cas d'utilisation. Un « acteur primaire » est un acteur qui pilote l'application (autrement dit de la faire sortir de son état de veille pour exécuter une des fonctions présentes). Un « acteur secondaire » quant à lui se voit piloté par l'application, soit pour en obtenir des informations soit pour simplement émettre une notification. La distinction entre « primaire » et « secondaire » repose sur qui va déclencher ou qui est en charge de la conversation.

The natural test adapter to substitute for a ‘’primary’’ actor is FIT, since that framework is designed to read a script and drive the application. The natural test adapter to substitute for a ‘’secondary’’ actor such as a database is a mock, since that is designed to answer queries or record events from the application.

L'adaptateur de test pour substituer un acteur « primaire » est tout naturellement FIT, ce _framework_ étant conçu pour lire un script et piloter l'application. L'adaptateur de test pour substituer un acteur « secondaire » comme par exemple une base de donnée est tout naturellement un _mock_, étant donné qu'il est conçu pour répondre à des requêtes ou pour enregistrer les évènements de l'application.

These observations lead us to follow the system’s use case context diagram and draw the ‘’primary ports ‘’and’’ primary adapters’’ on the left side (or top) of the hexagon, and the ‘’secondary ports’’ and ‘’secondary adapters’’ on the right (or bottom) side of the hexagon.

Ces observations nous conduisent à suivre le diagramme de contexte des cas d'utilisation du système et à dessiner les « ports primaires  » et les « adaptateurs primaires » du côté gauche (ou en haut) de l'hexagone et les « ports secondaires » et les « adaptateurs secondaires » sur le côté droit (ou bas) de l'hexagone.

The relationship between primary and secondary ports/adapters and their respective implementation in FIT and mocks is useful to keep in mind, but it should be used as a consequence of using the ports and adapters architecture, not to short-circuit it. The ultimate benefit of a ports and adapters implementation is the ability to run the application in a fully isolated mode.

Les relations entre ports & _adapters_ primaires et secondaires et leurs implémentations respectives avec FIT ou à l'aide de _mocks_ est quelque chose d'important à garder à l'esprit, mais elles devraient être utilisées comme étant une conséquence de l'utilisation de l'architecture ports & _adapters_, et non pour prendre un raccourci. Le bénéfice ultime d'une implémentation ports & _adapters_ est la capacité d'exécuter l'application en mode isolé.

#### Use Cases And The Application Boundary

#### Cas d'utilisation et frontières de l'application

It is useful to use the hexagonal architecture pattern to reinforce the preferred way of writing use cases.

L'utilisation du _pattern_ de l'architecture hexagonale permet de réaffirmer sur quelle est la manière privilégiée de rédiger les cas d'utilisation.

A common mistake is to write use cases to contain intimate knowledge of the technology sitting outside each port. These use cases have earned a justifiably bad name in the industry for being long, hard-to-read, boring, brittle, and expensive to maintain.

Une erreur assez répandue dans l'écriture des cas d'utilisation est de vouloir y mettre une connaissance implicite de la technologie utilisée en dehors des ports. Ces cas d'utilisations ont gagné à juste titre une mauvaise réputation dans l'industrie informatique comme étant trop longs, difficiles à lire, ennuyeux, non fiables et coûteux à maintenir.

Understanding the ports and adapters architecture, we can see that the use cases should generally be written at the application boundary (the inner hexagon), to specify the functions and events supported by the application, regardless of external technology. These use cases are shorter, easier to read, less expensive to maintain, and more stable over time.

Si l'on réfléchit bien à l'architecture _ports & adapters_ , nous pouvons voir que les cas d'utilisation devraient être écrit à l'intérieur des limites de l'application (autrement dit la partie interne de l'hexagone) pour spécifier les fonctions et les évènements supportés par l'application, et ce quelque soit la technologie externe derrière. Dans ces conditions, les cas d'utilisations peuvent être plus courts, plus facile à lire, moins coûteux à maintenir et davantage pérenne.

#### How Many Ports?

#### Combien de ports ?

What exactly a port is and isn’t is largely a matter of taste. At the one extreme, every use case could be given its own port, producing hundreds of ports for many applications. Alternatively, one could imagine merging all primary ports and all secondary ports so there are only two ports, a left side and a right side.

Qu'est-ce qu'exactement un port ou ce qu'il n'est pas est largement une question de goût.  D'un côté du spectre, chaque cas d'utilisation pourrait avoir son propre port, ce qui donnerait des centaines de ports pour différentes applications. De l'autre côté, on pourrait imagine fusionner tous les ports primaires et tous les ports secondaires de telle sorte qu'il n'y ait plus que deux ports, l'un du côté gauche et l'autre de côté droit.

Neither extreme appears optimal.

Aucun de ces deux côtés n'est optimal.

The weather system described in the Known Uses has four natural ports: the weather feed, the administrator, the notified subscribers, the subscriber database. A coffee machine controller has four natural ports: the user, the database containing the recipes and prices, the dispensers, and the coin box. A hospital medication system might have three: one for the nurse, one for the prescription database, and one for the computer-controller medication dispensers.

Le système météo décrit ci-dessous dans les cas d'usages connus a quatre ports dits naturels : le flux météo, l'administrateur, les souscripteurs notifiés, la base de données souscriptrice. Un contrôleur de machine à café a quatre ports naturels : l'utilisateur, la base de données contenant les recettes et les prix, les distributeurs et le monnayeur. Un système pharmaceutique dans un hôpital pourrait en avoir trois : un pour l'infirmière, un pour la base de données des prescriptions, et un pour l'ordinateur pilotant la distribution de médicaments

It doesn’t appear that there is any particular damage in choosing the “wrong” number of ports, so that remains a matter of intuition. My selection tends to favor a small number, two, three or four ports, as described above and in the Known Uses.

À priori, il n'y a aucun risque particulier à se tromper à faire le « mauvais » choix du nombre de ports, cela reste une question d'intuition. J'ai tendance à favoriser un petit nombre de ports, deux, trois ou quatre ports comme évoqué précédemment et également ci-dessous dans les usages connus.

### Known Uses

### Cas d'usages connus

Figure 4 : [Hexagonal architecture complex example.gif](https://alistair.cockburn.us/Hexagonal+architecture+complex+example.gif)

Illustration 4 : [Exemple complexe de l'architecture hexagonale.gif](https://alistair.cockburn.us/Hexagonal+architecture+complex+example.gif)

![Hexagonal architecture complex example.gif](https://alistair.cockburn.us/wp-content/uploads/2018/02/Hexagonal-architecture-complex-example.gif "Hexagonal architecture complex example.gif")

![Exemple complexe de l'architecture hexagonale.gif](https://alistair.cockburn.us/wp-content/uploads/2018/02/Hexagonal-architecture-complex-example.gif "Exemple complexe de l'architecture hexagonale.gif")

Figure 4 shows an application with four ports and several adapters at each port. This was derived from an application that listened for alerts from the national weather service about earthquakes, tornadoes, fires and floods, and notified people on their telephones or telephone answering machines. At the time we discussed this system, the system’s interfaces were identified and discussed by ‘’technology, linked to purpose’’. There was an interface for trigger-data arriving over a wire feed, one for notification data to be sent to answering machines, an administrative interface implemented in a GUI, and a database interface to get their subscriber data.

L'illustration n°4 montre une application comportant quatre ports et pour chacun d'eux plusieurs adaptateurs. Cette illustration a été faite sur la base d'une application qui surveille les alertes sismiques, tornades, incendies et inondations du service de météorologie nationale, et qui, lorsqu'elles se produisent, notifie les populations sur leur téléphone ou sur leur répondeur. À l'époque où nous discutions de ce système, les interfaces de celui-ci étaient identifiées et abordées par « technologie, liées à leur objectif premier  ».  Il y avait une interface pour le déclencheur de données arrivant par le réseau filaire,  une pour les données de notification à envoyer aux répondeurs, une interface pour l'IHM d'administration et une interface pour la base de données pour les données des abonnés.

The people were struggling because they needed to add an http interface from the weather service, an email interface to their subscribers, and they had to find a way to bundle and unbundle their growing application suite for different customer purchasing preferences. They feared they were staring at a maintenance and testing nightmare as they had to implement, test and maintain separate versions for all combinations and permutations.

Les gens se tiraient les cheveux parce qu'ils devaient ajouter une interface http pour le service météorologique, une interface pour les courriels à destination des abonnés, et ils devaient trouver une manière d'empaqueter et de désempaqueter leur suite applicative qui grossissait pour satisfaire les préférences de ses différents clients. Ils craignaient d'être bloqués lors d'une maintenance et les tests des nouvelles fonctionnalités devenaient un cauchemar car ils devaient implémenter, tester et maintenir toutes les différentes versions demandées par leurs clients.

Their shift in design was to architect the system’s interfaces ‘’by purpose’’ rather than by technology, and to have the technologies be substitutable (on all sides) by adapters. They immediately picked up the ability to include the http feed and the email notification (the new adapters are shown in the drawing with dashed lines). By making each application executable in headless mode through APIs, they could add an app-to-add adapter and unbundle the application suite, connecting the sub-applications on demand. Finally, by making each application executable completely in isolation, with test and mock adapters in place, they gained the ability to regression test their applications with stand-alone automated test scripts.

Les changements apportés en terme de conception a été d'une part d'élaborer les interfaces du système « par objectif » plutôt que par technologie, et d'autre part de faire en sorte que les technologies soient substituables (peu importe le côté) au niveau de chaque adaptateur. Ils ont alors immédiatement eu la possibilité d'inclure le flux http et la notification par courriel (les nouveaux adaptateurs sont identifiables sur l'illustration avec les lignes en pointillés). En rendant chaque application exécutable en mode _headless_ à travers des API, ils ont pu à la fois ajouter un adaptateur « application-prêt-à-ajouter » et désempaqueter la suite applicative, permettant ainsi d'y connecter des sous-applications à la demande. Enfin, en rendant chaque application exécutable de manière isolée, à l'aide adaptateurs de tests, de _mocks_ et de scripts de tests automatisés autonomes, ils ont acquis la capacité de faire des tests de non-régression de leurs applications.

#### Mac, Windows, Google, Flickr, Web 2.0

#### Mac, Windows, Google, Flickr, Web 2.0

In the early 1990s, MacIntosh applications such as word processor applications were required to have API-drivable interfaces, so that applications and user-written scripts could access all the functions of the applications. Windows desktop applications have evolved the same ability (I don’t have the historical knowledge to say which came first, nor is that relevant to the point).

Au début des années 90, les applications Macintosh telles que les applications de traitement de texte devaient avoir des interfaces pilotables par API, afin que d'autres applications ou des scripts faits par des utilisateurs puissent accéder à l'ensemble des fonctionnalités des applications. Les applications de bureau sur Windows ont depuis évolué pour avoir les mêmes possibilités (Je n'ai pas de connaissances historiques suffisantes pour savoir laquelle de ces deux plateformes a eu cette possibilité en premier, mais ce n'est pas important dans le cadre de cet article).

The current (2005) trend in web applications is to publish an API and let other web applications access those APIs directly. Thus, it is possible to publish local crime data over a Google map, or create web applications that include Flickr’s photo archiving and annotating abilities.

La tendance actuelle (en 2005) pour les applications web est de mettre à disposition une API et de laisser d'autres applications web accéder à celles-ci directement. Par exemple, il est possible de diffuser des données relatives aux crimes locaux sur une carte Google ou de créer des applications web qui incluent les fonctionnalités de Flickr d'archivage et d'annotations de photos.

All of these examples are about making the ‘’primary ‘’ports’ APIs visible. We see no information here about the secondary ports.

Tous ces exemples portent sur le fait de rendre visible les API des « ports primaires ». Ils n'évoquent en rien l'existence de ports secondaires. 

#### Stored Outputs

#### Sorties stockées

This example written by Willem Bogaerts on the C2 wiki:

Cet exemple a été écrit par Willem Bogaerts sur le wiki C2 :

“I encountered something similar, but mainly because my application layer had a strong tendency to become a telephone switchboard that managed things it should not do. My application generated output, showed it to the user and then had some possibility to store it as well. My main problem was that you did not need to store it always. So my application generated output, had to buffer it and present it to the user. Then, when the user decided that he wanted to store the output, the application retrieved the buffer and stored it for real.

« J'ai déjà été confronté à quelque chose de similaire, mais cela était dû principalement à ma couche applicative qui avait fini par ressembler à un central téléphonique gérant des choses qu'elle n'avait pas vocation à gérer. Mon application générait la sortie, la montrait à l'utilisateur et avait aussi la possibilité de la stocker. Mon principal problème étant qu'il n'était pas toujours nécessaire de la stocker. Donc mon application générait la sortie vers un tampon et la présentait.à l'utilisateur. Celui-ci décidait alors s'il voulait la stocker, l'application la récupérait alors du tampon et la stockait pour de vrai. 

I did not like this at all. Then I came up with a solution: Have a presentation control with storage facilities. Now the application no longer channels the output in different directions, but it simply outputs it to the presentation control. It’s the presentation control that buffers the answer and gives the user the possibility to store it.

En fait, je n'aimais pas du tout cette situation. Puis je suis arrivé à une solution : mettre en place un contrôle de la (couche de) présentation avec des capacités de stockage. Aujourd'hui l'application n'oriente plus la sortie à tel ou tel endroit, mais elle l'envoie au contrôle de la présentation. C'est celui-ci qui met en tampon la réponse et donne à l'utilisateur la possibilité de la stocker.

The traditional layered architecture stresses “UI” and “storage” to be different. The Ports and Adapters Architecture can reduce output to being simply “output” again. ”

L'architecture traditionnelle en couche insiste pour que « l'IHM » et le « stockage » soit différentes. L'architecture _Ports & Adapters_ peut restreindre la sortie de telle manière à ce qu'elle ne soit plus qu'une simple « sortie » à nouveau ».

#### Anonymous example from the C2-wiki

#### Exemple anonyme issu du wiki C2

“In one project I worked on, we used the SystemMetaphor of a component stereo system. Each component has defined interfaces, each of which has a specific purpose. We can then connect components together in almost unlimited ways using simple cables and adapters.”

« Dans un projet sur lequel j'ai travaillé, nous avons utilisé le `_SystemMetaphor_` pour un composant système stéréo. Chaque composant avait des interfaces définies, chacune ayant un but spécifique. Nous avons pu alors y connecter plusieurs composants ensemble pour ainsi dire de manière illimitée en utilisant simplement des câbles et des adaptateurs. »

#### Distributed, Large-Team Development

#### Développement avec des équipes de grande taille distribuées

This one is still in trial use and so does not properly count as a use of the pattern. However, it is interesting to consider.

Ce cas d'usage de l'architecture hexagonale est en cours d'évaluation et ne peut donc pas être tout à fait considéré comme une utilisation éprouvée de ce _pattern_. Toutefois, il est intéressant de regarder en quoi il consiste.

Teams in different locations all build to the Hexagonal architecture, using FIT and mocks so the applications or components can be tested in standalone mode. The CruiseControl build runs every half hour and runs all the applications using the FIT+mock combination. As application subsystem and databases get completed, the mocks are replaced with test databases.

Dans ce cas d'usage, les équipes sont réparties en différents lieux géographiques, elles élaborent ensemble une solution logicielle en architecture hexagonale en utilisant FIT et des _mocks_ afin que les applications ou les composants puissent être testés de manière indépendante. La compilation avec CruiseControl est faite toutes les demi-heure sur l'ensemble des applications à l'aide de la combinaison FIT + _mock_. Au fur et à mesure que le sous-système applicatif et les sous-systèmes de bases de données sont terminées, les _mocks_ sont remplacés par de « vraies » bases de données de test.

#### Separating Development of UI and Application Logic

#### Séparer le développement de l'IHM de la logique applicative.

This one is still in early trial use and so does not count as a use of the pattern. However, it is interesting to consider.

Ce cas d'usage de l'architecture hexagonale en est au tout début de son évaluation et ne peut donc pas vraiment être considéré comme une utilisation éprouvée de ce _pattern_. Regardons en quoi il consiste.

The UI design is unstable, as they haven’t decided on a driving technology or a metaphor yet. The back-end services architecture hasn’t been decided, and in fact will probably change several times over the next six months. Nonetheless, the project has officially started and time is ticking by.

(Quelques éléments de contexte - NdT) Aucune décision n'ayant été vraiment prise au niveau de la technologie à utiliser ou au niveau de la métaphore de navigation, la conception de l'IHM est actuellement immature. L'architecture des services côté _back-end_ n'a pas été non plus décidée et il y a de fortes chances que tout cela changera plusieurs fois dans les 6 mois à venir. Toutefois, le projet a été officiellement lancé et l'horloge tourne.

The application team creates FIT tests and mocks to isolate their application, and creates testable, demonstrable functionality to show their users. When the UI and back-end services decisions finally get met, it “should be straightforward” to add those elements the application. Stay tuned to learn how this works out (or try it yourself and write me to let me know).

L'équipe du côté logique applicative a créé des tests FIT et des _mocks_ pour isoler leur application et elle crée des fonctionnalités testables et démontrables à ses utilisateurs. Lorsque les décisions concernant l'IHM et les services seront finalement prises, cela « devrait être une formalité » d'ajouter ces éléments à l'application. Tenez-vous au courant en venant lire ici pour savoir comment cela avance (ou essayez vous-même de votre côté et écrivez-moi).

### Related Patterns

### _Patterns liés_

#### Adapter

#### _Adapter_

The ‘’Design Patterns’’ book contains a description of the generic ‘’Adapter’’ pattern: “Convert the interface of a class into another interace clients expect.” The ports-and-adapters pattern is a particular use of the ‘’Adapter’’ pattern.

L'ouvrage « _Design Patterns_ » comporte la description d'un _pattern_ « _Adapter_ » générique : « Convertir l'interface d'une classe en une autre interface que les clients attendent ». Le _pattern_ Ports & _Adapters_ est une utilisation spécifique du _pattern_ « _Adapter_ ».

#### Model-View-Controller

#### Modèle - Vue - Contrôleur

The MVC pattern was implemented as early as 1974 in the Smalltalk project. It has been given, over the years, many variations, such as Model-Interactor and Model-View-Presenter. Each of these implements the idea of ports-and-adapters on the primary ports, not the secondary ports.

L'implémentation la plus ancienne connue du _pattern_ MVC a été en 1974 dans un projet Smalltalk. Il a connu au cours des années différentes variations, comme les  _patterns_ `Model-Interactor` et `Model-View-Presenter`. Toutes ces variations implémentent l'idée des ports primaires du _pattern_ `Ports & _Adapters_` mais pas celle des ports secondaires.

#### Mock Objects and Loopback

#### Objects _Mocks_ et Loopback (rebouclage)

“A mock object is a “double agent” used to test the behaviour of other objects. First, a mock object acts as a faux implementation of an interface or class that mimics the external behaviour of a true implementation. Second, a mock object observes how other objects interact with its methods and compares actual behaviour with preset expectations. When a discrepancy occurs, a mock object can interrupt the test and report the anomaly. If the discrepancy cannot be noted during the test, a verification method called by the tester ensures that all expectations have been met or failures reported.” — From [http://MockObjects.com](http://MockObjects.com)

« Un objet _mock_ est un “ agent double ” utilisé  pour tester le comportement d'autres objets. tout d'abord un objet _mock_ se comporte comme une fausse implémentation d'une interface ou d'une classe et en imite son comportement extérieur. Ensuite, un objet _mock_ observe comment les autres objets interagissent avec ses méthodes et comparent le comportement observé avec le comportement attendu pré paramétré. Lorsqu'une divergence apparaît, un objet _mock_ peut interrompre le test et rapporter l'anomalie. Si la divergence ne peut être rapporté lors des tests, un appel de méthode de vérification effectué par le testeur s'assurera que tous les attendus aient été atteints ou que les anomalies aient été rapportées » — extrait de la page [http://MockObjects.com](http://MockObjects.com)

Fully implemented according to the mock-object agenda, mock objects are used throughout an application, not just at the external interface The primary thrust of the mock object movement is conformance to specified protocol at the individual class and object level. I borrow their word “mock” as the best short description of an in-memory substitute for an external secondary actor.

Si le _mock_ est complètement implémenté celui-ci peut être utilisé à part entière au sein de l'application, et pas uniquement en tant qu'interface externe. Le périmètre initial des objets _mock_ est de se conformer au protocole spécifié au niveau d'une classe donnée ou d'un objet donné. Je me suis permis d'emprunté leur mot _mock_ car il s'agit de la description qui correspond le mieux à un substitut en mémoire pour un acteur secondaire externe.

The Loopback pattern is an explicit pattern for creating an internal replacement for an external device.

Le _pattern_ `Loopback` est un _pattern_ explicite pour créer un remplacement interne pour un périphérique externe.

#### Pedestals

#### _Pattern Pedestals_

In “Patterns for Generating a Layered Architecture”, Barry Rubel describes a pattern about creating an axis of symmetry in control software that is very similar to ports and adapters. The ‘’Pedestal’’ pattern calls for implementing an object representing each hardware device within the system, and linking those objects together in a control layer. The ‘’Pedestal’’ pattern can be used to describe either side of the hexagonal architecture, but does not yet stress the similarity across adapters. Also, being written for a mechanical control environment, it is not so easy to see how to apply the pattern to IT applications.

Dans son ouvrage « Patterns for Generating a Layered Architecture », Barry Rubel décrit un _pattern_ permettant de créer un axe de symétrie pour contrôler un logiciel qui est très similaire au _pattern_ `Ports & Adapters`. Le _pattern_ `Pedestal` incite à implémenter un objet représentant un périphérique matériel au sein du système et à lier ces objets ensemble  dans une couche de contrôle.  Le _pattern_ `Pedestal`peut être utilisé pour décrire les deux côtés (interne et externe) de l'architecture hexagonale, mais n'insiste pas sur la similarité au niveau des _adapters_. De plus, il a été écrit dans le cadre d'un environnement de contrôle mécanique, il n'est pas évident de prime abord de voir comment il peut s'appliquer à des applications informatiques.

#### Checks

#### Vérifications

Ward Cunningham’s pattern language for detecting and handling user input errors, is good for error handling across the inner hexagon boundaries.

Le langage de _pattern_ développé par Ward Cunningham pour détecter et gérer les erreurs de saisies des utilisateurs est très bien adapté pour gérer les erreurs traversant les frontières de l'hexagone interne.

#### Dependency Inversion (Dependency Injection) and SPRING

#### Inversion de dépendance (injection de dépendance) et SPRING

Bob Martin’s Dependency Inversion Principle (also called Dependency Injection by Martin Fowler) states that “High-level modules should not depend on low-level modules. Both should depend on abstractions. Abstractions should not depend on details. Details should depend on abstractions.” The ‘’Dependency Injection ‘’pattern by Martin Fowler gives some implementations. These show how to create swappable secondary actor adapters. The code can be typed in directly, as done in the sample code in the article, or using configuration files and having the SPRING framework generate the equivalent code.

Le principe d'inversion de dépendance de Bob Martin (appelé également injection de dépendance par Martin Fowler) définit que « les modules de haut niveau ne devraient pas dépendre de modules de bas niveau. Les deux devraient dépendre d'abstractions. Les abstractions ne devraient pas dépendre de détails. Les détails devraient dépendre d'abstractions ».  Le _pattern_ d' « injection de dépendance » de Martin Fowler donne quelques exemples d'implémentations. Ces derniers montrent comment créer des adaptateurs d'acteurs secondaires interchangeables. Le code peut être saisit directement, tel que cela est fait dans l'exemple de code dans cet article, ou utilisé via des fichiers de configuration puis le code équivalent est généré via le _framework_ `SPRING`.

### Acknowledgements

### Remerciements

Thanks to Gyan Sharma at Intermountain Health Care for providing the sample code used here. Thanks to Rebecca Wirfs-Brock for her book ‘’Object Design’’, which when read together with the ‘’Adapter’’ pattern from the ‘’Design Patterns’’ book, helped me to understand what the hexagon was about. Thanks also to the people on Ward’s wiki, who provided comments about this pattern over the years (e.g., particularly Kevin Rutherford’s [http://silkandspinach.net/blog/2004/07/hexagonal_soup.html](http://silkandspinach.net/blog/2004/07/hexagonal_soup.html)).

Je tiens à remercier Gyan Sharma d'Intermountain Health Care pour m'avoir fourni les exemples de code présents dans cet article. Je remercie également Rebecca Wirfs-Brock pour son ouvrage « Object Design » qui conjugué à la lecture du _pattern « Adapter »_ dans l'ouvrage « Design Pattern » m'a aidé à comprendre ce qu'était l'architecture hexagonale. Merci aussi à toutes les personnes qui via le wiki de Ward m'ont donné de précieux commentaires sur ce _pattern_ ces dernières années (et tout particulièrement Kevin Rutherford [http://silkandspinach.net/blog/2004/07/hexagonal_soup.html](http://silkandspinach.net/blog/2004/07/hexagonal_soup.html)).

### References and Related Reading

### Bibilographie et lectures recommandées

FIT, A Framework for Integrating Testing: Cunningham, W., disponible en ligne à l'adresse suivante [http://fit.c2.com](http://fit.c2.com), ainsi que l'ouvrage « Fit for Developing Software », aux éditions Prentice-Hall PTR, 2005 par Mugridge, R. et Cunningham, W., 

Le _pattern_ « Adapter » figure dans l'ouvrage « Design Patterns », Addison-Wesley, 1995, pp. 139-150. par Gamma, E., Helm, R., Johnson, R., Vlissides, J.,

Le _pattern_ « Pedestal » évoqué par Rubel, B. évoqué dans son ouvrage , et aussi dans « Patterns for Generating a Layered Architecture » écrit par , par Coplien, J., Schmidt, D., « PatternLanguages of Program Design », Addison-Wesley, 1995, pp. 119-150.

Le _pattern_ « Checks » de W. Cunningham, W., disponible en ligne à l'adresse suivante [http://c2.com/ppr/checks.html](http://c2.com/ppr/checks.html)

Le « Principe d'inversion de dépendance » évoqué dans l'ouvrage  « Agile Software Development Principles Patterns and Practices » de Robert C. Martin, Prentice Hall, 2003, dans le chapitre 11 « The Dependency-Inversion Principle » ainsi qu'en ligne sur la page [http://www.objectmentor.com/resources/articles/dip.pdf](http://www.objectmentor.com/resources/articles/dip.pdf)

Le _pattern_ d' « Injection de dépendance » de M. Fowler disponible en ligne à l'adresse suivante  [http://www.martinfowler.com/articles/injection.html](http://www.martinfowler.com/articles/injection.html)

Le _pattern_ « Mock Object » de S. Freeman, S. disponible en ligne à l'adresse suivante [http://MockObjects.com](http://MockObjects.com)

Le _pattern_ « Loopback » d'A. Cockburn disponible en ligne à l'adresse suivante [http://c2.com/cgi/wiki?LoopBack](http://c2.com/cgi/wiki?LoopBack)

Les « cas d'utilisation » expliqués en détail dans « Rédiger des cas d'utilisation efficaces »  par A. Cockburn, Addison-Wesley, 2001, ainsi que dans Cockburn, A.,« Structurer les cas d'utilisation à l'aide de buts », disponible en ligne à l'adresse suivante [http://alistair.cockburn.us/crystal/articles/sucwg/structuringucswithgoals.htm](http://alistair.cockburn.us/crystal/articles/sucwg/structuringucswithgoals.htm)

* * *

Comments from the old site:

Commentaires de l'ancien site :

* * *

André Boonzaaijer’s blog [While True](http://whiletrue.nl/blog/?p=28) discusses an application using the [Hexagonal architecture](https://alistair.cockburn.us/Hexagonal+architecture) [(discussion: Re: Hexagonal architecture)](https://alistair.cockburn.us/Re%3a+Hexagonal+architecture) and also has a cool picture of the architecture.

Dans un de ses articles sur son blog [While True](http://whiletrue.nl/blog/?p=28) André Boonzaaijer évoque une application élaborée avec l' [architecture hexagonale](https://alistair.cockburn.us/Hexagonal+architecture) [(discussion: Re: Hexagonal architecture)](https://alistair.cockburn.us/Re%3a+Hexagonal+architecture)

Kevin Rutherford has started several notes and discussions around it:
Kevin Rutherford a écrit plusieurs notes et a lancé plusieurs discussions à propos de l'architecture hexagonale que vous pouvez retrouver dans les pages suivantes :

> [Gravity and software adaptability](http://silkandspinach.net/2005/11/28/gravity-and-software-adaptability)  
> [Hexagonal architecture](http://wordpress.com/tag/hexagonalarchitecture)  
> [Databases as life-support for domain objects](http://silkandspinach.net/2005/05/23/databases-as-life-support-for-domain-objects)  
> [Hexagonal soup](http://silkandspinach.net/2004/07/16/hexagonal-soup)

Timo wrote a piece called [Wrap it thinly](http://ng-embedded.blogspot.com/2007/07/wrap-it-thinly.html) about its use with TDD.
Timo a écrit ce bref article intitulé [Wrap it thinly](http://ng-embedded.blogspot.com/2007/07/wrap-it-thinly.html) sur l'utilisation de l'architecture hexagonale conjointement avec le développement piloté par les tests.

Gerard Meszaros in his book on Xunit patterns wrote [http://xunitpatterns.com/Hexagonal%20Architecture.html](http://xunitpatterns.com/Hexagonal%20Architecture.html).
Dans son ouvrage traitant des _patterns_ Xunit Gerard Meszaros y évoque l'architecture hexagonale que vous pouvez retrouver à l'adresse suivante : [http://xunitpatterns.com/Hexagonal%20Architecture.html](http://xunitpatterns.com/Hexagonal%20Architecture.html).

Brian Anderson spent several blog entries noodling over it:
Brian Anderson a écrit plusieurs articles de blog sur le sujet dont voici les liens :

> [Success!](http://www.brianmandersen.com/blog/2005/03/29/success)  
> [Problems with Smart Clients today](http://www.brianmandersen.com/blog/2005/04/02/the-turning-point-for-smart-clients)  
> [compile time vs runtime views](http://www.brianmandersen.com/blog/2005/04/02/compile-time-vs-runtime-views)  
> [the use of symmetry in the hexagonal approach](http://www.brianmandersen.com/blog/2005/04/04/the-use-of-symmetry-in-the-hexagonal-approach)  
> [Back to Hexagonal Architecture](http://www.brianmandersen.com/blog/2005/04/07/back-to-hexagonal-architecture)  
> [some thoughts on the “Design Pattern” pattern](http://www.brianmandersen.com/blog/2005/06/05/some-thoughts-on-the-design-pattern-idea)  
> [http://www.brianmandersen.com/blog/page/2/](http://www.brianmandersen.com/blog/page/2/)

The original page was on Ward’s wiki at [http://c2.com/cgi/wiki?HexagonalArchitecture](http://c2.com/cgi/wiki?HexagonalArchitecture)
La page d'origine sur l'architecture hexagonale est disponible sur le wiki de Ward à l'adresse suivante [http://c2.com/cgi/wiki?HexagonalArchitecture](http://c2.com/cgi/wiki?HexagonalArchitecture)

* * *

### Utah Code Camp Sept 19, 2009 : Coding Assignment

### Utah Code Camp Sept 19, 2009 : mission codage

The simplest application comes with the FIT documentation. It is a simple discount computing application:

L'exemple d'application ci-dessous, une application de calcul de remise commerciale, illustre de la manière la plus simple possible ce qu'est concrètement l'architecture ports et adaptateurs. Il est fourni avec la documentation FIT qui va bien.

~~~ java
discount(amount) = amount * discountRate(amount);
~~~

- ‘Amount’ comes from the user or a test framework (or a file)
- ‘Rate’ comes from a database or an in-memory mock of a database

- La variable `amount` est saisie par l'utilisateur ou provient du _framework_ de test (ou d'un fichier)
- La variate `rate` provient d'une base de données ou d'une base de données _mock_ en mémoire

Implement the pp in stages:

Implémenter le pp en étapes :

1. Input from a test framework, using a constant for the discountRate,
2. Input from a GUI, still using a constant for the discountRate.
3. Input from either test or GUI, discountRate from a mock database that can be swapped out for a real database.

1. Les données en entrée proviennent du _framework_ de test, une constante est utilisée pour le taux `discountRate`.
2. Les données en entrée sont saisies via une IHM, le taux `discountRate` est toujours une constante.
3. Les données en entrée proviennent soit des tests soit d'une IHM, le taux `discountRate` provient d'une base de données _mock_ qui peut être dans le futur échangée avec une vraie base de données.


* * *

### Ruby / Rack (no Rails) implementation

### Implémentation en Ruby / Rack (sans Rails)

I made a small web reader version of this, see it at

J'ai fait une petite version web de cette application, vous la consulter à l'adresse suivante [https://github.com/totheralistair/SmallerWebHexagon](https://github.com/totheralistair/SmallerWebHexagon)

That one takes either browser, or Rack driver, or just a test driver on the left side, and either a constant, or in-code, or from-a-file rate db on the right side. I wrote this to show the implementation in a simple but real (2014) setting.

Celle-ci utilise du côté gauche un navigateur, un pilote Rack ou simplement un pilote de test et du côté droit une constante, du code ou un fichier de base de données. Je l'ai écrite en 2014 pour montrer une implémentation simple mais concrète de cette architecture. 


* * *

## Other discussions and implementations

## Autres discussions et implémentations

You can find more online about this architecture by searching through Google or Twitter (in particular). Also see:
Vous pouvez bien sûr trouver d'autres ressources à propos de l'architecture hexagonale en cherchant via Google ou via Twitter notamment. Vous pouvez aussi consulter : 

- Cet article de Thierry Pierrain [http://tpierrain.blogspot.fr/2013/08/a-zoom-on-hexagonalcleanonion.html](http://tpierrain.blogspot.fr/2013/08/a-zoom-on-hexagonalcleanonion.html)
- Le support de la présentation que j'ai pu donner à l'Utah Code  [http://alistair.cockburn.us/Hexagonal+Architecture+Keynote+at+Utah+Code+Camp+September+2009.pps](http://alistair.cockburn.us/Hexagonal+Architecture+Keynote+at+Utah+Code+Camp+September+2009.pps)
- une autre axe de présentation de l'architecture hexagonale fait par Duncan Nisbet sous l'angle de prises de notes faites à sa propre intention [http://www.duncannisbet.co.uk/hexagonal-architecture-for-testers-part-1](http://www.duncannisbet.co.uk/hexagonal-architecture-for-testers-part-1)
- Une courte vidéo d'une présentation que j'ai donné lors de la conférence Mountain West Ruby en 2010: [Video of Alistairs hexagonal architecture CQRS lightning talk Mountain West Ruby Conference 2010](https://alistair.cockburn.us/Video+of+Alistairs+hexagonal+architecture+CQRS+lightning+talk+Mountain+West+Ruby+Conference+2010) [(discussion: Re: Video of Alistairs hexagonal architecture CQRS lightning talk Mountain West Ruby Conference 2010)](https://alistair.cockburn.us/Re%3a+Video+of+Alistairs+hexagonal+architecture+CQRS+lightning+talk+Mountain+West+Ruby+Conference+2010)
- en recherchant directement sur Twitter à l'aide de ce lien [https://twitter.com/search?q=%22hexagonal%20architecture%22](https://twitter.com/search?q=%22hexagonal%20architecture%22)
- ce tweet [http://twitter.com/andrzejkrzywda/status/267420878487310336](http://twitter.com/andrzejkrzywda/status/267420878487310336)
- ce minuscule CMS implémentant l'architecture hexagonale (avec uniquement un port du côté utilisateur) [https://github.com/totheralistair/SmallWebHexagon](https://github.com/totheralistair/SmallWebHexagon)
- Pat Maddox a fait un autre exemple intégrant architecture hexagonale, programmation évènementielle et le _pattern_ CQRS [https://github.com/patmaddox/hexarch2](https://github.com/patmaddox/hexarch2). Jetez-y un coup d'œil.
- Un très bel échange vidéo sur l'architecture hexagonale et Rails entre BadrinathJanakiraman et Martin Fowler: [http://thoughtworks.wistia.com/medias/uxjb0lwrcz](http://thoughtworks.wistia.com/medias/uxjb0lwrcz)
- le récit d'une réflexion sur [https://github.com/Lunch-box/SimpleOrderRouting/wiki/Logbook-4#day-15-october-27th-2014](https://github.com/Lunch-box/SimpleOrderRouting/wiki/Logbook-4#day-15-october-27th-2014)

* * *

### Configurable Dependencies, Primary and Secondary Actors

### Dépendances configurables, acteurs primaires et secondaires

I tried to make this pattern truly symmetric, hence the hexagon. However, watching several implementations, it slowly became clear that there is an asymmetry (which is one thing that makes this fundamentally different from neighboring patterns such as the onion architecture). As stated above (see The Left-Right Asymmetry), the asymmetry matches Ivar Jacobson’s **primary** and **secondary actors** concept, and affects how the [Configurable Dependency](https://alistair.cockburn.us/Configurable+Dependency) [(discussion: Re: Configurable Dependency)](https://alistair.cockburn.us/Re%3a+Configurable+Dependency) is implemented. (This is shown briefly in the Configurable Dependency sketch:

J'ai essayé de faire en sorte que ce _pattern_ soit vraiment symétrique, d'où l'hexagone. Toutefois en regardant plusieurs de ses implémentations, il est devenu clair avec le temps qu'il existe une asymétrie (ce qui rend l'architecture hexagonale fondamentalement différentes des autres _patterns_ comme l'architecture en oignon). Cette asymétrie décrite précédemment (cf. l'asymétrie gauche-droite) rejoint le concept d'Ivar Jacobson d'**acteurs primaires** et **secondaires** et impacte la manière dont la Dépendance Configurable peut être implémentée comme nous pouvons le deviner sur ce dessin :

![Configurable Dependency illustrated1-800pxV.jpg](https://alistair.cockburn.us/wp-content/uploads/2018/02/Configurable-Dependency-illustrated1-800pxV.jpg "Configurable Dependency illustrated1-800pxV.jpg")  
[Configurable Dependency illustrated1-800pxV.jpg](https://alistair.cockburn.us/Configurable+Dependency+illustrated1-800pxV.jpg) [(discussion: Re: Configurable Dependency illustrated1-800pxV.jpg)](https://alistair.cockburn.us/Re%3a+Configurable+Dependency+illustrated1-800pxV.jpg)

The difference between a primary and secondary actor lies only in who _initiates_ the conversation. A **primary actor** knows about and initiates the conversation with the system or application; for a **secondary actor**, it is the system or application that knows about and initiates the discussion with the other. That is actually the only difference between the two, in use case land.

Cette différence entre acteur primaire et secondaire repose uniquement sur lequel des deux _initie_ la conversation. Un **acteur primaire** sait le propos de cette conversation et l'initie avec le système ou l'application ; pour un **acteur secondaire**, c'est le système ou l'application qui sait le propos et qui initie la discussion avec autrui. C'est en réalité la seule différence entre les deux au pays des cas d'utilisation en tout cas. 

In implementation, that difference matters: Whomever will initiate the conversation must be handed the handle for the other.

Au niveau de l'implémentation, cette différence est importante : quiconcque initiera la conversation doit passer le relais à l'autre.

In the case of **primary actor ports**, the macro constructor will pass to the UI, test framework, or driver the handle for the app and say, “Go talk to that”. The primary actor will call into the app, and the app will probably never know who called it. (That is normal for recipients of a call).

Dans le cas des **ports de l'acteur primaire**, le constructeur macro devra passer le relais à l'IHM, le _framework_ de test ou au pilote de l'application et lui dire « allez, parle-lui ». L'acteur primaire parlera alors à l'app et l'app ne saura probablement jamais qui l'a appelé. (Ce qui est normal pour les destinataitres d'un appel).

In stark contrast, for **secondary actor ports**, the macro constructor will pass to the UI, test framework, or driver the handle for the secondary actor to be used, that will get passed in as a parameter to the app, and the app will now know who/what is the recipient of the outgoing call. (This is again normal for sending out a call).

En contraste, dans le cas des **ports de l'acteur secondaire**, le constructeur macro devra passer le relais à l'IHM, le _framework_ de test ou au pilote à l'acteur secondaire identifié passé en paramètre à l'application, et c'est l'application qui saura désormais qui/quel est le destinataire de l'appel sortant. (Ce qui est là aussi normal lorsque l'on émet un appel).

Thus, the system or application is constructed differently for primary and secondary actor ports: ignorant and initially passive for the primary actors, and having a way to store and call out to the secondary actor ports.

Par conséquent, le système ou l'application sera construite différemment pour les ports des acteurs primaires et secondaires : d'une part ignorante et initialement passive pour les acteurs primaires et d'autre part avoir une manière de stocker et d'appeler les ports des acteurs secondaires.

Both ports implement [Configurable Dependency](https://alistair.cockburn.us/Configurable+Dependency) [(discussion: Re: Configurable Dependency)](https://alistair.cockburn.us/Re%3a+Configurable+Dependency), but differently.

Ces deux types de ports implémentent la [Dépendance Configurable]https://alistair.cockburn.us/Configurable+Dependency) [(discussion: Re: Configurable Dependency)](https://alistair.cockburn.us/Re%3a+Configurable+Dependency), mais de manière différente.

Simple example for a 3-port system, such as a coffee machine or a hospital medical unit dispensing medications intravenously (How odd that they come out the same, architecturally!):

Voici un exemple simple d'un système à 3 ports comme une machine à café, une unité médicale de distribution par intraveineuse (cela paraît vraiment étrange que les deux partagent la même architecture)

- The purchaser, test harness or hospital admin is a primary actor driving the system
- The recipe database or medical database is a secondary actor, offering its information
- The chemical dispensers in either are secondary actors.

- L'acheteur, l'harnais de test ou l'administrateur de l'hôpital est l'acteur primaire qui pilote le système
- La base de données de recettes ou la base de données médicale est l'acteur secondaire qui délivre ses informations
- Le système de distribution (café ou médicamenteux) est dans les deux cas des acteurs secondaires.

End result: the primary / secondary aspect of a port cannot be ignored.

En conclusion : l'aspect primaire / secondaire d'un port ne peut pas être ignoré

* * *

See also [Hexagonal Architecture FAQ](https://alistair.cockburn.us/Hexagonal+Architecture+FAQ) [(discussion: Re: Hexagonal Architecture FAQ)](https://alistair.cockburn.us/Re%3a+Hexagonal+Architecture+FAQ)

Vous pouvez aussi vous reporter à la [FAQ Architecture hexagonale](https://alistair.cockburn.us/Hexagonal+Architecture+FAQ) [(discussion: Re: Hexagonal Architecture FAQ)](https://alistair.cockburn.us/Re%3a+Hexagonal+Architecture+FAQ)


---
Auteur : [Alistair Cockburn](https://alistair.cockburn.us)  
Source : [Hexagonal architecture](https://alistair.cockburn.us/hexagonal-architecture/)  
Date de parution originale : 04 Janvier 2005  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 06/11/2023  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}


[^1]: Ports et adaptateurs
[^2]: littéralement sans tête c'est-à-dire sans interface utilisateur
[^3]: un mock simule l'existence d'un véritable service comme une base de données, on peut employer en français le terme de simulacre
[^4]: un pattern est une structure, un modèle permettant de répondre à certaines problématiques connues
[^5]: une fixture est un morceau de code qui permet de figer (fixer) un environnement logiciel pour exécuter des tests logiciels. Cet environnement constant est toujours le même à chaque exécution des tests. Il permet de répéter les tests indéfiniment et d'avoir toujours les mêmes résultats. (source : [wikipedia](https://fr.wikipedia.org/wiki/Test_fixture))
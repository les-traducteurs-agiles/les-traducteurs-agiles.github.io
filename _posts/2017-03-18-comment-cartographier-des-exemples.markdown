---
layout: post
title:  "Présentation de la carte des exemples"
date:   2017-03-18 00:00:01
published: true
tags: 
- user story
- outils
---

![Cartes et stylos]({{ site.url }}assets/cartographier_exemples/titre_cartographie_exemple.png)

Avant de mettre en développement une _user story_, avoir une [conversation pour clarifier et valider](http://wiki.ayeba.fr/XP%2C+l%27essentiel+-+Carte%2C+Conversation%2C+Confirmation) les critères d’acceptation est vital.

Certaines personnes le font pendant leurs sessions d’affinage de _backlog_ ou de _planning poker_. D’autres équipes font une réunion spécifique des [trois amigos](http://www.velocitypartners.net/blog/2014/02/11/the-3-amigos-in-agile-teams/), un [atelier de spécification](http://gojko.net/2008/11/12/specification-workshops-an-agile-way-to-get-better-requirements/) ou de [découverte](http://dannorth.net/2010/08/30/introducing-deliberate-discovery/). 

Peu importe le nom que vous donnez à cette conversation, un certain nombre d’équipes éprouvent des difficultés à la tenir : la conversation n’est pas structurée, elle est trop longue et ennuyeuse. Par conséquent, ces réunions ne sont pas faites régulièrement ou systématiquement, ou abandonnées tout simplement.

J’ai découvert une méthode simple, rudimentaire pour faire en sorte que cette conversation demeure la plus brève possible tout en restant très productive. Je la nomme la [carte des exemples](https://twitter.com/search?q=%23ExampleMapping).

## Comment ça marche ?

Les exemples concrets sont des moyens formidables pour nous permettre d’explorer le domaine d’un problème, ils constituent le socle sur lequel se baseront nos tests d’acceptation. Mais au fur et à mesure que nous discutons des exemples, d’autres choses émergent de la conversation qui méritent également d’être notés, il s’agit :

* des _règles_ qui résument un ensemble d’exemples, ou qui expriment d’autres contraintes qui sont reconnues par tous comme étant présentes au niveau du périmètre de la _story_.
* des _questions_ sur des scénarii dont personne ne sait quel devrait être le résultat. Ou des _hypothèses_ que nous faisons au fur et à mesure que nous avançons.
* de nouvelles _user stories_ que nous découvrons, affinons ou écartons sur ce périmètre.

Pour faire une carte des exemples, il vous faut un [paquet de fiches cartonnées de 4 couleurs différentes](http://www.staples.com/Staples-Assorted-Color-Index-Cards/product_SS1037669) et des stylos pour noter les différents types d’information qui arrivent pendant la conversation. Au cours de la discussion, nous les notons sur les fiches cartonnées et nous les organisons sous la forme d’une carte :

![Carte des exemples]({{ site.url }}assets/cartographier_exemples/cartographie_exemple_fr.jpg)

Nous commençons par écrire la **story** dont nous discutons sur une carte **jaune** et la plaçons en haut de la table.

Ensuite nous écrivons chaque critère d’acceptation, ou **règles** que nous connaissons déjà sur une carte **bleue** et en les plaçant horizontalement en-dessous de la carte jaune.

Pour chaque règle, nous avons besoin d’un ou de plusieurs **exemples**  pour l’illustrer. Nous les écrivons sur des cartes **vertes** que nous plaçons en-dessous de la règle idoine.

Au cours de notre discussion sur ces exemples, nous pouvons découvrir des **questions** pour lesquelles aucune des personnes présentes dans la pièce n’a la réponse. Ces questions, nous les notons sur des cartes **rouges** et poursuivons notre discussion.

Nous continuons jusqu’à ce que le groupe estime que tout le périmètre de la story ait été traité ou que nous soyons à court de temps.

Et voilà. Je vous avais bien dit que c’était simple !

## Retour d’informations immédiat

Au cours de notre conversation, nous construisons une représentation visuelle sur la table en face de nous illustrant notre compréhension en cours de la _story_.

* Une table couverte de cartes rouges (de questions) nous indique que nous avons encore beaucoup à apprendre de cette _story_.
* Une table couverte de cartes bleues (de règles) nous indique que cette _story_ est grosse et compliquée. Peut-être pouvons-nous la fractionner ? C’est le moment de prendre alors un nouvelle carte jaune (_story_) et de mettre cette _story_ fractionnée dans le backlog.
* Une règle avec énormément d’exemples pourrait s’avérer trop complexe. Est-ce qu’il y a plusieurs règles en jeu qui auraient besoin d’être clarifiées ?

Quelque fois, vous trouverez que certaines règles seront si évidentes que vous n’aurez pas besoin d’exemples. La conversation aura été suffisamment claire pour que chacun soit en mesure de comprendre la règle. Super ! Vous pouvez continuez, vous n’êtes pas forcé de pondre des exemples comme des automates BDD[^1] sans cerveaux. 

## Réfléchir dans le temps impartit

Un petit groupe d’amigos devrait être capable de cartographier une story de taille raisonnable en **environ 25 minutes** et ainsi s’en faire une bonne compréhension

Si vous ne pouvez pas, soit c’est parce que vous êtes toujours en train d’essayer de piger le truc (ce qui est normal et bien), soit la _story_ est vraiment trop grosse (ce qui n’est pas bien du tout), soit il reste trop d’incertitude. Soyez bien attentif à cela, et soit vous essayez de continuez en fractionnant la _story_, soit vous laissez repartir la personne du métier et vous allez faire vos devoirs avant de remettre sur le tapis cette _story_ lors d’une prochaine session de cartographie des exemples à une date ultérieure.

Chez Cucumber[^2], après 25 minutes de conversation nous utilisons une technique de vote très rapide, celle du [vote avec le pouce](http://www.conferencesthatwork.com/index.php/event-design/2012/06/testing-consensus-using-roman-voting/), pour déterminer si la story est prête à aller en développement. Même s’il y a quelques questions qui restent, vous pouvez estimer qu’elles sont suffisamment secondaires et que vous pourrez les résoudre lorsque vous y travaillerez. Laissons-le groupe décider.

## Bénéfices

Ce type de carte vous aide à zoomer et à vous concentrer sur les plus petites éléments de comportements présents dans votre _story_. En la cartographiant, vous pouvez clarifier les règles, trouver l’essence même du comportement que vous souhaitez, et différer le reste à plus tard. Avec ce type examen approfondi, une carte des exemples agit comme un filtre, elle empêche les trop grosses _stories_ de s’introduire dans votre sprint et d’exploser en surprises de dernière minute trois jours avant la démo.

Elle permet aussi de gagner du temps, et de continuer d’impliquer l’intérêt des personnes du métier dans le processus.

![Tweet de Lisa Crispin]({{ site.url }}assets/cartographier_exemples/tweet_lisa_crispin.jpg)

Un certain nombre d’équipes pensent que les trois amigos devraient écrire les tests d’acceptations (par exemple sous la forme de scénarios Cucumber[^3]) _lors_ de cette session, en s’asseyant dans une salle avec un projecteur pendant que quelqu’un saisit des scénarios gherkin[^4] dans un environnement de développement. Il y a des moments où cela peut valoir le coup de faire comme cela, mais je pense que c’est généralement une mauvaise idée. Cela nous détourne du véritable objectif de la conversation.

C’est facile de voir pourquoi les personnes font cette erreur : le but apparent est de prendre une _user story_, ayant déjà quelques _critères d’acceptation_ pré-définis, et d’obtenir des _exemples_ qui peuvent être transformés en _tests d’acceptation_.

Je pense que le véritable objectif, est d’obtenir une _compréhension partagée_ de ce qu’il faudra faire pour qu’une story soit terminée. Vous pouvez atteindre cet objectif plus rapidement avec cette technique rudimentaire.

## Où il est question du titre des épisodes dans la série Friends

Donc à la place de vouloir obtenir des scenarii Gherkin complets et formels, essayez seulement de noter une liste d’_exemples bruts_, en utilisant la convention de nommage dite des _épisodes de Friends_[^5].

Par exemple :

* Celui dans lequel le client a perdu sa facture
* Celui dans lequel le produit est endommagé
* Celui dans lequel le produit a été acheté il y a quinze jours

Certaines fois, lorsque l’incertitude monte, instinctivement vous pourriez vouloir  avoir quelque chose de plus concret. À ce niveau-là, vous n’avez pas toujours pas besoin pour l’instant d’avoir recours à la structure rigide _Give When Then_[^6] (Étant donné Quand Alors en VF) :

![Carte verte]({{ site.url }}assets/cartographier_exemples/carte_verte.jpg)

Lorsque le résultat (Then ou Alors en VF) n’est pas clair, alors c’est que vous n’avez pas un exemple mais que vous avez une question.

## Inconnus connus

Lorsqu’une conversation comme celle-ci tourne en rond, c’est parce que vous n’avez pas assez d’informations. C’est sans doute parce qu’il manque quelqu’un pour participer à la conversation, ou peut-être parce que vous devez faire des recherches du côté utilisateur, ou d’essayer quelque [chose](http://www.extremeprogramming.org/rules/spike.html)

![Carte rouge]({{ site.url }}assets/cartographier_exemples/carte_rouge.jpg)

À la place de laisser chacun faire part de son opinion sur ce qu’il pense que le résultat devrait être, essayez simplement de noter la question et de poursuivre. Félicitations ! Vous avez simplement transformé quelque chose d’inconnu inconnu en _inconnu connu_. C’est un net progrès.

Beaucoup de personnes me disent que ce seul aspect de la carte des exemples a transformé leurs atelier de découverte de randonnée sans fin et ennuyeuses à des sessions éclairs de remues-méninges productives.

## Qui devrait venir ?

Au minimum, vos trois amigos : un développeur, un testeur et une personne du métier. C’est juste le strict minimum. Au mieux, invitez les administratifs, les spécialistes en expériences utilisateurs ou toute autre personne jugée pertinente pour la _story_ en cours de discussion. N’importe qui susceptible de vous aider à découvrir de nouvelles questions, ou à transformer les questions en décisions pendant la discussion sera également utile.

Pendant que vous apprenez cette technique, il peut être utile que quelqu’un puisse prendre un rôle formel de facilitateur, dont le boulot sera de faire en sorte que tout ce qui est dit soit noté sur une fiche. Les exemples et les questions fusent rapidement dans la pièce, et cela exige de la discipline de les saisir au vol et de les mettre sur la table afin de visualiser ce dont vous êtes en train de parler.

## Alors quand est-ce que l’on écrit en Gherkin ?

Ne laissez pas cet article vous troubler : il y a un grand intérêt à écrire en Gherkin en même temps aussi, tout spécialement au tout début du projet. C’est à ce moment-là que vous développez votre langage universel et il est vital que ces scénarios  soient exprimés de telle manière à ce que tout le monde dans l’équipe y croit.

Mais exprimer des exemples de cette manière exige une réflexion différente pour décider quels sont les exemples dans le périmètre et clarifier les règles sous-jacentes.

Pour une équipe déjà à niveau ayant un vocabulaire métier plutôt mature, je préfère que la personne du métier consacre son temps et son énergie dans les sessions de cartographie des exemples, et laisser la charge de l’écriture en Gherkin aux deux autres amigos. Une fois qu’ils ont fait un brouillon de spécifications Gherkin, la personne du métier peut alors leur faire un retour.

> Est-ce que c’est comme cela que j’aurais dû l’écrire ?

Cela vous laisse l’opportunité de tester de l’efficacité de la conversation de cartographie des exemples pour transférer la connaissance de la personne du métier à ses amigos 

## À quelle périodicité devrions-nous faire cela ?

Les gens du métier sont souvent occupés. Respectez cela en planifiant ces sessions de telle manière à ce qu’ils soient en capacité de vous donner toute leur attention.

Ma recommandation, basée sur ce que j’ai pu observer dans plusieurs équipes et qui a bien fonctionné en pratique, c’est de les faire fréquemment : un rythme d’un jour sur deux se révèle être souvent un bon rythme. Prenez une et une seule _story_, accordez-lui 25 minutes d’attention, puis chacun retourne vaquer à ses occupations. En faire par paquets de 10 ne ferait qu’épuiser votre énergie. 

## Mais mon équipe est une équipe distribuée !

J’ai observé déjà quelques variations innovantes sur ce type de cartographie : j’ai vu certaines personnes utiliser des listes à puces dans un Google doc partagé, j’en ai vu d’autres utiliser une feuille de calcul avec des cellules colorées pour représenter les cartes. Vous pourriez aussi utiliser une carte heuristique. La clé est que la démarche reste rapide et facile., _afin que vous puissiez vous concentrez sur la conversation_.

## Quelques trucs et astuces pour terminer

Il est important de comprendre clairement la distinction entre [règles et exemples](http://lizkeogh.com/2011/06/20/acceptance-criteria-vs-scenarios/) avant de commencer à utiliser la carte des exemples. J’ai un petit [exercice amusant](https://speakerdeck.com/mattwynne/rules-vs-examples-bddx-london-2014) pour en facilement l’apprentissage que je partagerai avec vous dans un futur proche.

Rappelez-vous que tout l’objectif de cette conversation est de **découvrir des choses que vous ne connaissez pas encore**. Donc il n’y a pas de questions stupides. Prenez plaisir et explorer vraiment à fond le problème.

Vous trouverez que les règles font des lignes de fractures naturelles pour fractionner votre story. Rassurez-vous et soyez à l’aise en différant certains éléments autant que possible, cela vous permettra de vous concentrer sur la résolution du cœur du problème. Vous pourrez ajouter de la sophistication (et de la complexité) plus tard.

> Merci à Janet Gregory, Aslak Hellesøy et Seb Rose pour leur retours sur cet article et à Theo England pour sa patience alors que je perfectionnais mon article, et à Tom Stuart pour [m’avoir sortis les doigts du c…](https://twitter.com/tomstuart/status/673447106506563584)

[^1]: BDD ou Behaviour Driven Development : approche de développement piloté par les tests et plus particulièrement les tests d’acceptation - NdT

[^2]: Nom de l’entreprise dont l’auteur est co-fondateur - NdT

[^3]: C’est aussi le nom du framework de BDD - NdT

[^4]: Langage de description des tests dans Cucumber - NdT

[^5]: Tous les titres des épisodes de la série Friends commencent par The One Where … soit Celui dans lequel - NdT

[^6]: Les mots Given When Then sont les mots-clés utilisés dans la syntaxe Gherkin - NdT

---
Auteur : [Matt Wynne](https://cucumber.io/#company)  
Source : [Introducing Example Mapping](https://cucumber.io/blog/2015/12/08/example-mapping-introduction)  
Date de parution originale : 08 Décembre 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 21/3/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}




---
layout: post
title:  "Comment cartographier des exemples"
date:   2016-03-18 00:00:01
published: false
tags: 
- user story
- outils
---

# Introducing Example Mapping

![Cards and pens](https://cucumber.io/images/blog/example-mapping/title.jpg)

![Cartes et stylos]({{ site.url }}assets/cartographier_exemples/titre_cartographie_exemple.png)


Before you pull a user story into development, it’s crucial to have a [conversation to clarify and confirm](http://ronjeffries.com/xprog/articles/expcardconversationconfirmation/) the acceptance criteria.

Avant de mettre en développement une _user story_, avoir une [conversation pour clarifier et valider](http://wiki.ayeba.fr/XP%2C+l%27essentiel+-+Carte%2C+Conversation%2C+Confirmation) les critères d’acceptation est vital.

Some people do this during their backlog refinement or planning poker sessions. Other teams have a specific [three amigos](http://www.velocitypartners.net/blog/2014/02/11/the-3-amigos-in-agile-teams/) meeting, [specification workshop](http://gojko.net/2008/11/12/specification-workshops-an-agile-way-to-get-better-requirements/) or [discovery workshop](http://dannorth.net/2010/08/30/introducing-deliberate-discovery/).

Certaines personnes le font pendant leurs sessions d’affinage de _backlog_ ou de _planning poker_. D’autres équipes font une réunion spécifique des [trois amigos](http://www.velocitypartners.net/blog/2014/02/11/the-3-amigos-in-agile-teams/), un [atelier de spécification](http://gojko.net/2008/11/12/specification-workshops-an-agile-way-to-get-better-requirements/) ou de [découverte](http://dannorth.net/2010/08/30/introducing-deliberate-discovery/). 

Whatever you call this conversation, many teams find it hard; it’s unstructured, it takes too long and gets boring. The result is they don’t do it regularly or consistently, or maybe they just give up on it entirely.

Peu importe le nom que vous donnez à cette conversation, un certain nombre d’équipes éprouvent des difficultés à la tenir : la conversation n’est pas structurée, elle est trop longue et ennuyeuse. Par conséquent, ces réunions ne sont pas faites régulièrement ou systématiquement, ou tout simplement abandonnées.

I’ve discovered a simple, low-tech method for making this conversation short and powerfully productive. I call it [Example Mapping](https://twitter.com/search?q=%23ExampleMapping).

J’ai découvert une méthode simple, rudimentaire pour faire en sorte que cette conversation reste brève tout en étant très productive. Je la nomme la [cartographie des exemples](https://twitter.com/search?q=%23ExampleMapping).

## How it works

## Comment ça marche ?

Concrete examples are a tremendous way to help us explore the problem domain, and they make a great basis for our acceptance tests. But as we discuss these examples, there are other things coming out in the conversation that deserve to be captured too:

Les exemples concrets sont des outils formidables pour nous permettre d’explorer le domaine d’un problème, ils constituent le socle sur lequel se base nos tests d’acceptation. Mais au fur et à mesure que nous discutons des exemples, d’autres choses émergent de la conversation qui méritent d’être notés également, il s’agit :

* _rules_ that summarise a bunch of examples, or express other agreed constraints about the scope of the story.
* _questions_ about scenarios where nobody in the conversations knows what the right outcome is. Or _assumptions_ we're making in order to progress.
* new _user stories_ we discovered or sliced and deferred out of scope.

* des _règles_ qui résument un ensemble d’exemples, ou qui expriment d’autres contraintes qui sont reconnues par tous comme étant présentes au niveau du périmètre de la _story_.
* des _questions_ sur des scénarii dont personne ne sait quel devrait être le résultat. Ou des _hypothèses_ que nous faisons au fur et à mesure que nous avançons.
* de nouvelles _user stories_ que nous découvrons, affinons ou écartons sur ce périmètre.

Example Mapping uses a [pack of 4-coloured index cards](http://www.staples.com/Staples-Assorted-Color-Index-Cards/product_SS1037669) and some pens to capture these different types of information as the conversation unfolds. As we talk, we capture them on index cards, and arrange them in a map:

Pour faire une cartographie des exemples, il vous faut un [paquet de fiches cartonnées de 4 couleurs différentes](http://www.staples.com/Staples-Assorted-Color-Index-Cards/product_SS1037669) et quelques stylos pour noter les différents types d’information au fur et à mesure du déroulement de la conversation. Au cours de la conversation, nous les notons sur les fiches cartonnées et nous les organisons sous la forme d’une carte :

![Example Mapping](https://cucumber.io/images/blog/example-mapping/map.png)

![Cartographie des exemples]({{ site.url }}assets/cartographier_exemples/cartographie_exemple_fr.jpg)

We start by writing the **story** under discussion on a **yellow** card and placing it at the top of the table.

Nous commençons par écrire la **story** dont nous discutons sur une carte **jaune** et la plaçons en haut de la table.

Next we write each of the acceptance criteria, or **rules** that we already know, on a **blue** card and placing those across the table beneath the yellow story card.

Ensuite nous écrivons chaque critère d’acceptation, ou **règles** que nous connaissons déjà sur une carte **bleue** et en les plaçant horizontalement en-dessous de la carte jaune.

For each rule, we may need one or more **examples** to illustrate it. We write those on a **green** card and place them under the relevant rule.

Pour chaque règle, nous avons besoin d’un ou de plusieurs **exemples**  pour l’illustrer. Nous les écrivons sur des cartes **vertes** que nous plaçons en-dessous de la règle idoine.

As we discuss these examples, we may uncover **questions** that nobody in the room can answer. We capture those on a **red** card and move on with the conversation.

Au cours de notre discussion sur ces exemples, nous pouvons découvrir des **questions** qu’aucune des personnes présentes dans la pièce n’a la réponse. Ces questions, nous les notons sur des cartes **rouges** et poursuivons notre discussion.

We keep going until the group is satisfied that the scope of the story is clear, or we run out of time.

Nous continuons jusqu’à ce que le groupe estime que le périmètre de la story ait été traité ou que nous soyons à court de temps.

And that’s it. I told you it was simple!

Et voilà. Je vous avais bien dit que c’était simple !

## Instant Feedback

## Retour d’informations immédiat

As the conversation flows, we quickly build up a visual representation on the table in front of us reflecting back our current understanding of the story:

Lors de notre conversation, nous construisons une représentation visuelle sur la table en face de nous illustrant notre compréhension en cours de la _story_.

* A table covered in red (question) cards tells us that we still have a lot to learn about this story.
* A table covered in blue (rule) cards tells us that this story is big and complicated. Perhaps we can slice it? Take another yellow (story) card and put the sliced story on the backlog.
* A rule with many examples might be over-complex. Are there multiple rules at play that need to be teased apart?

* Une table couverte de cartes rouges (de questions) nous indique que nous avons encore beaucoup à apprendre de cette _story_.
* Une table couverte de cartes bleues (de règles) nous indique que cette _story_ est grosse et compliquée. Peut-être pouvons-nous la fractionner ? C’est le moment de prendre alors un nouvelle carte jaune (_story_) et de mettre cette _story_ fractionnée dans le backlog.
* Une règle avec énormément d’exemples pourrait s’avérer trop complexe. Est-ce qu’il y a plusieurs règles en jeu qui auraient besoin d’être clarifiées ?

You’ll find that some rules are so obvious you don’t need examples at all. It’s clear from the conversation that everyone understands the rule. Great! You can all move on with your lives without forcing yourselves to grind out examples like BDD-brainwashed automatons.

Quelque fois, vous trouverez que certaines règles seront si évidentes que vous n’aurez pas besoin du tout d’exemples pour celles-ci. La conversation aura été suffisamment claire pour que chacun soit en mesure de comprendre la règle. Super ! Vous pouvez continuez, vous n’êtes pas forcés de pondre des exemples comme des automates BDD sans cerveaux. 

## Thinking inside the time-box

## Réfléchir dans le temps impartit

A small group of amigos should be able to map out a well-understood, well-sized story in **about 25 minutes**.

Un petit groupe d’amigos devrait être capable de cartographier une story de taille raisonnable en **environ 25 minutes** et de s’en faire une bonne compréhension

If you can’t, either you’re still getting the hang of this (which is fine), the story is too big (definitely not fine), or it still has too much uncertainty in it. Listen to that, and either try and slice the story, or let the product person go off and do some homework before you put story back into another example mapping session at a later date.

Si vous ne pouvez pas, soit c’est parce que vous êtes toujours en train d’essayer de piger le truc (ce qui est normal et bien), soit la story est vraiment trop grosse (ce qui n’est pas bien du tout), soit il reste trop d’incertitude. Soyez bien attentif à cela, et soit vous essayez de continuez en fractionnant la story, soit vous laissez repartir la personne du métier et vous allez vos devoirs avant de remettre sur le tapis cette _story_ lors d’une prochaine session de cartographie des exemples à une date ultérieure.

At Cucumber, we use a quick [thumb-vote](http://www.conferencesthatwork.com/index.php/event-design/2012/06/testing-consensus-using-roman-voting/) after 25 minutes to determine whether we think the story is ready to pull into development. Even if there are some questions remaining, you might think they’re minor enough that you can resolve them as you go. Let the group decide.

Chez Cucumber, après 25 minutes nous utilisons une technique de vote très rapide, celle du [vote avec le pouce](http://www.conferencesthatwork.com/index.php/event-design/2012/06/testing-consensus-using-roman-voting/), pour déterminer si la story est prête à aller en développement. Même s’il y a quelques questions qui restent, vous pouvez estimer qu’elles sont suffisamment secondaires et que vous pourrez les résoudre lorsque vous y travaillerez. Laissons-le groupe décider.

## Benefits

## Bénéfices

Example Mapping helps you zoom in and focus on the smallest pieces of behaviour inside your story. By mapping it out you can tease apart the rules, find the core of the behaviour you want, and defer the rest until later. With this level of scrutiny, example mapping acts like a filter, preventing big fat stories from getting into your sprint and exploding with last-minute surprises three days before demo-day.

La cartographie vous aide à zoomer et à vous concentrer sur les plus petites éléments de comportements présents dans votre _story_. En la cartographiant, vous pouvez clarifier les règles, trouver l’essence même du comportement que vous souhaitez, et différer le reste à plus tard. Avec ce type examen approfondi, la cartographie des exemples agit comme un filtre, elle empêche les trop grosses _stories_ de s’introduire dans votre sprint et d’exploser en surprises de dernière minute trois jours avant la démo.

It also saves time, and so helps maintain busy product people’s interest in the process.

Elle permet aussi de gagner du temps, et de continuer d’impliquer l’intérêt des personnes du métier dans le processus.

![Tweet Lisa Crispin](https://cucumber.io/images/blog/example-mapping/lisa-crispin-tweet.png)

![Tweet de Lisa Crispin]({{ site.url }}assets/cartographier_exemples/tweet_lisa_crispin.jpg)

Many teams assume that the three amigos should write acceptance tests (e.g. Cucumber scenarios) _during_ this session, sitting around a projector while someone types formal gherkin scenarios into an IDE. There are occasions when this is valuable, but generally I think it’s a bad idea. It can actually be distracting from the true purpose of the conversation.

Un certain nombre d’équipes pensent que les trois amigos devraient écrire les tests d’acceptations (par exemple sous la forme de scénarios Cucumber) _lors_ de cette session, en s’asseyant dans une salle avec un projecteur pendant que quelqu’un saisit des scénarios gherkin dans un environnement de développement. Il y a des moments où cela peut valoir le coup de faire comme cela, mais je pense que c’est généralement une mauvaise idée. Cela nous détourne du véritable objectif de la conversation.

It’s easy to see why people make this mistake: the apparent purpose is to take a user story, which already has some pre-defined _acceptance criteria_, and come up with _examples_ that can be turned into _acceptance tests_.

C’est facile de voir pourquoi les personnes font cette erreur : le but apparent est de prendre une _user story_, ayant déjà quelques _critères d’acceptation_ pré-définis, et d’obtenir des _exemples_ qui peuvent être transformés en _tests d’acceptation_.

I think the true purpose, however, is to reach a _shared understanding_ of what it will take for the story to be done. You can move much more quickly towards this goal by staying low-tech.

Je pense que le véritable objectif, est d’obtenir une _compréhension partagée_ de ce qu’il faudra faire pour qu’une story soit terminée. Vous pouvez atteindre cet objectif plus rapidement avec cette technique rudimentaire.

## Friends episodes

## Épisode Friends

So instead of going for full-blown formal Gherkin scenarios, just try to capture a list of _rough examples_, using the _friends episode_ naming convention.

Donc à la place de vouloir obtenir des scenarios Gherkin complet et formel, essayez seulement de noter une liste d’_exemples bruts_, en utilisant la convention de nommage dite des _épisodes de Friends_ ^NdT

For example:

Par exemple :

* The one where the customer forgot his receipt
* The one where the product is damaged
* The one where the product was bought 15 days ago

* Celui dans lequel le client a perdu sa facture
* Celui dans lequel le produit est endommagé
* Celui dans lequel le produit a été acheté il y a quinze jours

Sometimes, when uncertainty lurks, you’ll instinctively want to be more concrete than this. You still don’t need to resort to the rigid structure of _Given When Then_ just yet:

Certaines fois, lorsque l’incertitude monte, instinctivement vous pourriez vouloir  avoir quelque chose de plus concret. À ce niveau-là, vous n’avez pas toujours pas besoin pour l’instant d’avoir recours à la structure rigide _Give When Then_ :

![Green card](https://cucumber.io/images/blog/example-mapping/no-gherkin.jpg)

![Carte verte]({{ site.url }}assets/cartographier_exemples/carte_verte.jpg)

When the outcome (Then) is unclear, you don’t have an example, you have a question.

Lorsque le résultat (Then) n’est pas clair, alors c’est que vous n’avez pas un exemple mais que vous avez une question.

## Known unknowns

## Inconnus connus

Whenever a conversation like this is going round in circles, it’s because you don’t have enough information. Probably someone is missing from the conversation, or maybe you need to do some user research, or a [spike](http://www.extremeprogramming.org/rules/spike.html).

Lorsqu’une conversation comme celle-ci tourne en rond, c’est parce que vous n’avez pas assez d’informations. C’est sans doute parce qu’il manque quelqu’un pour participer à la conversation, ou peut-être parce que vous devez faire des recherches du côté utilisateur, ou d’essayer quelque [chose](http://www.extremeprogramming.org/rules/spike.html)

![Red card](https://cucumber.io/images/blog/example-mapping/question.jpg)

![Carte rouge]({{ site.url }}assets/cartographier_exemples/carte_rouge.jpg)

Instead of letting everyone share their opinion about what they think the outcome should be, simply capture the question and move on. Congratulations! You’ve just turned an unknown unknown into a _known unknown_. That’s great progress.

À la place de laisser chacun faire part de son opinion sur ce qu’il pense que le résultat devrait être, essayez simplement de noter la question et de poursuivre. Félicitations ! Vous avez simplement transformé quelque chose d’inconnu inconnu en _inconnu connu_. C’est un net progrès.

Many people tell me that just this one aspect of example mapping has transformed their discovery workshops from dull ramble-athons into snappy productive mind-melds.

Beaucoup de personnes me disent que ce seul aspect de la cartographie des exemples a transformé leurs atelier de découverte de randonnée sans fin et ennuyeuses à des sessions de remues-méninges productives éclairs.

## Who should come?

## Qui devrait venir ?

The bare minimum is your three amigos: a developer, a tester and a product person. That’s just a minimum though. By all means invite your operations, user experience people or whoever else is relevant to the story being discussed. Anyone likely to help you discover new questions, or to turn questions into decisions during the conversation will be useful.

Au minimum, vos trois amigos : un développeur, un testeur et une personne du métier. C’est juste le strict minimum. Au mieux, invitez les administratifs, les spécialistes en expériences utilisateurs ou toute personne jugée pertinente pour la story en cours de discussion. N’importe qui susceptible de vous aider à découvrir de nouvelles questions, ou à transformer les questions en décisions pendant la discussion sera également utile.

While you’re learning this technique, it can help to have someone in the formal role of facilitator, whose job it is to make sure everything that’s being said is being captured on a card. Examples and questions fly around the room quickly, and it takes discipline to capture them on the table so you can see what you’re talking about.

Pendant que vous apprenez cette technique, il peut être utile que quelqu’un prenne un rôle formel de facilitateur, dont le boulot sera de faire en sorte que tout ce qui est dit soit noté sur une fiche. Les exemples et les questions fusent rapidement dans la pièce, et cela exige de la discipline de les saisir au vol et de les mettre sur la table afin de visualiser ce dont vous êtes en train de parler.

## So when do we write Gherkin?

## Alors quand est-ce que l’on écrit en Gherkin ?

Don’t let this post confuse you: there is immense value in writing Gherkin together too, especially during the early days of a project. That’s where you develop your ubiquitous language, and it’s vital to have those scenarios expressed in a way that everyone on the team believes in.

Ne laissez pas cet article vous troubler : il y a un grand intérêt à écrire en Gherkin en même temps aussi, tout spécialement au tout début du projet. C’est à ce moment-là que vous développez votre langage universel et il est vital que ces scénarios  soient exprimés de telle manière à ce que tout le monde dans l’équipe y croit.

But expressing examples in that way requires a different mode of thinking from deciding which examples are in scope, and clarifying the underlying rules.

Mais exprimer des exemples de cette manière exige une réflexion différente pour décider quels sont les exemples dans le périmètre et clarifier les règles sous-jacentes.

For a team that’s up and running, with a fairly mature domain language, my preference is for the product person to spend their time and energy in the example mapping session, and leave the actual writing of Gherkin to their other two amigos. Once they’ve drafted a Gherkin specification, the product person can give them feedback.

Pour une équipe déjà à niveau ayant un vocabulaire métier plutôt mature, je préfère que la personne du métier consacre son temps et son énergie dans les sessions de cartographie des exemples, et laisse la charge de l’écriture en Gherkin aux deux autres amigos. Une fois qu’ils ont fait un brouillon de spécification Gherkin, la personne du métier peut leur faire un retour.

> Is that how I would have written it?

> Est-ce que c’est comme cela que j’aurais dû l’écrire ?

This gives you an opportunity to test how effective the example mapping conversation was in transferring the product person’s knowledge to their amigos.

Cela vous laisse l’opportunité de tester de l’efficacité de la conversation de cartographie des exemples pour transférer la connaissance de la personne du métier à ses amigos 

## How often should we do this?

## À quelle périodicité devrions-nous faire cela ?

Product people are often busy. Respect their time by scheduling these sessions in a way that they’ll be able to give you their full attention.

Les gens du métier sont souvent occupés. Respectez cela en planifiant ces sessions de telle manière à ce qu’ils soient en capacité de vous donner toute leur attention.

My recommendation, based on what I’ve seen work for several teams in practice, is to run them frequently: every other day is often a good rhythm. Just pick one story and give it 25 minutes of attention, then go back to work. Trying to do more in a big batch will just drain your energy.

Ma recommandation, basée sur ce que j’ai pu observer dans plusieurs équipes et qui a bien fonctionner en pratique, c’est de les faire fréquemment : un rythme d’un jour sur deux se révèle être souvent un bon rythme. Prenez une et une seule _story_, accordez-lui 25 minutes d’attention, puis chacun retourne vaquer à ses occupations. En faire par paquets de 10 ne ferait qu’épuiser votre énergie. 

## But my team is distributed!

## Mais mon équipe est une équipe distribuée !

I’ve seen innovative hacks on this already: some people use bullet lists in a shared Google doc, I’ve seen people using a spreadsheet with coloured cells to represent the cards. You could also use a mind-map. The key is to keep it quick and easy to work with, _so you can focus on the conversation_.

J’ai observé déjà quelques variations innovantes sur cette cartographie : j’ai vu certaines personnes utiliser des listes à puces dans un Google doc partagé, j’en ai vu d’autres utilisé une feuille de calcul avec des cellules colorées pour représenter les cartes. Vous pourriez aussi utiliser une carte heuristique. La clé est que la démarche reste rapide et facile., _afin que vous puissiez vous concentrez sur la conversation_.

## Some final tips

## Quelques trucs et astuces pour terminer

It’s important to clearly understand the distinction between [rules and examples](http://lizkeogh.com/2011/06/20/acceptance-criteria-vs-scenarios/) before you can make use of Example Mapping. I have a [fun exercise](https://speakerdeck.com/mattwynne/rules-vs-examples-bddx-london-2014) for teaching this that I’ll share in a future post.

Il est important de comprendre clairement la distinction entre [règles et exemples](http://lizkeogh.com/2011/06/20/acceptance-criteria-vs-scenarios/) avant de commencer à utiliser la cartographie des exemples. J’ai un petit [exercice amusant](https://speakerdeck.com/mattwynne/rules-vs-examples-bddx-london-2014) pour enseigner cela que je partagerai avec vous dans un futur proche.

Remember that the whole purpose of this conversation is to **discover the stuff you don’t already know**. So there are no stupid questions. Have some fun and really explore the problem.

Rappelez-vous que tout l’objectif de cette conversation est de **découvrir des choses que vous ne connaissez pas encore**. Donc il n’y a pas de questions stupides. Prenez plaisir et explorer vraiment à fond le problème.

You’ll find that rules make natural fault lines for slicing your story. Try to feel comfortable deferring as much as possible, so that you can focus on solving the core of the problem. You can add more sophistication (and complexity) later.

Vous trouverez que les règles font des lignes de fractures naturelles pour fractionner votre story. Rassurez-vous et soyez à l’aise en différant certains éléments autant que possible, cela vous permettra de vous concentrer sur la résolution du cœur du problème. Vous pourrez ajouter de la sophistication (et de la complexité) plus tard.

_Thanks to Janet Gregory, Aslak Hellesøy and Seb Rose for their feedback on this post, to Theo England for his patience while I perfected it, and to Tom Stuart for [getting me to pull my finger out](https://twitter.com/tomstuart/status/673447106506563584)_.

_Merci à Janet Gregory, Aslak Hellesøy et Seb Rose pour leur retours sur cet article et à Theo England pour sa patience alors que je perfectionnais mon article, et à Tom Stuart pour [m’avoir fait me retrousser les manches](https://twitter.com/tomstuart/status/673447106506563584)_

---
Auteur : [Matt Wynne](https://cucumber.io/#company)  
Source : [Introducing Example Mapping](https://cucumber.io/blog/2015/12/08/example-mapping-introduction)  
Date de parution originale : 08 Décembre 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : /3/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}




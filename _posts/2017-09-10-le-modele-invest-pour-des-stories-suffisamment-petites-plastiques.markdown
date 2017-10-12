---
layout: post
title:  "Le modèle INVEST - S comme stories Suffisamment petites, eScalable "
date:   2017-09-10 00:00:01
published: true
tags: 
- user stories
---

**S** is for Small in the [INVEST](http://xp123.com/articles/invest-in-good-stories-and-smart-tasks/) acronym. I now use another **S** that I think captures the idea even better: Scalable.

Le **S** du modèle INVEST est pour “Suffisamment petites”. J’utilise désormais ce **S** pour quelque chose d’autre qui je pense capture cette idée encore mieux : plaStique[^1]. 

Scalable means “able to be changed in size or scale,” and that’s handy in a story: We want stories sized to what we’re trying to do.

_Scalable_[^2] signifie “pouvoir changer de taille ou d’échelle”, ce qui est plutôt pratique dans une _storie_. Nous voulons des _stories_ taillées selon ce que nous essayons de faire.

It’s helpful to think about stories at three levels: high, medium, and low.

Il est utile d’envisager les _stories_ sur trois niveaux : haut, moyen et bas.

## High-Level Stories: Themes and Activities

## Les _stories_ de haut niveau : Thèmes et activités

The highest level view helps us learn the shape and extent of the system we need.

La vue de plus haut niveau nous permet d’appréhender la forme et la portée du système dont nous avons besoin.

These items are so big that most people don’t even call them stories. You may know them as “themes” (Kent Beck), “activities” (Jeff Patton), “epics” (SaFE), or “kite level” (Alistair Cockburn). (We’ll ignore the subtle differences.)

Ces items sont si gros que la plupart des gens ne les appellent pas des _stories_. Vous les connaissez sans doute sous le nom de “Thèmes” (Kent Beck), d’“activités” (Jeff Patton), d’“épiques” (SaFE), ou de “niveau cerf-volant” (Alistair Cockburn). (Nous n’irons pas plus loin dans les détails).

For example, suppose we’re creating a new car rental system. We might talk about:

Par exemple, supposons que nous voulons créer un nouveau système de location de voiture. Nous pourrions envisager de parler de :

* Reserving cars
* Renting cars
* Returning cars
* Analytics

* Réservation des véhicules
* Location des véhicules
* Retour des véhicules
* Statistiques

As we look at this list, we may realize we haven’t thought about “Loss and Damage”: what happens if a car is stolen or damaged? Perhaps the concept should be “Fleet Management,” and include prepping cars.

En regardant cette liste, nous pourrions réaliser tout d’un coup que nous n’avions pas pensé aux “Vols et Accidents” : que se passe t’il si un véhicule est volé ou endommagé ? Peut-être que le concept devrait être “Gestion de flotte” et qu’il pourrait inclure la préparation des véhicules.

I’m not a car rental expert, so surely there are other major areas of the system. But it’ll be closer to a dozen than a hundred at this level.

Je ne suis pas un expert en location de véhicules, mais il y a sûrement d’autres domaines importants à envisager pour ce système. À ce niveau de vision, ce nombre est sans doute plus proche de la douzaine que de la centaine.

These aren’t stories somebody can just go implement. We use these to answer, “Have we forgotten anything big?”

Ici, il ne s’agit donc pas de _stories_ que quelqu’un peut d’ores et déjà implémenter. Il s’agit juste de répondre à la question “Avons-nous oublier quelque chose d’important ?”

## Middle Level: The Headline

## Niveau intermédiaire : les gros titres 

The middle level is where stories’ headlines are. This is the level of story maps and release plans.

Le niveau intermédiaire se situe au niveau des gros titres des _stories_. Plus précisément du niveau où se situe la cartographie des _stories_ et les plannings de livraison.

For a headline to make sense, we have to talk about a particular kind of story: External and [Valuable](http://xp123.com/articles/valuable-stories-in-the-invest-model/). Such stories start from outside a system, and describe a user or system action that accomplishes something a stakeholder cares about.

Pour qu’un gros titre ait du sens, nous devons parler d’un type particulier de _story_ : Externe et [valable](à remplir). Ce genre de _stories_ commence à l’extérieur d’un système, et décrit une action d’un utilisateur ou d’un système qui accomplit quelque chose d’important pour une partie prenante.

Headlines don’t need to follow a template, but I default to the one Industrial Logic suggests: **Role-Action-Context**:

Il n’est pas nécessaire que les gros titres suivent un modèle en particulier ; par défaut, j’utilise celui proposé par _Industrial Logic” : **Rôle - Action - Contexte** :

* Role – the user or system triggering the story
* Action – what happens
* Context [optional] – when, where, and/or how

* Rôle - l’utilisateur ou le système déclenchant la story
* Action - ce qu’il se passe
* Contexte [optionnel] - quand, où, et/ou comment

_Example_: Customer purchases item
_Example_: Customer purchases item with debit card

_Exemple_ : un client achète un article
_Exemple_ : un client achète un client avec une carte bancaire

Some teams create headlines and stories that are super-detailed, but only cover part of a system action. Don’t do that; make your stories describe a full (though possibly small) and valuable interaction. Keep the details a level down.

Certaines équipes écrivent des gros titres et des _stories_ super détaillés, mais qui couvrent seulement une partie de l’action du système. Ne faites pas ça - vos _stories_ doivent décrire une interaction aussi complète (tout en restant si possible concise) et apportant de la valeur à celles-ci. Gardez pour plus tard et à un niveau approprié le détail des informations qui s’y rattache.

Ironically, people sometimes create and excuse these partial “technical stories” (ugh) as their way to keep stories Small. They may be small, but they’re not user stories. A Product Owner can’t work with them effectively.

De manière assez ironique, les personnes créées parfois des “stories techniques” (sic) partielles pour garder d’une certaine manière des _stories_ de taille relativement petites. Elles sont peut être petites, mais il ne s’agit pas de _**user** stories_. Un _Product Owner_ ne pourra pas travailler avec efficacement.

> “Technical stories” (ugh) may be small, but they’re not _user_ stories.

> Les “_stories_ techniques” (sic) sont peut être petites, mais il ne s’agit pas de _**user** stories_

Stories that users value and that can scale up or down provide a lot of power in an Agile delivery model. If we can assemble the most critical stories and deliver them in a minimalistic way, we can quickly get a working version of the system. (See Alistair Cockburn’s idea of a [Walking Skeleton](http://alistair.cockburn.us/Walking+skeleton).)

Les _stories_ qui ont de l’importance aux yeux des utilisateurs et sur lesquelles il est possible d’avoir plusieurs niveaux de détails offrent beaucoup de souplesse dans un modèle de projet agile. Si nous pouvons rassembler les _stories_ les plus critiques et les livrer d’une manière minimale, nous pouvons avoir rapidement une version opérationnelle du système (cf. le concept d’Alistair Cockburn du [Squelette qui marche](http://alistair.cockburn.us/Walking+skeleton).)

Once the system is working, even if in a clunky way, we can start using it, while we simultaneously enhance it over time as usage scales. This may get us early payment (yay!) but will certainly give us early feedback.

Une fois que le système est opérationnelle même s’il est un peu bancal, nous pouvons commencer à l’utiliser, tout en pouvant l’améliorer simultanément au fur et mesure des usages. Cela peut nous permettre de commencer à gagner de l’argent (yay !) mais cela nous apportera plus certainement des retours d’informations bien plus vite.

We need feedback because… like it or not, we’re ignorant. We have theories about what’s valuable, but we’ve never put them to the test. We build a house of cards out of our assumptions. (Read about [Minimum Viable Products](https://www.amazon.com/gp/product/0307887898/ref=as_li_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=0307887898&linkCode=as2&tag=xp123com&linkId=fed7efbc854dc40e8fcd822721d4f9cb) too.)

Nous avons besoin de ces retours d’informations … parce que nous aimions ça ou pas, nous sommes ignorants. Nous avons sans doute des théories sur ce qui est valable, mais nous n’avions pas pu les mettre à l’épreuve jusqu’à présent. Nous avons construit un château de cartes basé sur nos suppositions. (Si vous voulez approfondir ce sujet, lisez donc [Minimum Viable Products](https://www.amazon.com/gp/product/0307887898/ref=as_li_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=0307887898&linkCode=as2&tag=xp123com&linkId=fed7efbc854dc40e8fcd822721d4f9cb).)

I’m sure there are domains where Product Owners exactly understand the value, but I don’t run into them. Where I go, people tend to have limited data about usage, sales, etc. Even when they have data about what users and customers do, they tend to guess about the future and about what would appeal to non-users and non-customers.

Je suis sûr et certain qu’il y a des domaines où les _Product Owners_ savent pertinemment la valeur des choses qu’ils demandent, mais j’avoue que je n’en rencontre pas souvent. Dans les endroits où j’interviens, souvent les gens n’ont que peu de données sur l’utilisation des applications, les ventes, etc. Et même lorsqu’ils ont des données sur ce que les utilisateurs et les clients font, ils ont tendance à essayer de prédire l’avenir et ce qui pourrait plaire aux non-utilisateurs ou aux non-clients.

## Low Level: The Details

## Bas niveau : les détails

At the bottom, we care about how we do things.

Tout en bas, nous nous occupons de savoir comment fonctionne les choses.

For example: __**Customer purchases item**__

Par exemple : __**Un client achète un article**__

This story can be delivered in many ways.

Cette _story_ peut être faite de plusieurs manières.

For example, I used to buy soda water cartridges from a website where you just emailed them a purchase request, including your phone number in the email. Then Joe called you to get your payment info and shipping details.

Par exemple, j’ai l’habitude d’acheter des cartouches à gaz pour soda sur un site web auquel vous pouvez envoyer votre commande par messagerie électronique avec votre numéro de téléphone. Ensuite Joe vous rappelle pour récupérer vos informations de paiement et de livraisons.

Other ways this story might work:

Voici d’autres manières parmi lesquelles 

* In a physical store, a customer might ask the clerk for an item. The clerk pulls it from the shelf behind them, hand-writes a receipt with a carbon copy, gives you the item and the original receipt, and sticks the carbon copy on a spike.

* Dans un magasin physique, un client pourrait demander à un vendeur un certain article. Le vendeur l’attrape sur une étagère derrière lui, écrit un reçu de manière manuscrite avec un papier carbone, vous donne l’article et l’original du reçu et met la copie carbone sur un pique.

* In a supermarket, a customer might walk through the store, put the items they want in a cart, then check out with clerks at registers in the front of the store. Some grocery stores have a self-checkout, where you scan your own items.

* Dans un supermarché, un client pourrait déambuler dans le magasin, prendre les articles qu’il souhaite dans un chariot, puis les payer à une caisse à la sortie du magasin. Certaines magasins ont des caisses en libre-service où vous pouvez passer vous-mêmes les articles en caisse.

* When you buy something at Amazon.com, you have your credit card on file, and Amazon attempts to cross-sell and up-sell while you check out. (Your purchase also feeds a lot of reports and analytics, perhaps described in other stories.)

* Quand vous achetez quelque chose sur Amazon.com, votre carte de crédit est déjà enregistré (lors d’un achat précédent), et Amazon essaye de vous vendre des produits connexes et des produits de gamme supérieure lors de la finalisation de votre commande. (Votre achat d’ailleurs viendra alimenter différente tableaux et statistiques, qui pourront être décrit dans d’autres _stories_.)

A single headline allows for many variations. That is scalability in stories.

De nombreuses variations peuvent naître d’un seul gros titre. C’est ça la flexibilité des _stories_.

We’re used to different stores doing things differently, but we sometimes forget that our own implementations can evolve as well.

Nous allons dans différents types de magasins pour pouvoir faire les choses de manière différentes, mais nous oublions quelque fois que nos implémentations peuvent évoluer elles-aussi.

>A single headline allows for many variations. _That_ is scalability in stories.

> Différentes variations peuvent naître d’un seul gros titre. _C’est_ ça la flexibilité des _stories_.

You may recognize this approach as being [iterative](http://jpattonassociates.com/dont_know_what_i_want/). It’s iterative not just in the software implementation, but also in the details of the story.

Vous avez bien sûr reconnu la nature [itérative](http://jpattonassociates.com/dont_know_what_i_want/) de cette approche. Ce qui est itératif ce n’est pas seulement l’implémentation logicielle mais aussi les détails de la _story_

## Scalability and Splitting

## Flexibilité et décomposition

One headline covers many potential stories.

Un gros titre peut couvrir plusieurs _stories_ potentielles.

You may already be used to the idea of [splitting stories](http://xp123.com/articles/twenty-ways-to-split-stories/). Given a story, the team comes back and says, “This story is too big—we need a smaller bite.”

Vous pouvez déjà être familier de l’idée de la [décomposition des _stories_](http://xp123.com/articles/twenty-ways-to-split-stories/). Par exemple, pour une _story_ donnée, l’équipe peut venir vous voir et vous dire “Cette _story_ est trop grosse nous en voudrions un plus petit morceau.

But splitting is painful: you build up a full description of a story, with all the capabilities and ideas you imagine for it. Then the team takes a scalpel, knife, or sledgehammer to it, tearing it apart.

Mais la décomposition est traumatisante : vous avez bâti une description complète d’une _story_ avec toutes les possibilités et toutes les idées possibles que vous ayez pu imaginer. Puis l’équipe prend un scalpel, un couteau, ou une massue, et la met en charpie. 

The process can drive a product owner to tears.

Ce processus peut amener au bord des larmes un _product owner_.

This is where Scalability comes in. Think of the [intensity](http://xp123.com/articles/intensifying-stories-running-with-the-winners/) of a story as a dial: skeletal, minimal, natural, elaborate, excessive. (These are fuzzy, not definitive levels.)

C’est là où la flexibilité entre en jeu. Pensez à l’[intensité](http://xp123.com/articles/intensifying-stories-running-with-the-winners/) d’une story comme d’un cadran : squelettique, minimal, naturel, élaboré, excessive. (Ce sont des niveaux dont les contours ne sont pas complètement définis)

![intensity scale](http://xp123.com/wp-content/uploads/2016/11/intensityScale.png)



Move from _splitting_ stories to __**intensifying*__ stories.

Passez de la _décomposition_ des _stories_ à __**intensification**___ des _stories_.

> Move from _splitting_ stories to __**intensifying**__ stories.

> Passez de la _décomposition_ des _stories_ à __**intensification**___ des _stories_.

As a product owner, work from the scaling-up perspective. Start small — smaller than you might expect — and grow your stories over time as you deliver.

En tant que _product owner_, travailler à partir d’une perspective de réponse graduée. Démarrez petit - encore plus petit que vous pourriez l’imaginer - et faites grandir vos _stories_  - 

## How Big?

## Quelle taille ?

Big stories are tricky.

Les grosses _stories_ c’est compliqué.

* It’s hard to know we’ve got exactly the right features (as we’re adding things without a lot of experience).

* Il est assez difficile de savoir si nous avons les bonnes fonctionnalités (étant donné que nous ajoutons beaucoup de choses sans avoir beaucoup de recul)

* Big stories often mix both more and less valuable parts, so it’s hard to separate out their contribution.

* Les grosses _stories_ sont souvent le résultat du mélange d’un ensemble de parties ayant plus ou moins de valeur, il est difficile de faire la part de leur contribution.

* Big stories strain the delivery team to digest and deliver a big chunk of work.

* Les grosses _stories_ obligent l’équipe de livraison à digérer et à livrer des grosses portions de travails

> Big stories are tricky.

> Les grosses _stories_ c’est compliqué 

You may have learned to make stories that are MMFs: Minimal Marketable Features. But even that’s too big in a continuous-delivery world. Instead, think of Minimum Useful Features – small things that still makes somebody’s life a little better (and can grow into big things).

Vous avez peut être appris à faire des _stories_ qui soient des FMM : Fonctionnalités Minimales mettable sur le Marché[^1]. Mais même ça, c’est trop gros dans un monde de livraison continue. À la place, pensez au Minimum de Fonctionnalités Utiles - un ensemble de petites choses qui rendent la vie de quelqu’un un peu plus facile (et qui peuvent se transformer en choses plus imposantes).

For example, consider an improvement in a search engine: the user interface stays the same, but search results are a little better. This is worth releasing even if it doesn’t merit bullet points in an ad.

Par exemple, si nous considérons une amélioration d’un moteur de recherche : l’interface utilisateur demeure inchangée, mais les résultats de la recherche seront un peu plus pertinents. Cela vaut le coup de livrer cette amélioration même si cela ne mérite pas de figurer sur une publicité.

I’ve often encouraged people to make stories smaller – hours to days of effort, not weeks to months.

J’encourage souvent les gens à faire des _stories_ plus petites - allant de quelques heures à quelques jours d’effort, et non de quelques semaines à quelques mois.

Can stories get too small? Definitely. I like Jeff Patton’s analogy of overly-atomized stories as a [bag of leaves](http://jpattonassociates.com/the-new-backlog/), stripped of structure and burying you in details.

Est-ce que des _stories_ peuvent devenir trop petites ? Tout à fait. J’aime bien l’analogie de Jeff Patton, du sac de feuilles dépourvues de structure et vous  ensevelissant sous une tonne de détails, pour parler des _stories_ trop atomisées.

How can you deal with too-small stories? Merge them. (This is one reason I like the “major” headline view – you can have stories that cover different details, then generalize and merge them to talk about the headline and the current state of implementation.)

Comment pouvez-vous gérer des _stories_ trop petites ? Fusionnez-les. (C’est l’une des raisons pour lesquelles j’aime bien voir les “gros” titres de première page - vous pouvez avoir des _stories_ couvrant différents niveaux de détails, en les généralisant et en les fusionnant par la suite, elles seront à même de parler des gros titres et de l’état actuel de l’implémentation.)

Unfortunately, many “agile” planning tools take a hierarchical, atomized view, and don’t help much when thinking in terms of scalable stories. It takes work to maintain the big picture.

Malheureusement, un certain nombre d’outils “agiles” de planification prennent une vue hiérarchique, atomisé, et n’aide pas beaucoup à penser en terme de _stories_ évolutives. Cela fait du boulot de maintenir une vision d’ensemble.

## Conclusion

## Conclusion

John Gall said, “A complex system that works is invariably found to have evolved from a simple system that worked. A complex system designed from scratch never works and cannot be patched up to make it work. You have to start over with a working simple system.” It’s a good reminder for stories.

John Gall a dit “Tout système complexe opérationnel est à l’origine un système simple opérationnel qui a évolué. Un système complexe créé à partir de rien ne fonctionnera jamais et ne pourra jamais être corrigé. Vous devrez recommencer avec système opérationnel simple.” Cela constitue un bon rappel pour les _stories_.

Remember the three levels from earlier:

Rappelez-vous les trois niveaux vus précédemment :

1. **Theme – Top-level**: Are we covering the right things?
2. **Headline – Mid-level**: Is the user getting a capability they care about?
3. **Details – Lowlevel**: Do we need a new capability, or can we improve an old one?

1. **Thème - Haut niveau** : Abordons-nous les bonnes choses ?
2. **Gros titre - Niveau intermédiaire** : Est-ce que l’utilisateur obtient quelque chose qui soit important à leurs yeux ? 
3. **Détails - Bas niveau** : Avons-nous besoin de quelque chose de nouveau, ou pouvons-nous en améliorer une existante ?

Rather than splitting too-big stories, train yourself to start with smaller versions, then extend and intensify them. If you have to split, take a user’s perspective, not a technology perspective.

Plutôt que de décomposer des _stories_ trop grosses, entraînez-vous à démarrer avec des versions plus petites, puis à les étendre et à les intensifier. Si vous devez les décomposer, faites-le d’un point de vue utilisateur et non d’un point de vue technologique.

You will find that scalable stories will:

Vous trouverez que des _stories_ évolutives vont vous :

* Help make progress visible
* Provide early utility
* Give you feedback that helps you steer to a more valuable result
* Help reduce market and technical risk

* Aider à rendre l’avancement visible
* Donner une utilité immédiate
* Donner du retour pour vous aider à aller vers un résultat plus valable
* Aider à réduire le risque commercial et technique

[^1]: NdT - la lettre S dans l’acronyme INVEST est Small puis comme l’indique l’auteur a acquis une nouvelle signification Scalable.
Pour Small, la traduction vers petit(e) était facile même s’il a fallu trouver une astuce pour conserver le S de l’acronyme INVEST avec Suffisamment Petite car cela respectait bien l’esprit de l’article.
Pour Scalable, la traduction est ici plus problématique, il suffit de regarder la [page de discussion de Wikipedia pour un essai de francisation de ce terme](https://fr.wikipedia.org/wiki/Discussion:Scalability) même si pour l’acronyme le terme Scalabilité serait bien pratique mais je n’y retrouve pas exactement le sens du texte. C’est la même chose pour évolutivité, extensibilité … Après réflexion (toujours par rapport au sens du texte) pour le côté malléable de la _story_ tel que l’auteur semble l’exprimer, le terme plaStique me semble approprié - et en plus il y a un S pour l’acronyme ;)

[^2]: NdT - terme conservé en vo - cf. NdT précédente

---
Auteur : [Bill Wake](http://xp123.com/about/)  
Source : Small – Scalable – Stories in the INVEST Model](http://xp123.com/articles/small-scalable-stories-in-the-invest-model/)  
Date de parution originale : 02 Novembre 2016  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 08/08/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



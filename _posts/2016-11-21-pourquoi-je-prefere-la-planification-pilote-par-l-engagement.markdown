---
layout: post
title:  "Pourquoi je préfère la planification pilotée par l’engagement"
date:   2016-10-25 00:00:01
published: true
categories: 
- scrum
- planification
---

Over the past two weeks, I’ve described two alternative approaches to sprint planning:

![Female Boxers Facing Off](https://www.mountaingoatsoftware.com/uploads/blog/boxer-tattoos.jpg)

![Boxeuses se faisant face](https://www.mountaingoatsoftware.com/uploads/blog/boxer-tattoos.jpg)

Ces dernières semaines, j’ai décris deux approches alternatives de la planification de sprint : 

<div align="right" style="float:right; padding-left:30px" >
  <img title="Main" src="{{ site.url }}assets/mountain_goat/velocite_sprint_pourquoi.jpg" />
</div>

* [Velocity-Driven Sprint Planning](https://www.mountaingoatsoftware.com/blog/velocity-driven-sprint-planning)
* [Commitment-Driven Sprint Planning](http://www.mountaingoatsoftware.com/blog/commitment-driven-planning)

* [La planification de sprint pilotée par la vélocité](http://www.les-traducteurs-agiles.org/scrum/planification/2016/10/25/planification-sprint-pilotee-par-la-velocite.html)
* [La planification de sprint pilotée par l’engagement](http://www.les-traducteurs-agiles.org/scrum/planification/2016/11/09/planification-sprint-pilotee-par-l-engagement.html)

This week I want to address why I prefer commitment-driven sprint planning. First, though, here is a very brief refresher on each of the approaches.

Cette semaine, je voudrais expliquer pourquoi je préfère la planification de sprint pilotée par l’engagement. Tout d’abord, voici un bref récapitulatif de chacune des approches.

### Brief Summary of Sprint-Planning Approaches

### Résumé succinct des approches de planification de sprint

In velocity-driven sprint planning, a team selects a set of product backlog items whose high-level estimates (usually in story points or ideal days) equals their average velocity.

Dans la planification de sprint pilotée par la vélocité, l’équipe sélectionne un ensemble d’items du _product backlog_ dont la somme des estimations à grosses mailles (généralement en points de story ou en jours idéaux) se rapproche le plus possible de leur vélocité moyenne.

In commitment-driven sprint planning, a team commits to one product backlog item at a time by roughly identifying and estimating the tasks that will be involved, and stopping when they feel the sprint is full.

Dans la planification de sprint pilotée par l’engagement, l’équipe s’engage sur un item du _product backlog_ en identifiant et en estimant grosso modo les tâches qui y sont rattachées, et elle arrête ce processus lorsqu’elle estime que le sprint est remplit.

Because “commitment” is often mistaken as “guarantee,” this approach is becoming more commonly referred to as capacity-based sprint planning.

Comme l’“engagement” est souvent confondu avec “garantie”, cette approche est plus connue sous le nom de planification de sprint basée sur la capacité

### Velocity is Variable

### La vélocité est variable

To begin to see why I prefer a commitment-driven approach to sprint planning, consider the graph below which shows the velocities of a team over the course of nine sprints. The first thing you should notice is that velocity is not stable. It bounces around from sprint to sprint.

Pour commencer à comprendre pourquoi je préfère l’approche pilotée par l’engagement pour la planification de sprint, considérons le diagramme ci-dessous nous montrant les vélocités d’une équipe sur une période de neuf sprints. La première chose que vous devriez remarquer est que la vélocité n’est pas stable. Elle fluctue de sprint en sprint.

![Chart of Relationship Between Sprints and Velocity](https://www.mountaingoatsoftware.com/uploads/blog/velocity_blog1.jpg)

![Diagramme de représentation de la vélocité par rapport aux sprints](https://www.mountaingoatsoftware.com/uploads/blog/velocity_blog1.jpg)

The first big drawback to velocity-driven planning is that velocity is too variable to be reliable for short-term (i.e., sprint) planning. My experience is that velocity bounces around in about a plus or minus 20% range. This means that a team whose true velocity is 20 could easily experience a velocity of 16 this sprint and 24 next sprint, and have that just be random variation.

Un premier inconvénient majeure d’une planification pilotée par la vélocité est que la vélocité fluctue trop pour être vraiment  fiable dans une planification à court terme (c’est-à-dire au niveau du sprint). Mon expérience montre que la vélocité fluctue de plus ou moins 20%. Cela signifie qu’une équipe dont la vélocité est de 20 pourrait facilement se retrouver avec une vélocité de 16 sur un sprint puis 24 au prochain sprint, ou avoir une toute autre fluctuation tout aussi aléatoire.

When a team that averages 20 sometimes completes 24 units of work, but sometimes completes only 16, we might be tempted to say they are accomplishing more or less work in those sprints. And that is undoubtedly part of it for many teams. However, some part of the variation is attributable to the imprecision of the units used to estimate the product backlog items.

Nous pourrions être tenté de dire d’une équipe, dont la vélocité moyenne de 20, qui réalise parfois pour 24 points d’unités de travail, mais qui peut parfois n’en faire que 16,  qu’elle accomplit plus ou moins de travail pendant ces différents sprints. Et cela doit être indéniablement le cas pour un certain nombre d’équipes. Toutefois, une certaine partie de cette fluctuation est imputable à l’imprécision des unités de mesures utilisées pour estimer les items du _product backlog_.

For example, most teams who estimate in story points use a subset of possible estimates such as the Fibonacci sequence of 1, 2, 3, 5, 8, 13 or a simple doubling (1, 2, 4, 8, 16). When a team using the Fibonacci sequence takes credit for finishing a 5-point story, they may have really only finished a 4-point story. This tends to lead to a slight overstating of velocity.

Par exemple, la plupart des équipes qui font des estimations en points de story utilisent un sous-ensemble de type d’estimations possibles tel que la suite de Fibonacci 1, 2, 3, 5, 8, 13 ou une autre suite mathématique (par exemple 1, 2, 4, 8, 16). Lorsqu’une équipe utilise la suite de Fibonacci a fini une story estimée à 5 points, elle aura peut être en réalité terminée une story valant que 4 points. Cela tends à une légère surévaluation de la vélocité.

In the long-term this won’t be a problem as the law of big numbers can kick in and things will average out. In the short term, though, it can create problems.

Dans le long terme, cela ne sera sans doute pas un problème, la loi des grands nombres peut se manifester et les choses pourront alors être lissées dans le temps. Dans le court terme, toutefois, cela peut créer des problèmes.

### Anchoring

### Ancrage[^1]

A second problem with velocity-driven sprint planning is due to the effect of anchoring. Anchoring is the tendency for an estimate to be unduly influenced by earlier information.

Un deuxième problème avec la planification de sprint basée sur la vélocité est due à l’effet d’ancrage. L’ancrage est la propension pour une estimation d’être influencée de manière indue par une information arrivée précédemment.

A good example of anchoring is coming up as we approach the Christmas season. Suppose you go into a store and see a jacket you like. There’s a sign saying $400 but that price is crossed out and a new price of $200 is shown. Your brain instantly thinks, “Awesome! A $400 jacket for only $200!” And, of course, this is why the store shows you the original price.

Un bon exemple d’ancrage qui me vient à l’esprit, c’est lorsque approche les fêtes de Noël. Supposez que vous allez dans un magasin et que vous voyez une veste qui vous plait. Il y a une étiquette indiquant $400 mais le prix est barré et un nouveau prix de $200 est marqué. Votre cerveau pense instantanément “Super ! Une veste de $400 pour seulement $200 !”. Et c’est bien la raison pour laquelle le magasin vous a indiqué l’ancien prix.

Who cares what that jacket used to sell for? It’s $200 today. That should be all that matters in your buy-or-not decision. However, once that $400 price is in your brain, it’s hard to ignore it. It anchors you into thinking you’re getting a good deal when the jacket is $200.

Qui se préoccupe de savoir à quel prix se vendait cette veste avant ? C’est $200 aujourd’hui. C’est tout ce qui devrait compter dans votre décision d’acheter ou pas. Toutefois, une fois que l’information du prix de $400 est entrée dans votre cerveau, il est difficile de l’ignorer. Elle s’est insinuée dans votre esprit pour vous dire que vous faisiez une bonne affaire avec cette veste à $200.

_I won't go into the details here, but the best paper I've read on anchoring is from Magne Jørgensen and Stein Grimstad and is called_ “[The Impact of Irrelevant and Misleading Information on Software Development Effort Estimates.](https://www.simula.no/research/se/publications/Simula.SE.299/simula_pdf_file/)”)

_Je ne m’appesantirai pas plus sur le sujet ici, le meilleur papier que j’ai pu lire sur l’ancrage est de Magne Jørgensen et de Stein Grimstad, dont le titre est_ “[The Impact of Irrelevant and Misleading Information on Software Development Effort Estimates.](https://www.simula.no/research/se/publications/Simula.SE.299/simula_pdf_file/)”)

### Anchoring and Velocity-Driven Planning

### Ancrage et planification pilotée par la vélocité

But what does anchoring have to do with sprint planning?

Mais qu’est-ce que l’ancrage a à voir avec la planification de sprint ?

Consider a team in a velocity-driven sprint planning meeting. They’ve selected a set of stories equal to their average velocity. They then ask themselves if that set of stories feels like the right amount of work. (As described, in the post on velocity-driven sprint planning they may also identify tasks and estimate those tasks as an aid in answering that.)

Prenons une équipe dans une réunion de planification de sprint pilotée par la vélocité. Elle a sélectionné un nombre de stories équivalent à sa vélocité moyenne. Les membres de l’équipe se demandent ensuite si cet ensemble de stories représente la bonne quantité de travail à accomplir; (Comme cela a été décrit, dans l’article sur la planification de sprint pilotée par la vélocité, ils peuvent aussi identifier les tâches et estimer ces tâches pour pouvoir répondre à cette question.)

A team doing velocity-driven sprint planning is pre-disposed to say, “Yes, we can do this,” even if they can’t. They are anchored by knowing that the selected amount of work is the same as their average velocity.

Une équipe faisant une planification de sprint pilotée par la vélocité est prédisposée à dire “Oui, nous pouvons faire cela” même si elle ne peut pas le faire. Elle est ancrée par le fait de savoir que la quantité de travail sélectionnée est identique à sa vélocité moyenne.

It’s like me showing you that jacket with the $400 sign next to it and asking, “How much do you think this jacket sells for?” Even if you don’t say exactly $400, that $400 is in your head and will anchor you.

C’est exactement comme lorsque je vous ai expliqué que l’étiquette du prix de $400 sur la veste et que je vous ai posé la question “À quel prix pensez-vous que cette veste est à vendre ?”. Même si vous n’avez pas dit exactement $400, ce prix de $400 est dans votre tête et il se sera ancré en vous.

So, because of anchoring, a team with an average velocity of 20 is inclined to say the sprint is appropriately filled with 20 points – even if that work is really more like 16 or 24 units of work.

Donc, à cause de l’ancrage, une équipe avec une vélocité moyenne de 20 est incline à dire que le sprint est remplit de manière approprié avec 20 points - même si le travail se situe plus vraisemblablement à 16 ou à 24 unités de travail.

This will lead to teams sometimes doing less than they could have. It could also lead to teams sometimes doing more. But in those cases, my experience is that teams will be more likely to drop a product backlog item or two. Experience definitely tells me that teams are more likely to drop than to add.

Cela conduira parfois les équipes à en faire moins qu’elles ne pourraient en faire. Cela pourrait aussi mener parfois les équipes à en faire plus. Mais dans ces cas de figure, mon expérience montre que les équipes sont plus enclines à laisser tomber un ou deux items de backlog. De manière générale, mon expérience montre aussi que les équipes ont plutôt tendance à abandonner des items plutôt qu’à en ajouter.

### Velocity Is Great for Longer-Term Planning

### La vélocité est très utile dans le cadre d’une planification à long terme

By this point, you may be thinking I’m pretty opposed to velocity-driven planning. That’s only half true. Although I’m not a fan of using velocity to plan a single sprint, I am quite likely the world’s biggest fan of using velocity to plan for the longer term. I’ve certainly written more about it than anyone I know.

À partir de là, vous pouvez pensez que je suis plutôt contre la planification de sprint pilotée par la vélocité. C’est seulement à moitié vrai. Même si je ne suis pas un fan de l’utilisation de la vélocité pour planifier un sprint, je suis sûrement l’un de ses plus grands fans au monde pour l’utilisation de la vélocité pour le long terme. J’ai certainement écris plus que quiconque à ce sujet.

The problem with velocity-driven sprint planning is that velocity is simply too variable to be useful in the short term. To illustrate why, suppose you get a job working at a car wash. On your first morning, your boss announces that you have a quota: You need to wash four cars per hour.

Le problème avec la planification de sprint pilotée par la vélocité est que la vélocité est trop fluctuante pour être utile à court terme. Pour illuster ceci, supposez que vous travaillez dans une entreprise de lessivage de voiture. Le matin de votre premier jour, votre patron vous annonce un quota de travail à faire : vous devez lavez quatre voiture à l’heure.

At the end of the first hour, though, you’ve only washed three cars. Should you be fired? Of course not. It was only one hour and perhaps you washed three large cars. Or perhaps it was overcast and only three drivers brought cars in to be washed.

À la fin de la première heure, vous avez lavé seulement trois voitures. Serez-vous viré ? Bien sûr que non. Ce n’était que votre première heure de travail et peut être que les voitures que vous avez lavées étaient trois grosses voitures. Ou peut être que le temps était nuageux et que seulement trois personnes ont amené leurs voitures se faire laver.

What about at the end of your first day, an 8-hour shift? By then you should have washed 32 cars. But you’ve only washed 30. Should you be fired now? Again, almost certainly not.

Qu’en est-il à la fin du premier jour, soit 8 heures plus tard ? Vous devriez avoir lavé 32 voitures. Mais vous en lavez seulement 30. Est-ce que vous serez viré alors ? De nouveau, sûrement pas.

What about the end of your first month? Figuring 20 days and 32 cars per day means you should have washed 640 cars. Suppose, though, you only washed 600. (That’s the same percentage as washing 30 instead of 32 in a day.) Should your boss fire you now? Perhaps still not, but it’s starting to be clear that you are not making quota.

Qu’en sera t’il à la fin du mois ? En prenant 20 jours dans le mois et 32 voitures par jour cela signifie que vous devriez avoir lavé 640 voitures. Supposons néanmoins que vous en ayez nettoyé 600. (C’est le même pourcentage de nettoyage que précédemment avec les 30 voitures lavées à la place des 32 voitures par jour). Est-ce que votre patron devrait vous virer maintenant. Peut être pas encore, mais il devient clair que vous n’atteignez pas votre quota.

What if you’re off by the same percentage at the end of the year? If that quota was well chosen—and all other employees are meeting it—your boss at some point should consider letting you go (or dealing with your below expected productivity in some way, but this post isn’t about good ways of dealing with productivity issues).

Qu’en sera t’il si vous accomplissez le même pourcentage à la fin de l’année ? Si ce quota est bien choisit - et que tous les autres employés l’atteignent -  votre patron à un certain moment devrait considérer de se séparer de vous (ou de s’occuper d’une manière ou d’une autre de gérer votre productivité quelque peu réduite, mais cet article ne porte pas sur les bonnes manières de gérer des problèmes de productivité).  

That quota is useful in the same way velocity is useful: over the long term. Think of how poorly run we’d consider that car wash if an employee was fired in the first hour of missing quota. The longest tenured employee would have been on the job for three days. So while that quota may be useful when measured over a month, it is not useful when measured hourly.

Le quota est utile de la même manière que la vélocité peut l’être : sur le long terme. Pensez donc au jugement que nous pourrions avoir vis-à-vis de cette entreprise de lavage et de sa  gestion si un employé était viré dans l’heure qui suit la non-atteinte de son quota de voitures lavées. Le titulaire du poste qui est resté le plus longtemps l’aura été pendant 3 jours. Donc même si ce quota peut être utile lorsqu’il est mesuré mensuellement, il est inutile lorsqu’il est mesuré toutes les heures.

Velocity is useful in the long term, not the short term. A team with 30 product backlog items to deliver can sum the estimates (likely in story points) on those items and forecast when they’ll be done. A team with three product backlog items to deliver would be better off doing good ol’ task decomposition on those three items rather than relying on velocity.

La vélocité est utile dans le long terme, pas dans le court terme. Une équipe avec 30 items dans le _product backlog_ à livrer peut faire la somme des estimations de ces items et prévoir quand ils seront terminés. Une équipe avec trois items dans le _product backlog_ à terminer aurait tout intérêt à faire la bonne vieille décomposition en tâches de ces trois items plutôt que de se reposer sur la vélocité.

### So, Now What?

### Et maintenant, quoi ?

If you are already doing velocity-driven sprint planning and it’s working for you, don’t switch. However, if your team is new to Scrum or if your team is experiencing some of the issues I’ve described here, then I recommend using commitment-driven sprint planning.

Si vous avez déjà fait des planifications de sprints basées sur la vélocité et que cela fonctionne pour vous, ne changez rien. Toutefois, si votre équipe ou vous-même êtes novices en Scrum ou si votre équipe connaît certaines des difficultés que j’ai pu décrire ici, alors je vous recommande d’utiliser la planification de sprint basée sur l’engagement.


---  
Auteur : [Mike Cohn](https://www.mountaingoatsoftware.com/company/about-mike-cohn)  
Source : [Why I Prefer Commitment-Driven Sprint Planning](https://www.mountaingoatsoftware.com/blog/why-i-prefer-commitment-driven-sprint-planning)  
Date de parution originale : 21 Octobre 2014  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 25/10/2016

---

Copyright ©1998-2016 Mountain Goat Software. All Rights Reserved.

---

{% include share_buttons.html %}

---
layout: post
title:  "Devrions-nous estimer les projets ... du tout ?"
date:   2015-09-14 21:00:55
published: true
categories: 
- estimation
---



http://neilkillick.com/wp-content/uploads/2012/04/estimation-300x201.jpg

## Introduction

After a year or two of “having a hunch” about this, and after many years of either estimating work or working to someone else’s estimates, I’ve now finally come to the conclusion that the use of estimation of any kind in a project is not only a waste of time but is actually destructive.

Après une année ou deux à en "avoir eu le pressentiment", et avoir passé plusieurs années à faire des estimations ou à travailler sur les estimations de quelqu'un d'autre, j'en suis finalement arrivé à la conclusion que l'utilisation de l'estimation sur tout type de projet est non seulement une perte de temps mais est réellement destructrice. 

I am fully aware this is an extremely controversial statement, so I am going to be as thorough as I can in explaining how I came to this conclusion via experience, data and validation. Indeed, when I read [Vasco Duarte’s post](http://softwaredevelopmenttoday.blogspot.com.au/2012/01/story-points-considered-harmful-or-why.html) about this several months ago, I saw his “point” (no pun intended) but also argued the merits of using story point estimation for the purposes of:

Je suis tout à fait conscient que c'est une déclaration vivement polémique donc je vais essayer d'être aussi rigoureux que possible dans mon explication à propos de la manière dont je suis arrivée à cette conclusion à travers une expérience, des données et une vérification.  
En effet, lorsqu'il y a quelques mois, j'ai lu [l'article de Vasco Duarte](http://www.les-traducteurs-agiles.org/estimation/2015/09/13/les-story-consideres-comme-dangereux.html), je l'ai vu "pointer" le bout de son nez (aucun jeu de mots là-dessus) mais j'ai aussi débattu des mérites de l'estimation en story points faite dans le dessein de :

* Up-front sizing of a project to determine its validity within a given budget or timeframe
* Increasing shared understanding and knowledge within the team based on the discussions that arise from a Planning Poker session
* Allowing the PO to make trade-off decisions between different sized stories (based on ROI)
* Measuring team velocity
  * To continually validate the initial project sizing by predicting scope-fit within a given release date
  * To allow the team to measure and improve its performance

* Dimensionner au préalable un projet pour déterminer sa validité au sein d'un budget ou d'une période donnée. 
* Accroître la compréhension et la connaissance commune de l'équipe sur la base des discussions qui sont survenues lors d'une session de _planning poker_
* Permettre au PO de faire des arbitrages (basés sur le retour sur investissement) entre des stories de différentes tailles  
* Mesurer la vélocité de l'équipe
  * pour valider en continu le dimensionnement initial du projet en prévoyant l'adéquation du périmètre par rapport à une date d'une livraison de version donnée

## Why shouldn’t we estimate?

## Pourquoi ne devrions-nous pas estimer ?

I have since come to the conclusion that some of these things do not need to be done at all, and the other things can be done without the need for estimating (guesswork) of any kind. I would now additionally argue that even if you acknowledge the shortcomings of estimation and use ranges, account for uncertainty, etc., the act of estimation in itself is destructive for the following reasons:

J'en suis arrivé depuis à la conclusion que certains de ces points n'ont pas besoin d'être fait du tout, et que d'autres peuvent être faits sans avoir besoin de les estimer (approximation) en aucune façon. Je voudrai maintenant discuté davantage que même si vous reconnaissez les limites de l'estimation et que vous utilisez des fourchettes, que vous prenez en compte l'incertitude, etc... , l'acte de l'estimation en lui-même est destructeur pour les raisons suivantes :

* **“Fixed” scope project delivery expectations are often (always?) based on an up-front estimate of scope (guess) and how long that scope will take to be delivered (another guess), leading to the obvious dysfunctions like death-marches, low quality, etc.**

* **Les attentes sur la livraison de projets à périmètre "fixe" sont souvent (toujours ?) basées sur une estimation initiale du périmètre (approximation) et combien de temps cela prendra pour livré ce périmètre (une nouvelle approximation) conduisent à des dysfonctionnements patents comme les marches forcées, une qualité médiocre, etc ...**

If the budget is fixed, there is no way of going “over budget” in order to deliver the fixed scope. Yet “over budget” is a common term used when describing failed projects. If your budget is truly a constraint then you will only deliver what can be delivered. Agile methods ensure that what you deliver is of the highest value to the business.

Si le budgest est fixé, alors il n'y aucune manière de "dépasser le budget" afin de livrer le périmètre fixé. Toutefois "dépasser le budget" est un terme habituellement utilisé lorsque l'on parle de projets qui ont échoué. Si votre budget est vraiment une contrainte alors vous livrerez seulement ce qui peut être livré. Les méthodes agiles veillent à que vous livrez la plus forte valeur au métier. 

_I chatted to a team member earlier and he complained of feeling pressure to increase velocity. I asked him where this pressure was coming from and he said that it stemmed from the concern that the project will fail if the team isn’t able to deliver more stories more quickly. No one is actually specifically asking the team to deliver more, but there is an implied pressure to do so because they are aware the budget is running out. This mindset comes from years of poorly funded, gated projects, death marches, focus on productivity rather than quality and canned or failed projects._

_Un peu plus tôt, j'avais chatté avec un membre de l'équipe et il se plaignait de sentir une pression pour augmenter la vélocité. Je lui ai demandé d'où cette pression venait et il me répondit qu'elle provenait du soucis que le projet puisse échoué si l'équipe n'était pas capable de livrer plus de stories plus rapidement. En réalité, personne ne demandait spécifiquement à l'équipe de livrer plus, mais il y avait une pression implicite de le faire parce qu'elle était au courant que le budget arrivait à épuisement. Cette tournure d'esprit vient d'années de projets mal financés, de marches forcées, de focalisation sur la productivité plutôt que sur la qualité et de projets étouffés ou ayant échoués._

* **Asking teams to estimate how long their work will take (or how many points they will deliver in a Sprint or a Release, same thing) has connotations that their output is being measured by an external party (manager), creating an environment of fear and massaging figures to reflect what is desired rather than what is predicted**

* **Demander aux équipes d'estimer la durée de leur travail (ou combien de points elles livreront en un sprint ou en une livraison de version, ce qui revient au même) a des connotations de mesure de leurs travails par une tierce partie (le responsable), créant un environnement de peur et de manipulation de chiffres pour refléter ce qui est désiré plutôt que ce qui prévisible** 

To increase velocity the team simply needs to over-estimate stories to give the illusion of delivering more. They may not consciously do this but it may happen sub-consciously. The project manager pats them on the back, but all that has happened is the same amount of “done” working software has been delivered.

Pour accroître la vélocité, l'équipe doit simplement surestimer les stories pour donner l'illusion de livrer plus. Ils ne font peut être pas consciemment mais cela peut arriver inconsciemment. Le chef de projet leur fait une tape dans le dos, mais tout ce qui s'est passé est que la même quantité de logiciel fonctionnel "fini" a été livré. 

It’s time to get real and use real data to reflect real progress, whether it’s good news or bad.

C'est le moment d'avoir et d'utiliser de vrais données pour refléter la progression réelle, qu'elle soit bonne ou mauvaise.

* **We shouldn’t be defining all our scope up front, meaning we shouldn’t estimate all our scope up front, meaning we shouldn’t be defining our delivery date based on our scope**

* **Nous ne devrions pas définir la totalité du périmètre initial, ce qui veut dire que nous ne devrions pas estimer tout le périmètre initiale, ce qui veut dire que nous ne devrions pas définir notre date de livraison sur la base de notre périmètre**

We should be fixing our Release 1 delivery date and aiming to build the best possible product by that date (variable scope).

Nous devrions fixer notre date de la livraison de la version 1 et avoir l'objectif de réaliser le meilleur produit possible pour cette date (périmètre variable).

As soon as we introduce the word “estimation”, the default mindset is to consider “how long will this project take?” (if this isn’t asked explicitly). This causes us to consider the complete scope and duration of the project (this is anti-Agile and I won’t go into why it’s a bad idea because enough has been written about that already elsewhere)

Dès que nous introduisons le mot "estimation", l'attitude par défaut est de penser à "combien de temps ce projet prendra ?" (même si cela n'a pas été demandé explicitement). Cela provoque en nous la prise en compte du périmètre et de la durée complète du projet (c'est anti-agile et je n'expliquerai pas ici pourquoi il s'agit d'une mauvaise idée parce qu'il y a eu suffisamment d'écrits à ce sujet ailleurs)

## How do we size a project?

## Comment déterminons-nous la taille d'un projet ?

Short answer – you shouldn’t. If you don’t have a firm deadline for your project (e.g. day 1 of the Grand Prix for a Grand Prix app), you will have a budget for your project (set by the PMO or the external customer), from which you can derive a deadline. The smart thing to do is to then plan an interim release (say at the halfway point) where you can gauge how the project is going based on the working software measure.

Réponse courte - vous ne devriez pas. Si vous n'avez pas une date butoir ferme pour votre projet (par exemple le 1er jour du Grand Prix pour une application de Grand Prix), vous aurez un budget pour votre projet (fixé par le PMO ou par le client externe) à partir duquel vous pourrez dériver une date butoir. La chose maline à faire est alors de planifier une version intermédiaire (disons à mi-chemin) où vous pourrez jauger de la façon  dont le projet se déroule sur la base d'une mesure d'un logiciel qui fonctionne.

For example, if your budget gives you enough cash for ten 2-week Sprints (given a fixed, 100% allocated team), clearly you need to assume that your go-live date is in 20 weeks time. But the aim should be to get working software in a production environment in 2 weeks time (after Sprint 1). You should then iterate over the product, allowing requirements (scope) to emerge and shape the direction the product takes, and take time to reassess after Sprint 5.

Par exemple, si votre budget vous donne assez d'argent pour dix sprints de 2 semaines (avec une équipe dédiée à 100 %), de manière évidente vous devriez supposer que votre date de mise en production sera dans un délai de 20 semaines. Mais l'objectif devrait être d'avoir un logiciel opérationnel en environnement de production dans un délai de 2 semaines (après le sprint 1). Vous devriez alors itérer sur le produit, permettre aux exigences (le périmètre) d'émerger et de tracer la direction que le produit prendra, et de prendre le temps de réexaminer après le sprint 5. 

These things are not predictable up front – estimation will set you up with a load of scope (expectations) that will not get delivered and will only create unnecessary analysis time (money) and pressure.

Ces choses ne sont pas prévisibles initialement - l'estimation va vous balancer avec un périmètre gigantesque (les attentes) qui ne sera pas livré et qui génèrera un temps d'analyse inutile (argent) et de la pression.

## How does the team get shared understanding of a story?

## Comment l'équipe aura-t-elle une compréhension commune d'une story ?

Simple. When a new item is added to the top of the product backlog, the team will discuss it in Sprint Planning and break it down if necessary. If it doesn’t need breaking down then it is likely already well understood. If it does then the act of breaking it down will necessitate conversations around the implementation detail that will facilitate shared understanding.

C'est simple. Lorsqu'un élément est ajouté au-dessus du _product backlog_, l'équipe le discute lors du _sprint planning_ et le scinde si nécessaire. S'il n'a pas besoin d'être scindé alors il est probable qu'il est déjà bien appréhendé. S'il l'est alors l'acte de le scinder nécessitera des discussions autour de l'implémentation qui faciliteront une compréhension commune.

In short, the team does not need to be in an estimation session to discuss and break down a story.

En bref, l'équipe n'a pas besoin d'être dans une réunion d'estimation pour discuter et scinder une story.

## How can the PO make trade-off decisions?

## Comment le PO prend-t-il des décisions d'arbitrage ?

The PO probably needs to know the ROI of a story when introducing it to the team to be delivered. In order to calculate the ROI she needs to know how much it will cost to be delivered (how long).

Here a team would estimate the item using story points and then the PO, armed with the team’s velocity, can estimate the item’s ROI. But without story points how can this be done?

This is where the concept of “implicit estimation” comes into play. In order to create predictability in the flow of work, the team will break down stories just-in-time (in Sprint Planning) so that they are all roughly the same size. This is something that happens naturally throughout the course of the project. Over time the size of stories normalises because the team naturally wants bite-size chunks to work on in the short time period of the Sprint. They get used to delivering a certain number of stories, give or take, in a Sprint.

So for the PO to cost the item, she just needs to ask the team if it is understood or needs breaking down. If the PO considers it high enough priority she will want to introduce it in Sprint Planning so that it gets built right away, if it makes sense to do so. Sprint Planning is the place for the team to break down the story if required and decide if it can be delivered in the Sprint. If it can, the cost of the item is essentially 2 weeks of team wages (assuming production deployment is done at the end of the Sprint – a continuous delivery model can improve speed to market and ROI, but that’s a discussion for another day).

If the item can’t be delivered in the Sprint, the PO can simply look at how many stories have been spawned from the epic item and determine the likelihood of it being delivered in the next Sprint or the Sprint after, based on how many stories the team usually gets through. This leads me nicely on to the topic of how we measure velocity in the absence of story points.

## How do we measure velocity?

Now I’m moving firmly into Duarte territory. The answer is we count stories rather than accumulate story points, hence negating the need to estimate. As I mentioned before, teams break stories down into roughly the same size, so counting how many stories are delivered in each Sprint makes for a satisfactory measure of velocity. If the team usually delivers 5 stories with zero defects and then one Sprint delivers 6 or 7 stories with zero defects, an improvement has been made (disregarding variance, which exists whatever unit you use to measure velocity).

Due to the hunch I mentioned earlier, I have been tracking velocity as both story count and points for my current team and making projections using both methods. As I suspected (and as [Duarte points out](http://softwaredevelopmenttoday.blogspot.com.au/2012/01/story-points-considered-harmful-or-why.html) with much supporting data), story count provides just as good, if not better a measure of progress and predictability as story points do. Therefore why spend all the time, cost and effort on estimation sessions and velocity calculations?

While story count works great for velocity, I would still warn against using this or any other velocity measure as a way of predicting when you can deliver. You should know when you are delivering and only be predicting what you can deliver at that date. Don’t leave your delivery date to chance, even if you are using historical data rather than guesswork to predict how many stories can be done.

What you can do, however, is use velocity to help the PO understand scoping trade-offs in the backlog (_“the data tells me the team can deliver 20 more stories before the release date, so I’ll make sure the most important 20 are at the top of the backlog“)_.

## Conclusion

It’s taken me several years to come to this conclusion. But, if you think about it, people laugh and joke about estimates all the time. Everyone knows they’re a guess. Everyone knows they’re wrong. Yet we continue to do them. I believe it is time for us to acknowledge that it makes far more sense to eliminate the risk and cost of estimation completely and use only empirical data (as Agile and Scrum promotes) to make predicitions.

In a world without estimation overhead the team is likely to be more happy and productive, the inefficiency of spending time on estimating rather than delivering working software is eliminated and the PO will have real data with which to make decisions rather than guesses made under pressure.

To summarise:

* Don’t estimate your delivery date – base it on your budget or a firm deadline
* Don’t estimate your scope – allow it to emerge in order to reap the benefits of building products with agility
* Don’t explicitly estimate product backlog items (stories)
* Use historical data (story count) to predict scope delivery on a given date
* Use just-in-time implicit estimation (story breakdown in Sprint Planning) and past data to estimate cost (ROI) of story delivery

I don’t like to guess, but I predict that not estimating your projects will make success far more probable :)

---
Auteur : [Neil Killick](https://plus.google.com/u/0/+NeilKillick/about)  
Source : [Should We Estimate Software Projects… At All?](http://neilkillick.com/2012/04/12/do-not-estimate-software-projects-at-all/)  
Date de parution originale : 12 Avril 2012  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 14/09/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}


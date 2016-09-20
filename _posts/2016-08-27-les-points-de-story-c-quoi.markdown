---
layout: post
title:  "Les points de story, c’est quoi ?"
date:   2016-08-27 00:00:01
published: false
categories: 
- estimation
---

Story points are a unit of measure for expressing an estimate of the overall effort that will be required to fully implement a product backlog item or any other piece of work.

Les points de story sont une unité de mesure pour exprimer une estimation de l’effort général qui sera exigé pour implémenter complètement un item du _product backlog_ ou n’importe quel autre élément de travail à faire.

When we estimate with story points, we assign a point value to each item. The raw values we assign are unimportant. What matters are the relative values. A story that is assigned a 2 should be twice as much as a story that is assigned a 1. It should also be two-thirds of a story that is estimated as 3 story points.

Lorsque nous estimons avec des points de story, nous donnons une certaine valeur en point à chaque item. Les valeurs brutes que nous donnons en tant que tel ne sont pas importantes. Ce qui compte c’est les valeurs relatives. Une story à laquelle est donnée une valeur de 2 devrait valoir deux fois plus qu’une story valant 1. Elle devrait valoir également les 2/3 d’une story valant 3 points.

Instead of assigning 1, 2 and 3, that team could instead have assigned 100, 200 and 300. Or 1 million, 2 million and 3 million. It is the ratios that matter, not the actual numbers.

À la place de mettre 1, 2 et 3, cette équipe aurait pu mettre 100, 200 et 300. Ou 1 million, 2 millions et 3 millions. C’est le ratio qui compte, pas les nombres en tant que tel.

## What Goes Into a Story Point?

## Qu’est ce qu’il y a dans un point de story ?

Because story points represent the effort to develop a story, a team’s estimate must include everything that can affect the effort. That could include:

Parce que les points de _story_ représente l’effort pour développer une story, l’estimation d’une équipe doit inclure tout ce qui peut impacter l’effort. Cela pourrait être

* The amount of work to do
* The complexity of the work
* Any risk or uncertainty in doing the work

* La quantité de travail à faire
* La complexité de ce travail
* Tout risque ou incertitude pouvant arriver en accomplissant le travail

When estimating with story points, be sure to consider each of these factors. Let’s see how each impacts the effort estimate given by story points.

Lorsque vous estimez avec des points de _story_, soyez certain de prendre en considération ces éléments. Voyons comment chacun impacte l’estimation de l’effort donné par les points de _story_.

##The Amount of Work to Do

##La quantité de travail à faire

Certainly, if there is more to do of something, the estimate of effort should be larger. Consider the case of developing two web pages. The first page has only one field and a label asking to enter a name. The second page has 100 fields to also simply be filled with a bit of text.

C’est sûr que s’il y a plus de chose à faire sur quelque chose, l’estimation de l’effort devrait être plus élevée. Prenez par exemple le cas du développement de deux pages web.  La première page possède un seul champ et un seul libellé demandant de saisir un nom. La seconde page comporte 100 champs dans lesquels seront à remplir des informations textuelles.

The second page is no more complex. There are no interactions among the fields and each is nothing more than a bit of text. There’s no additional risk on the second page. The only difference between these two pages is that there is more to do on the second page.

La seconde page n’est pas plus complexe que la première. Il n’existe aucune interaction spécifique dans les champs et chacun ne contient rien de plus que quelques éléments textuels. Il n’y a pas plus de risques sur cette seconde page. La seule différence entre ces deux pages est qu’il y a davantage à faire sur la seconde page.

The second page should be given more story points. It probably doesn’t get 100 times more points even though there are 100 times as many fields. There are, after all, economies of scale and maybe making the second page is only 2 or 3 or 10 times as much effort as the first page.

La seconde page devrait obtenir plus de points de _story_. Elle n’aura probablement pas 100 fois plus de points que la première page tant bien même qu’elle aurait 100 fois plus de champs. Il y a, après tout, des économies d’échelle et peut être que la réalisation de la deuxième page prendra 2, 3 ou 10 fois plus d’effort que la première page.

##Risk and Uncertainty

##Risque et incertitude

The amount of risk and uncertainty in a product backlog item should affect the story point estimate given to the item.

La quantité de risque et d’incertitude d’un item de _product backlog_ devrait impacter l’estimation en points de _story_ de cet item.

If a team is asked to estimate a product backlog item and the stakeholder asking for it is unclear about what will be needed, that uncertainty should be reflected in the estimate.

S’il est demandé à une équipe d’estimer un item de _product backlog_ et que la demande de la partie prenante n’est pas claire à ce sujet, cette incertitude devrait se refléter dans l’estimation.

If implementing a feature involves changing a particular piece of old, brittle code that has no automated tests in place, that risk should be reflected in the estimate.

Si l’implémentation d’une fonctionnalité implique de modifier un vieux morceaux de code sensible n’ayant pas de tests automatisés, ce risque devrait se refléter dans l’estimation. 

##Complexity

##Complexité

Complexity should also be considered when providing a story point estimate. Think back to the earlier example of developing a web page with 100 trivial text fields with no interactions between them.

La complexité devrait prise en compte lors de l’estimation. Rappelez-vous de l’exemple précédent du développement d’une page web comportant 100 champs textes n’ayant acune interaction entre eux.

Now think about another web page also with 100 fields. But some are date fields with calendar widgets that pop up. Some are formatted text fields like phone numbers or Social Security numbers. Other fields do checksum validations as with credit card numbers.

Maintenez pensez à une autre page  contenant elle aussi 100 champs. Mais certains d’entre eux sont des champs dates avec des contrôles calendriers. Certains autres sont des champs textes formatés comme des numéros de téléphones ou des numéros de sécurité sociale. D’autres encore sont des champs de validations calculés comme pour les numéros de cartes de crédit.

This screen also requires interactions between fields. If the user enters a Visa card, a three-digit CVV field is shown. But if the user enters an American Express card, a four-digit CVV field is shown.

Ce type d’écran demande des interactions entre les champs. Si l’utilisateur sélectionne une carte Visa, alors un champ CVV sur trois positions apparaît. Mais si l’utilisateur sélectionne une carte American Express, alors un champ CVV sur quatre position apparaît.

Even though there are still 100 fields on this screen, these fields are harder to implement. They’re more complex. They’ll take more time. There’s more chance the developer makes a mistake and has to back up and correct it.

Même s’il y a toujours 100 champs sur cet écran, ils sont plus difficiles à implémenter. Ils sont plus complexes. Ils prendront plus de temps. Il y a plus de chances qu’un développeur fasse une erreur, soit amené à y revenir et à la corriger.

This additional complexity should be reflected in the estimate provided.

Cette complexité supplémentaire devrait se refléter dans l’estimation.

##Consider All Factors: Amount of Work, Risk and Uncertainty, and Complexity

##Prendre en compte tous les éléments : quantité de travail, risque et incertitude, et complexité

It may seem impossible to combine three factors into one number and provide that as an estimate. It’s possible, though, because effort is the unifying factor. Estimators consider how much effort will be required to do the amount of work described by a product backlog item.

Il semble impossible de combiner les trois éléments en un seul nombre et d’en donner une estimation. C’est possible, tout de même, parce que l’effort est l’élément unificateur. Les personnes qui estiment prennent en compte la quantité d’effort qui sera exigé pour faire la quantité de travail décrite dans l’item du _product backlog_.

Estimators then consider how much effort to include for dealing with the risk and uncertainty inherent in the product backlog item. Usually this is done by considering the risk of a problem occurring and the impact if the risk does occur. So, for example, more will be included in the estimate for a time-consuming risk that is likely to occur than for a minor and unlikely risk.

Ils prendront alors en considération la quantité d’effort pour gérer le risque et l’incertitude inhérent à cet item. Généralement, cela est fait en prenant en considération que le risque de survenance d’un problème et l’impact si le risque survient. Donc, par conséquent, il y aura une majoration de l’estimation pour un risque de perte de temps ayant une forte probabilité de se produire plutôt que pour un risque ayant peu de chance de se produire.

Estimators also consider the complexity of the work to be done. Work that is complex will require more thinking, may require more trial-and-error experimentation, perhaps more back-and-forth with a customer, may take longer to validate and may need more time to correct mistakes.

Est pris aussi en compte la complexité du travail à faire. Un travail qui est plus complexe exigera plus de réflexion, pourra exigé plus d’expérimentation par essais et erreurs successifs, peut-être plus d’allers-retours avec le client, pourra prendre plus de temps à être valider et peut-être plus de temps à en corriger les erreurs.

All three factors must be combined.

L’ensemble de ces trois éléments doivent être combinés

##Consider Everything in the Definition of Done

##Prendre en compte l’ensemble dans la définition de fini

A story point estimate must include everything involved in getting a product backlog item all the way to done. If a team’s definition of done includes creating automated tests to validate the story (and that would be a good idea), the effort to create those tests should be included in the story point estimate.

Une estimation en points de _story_ doit inclure l’ensemble des trois éléments pour mener à bien un item du _product backlog_. Si la définition de fini d’une équipe inclue la création de tests automatisés pour valider la _story_ (et cela devrait être une bonne idée), alors l’effort pour créer ces tests devrait être ajouté à l’estimation en point de _story_.

Story points can be a hard concept to grasp. But the effort to fully understand that points represent effort as impacted by the amount of work, the complexity of the work and any risk or uncertainty in the work will be worth it.

Les points de _story_ peuvent être un concept difficile à appréhender. Mais l’effort pour comprendre vraiment ça représente l’effort à fournir impacté par la quantité de travail, la complexité du travail et les risques ou les incertitudes dans le travail le vaut bien ++fin de phrase à revoir

---  
Auteur : [Mike Cohn]()  
Source : [What Are Story Points?](https://www.mountaingoatsoftware.com/blog/what-are-story-points)  
Date de parution originale : 23 Août 2016  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 07/09/2016  

NdT : Fabrice Aimetti et moi-même avons traduit ce texte, chacun de notre côté, chacun ignorant que l’autre le faisait (ce sont des choses qui arrivent), Fabrice ayant publié le premier sur le wiki d’Ayeba, cette traduction ne sera pas publiée sur le site des traducteurs agiles - néanmoins, je laisse le texte de la traduction disponible en l’état au cas où.
---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}
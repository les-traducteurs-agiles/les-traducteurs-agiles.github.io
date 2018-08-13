---
layout: post
title:  "Pourquoi je préfère la planification pilotée par l’engagement"
date:   2016-11-27 00:00:01
published: true
tags: 
- scrum
- planification
---

Ces dernières semaines, j’ai décris deux approches alternatives de la planification de sprint :

<div align="right" style="float:right; padding-left:30px" >
  <img title="Main" src="{{ site.url }}assets/mountain_goat/boxer-tattoos.jpg" />
</div>

* [La planification de sprint pilotée par la vélocité](http://www.les-traducteurs-agiles.org/scrum/planification/2016/10/25/planification-sprint-pilotee-par-la-velocite.html)
* [La planification de sprint pilotée par l’engagement](http://www.les-traducteurs-agiles.org/scrum/planification/2016/11/09/planification-sprint-pilotee-par-l-engagement.html)

Cette semaine, je voudrais expliquer pourquoi je préfère la planification de sprint pilotée par l’engagement. Tout d’abord, voici un bref récapitulatif de chacune de ces approches.

&nbsp;

### Petit résumé des approches de planification de sprint

Dans la planification de sprint pilotée par la vélocité, l’équipe sélectionne un ensemble d’items du _product backlog_ dont la somme des estimations à grosses mailles (en points de story ou en jours idéaux généralement) se rapproche le plus possible de leur vélocité moyenne.

Dans la planification de sprint pilotée par l’engagement, l’équipe s’engage sur un item du _product backlog_ en identifiant et en estimant grosso modo les tâches qui y sont rattachées, et elle arrête ce processus lorsqu’elle estime que le sprint est remplit.

Comme l’ “engagement” est souvent confondu avec “garantie”, cette approche est plus connue sous le nom de planification de sprint basée sur la capacité.

### La vélocité est fluctuante

Pour commencer à comprendre pourquoi je préfère l’approche pilotée par l’engagement pour la planification de sprint, considérons le diagramme ci-dessous nous montrant les vélocités d’une équipe sur une période de neuf sprints. La première chose que vous devriez remarquer est que la vélocité n’est pas stable. Elle fluctue de sprint en sprint.

![Diagramme de représentation de la vélocité par rapport aux sprints]({{ site.url }}assets/mountain_goat/velocite_sprint_pourquoi.jpg)

Un premier inconvénient majeure d’une planification pilotée par la vélocité est que la vélocité fluctue trop pour vraiment être fiable dans une planification à court terme (c’est-à-dire au niveau du sprint). Mon expérience montre que la vélocité fluctue de plus ou moins 20%. Cela signifie qu’une équipe dont la vélocité est de 20 pourrait facilement se retrouver avec une vélocité de 16 sur un sprint puis 24 au prochain sprint, ou avoir une toute autre fluctuation tout aussi aléatoire.

Nous pourrions être tenté de dire d’une équipe, dont la vélocité moyenne de 20 et qui réalise parfois pour 24 points d’unités de travail mais qui peut parfois n’en faire que 16,  qu’elle accomplit plus ou moins de travail pendant ces différents sprints. Et cela doit être indéniablement le cas pour un certain nombre d’équipes. Toutefois, une certaine partie de cette fluctuation est imputable à l’imprécision des unités de mesures utilisées pour estimer les items du _product backlog_.

Par exemple, la plupart des équipes qui font des estimations en points de story utilisent un sous-ensemble de type d’estimations tel que la suite de Fibonacci 1, 2, 3, 5, 8, 13 ou une autre suite mathématique (par exemple 1, 2, 4, 8, 16). Lorsqu’une équipe utilisant la suite de Fibonacci finie une story estimée à 5 points, elle aura peut être en réalité terminée une story valant que 4 points. Ceci donc tend à donner une légère surévaluation de la vélocité.

Dans le long terme, cela ne sera sans doute pas un problème, la loi des grands nombres peut se manifester et les choses pourront alors être se lisser dans le temps. Dans le court terme, toutefois, cela peut créer des problèmes.

### Ancrage[^1]

Un deuxième problème avec la planification de sprint basée sur la vélocité est due à l’effet d’ancrage. L’ancrage est la propension pour une estimation à être influencée de manière indue par une information parvenue précédemment.

Un bon exemple d’ancrage qui me vient à l’esprit, c’est lors de l’approche des fêtes de Noël. Supposez que vous allez dans un magasin et que vous voyez une veste qui vous plait. Il y a une étiquette indiquant $400 mais le prix est barré et un nouveau prix de $200 est marqué. Votre cerveau pense instantanément “Super ! Une veste de $400 pour seulement $200 !”. Et c’est bien la raison pour laquelle le magasin vous a indiqué l’ancien prix.

Qui se préoccupe de savoir à quel prix se vendait cette veste avant ? C’est $200 aujourd’hui. C’est tout ce qui devrait compter dans votre décision d’acheter ou pas. Toutefois, une fois que l’information du prix de $400 est entrée dans votre cerveau, il est difficile de l’ignorer. Elle s’est insinuée dans votre esprit pour vous dire que vous faisiez une bonne affaire avec cette veste à $200.

_Je ne m’appesantirai pas plus sur le sujet ici, le meilleur papier que j’ai pu lire sur l’ancrage est de Magne Jørgensen et de Stein Grimstad, dont le titre est_ “[The Impact of Irrelevant and Misleading Information on Software Development Effort Estimates.](https://www.simula.no/research/se/publications/Simula.SE.299/simula_pdf_file/)”)

### Ancrage et planification pilotée par la vélocité

Mais qu’est-ce que l’ancrage a à voir avec la planification de sprint ?

Prenons une équipe dans une réunion de planification de sprint pilotée par la vélocité. Elle a sélectionné un nombre de stories équivalent à sa vélocité moyenne. Les membres de l’équipe se demandent ensuite si cet ensemble de stories représente la bonne quantité de travail à accomplir; (Comme cela a été décrit, dans l’article sur la planification de sprint pilotée par la vélocité, ils peuvent aussi identifier les tâches et estimer ces tâches pour pouvoir répondre à cette question.)

Une équipe faisant une planification de sprint pilotée par la vélocité est prédisposée à dire “Oui, nous pouvons faire cela” même si elle ne peut pas le faire. Elle est ancrée par le fait de savoir que la quantité de travail sélectionnée est identique à sa vélocité moyenne.

C’est exactement pareil que ce que j’ai pu vous expliquer sur l’étiquette du prix de $400 sur la veste et que je vous ai posé la question “À quel prix pensez-vous que cette veste est à vendre ?”. Même si vous n’avez pas dit exactement $400, ce prix de $400 est dans votre tête et il se sera ancré en vous.

Donc, à cause de l’ancrage, une équipe avec une vélocité moyenne de 20 est encline à dire que le sprint est remplit de manière approprié avec 20 points - même si le travail se situe plus vraisemblablement à 16 ou à 24 unités de travail.

Cela conduira parfois les équipes à en faire moins qu’elles ne pourraient en faire. Cela pourrait aussi mener parfois les équipes à en faire plus. Mais dans ces cas de figure, mon expérience montre que les équipes sont plus enclines à laisser tomber un ou deux items de backlog. De manière générale, mon expérience montre aussi que les équipes ont plutôt tendance à abandonner des items plutôt qu’à en ajouter.

### La vélocité est très utile dans le cadre d’une planification sur le long terme

J’imagine que vous pensez maintenant que je suis plutôt contre la planification de sprint pilotée par la vélocité. C’est seulement à moitié vrai. Même si je ne suis pas un grand fan de l’utilisation de la vélocité pour planifier un sprint, je suis sûrement l’un de ses plus grands fans au monde pour l’utilisation de la vélocité pour le long terme. Et j’ai certainement écris plus que quiconque à ce sujet.

Le problème avec la planification de sprint pilotée par la vélocité est que la vélocité est trop fluctuante pour être utile à court terme. Pour illuster mes propos, supposez que vous travaillez dans une entreprise de lessivage de voiture. Le matin de votre premier jour, votre patron vous annonce que vous aurez un quota de travail à respecter : vous devez lavez quatre voitures à l’heure.

À la fin de la première heure, vous n’avez lavé que trois voitures. Serez-vous viré ? Bien sûr que non. Ce n’était que votre première heure de travail et peut être que les voitures que vous avez lavées étaient trois grosses voitures. Ou peut être que le temps était nuageux et que seulement trois personnes ont amené leurs voitures se faire laver.

Qu’en est-il à la fin du premier jour, soit 8 heures plus tard ? Vous devriez avoir lavé 32 voitures. Mais vous en lavez seulement 30. Est-ce que vous serez viré alors ? À nouveau, sûrement pas.

Qu’en sera t’il à la fin du mois ? En prenant 20 jours dans le mois et 32 voitures par jour, cela signifie que vous devriez avoir lavé 640 voitures. Supposons néanmoins que vous en ayez nettoyé 600. (C’est le même pourcentage de nettoyage que celui avec les 30 voitures lavées à la place des 32 voitures par jour). Est-ce que votre patron devrait vous maintenant virer ? Peut être pas encore, mais il devient clair que vous n’atteignez pas votre quota.

Qu’en sera t’il si vous accomplissez le même pourcentage à la fin de l’année ? Si ce quota est bien définit - et que tous les autres employés l’atteignent -  arrivé à un certain moment votre patron devrait considérer se séparer de vous (ou de gérer d’une manière ou d’une autre votre productivité quelque peu déficiente, mais cet article ne porte pas sur comment gérer efficacement des problèmes de productivité).  

Le quota est utile de la même manière que la vélocité peut l’être : sur le long terme. Réfléchissez donc à ce que nous pourrions penser de cette entreprise de lavage et de sa gestion si un employé était viré dans l’heure qui suit la non-atteinte de son quota de voitures lavées. Le titulaire du poste qui serait resté le plus longtemps l’aurait été pendant 3 jours. Donc même si ce quota peut être utile lorsqu’il est mesuré mensuellement, il est inutile lorsqu’il est mesuré toutes les heures.

La vélocité est utile dans le long terme, pas dans le court terme. Une équipe avec 30 items dans le _product backlog_ à livrer peut faire la somme des estimations de ces items et prévoir quand ils seront terminés. Une équipe avec trois items dans le _product backlog_ à terminer aurait tout intérêt à faire la bonne vieille décomposition en tâches de ces trois items plutôt que de se reposer sur la vélocité.

### Et maintenant, je fais quoi ?

Si vous avez déjà fait des planifications de sprints basées sur la vélocité et que cela fonctionne pour vous, ne changez rien. Toutefois, si votre équipe ou vous-même êtes novices en Scrum ou si votre équipe connaît certaines des difficultés que j’ai pu décrire ici, alors je vous recommande d’utiliser la planification de sprint basée sur l’engagement.

[^1]: une définition simple de l’ancrage est disponible sur [Wikipedia](https://fr.wikipedia.org/wiki/Ancrage_(psychologie)) (NdT)

---  
Auteur : [Mike Cohn](https://www.mountaingoatsoftware.com/company/about-mike-cohn)  
Source : [Why I Prefer Commitment-Driven Sprint Planning](https://www.mountaingoatsoftware.com/blog/why-i-prefer-commitment-driven-sprint-planning)  
Date de parution originale : 04 Novembre 2014  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 27/11/2016

---

Copyright ©1998-2016 Mountain Goat Software. All Rights Reserved.

---

{% include share_buttons.html %}

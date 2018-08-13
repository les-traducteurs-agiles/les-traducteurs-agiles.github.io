---
layout: post
title:  "LeSS - La Définition du Fini"
date:   2017-10-29 00:01
published: true
tags:
- less
---


[<< Portail LeSS < Portail Framework](http://www.les-traducteurs-agiles.org/2016/12/28/less-portail-framework.html)

Dans un objectif d’efficacité, les cycles inspection-adaptation de Scrum exigent de la transparence. Définir formellement ce qui est “fini” permet de réduire la variabilité, la probabilité d’avoir du travail non terminé, de pouvoir mesurer de manière non ambigüe l’avancement (“fini” ou “non fini”) et ainsi d’accroître le niveau de transparence.

Une Définition du Fini parfaite inclut tout ce que l’organisation doit faire afin de livrer un produit aux clients. Cela devrait être relativement facile pour une équipe produit. Lorsqu’une équipe n’est pas capable de proposer une Définition du Fini parfaite alors elle définit le “fini” comme étant un sous-ensemble de l’ensemble parfait. L’objectif de l’équipe est de s’améliorer, afin qu’un jour, sa Définition du Fini soit parfaite et qu’elle soit en capacité de livrer une fois ou plus par Sprint.

La Définition du Fini est une liste de critères sur laquelle l'équipe s’est mis d’accord et que le logiciel devra respecter au niveau de chaque item du Backlog Produit. Atteindre ce niveau de complétude exige que l’équipe accomplisse un ensemble de tâches. Lorsque toutes les tâches sont faites, l’item est fini. Ne confondez pas la Définition du Fini avec les critères d’acceptation, qui représentent les conditions spécifiques qu’un item doit respecter afin d’être accepté. La Définition du Fini s’applique uniformément à tous les items du Backlog Produit.

## Création de la Définition du Fini

La Définition du Fini initiale doit être acceptée avant le premier Sprint. Cela se fait généralement pendant l’[atelier d’affinage initial du Backlog Produit (fr)](http://www.les-traducteurs-agiles.org/2017/10/30/less-l-affinage-initial-du-backlog-produit.html).

La création d’une Définition du Fini suit les étapes suivantes :

* Définir les activités nécessaires pour livrer aux clients finaux.
* Décider quelles activités peuvent être faites lors de chaque Sprint.


Explorons ces différentes étapes en détails.

### Définir les activités nécessaires pour livrer aux clients finaux

La question clé est : “Quelles sont les activités nécessaires afin de livrer notre produit ?”

* Livrer veut dire “livrer aux clients finaux” et non “sortir le produit du département développement”.
* Remettre en cause le besoin des artefacts intermédiaires. Avons-nous vraiment besoin des documents de spécifications ?


Les équipes écrivent sur des notes adhésives les activités nécessaires. Ces activités incluent le codage, le test et peut inclure aussi le support client, la création d'un matériel informatique, voire même des activités marketing. Nous désignons cette liste sous le nom de “liste d’activités nécessaires pour avoir un Produit Potentiellement Déployable”.

À cette étape, vous avez créé pour l’organisation un [objectif de perfection (en)](https://less.works/less/principles/continuous-improvement-towards-perfection.html) : faire l’ensemble de ces activités pour chaque item à chaque Sprint. Les groupes Produit réalisent souvent à ce moment-là que cela va exiger d’eux beaucoup d’actions d’améliorations.

### Décider quelles activités peuvent être faites lors de chaque Sprint

La question clé est : “Compte tenu de notre contexte et de notre capacité actuelle, quelles sont les activités à faire lors de chaque Sprint ?”. Ce sous-ensemble est la Definition du Fini initial. Une Définition du Fini est bien fragile lorsque son périmètre se révèle être trop réduit et elle est robuste lorsque celle-ci s’étend jusqu’au Potentiellement Déployable.

Les équipes discutent de leur contexte et sélectionnent le sous-ensemble des activités que toutes les équipes pensent pouvoir accomplir de manière réaliste pendant le Sprint. C’est leur Définition du Fini initiale (voir l'exemple dans la figure ci-dessous). Les équipes qui peuvent faire plus étendront le périmètre de la Définition du Fini du produit et se l’appliqueront elles-mêmes.

La différence entre la Définition du Fini et le Potentiellement Déployable est appelé Travail Non Fini. Le Sprint se planifie à partir de la Définition du Fini, à l’exclusion du Travail Non Fini, dès le départ il est prévu qu’il reste non fini.

![Définition du fini]({{ site.url }}assets/less/definition-of-done-FR.png)

## Termes de la Définition du Fini

Les termes Potentiellement Déployable et Définition du Fini sont souvent utilisés de manière incohérentes, mais ils ont dans LeSS une signification très précise. Pour clarifier les termes :

**Potentiellement Déployable** — Ensemble des activités qui doivent être faites avant qu’un produit soit déployé.

**Définition du Fini** : Convention entre les équipes et le Product Owner à propos des activités à mener lors d’un Sprint. Une Définition du Fini est dite parfaite lorsqu’elle est équivalente au Potentiellement Livrable. Les équipes s'efforcent de s’améliorer pour atteindre une Définition du Fini parfaite.

**Travail Non Fini** : Différence entre la Définition du Fini et le Potentiellement Déployable. Lorsque la Définition du Fini est parfaite, alors il n’y a pas de Travail Non Fini. Dans le cas contraire, l’organisation doit alors décider : (1) Comment devons-nous gérer le Travail Non Fini, et (2) Comment pouvons-nous nous améliorer pour qu’il y ait moins de Travail Non Fini dans le futur.

**Inachevé, non abouti, ou non terminé** : Travail qui a été planifié dans un Sprint mais qui n’est pas terminé. On le confond souvent avec le Travail Non Fini. Du travail “inachevé” correspond à du travail que l’équipe a planifié mais qu’elle n’a pas terminé alors que du Travail Non Fini correspond à du travail qui n’a même jamais été planifié. Lorsqu’une équipe a du travail qui n’est pas terminé, elle devrait se sentir anxieuse et discuter d’actions d’améliorations pendant leurs rétrospectives.

Les équipes ne devraient jamais laisser du travail en cours à la fin d’un sprint et le "reporter" à celui d’après. Cela provoque un manque de transparence et réduit les possibilités de flexibilité. Si elles prévoient trop de travail, elles doivent retirer tout un tas d’items qu’elles n’ont pas encore commencé.

### Mathématiques de la Définition du Fini

**Potentiellement Déployable = Définition du Fini + Travail Non Fini**
**Travail dans l’Itération = Item du Backlog Produit * Définition du Fini**


## Travail Non Fini -> Risque et Retard

Explorons d'abord les effets d’un Travail Non Fini à travers un exemple.

Plusieurs équipes réalisent, conformément à la Définition du Fini, vingt Items du Backlog Produit lors du premier Sprint. Bien qu’aucun item ne soit laissé inachevé, il reste tout un tas de Travaux Non Finis en raison de leur pauvre Définition du Fini. Après que les équipes aient réalisé, conformément à leur Définition du Fini bien fragile, quarante items du Backlog Produit en trois Sprints. La quantité de Travail Non Fini a énormément augmenté donnant un faux sentiment d’avancement.

![Risque et retard]({{ site.url }}assets/less/causing-risk-and-delay-FR.png)

Mais ces équipes sont dans l’incapacité de déployer. Elles ont “fini” des fonctionnalités mais leur Définition du Fini bien précaire est la cause directe de la quantité de Travail Non Fini importante accumulée. Ce Travail Non Fini est à l’origine des retards constatés et d’un risque latent.

**Retard** — Pour mener à bien le Travail Non Fini des quantités d’efforts supplémentaires s’avèrent nécessaires. Cela génère un manque de flexibilité pour le Product Owner, il ne peut pas répondre tout de suite aux besoins et aux changements du marché. Les difficultés rencontrées par ce retard sont aggravées par le fait que l’effort fourni pour finir le Travail Non Fini est très variable et donc difficile à prédire.

**Risque** — Du Travail Non Fini a pour conséquence un manque de transparence. Les risques y sont latents. Par exemple, si les tests de performances restent Non Finis, cela retarde le risque d’avoir un système non-performant jusqu’au moment de la date de déploiement, là où ça fait le plus mal.

Un bon Product Owner veut une Définition du Fini parfaite car elle permet de réduire le facteur risque au niveau du produit et de réduire les retards.


---
Auteur : The LeSS Company B.V.  
Source : [Definition of Done - Large Scale Scrum (LeSS)](https://less.works/less/framework/definition-of-done.html)  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 29/10/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

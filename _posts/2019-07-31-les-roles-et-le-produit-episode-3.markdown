---
layout: post
title:  "les rôles et le produit - épisode 3"
date:   2019-07-31 00:01
published: false
tags:
- product owner
---

An agile approach requires a cross-functional team. That means that everyone on the team focuses on the same intent. That intent might be an entire product. It might be a feature set as part of a larger program. But, the team focuses as a team.

Une approche agile exige d'avoir une équipe pluridisciplinaire. Cela signifie que l'ensemble des personnes de l'équipe doit être focalisée sur le même but. Ce but peut être tout un produit. Cela peut être un ensemble de fonctionnalités qui font partie d'un programme plus grand. Mais l'équipe doit se concentrer à devenir une équipe.

That cross-functional team is a product team or a feature team. I tend to call them feature teams because they might move from feature set to feature set when they work as part of a program or over time as the product evolves.

L'équipe pluridisciplinaire est une équipe produit ou une équipe _feature_.  J'ai tendance à les appeler des équipes _feature_ parce qu'elle vont d'un ensemble de fonctionnalité à un autre lorsque lorsqu'elles travaillent dans le cadre d'un programme ou dans la durée au fur et à mesure que le produit évolue.

I don't actually care what you call these teams, as long as you have the same intent: the _team_ works together to finish work on a product or feature set.

Je ne me préocuppe pas vraiment comment vous pouvez appeler ces équipes, aussi longtemps que vous avez le même but : que l'équipe travaille de concert pour finir le travail à faire sur un produit ou sur un ensemble de fonctionnalités.

## Feature Teams Don't Have Cross-Team Interdependencies

## Les équipes _feature_ n'ont pas de dépendances interéquipes

[![implement by feature](https://www.jrothman.com/wp-content/uploads/2013/01/implementbyfeature1-300x191.jpg)](https://www.jrothman.com/wp-content/uploads/2013/01/implementbyfeature1.jpg)You might have seen my implement-by-feature images before. Notice the slicing of the feature through the architecture. When a team slices through the architecture, they are able to create small stories, the kind of stories that allow experiments and business value verification. (The minimums in Part 1.)

Vous avez peut-être déjà vu ces images[^1] que j'ai faites expliquant l'implémentation par fonctionnalité avant. Prêtez attention au découpage de la fonctionnalité à travers l'architecture. Lorsqu'une équipe fait ces découpages à travers l'architecture, elle est en capacité de créer plus facilement des _stories_ de petites tailles, le type de _stories_ qui nous permettent de faire des expérimentations et de vérifier la pertinence de la valeur métier. Les minimums évoqués dans le [1er épisode](http://www.les-traducteurs-agiles.org/2019/04/17/les-roles-et-le-produit.html)[^2] de cette série.

## Can Your Team Create Features Alone?

## Votre équipe est-elle seule à créer des fonctionnalités

[![](https://www.jrothman.com/wp-content/uploads/2019/04/curlicue.teamsbyarchlayer-300x184.png)](https://www.jrothman.com/wp-content/uploads/2019/04/curlicue.teamsbyarchlayer.png)But, I don't see teams being able to implement by feature often enough. I more often see this organization, where the teams focus _across_ the architecture, not through it.

Mais, je ne vois pas assez souvent des équipes qui soient en capacité d'implémenter par fonctionnalité. Je vois le plus souvent ce type d'organisation, dans lequel les équipes se concentrent à passer au-dessus de l'architecture et non à travers.

The platform team provides the red pieces at the bottom.  The platform team is a cross-functional team with developers and QA and maybe a DBA if they need it. However, even if they are cross-functional, they are still a component team because they can't create a feature slice through the architecture.

L'équipe en charge de la plateforme fournit les morceaux en rouge en bas du schéma. L'équipe de la plateforme est une équipe pluridisciplinaire avec des développeurs, un ou des testeurs et peut être un administrateur de base de données si nécessaire. Toutefois, même si elle est pluridisciplinaire, elle reste une équipe composant parce qu'elle est incapable de créer une tranche de fonctionnalité à travers l'architecture.

Neither can the Middleware team (dark green), or the App layer team(s) (blue) or the GUI (teal). (If you are color blind, can you see any of the colors in here? If not, what would work for you? Thanks.)

Et ce n'est pas mieux que ce soit pour l'équipe middleware (en vert foncé), ou l'équipe s'occupant de la couche applicative (en bleu) ou celle s'occupant de l'IHM (en opale). (Si vous êtes daltonien, êtes-vous en capacité de voir les couleurs ? Si ce n'est pas le cas, pourriez-vous me dire ce qu'il conviendrait à la place ? Merci).

When an organization is based around _project_ teams, they too often organize like this. The managers think the various component teams are more efficient if they focus on a layer of the architecture, rather than slicing through the architecture.

Lorsqu'une organisation est structurée autour d'équipes _projet_, elles sont trop souvent organisées de cette manière-là. Les responsables pensent que les équipes composant sont plus efficientes si elles se concentrent sur une couche de l'architecture, plutôt que de se frayer un chemin à travers l'architecture.

When organizations create component-based teams, even if the teams are cross-functional, they need to plan all together to see when a feature might be ready. They do need everyone in the room for Big Planning, where they have string connecting the various interdependencies. I explained about this in [How Long Are Your Iterations, Part 2.](https://www.jrothman.com/mpd/agile/2015/11/how-long-are-your-iterations-part-2/)

Lorsque des organisations mettent en place des équipes composants même si les équipes sont pluridisciplinaires, elles doivent planifier ensemble pour voir lorsqu'une fonctionnalité pourra être prête. Elles ont besoin que tout le monde soit présent dans la pièce pour faire le Grand Planning pendant lequel elles doivent relier les différentes interdépendances. J'ai déjà expliqué tout ceci dans mon article [How Long Are Your Iterations, Part 2.](https://www.jrothman.com/mpd/agile/2015/11/how-long-are-your-iterations-part-2/).

The planning is a problem because the team configuration means we interrupt the teams on a regular basis to replan. They're not working on new features. They spend time estimating and organization in prep for a new plan that might need to change the next week.

La planification est un problème en tant que tel parce que au niveau de la configuration de l'équipe cela signifie que nous interrompons les équipes régulièrement pour replanifier. Elles ne travaillent plus sur de nouvelles fonctionnalités. Elles passent un certain temps à estimer et à s'organiser en vue de préparer un nouveau plan qui pourrait être amené à changer la semaine d'après.

That's a problem, but it's even worse for the product value team. When teams organize by component, not features, the product value team cannot shepherd the business value of the product.

C'est un problème, mais c'est encore pire pour l'équipe valeur produit. Lorsque les équipes sont organisées par composants, non par fonctionnalités, l'équipe valeur produit s'avère incapable de guider et d'orienter la valeur métier du produit.

## Change Team Organization to Focus on Product or Features

## Changer l'organisation de l'équipe pour se concentrer sur le produit ou les fonctionnalités

I do recommend that the teams move from component-based teams to feature teams. I suggested one way everyone in a given location could do that in [One Experimental Possibility: Self-Organization from Component Teams to Feature Teams](https://www.jrothman.com/mpd/agile/2014/09/one-experimental-possibility-self-organization-from-component-teams-to-feature-teams/).

Je recommande vivement que les équipes passent d'équipes composants à des équipes features. J'ai proposé une certaine manière de faire pour que tout le monde dans un certain lieu géographique soit en capacité de le faire dans cet article [One Experimental Possibility: Self-Organization from Component Teams to Feature Teams](https://www.jrothman.com/mpd/agile/2014/09/one-experimental-possibility-self-organization-from-component-teams-to-feature-teams/).

The value of product or feature teams is that the product value team can then create small rolling waves and replan without a lot of pre-work in the form of story breakdown with estimation. Instead, they can use cycle time. For example, teams might always do an experiment in one day—they would timebox the work to one day and work on just that experiment as a team in one day.

L'intérêt et la valeur d'une équipe produit ou d'une équipe feature est que l'équipe valeur produit est en mesure de créer de petites vagues en continu et replanifier sans avoir à faire énormément de travail préparatoire de décomposition et d'estimation de _stories_. À la place de cela, elle peut utiliser le temps de cycle. Par exemple, les équipes devraient toujours faire une expérience sur une journée - elles devraient limiter le travail sur une journée et travailler en équipe uniquement sur cette expérience sur une seule journée.

When feature teams don't rely on anyone else to finish a feature, lots of the difficulties in product development becomes easier:

Lorsque les équipes feature ne sont pas dépendantes de qui que ce soit pour finir une fonctionnalité, un bon nombre de difficultés deviennent plus faciles à gérer :

* The team can deploy on its own
* The team can define its various cycle times, either with measurement or with timeboxing
* The product value team can replan more often with less pain
* Everyone spends much less time in meetings and in estimation because the  work has more ease.

* L'équipe peut déployer toute seule
* L'équipe peut définir ses propres temps de cycle, soit à partir d'un indicateur soit à partir d'une délai imparti
* L'équipe valeur produit est en mesure de replanifier plus souvent avec moins de difficultés
* Tout le monde passe moins de temps en réunions et en estimation parce que le travail est rendu plus confortable

I will have to write a post about the cost of creation. Argh, this series is getting longer!

Je pense que je vais devoir écrire un article à part entière sur le coût de la création. Argh, cette série d'articles devient de plus en plus longue !

When everyone focuses on _product-based_ roles instead of project-based roles, everyone wins. (You can still do projects. Yes, that's part of the next post, I think.)

Lorsque tout le monde est focalisé sur des rôles orientés produit plutôt qu'orientés proejt, tout le monde y gagne. (Vous pouvez toujours faire des projets. Et cela fera l'objet aussi, je pense, du prochain article).

[^1]: NdT : [ici](https://www.jrothman.com/mpd/program-management/2013/01/managing-the-stream-of-features-in-a-program/) pour être plus précis
[^2]: NdT : par minimum, l'auteure fait allusion aux notions de MVP et de MMF évoquées dans le 1er épisode de cette série d'articles
---
Auteur : [Prénom_Nom](url_bio)  nbsp
Source : [Titre_article_en_vo](url_article_en_vo)  nbsp
Date de parution originale : jj_MMMM_yyyy  nbsp

---
Traducteur : [Prénom_Nom](url_bio)  nbsp
Date de traduction : jj/mm/yyyy  nbsp

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

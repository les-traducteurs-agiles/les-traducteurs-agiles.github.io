---
layout: post
title:  "Les rôles et le produit - épisode 3 : équipes orientées produit ou feature vs équipes projet"
date:   2019-08-03 00:01
published: true
tags:
- product owner
---

Une approche agile nécessite d'avoir une équipe pluridisciplinaire. Cela veut dire aussi que toutes les personnes de l'équipe doivent être concentrées sur le même but. Il peut s'agir d'un produit dans sa globalité, d'un ensemble de fonctionnalités qui font partie d'un programme plus grand. Mais l'équipe doit se concentrer en équipe.

L'équipe pluridisciplinaire est une équipe produit dénommée aussi équipe _feature_.  J'ai tendance à les appeler des équipes _feature_ parce qu'elle vont d'un ensemble de fonctionnalité à un autre lorsque lorsqu'elles travaillent dans le cadre d'un programme ou dans la durée au fur et à mesure que le produit évolue.

Je ne me préoccuppe pas vraiment de comment vous pouvez appeler ces équipes, aussi longtemps que vous avez le même but : à savoir que l'équipe travaille de concert pour finir le travail à faire sur un produit ou sur un ensemble de fonctionnalités.

## Les équipes _feature_ n'ont pas à gérer de dépendances entre équipes

<div align="left" style="float:left; padding-right:30px" >
  <a href="{{ site.url }}assets/johanna/implementbyfeature1-fr.png"><img title="Implémenter par fonctionnalité" src="{{ site.url }}assets/johanna/implementbyfeature1-fr.png" width="300px" height="191px"/></a></div> Vous avez peut-être déjà vu auparavant ces images[^1] que j'ai faites expliquant l'implémentation par fonctionnalité. Remarquez bien au passage comment chaque tranche de la fonctionnalité se fraye un passage à travers l'architecture. Lorsqu'une équipe fait ce type de passage à travers l'architecture, elle est en capacité de créer plus facilement des _stories_ de petites tailles, c'est ce type de _stories_ qui nous permettent de faire des expérimentations et de vérifier la pertinence de la valeur métier (autrement dit les minimums évoqués dans le [1er épisode](http://www.les-traducteurs-agiles.org/2019/04/17/les-roles-et-le-produit.html)[^2] de cette série).

## Votre équipe est-elle en mesure seule de créer des fonctionnalités toute seule ?

<div align="left" style="float:left; padding-right:30px" >
  <a href="{{ site.url }}assets/johanna/curlicue.teamsbyarchlayer-fr.png"><img title="Implémenter par fonctionnalité" src="{{ site.url }}assets/johanna/curlicue.teamsbyarchlayer-fr.png" width="300px" height="214px"/></a></div> Je ne vois pas assez souvent des équipes qui soient en mesure de pouvoir implémenter par fonctionnalité. Ce que je vois le plus souvent c'est ce type d'organisation, dans lequel les équipes se concentrent à passer au-dessus de l'architecture et non à travers.

L'équipe en charge de la plateforme fournit les morceaux en rouge en bas du schéma. L'équipe en charge de la plateforme est bien une équipe pluridisciplinaire avec des développeurs, un ou plusieurs testeurs et peut être un administrateur de base de données si nécessaire. Toutefois, même si elle est pluridisciplinaire, elle reste une équipe orientée composant parce qu'elle est incapable de créer une tranche de fonctionnalité à travers l'architecture.

Et ce n'est pas mieux que ce soit pour l'équipe middleware[^3] (en vert foncé), ou l'équipe s'occupant de la couche applicative (en bleu) ou celle s'occupant de l'IHM (en opale). (Pour les personnes daltoniennes, pourriez-vous me dire si vous voyez les couleurs ? Si ce n'est pas le cas, pourriez-vous me dire qu'est-ce qu'il pourrait vous convenir ? Merci)[^4].

Lorsqu'une organisation est structurée autour d'équipes _projet_, elles sont trop souvent organisées de cette manière-là. Les responsables pensent que les équipes orientées composant sont plus efficientes si elles se concentrent sur une seule couche de l'architecture, plutôt que de se frayer un chemin à travers l'architecture tranche de fonctionnalité par tranche de fonctionnalité.

Lorsque des organisations créent des équipes orientées composant même si les équipes sont pluridisciplinaires, elles doivent planifier toutes ensembles pour déterminer quand une fonctionnalité pourra être prête. Elles ont besoin que tout le monde soit présent dans la pièce pour faire le Grand Planning pendant lequel elles doivent relier les différentes interdépendances avec de la ficelle. Tout cela est expliqué dans mon article [How Long Are Your Iterations, Part 2.](https://www.jrothman.com/mpd/agile/2015/11/how-long-are-your-iterations-part-2/).

La planification est un problème en tant que tel parce qu'au niveau de la configuration de l'équipe cela signifie que nous interrompons les équipes régulièrement pour replanifier. Elles ne travaillent plus sur de nouvelles fonctionnalités. Elles passent un certain temps à estimer et à s'organiser en vue de préparer un nouveau plan qui pourrait être changé la semaine d'après.

C'est un problème, mais c'est encore pire pour l'équipe orientée valeur produit. Lorsque les équipes sont organisées par composants, non par fonctionnalités, l'équipe orientée valeur produit s'avère incapable de guider et d'orienter la valeur métier du produit.

## Changer l'organisation de l'équipe pour se concentrer sur le produit ou les fonctionnalités

Je recommande vivement que les équipes passent d'équipes orientée composant à des équipes features. J'ai d'ailleurs, dans l'article suivant, proposé une certaine manière de faire pour que tout le monde dans un lieu donné [^5] soit en capacité de le faire  [One Experimental Possibility: Self-Organization from Component Teams to Feature Teams](https://www.jrothman.com/mpd/agile/2014/09/one-experimental-possibility-self-organization-from-component-teams-to-feature-teams/).

L'intérêt d'une équipe orientée produit (dite aussi l'équipe feature) est que l'équipe orientée valeur produit est en mesure de créer de petites vagues en continu et de replanifier sans avoir à faire énormément de travail préparatoire en amont de décomposition et d'estimation de _stories_. En remplacement elle peut utiliser le temps de cycle. Par exemple, les équipes devraient toujours faire une expérience sur une journée - elles devraient limiter le travail sur une journée et travailler en équipe uniquement sur cette expérience d'une journée.

Lorsque les équipes feature ne sont pas dépendantes de qui que ce soit pour finir une fonctionnalité, un bon nombre de difficultés deviennent plus faciles à gérer :

* L'équipe peut déployer toute seule
* L'équipe peut définir ses propres temps de cycle, soit à partir d'un indicateur soit sur la base d'un délai imparti[^6]
* L'équipe orientée valeur produit est en mesure de replanifier plus souvent avec moins de difficultés
* Tout le monde passe moins de temps en réunions et en estimation parce que le travail est rendu plus confortable

Je pense que je vais devoir écrire un article à part entière sur le coût de la création. Argh, cette série d'articles devient de plus en plus longue à écrire !

Lorsque tout le monde est focalisé sur des rôles orientés produit plutôt qu'orientés projet, tout le monde y gagne. (Vous pouvez toujours faire des projets. Et cela fera l'objet aussi, je pense, du prochain article).

[^1]: NdT : [ici](https://www.jrothman.com/mpd/program-management/2013/01/managing-the-stream-of-features-in-a-program/) pour être plus précis
[^2]: NdT : par minimum, l'auteure fait allusion aux notions de MVP et de MMF évoquées dans le 1er épisode de cette série d'articles  
[^3]: NdT : ou intergiciel pour la traduction française toutefois moins répandue
[^4]: NdT : question posée par l'auteure dans le texte original
[^5]: NdT : et pas uniquement dans un même lieu géographique, l'auteure dans cet article évoque aussi cela pour des équipes géographiquement distribuées
[^6]: NdT : Ou _timebox_ pour les personnes préférant le terme anglo-saxon
---
Auteur : [Johanna Rothman](https://www.createadaptablelife.com/about)  
Source : [Product Roles, Part 3: Product or Feature Teams vs Project Teams](https://www.jrothman.com/mpd/agile/2019/04/product-roles-part-3-product-or-feature-teams-vs-project-teams/)  
Date de parution originale : 11 Avril 2019  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 03/08/2019  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

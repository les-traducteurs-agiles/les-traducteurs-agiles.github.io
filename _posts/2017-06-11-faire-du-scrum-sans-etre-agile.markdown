---
layout: post
title:  "Faire du Scrum sans être agile"
date:   2017-06-25 00:00:01
published: true
tags: 
- agile
- scrum
---

Récemment, j’ai rencontré une équipe qui disait pratiquer ce qu’elle appelait du Scrum. Elle avait des sprints de deux semaines et se réunissait chaque jour. Pourtant, leur responsable disait que Scrum était inutile dans son cas car cette équipe implémentait une architecture graphique qui ne serait utiliser dans le jeu que dans 6 mois. Elle “devait être laissée dans son coin” durant ce laps de temps.

Il est vrai que Scrum n’aidait pas vraiment en l’occurence. Les personnes qui travaillaient sur l’architecture étaient toutes sur des tâches indépendantes les unes des autres. Elles n’avaient pratiquement rien à se dire durant la journée et ne s’étaient nullement engagées sur un objectif commun de sprint, donc peu d’entre elles avaient le sentiment de faire partie d’une “équipe”.

Au fur et à mesure que je posais des questions ici et là, je suis tombé sur les personnes dont le travail dépendait de celui de l’équipe de l’architecture graphique, elles avaient le sentiment que cette équipe livraient généralement en retard et que ce qui était livré n’était pas ce qu’elles avaient demandé. Elles étaient donc directement impactées par cette situation critique et la qualité du jeu était compromise.

Le responsable de l’architecture n’avait jamais eu ce type d’écho jusqu’à présent. C’était une “révélation” intéressante.

En approfondissant, j’ai trouvé que le travail de l’architecture graphique était mené à partir d’exigences détaillées écrites au démarrage du projet par les artistes et les concepteurs .

Les choses commençaient à devenir plus claires.

Lorsque nous planifions de manière très détaillée dès le début, nous créons souvent un système poussé qui implique différents comportements dans le processus de développement. Cela peut amener à la création d’un cercle vicieux.

![Le cercle vicieux de la planification]({{ site.url }}assets/clinton_keith/viscious cycle_fr.jpg)

Les conceptions détaillées conduisent à des spécifications détaillées, à de l’allocation de ressources et de l’assignation de tâches - tout cela en raison d’une planification exhaustive. 
Ce type de système est connu généralement sous le nom de système poussé, dans lequel le travail est défini à l’avance et poussé en développement.  Lorsque inévitablement quelque chose arrive en retard, il se produit alors un carambolage quelque part dans le système qui conduit à des problèmes. Après la livraison du jeu vidéo, la direction décide alors qu’une planification plus détaillée devra alors être faite la prochaine fois et le cercle vicieux empire.

Agile est un système tiré dans lequel le travail est tiré en direction de la vision vers laquelle nous voulons que le jeu vidéo aille en fonction de ce que le jeu nous inspire. Nous mesurons alors ce qui doit être tiré dans le jeu et nous ajustons nos plans en fonction de cela et en fonction des besoins des joueurs et des développeurs. 

Scrum ne leur faisait pas grand bien. Nous devions donc examiner comment Scrum avait pu être utilisé.

L’organisation de l’équipe de l’architecture graphique ressemblait à cela :

<div align="right" style="float:right; padding-left:30px" >
  <img title="Vélocité" src="{{ site.url }}assets/clinton_keith/hierarchical_fr.jpg" />
</div>

* Le responsable pousse la vision dans un calendrier avec des tâches qui sont assignées aux personnes
* Le responsable gère le calendrier
* L’équipe est un groupe de développeurs exécutant les tâches assignées dans le calendrier
* Le responsable coordonne les dépendances transverses
* Le responsable résout les problèmes transverses
* L’intégration se fait péniblement, ce qui a pour conséquence de la reporter à plus tard (ce qui la rend encore plus pénible).

Cela contraste avec la manière dont une équipe Scrum pluri-disciplinaire travaille :

<div align="right" style="float:right; padding-left:30px" >
  <img title="Tirage du travail vers l’équipe" src="{{ site.url }}assets/clinton_keith/IMG_1380.jpg" />
</div>

* L’équipe bosse sur la base d’une vision partagée qui tire l’activité
* Le travail est planifié par l’équipe
* L’équipe a la main sur le calendrier à court terme (itération)
* L’équipe est en capacité de gérer la plupart des problèmes
* L’équipe se compose d’individus qui peuvent s’entraider 
* L’équipe intègre fréquemment des éléments du jeu ou de l’architecture afin de tester de la valeur qui arrive et gérer les risques

## Passer du Pousser au Tirer

Les systèmes poussés ont largement été discrédités y compris dans l’industrie manufacturière, dont le domaine d’activité a un caractère beaucoup plus prévisible que le développement de jeux vidéos, mais le système poussé reste toujours prédominant dans un certain nombre d’entreprises de développement logiciel y compris de développement de jeux vidéos. De nombreuses raisons culturelles expliquent pourquoi ce type de système persiste :

* Des structures en silo
* Le manque de confiance
* L’encadrement par la peur
* Le mythe d’une planification (détaillée) dès le début

Ces raisons ne s’en vont pas du jour au lendemain d’un coup de baguette magique.  Elles s’effacent lentement au fur et à mesure de la lente application de l’agilité : 

* En passant de longs cycles d’intégration, de test et de validation (par exemple 6 mois) à de plus petits
* En itérant en vue de réaliser des objectifs métiers, et non des objectifs architecturaux, autant que possible 
* En passant d’énormes conception détaillées à des résultats basés sur des objectifs détaillés à court terme
* En remplaçant des documents écrits par des conversations en face à face

There is a slow transformation away from managing for components to managing for player outcomes that doesn't occur overnight, but this transformation can begin immediately and the benefits can be seen every iteration.

Passer de la gestion de composants à la gestion des résultats des joueurs est le fruit d’une transformation lente qui ne peut se produire d’un simple claquement de doigts, mais cette transformation peut commencer immédiatement et les bénéfices constatées à chaque itération.

---
Auteur : [Clinton Keith](http://clintonkeith.com/)  
Source : [Scrumming without Agility](http://blog.agilegamedevelopment.com/2017/05/scrumming-without-agility.html)  
Date de parution originale : 29 Mai 2017  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 25/06/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



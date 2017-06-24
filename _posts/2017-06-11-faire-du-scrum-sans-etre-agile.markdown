---
layout: post
title:  "Faire du Scrum sans être agile"
date:   2017-03-12 00:00:01
published: true
tags: 
- agile
- scrum
---

 
I recently encountered a team which was practicing what they called Scrum.  They had two week sprints and met every day. However, their manager pointed out that Scrum was useless to them because they were implementing a graphic architecture, which wouldn't make it into the game for six months.   They "needed to be left alone" for the duration.

Récemment, j’ai rencontré une équipe qui disait pratiquer Scrum. Elle avait des sprints de deux semaines et se réunissait chaque jour. Pourtant, leur responsable disait que Scrum était inutile dans son cas car cette équipe implémentait une architecture graphique qui ne serait utiliser dans le jeu que dans 6 mois. Elle “avait donc besoin d’être isolée” pendant ce laps de temps.

It was true that Scrum wasn't helping.  The group of people working on the architecture were all working on independent tasks. They had nothing to talk about throughout the day and didn't commit to a shared sprint goal, so there was little feeling of "team" among them.

Il est vrai que Scrum n’aidait pas vraiment en l’occurence. Les personnes qui travaillaient sur l’architecture étaient toutes sur des tâches indépendantes les unes des autres. Elles n’avaient pratiquement rien à se dire durant la journée et ne s’étaient nullement engagées sur un objectif commun de sprint, donc peu d’entre elles avaient le sentiment de faire partie d’une “équipe”.

As I asked around, I found that those dependent on the graphics architecture felt that this group usually delivered their work late and what was actually delivered wasn't exactly what they'd asked for.  As a result they were impacted through crunch and the game's quality was compromised.

Au fur et à mesure que je posais des questions ici et là, je suis tombé sur les personnes dont le travail dépendait de de celui de l’équipe de l’architecture graphique, elles avaient le sentiment que cette équipe livraient généralement en retard et que ce qui était livré n’était pas ce qu’elles avaient demandé. Par conséquent, elles étaient directement impactées par cette situation critique et la qualité du jeu était compromise.

The architectural manager had never heard this.  That was an interesting "tell".

Le responsable de l’architecture n’avait jamais eu ce type d’écho jusqu’à présent. C’était une “révélation” intéressante.

Asking around further, I found that the graphics architectural work was driven by detailed requirements from the artists and designers written at the start of the project.

En approfondissait, j’ai trouvé que le travail de l’architecture graphique était mené à partir d’exigences détaillées écrites au démarrage du projet par les artistes et les concepteurs .

Now the picture was becoming clear.

Les choses commençaient à devenir plus claires.

When planning starts with high detail, we often create a push system that drives many behaviors throughout a development process.  It can create a vicious cycle:
The vicious planning cycle

LorsquE nous planifions de manière très détaillée dès le début, nous créons souvent un système poussé qui implique différents comportements dans le processus de développement. Cela peut amener à la création d’un cercle vicieux.

![The vicious planning cycle](https://3.bp.blogspot.com/-t6s5WBWxcAg/WSrgBej4h6I/AAAAAAAADtg/SIRalaOBCuIDf6OgBQDPX2_LE3bsBYsIwCLcB/s400/viscious%2Bcycle.png)

![Le cercle vicieux de la planification]({{ site.url }}assets/A3/A3.png)

Detailed designs lead to detailed specs, resource allocations and task assignments all driven by a comprehensive schedule.  This is usually described as a push system, where work is defined up front and pushed through development.  When something is inevitably late, there's a pileup somewhere which leads to problems.  After the game is shipped, management decides that more detailed planning is needed next time and the cycle gets more vicious.

Les conceptions détaillées conduisent à des spécifications détaillées, à de l’allocation de ressources et de l’assignation de tâches - tout cela en raison d’une planification exhaustive. 
Ce type de système est connu généralement sous le nom de système poussé, dans lequel le travail est défini à l’avance et poussé en développement.  Lorsque inévitablement quelque chose arrive en retard, il se produit alors un carambolage quelque part dans le système qui conduit à des problèmes. Après la livraison du jeu vidéo, la direction décide alors qu’une planification plus détaillée devra alors être faite la prochaine fois et le cercle vicieux empire.

Agile is a pull system where the work is pulled towards a vision of what we want in the game and what the game is telling us.  We measure what's pulled into the game and adjust our plans based on the pace of that and what the needs of the players and developers are.

Agile est un système tiré dans lequel le travail est tiré en direction de la vision vers laquelle nous voulons que le jeu vidéo aille en fonction de ce que le jeu nous inspire. Nous mesurons alors ce qui doit être tiré dans le jeu et nous ajustons nos plans en fonction de cela et en fonction des besoins des joueurs et des développeurs. 

Scrum wasn't doing them much good. We needed to look at how it was being used.

Scrum ne leur faisait pas grand bien. Nous devons examiner comment Scrum a été utilisé.

The organization of the graphics group looked like this:

L’organisation de l’équipe de l’architecture graphique ressemblait à cela :

<div align="right" style="float:right; padding-left:30px" >
  <img title="Pulling work into a swarming team" src="https://2.bp.blogspot.com/-bgZkDaChwvE/WSw6-XdO7FI/AAAAAAAADuA/yQet4bbsBY8FH6ckOl6kEL6aF9G6gkmzwCLcB/s1600/hierarchical.png" />
</div>

<div align="right" style="float:right; padding-left:30px" >
  <img title="Vélocité" src="{{ site.url }}assets/clinton_keith/hierarchical_fr.jpg" />
</div>

* The manager pushes the vision through a schedule of assigned
* The manager owns the schedule
* The team is a group of developers which execute assigned tasks
* The manager coordinates cross-functional dependencies
* The manager solves cross-fucntional problems
* Integration is painful, which leads to deferring it (which makes it even more painful).

* Le responsable pousse la vision dans un calendrier avec des tâches qui sont assignées
* Le responsable gère le calendrier
* L’équipe est un groupe de développeurs exécutant les tâches assignées dans le calendrier
* Le responsable coordonne les dépendances transverses
* Le responsable résout les problèmes transverses
* L’intégration se fait péniblement, ce qui a pour conséquence de la reporter à plus tard (ce qui la rend encore plus pénible).

Contrast this with the way a cross-functional Scrum team works:

Cela contraste avec la manière dont une équipe Scrum pluri-disciplinaire travaille :

https://2.bp.blogspot.com/-bgZkDaChwvE/WSw6-XdO7FI/AAAAAAAADuA/yQet4bbsBY8FH6ckOl6kEL6aF9G6gkmzwCLcB/s1600/hierarchical.png

<div align="right" style="float:right; padding-left:30px" >
  <img title="Pulling work into a swarming team" src="https://2.bp.blogspot.com/-pr9jjS6bP8c/WSsYmE3xLTI/AAAAAAAADtw/BSeQxRXoudgFWaKa1FnoVotOP5qiqWt5ACLcB/s1600/IMG_1380.jpg" />
</div>

<div align="right" style="float:right; padding-left:30px" >
  <img title="Vélocité" src="{{ site.url }}assets/clinton_keith/IMG_1380.jpg" />
</div>

* The team executes based on a shared vision that pulls work.
* Work is planned by the team
* The team owns the short term schedule (iteration)
* The team can address most problems
* The team consists of people who can address each other's problems through swarming.
* The game or architecture has frequent integrations to test the emergent value and address risk.

* L’équipe bosse sur la base d’une vision partagée qui tire l’activité
* Le travail est planifié par l’équipe
* L’équipe a la main sur le calendrier à court terme (itération)
* L’équipe est en capacité de gérer la plupart des problèmes
* L’équipe se compose d’individus qui peuvent s’entraider 
* L’équipe intègre fréquemment des éléments du jeu ou de l’architecture afin de tester de la valeur qui arrive et gérer les risques

## Moving from Push to Pull

## Passer du Pousser au Tirer

Push systems have been largely discredited even in manufacturing industries, which have far more predictability than game development, but push is still prevalent in many software development companies as well as game development.  There are many cultural reasons it sticks around, such as:

### RELECTURE

Les systèmes poussés ont largement été discrédités y compris dans l’industrie manufacturière, qui est pourtant un domaine d’activité ayant un caractère beaucoup plus prévisible que le développement de jeux vidéos, mais le système poussé reste toujours prédominant dans un certain nombre d’entreprises de développement logiciel y compris de développement de jeux vidéos. De nombreuses raisons culturelles expliquent pourquoi ce type de système persiste :

* Silo'd discipline structures
* Lack of trust
* Management by fear
* The myth of up-front planning

* Des structures en silo
* Le manque de confiance
* L’encadrement par la peur
* Le mythe d’une planification (détaillée) dès le début

These don't go away overnight with the wave of a wand.  They melt away slowly through the slow application of agility:

Ces raisons ne s’en vont pas du jour au lendemain d’un coup de baguette magique.  Elles s’effacent lentement au fur et à mesure de la lente application de l’agilité : 

* Breaking large cycles of integration, test and validation (e.g. 6 months) into shorter ones.
* Iterating against end user goals, not architectural goals, as much as possible.
* Breaking large detailed designs into outcome based goals with shorter-term details.
* Replace documented hand-offs with face-to-face conversations.

* En passant de longs cycles d’intégration, de test et de validation (par exemple 6 mois) à de plus petits
* En itérant en vue de réaliser des objectifs métiers, et non des objectifs architecturaux, autant que possible 
* En passant d’énormes conception détaillées à des résultats basés sur des objectifs détaillés à court terme
* En remplaçant des documents écrits par des conversations en face à face

There is a slow transformation away from managing for components to managing for player outcomes that doesn't occur overnight, but this transformation can begin immediately and the benefits can be seen every iteration.

### RELECTURE

Une transformation graduelle de passer de gérer des composants à gérer des résultats ne se produit pas en une nuit,
mais cette transformation peut commencer immédiatement et les bénéfices peuvent être constatées à chaque itération.

---
Auteur : [Clinton Keith](http://clintonkeith.com/)  
Source : [Scrumming without Agility](http://blog.agilegamedevelopment.com/2017/05/scrumming-without-agility.html)  
Date de parution originale : 29 Mai 2017  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 23/05/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



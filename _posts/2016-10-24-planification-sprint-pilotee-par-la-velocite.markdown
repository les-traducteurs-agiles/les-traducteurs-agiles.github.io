---
layout: post
title:  "Planification de sprint pilotée par la vélocité"
date:   2016-10-25 00:00:01
published: true
categories: 
- scrum
- noir
---

There are two general approaches to planning sprints: velocity-driven planning and commitment-driven planning. Over the next three posts, I will describe each approach, and make my case for the one I prefer.

Il existe généralement deux approches pour planifier les sprints : la planification pilotée par la vélocité et la planification pilotée par l’engagement. Au cours des trois prochains articles, je décrirai chacune de ces approches, et j’expliquerai pourquoi je préfère l’une par rapport à l’autre.

Let’s begin with velocity-driven sprint planning because it’s the easiest to describe. Velocity-driven sprint planning is based on the premise that the amount of work a team will do in the coming sprint is roughly equal to what they’ve done in prior sprints. This is a very valid premise.

<div align="right" style="float:right; padding-right:30px" >
  <img title="Vélocité" src="{{ site.url }}assets/mountain_goat/velocity.jpg" />
</div>

La planification de sprint pilotée par la vélocité étant la plus facile à décrire, nous commencerons par celle-là. La planification de sprint pilotée par la vélocité est basée sur l’hypothèse que la quantité de travail qu’une équipe accomplira au prochain sprint sera à peu près équivalente à ce qu’elle a faite aux sprints précédents. Cette hypothèse est tout à fait valable.

This does assume, of course, things such as a constant team size, the team is working on similar work from sprint to sprint, consistent sprint lengths, and so on. Each of these assumptions is generally valid and violations of the assumptions are easily identified—that is, when a sprint changes from 10 to nine working days as in the case of a holiday, the team knows this in advance.

Cela suppose, bien sûr, que des choses telles que : l’équipe est à effectif constant, l’équipe travaille sur des choses similaires de sprint en sprint, la longueur des sprints est identique, et ainsi de suite. Chacune de ces suppositions est valable généralement et les violations de ces suppositions sont facilement identifiables, c’est-à-dire  que lorsque l’équipe change le nombre de jours ouvrés de 10 à 9 en cas de jours fériés, l’équipe le sait à l’avance.

The steps in velocity-driven sprint planning are as follows:

Les étapes de la planification de sprint pilotée par la vélocité sont les suivantes

1. Determine the team’s historical average velocity.
2. Select a number of product backlog items equal to that velocity.

1. Déterminer la vélocité moyenne de l’équipe dans le temps.
2. Sélectionner un nombre d’items du _product backlog_ équivalent à cette vélocité.

Some teams stop there. Others include the additional step of:

Certaines équipes s’arrêtent ici. D’autres équipes ajoutent cette étape supplémentaire :

3. Identify the tasks involved in the selected user stories and see if it feels like the right amount of work.

3. Identifier les tâches correspondantes aux _user stories_ sélectionnées et voir si cela correspond à la bonne quantité de travail.

And some teams will go even further and:

Et certaines équipes iront encore plus loin et iront :

4. Estimate the tasks and see if the sum of the work is in line with past sprints.

4. Estimer les tâches et voir si la quantité de travail est dans la droite ligne des sprints précédents.

Let’s look in more detail at each of these steps.

Regardons en détails chacune de ces étapes

### Step 1. Select the Team’s Average Velocity

### Étape 1. Déterminer la vélocité moyenne de l’équipe

The first step in velocity-driven sprint planning is determining the team’s average velocity. Some agile teams prefer to look only at their most recent velocity. Their logic is that the most recent sprint is the single best indicator of how much will be accomplished in the next sprint. While this is certainly valid, I prefer to look back over a longer period if the team has the data.

La première étape dans la planification de sprint pilotée par la vélocité est de déterminer la vélocité moyenne de l’équipe. Certaines équipes regardent uniquement la dernière vélocité. Leur logique étant que le dernier sprint est le meilleur indicateur de la quantité qui sera réalisée au prochain sprint. Bien que cela soit tout à fait correct, je préfère regarder en arrière sur une plus longue période à condition que l’équipe en ait gardé la trace.

I prefer to take the average of the eight most recent sprints. I’ve found that to be fairly predictive of the future. I certainly wouldn’t take the average over the last 10 years. How fast a team was going during the Bush Administration is irrelevant to that team’s velocity today. But, similarly, if you have the data, I don’t think you should look back only one sprint.

Je préfère habituellement calculer la moyenne sur les huit derniers sprints. Je trouve que cela permet d’avoir une assez bonne prédiction du futur. Il est certain que je ne prendrai pas la moyenne sur les 10 dernières années. À quelle vitesse  a pu aller une équipe pendant l’Administration Bush n’est pas du tout pertinent et n’a aucun rapport avec la vélocité de l’équipe aujourd’hui. Mais, de manière similaire, si vous avez gardé la trace de ce qui s’est passé, je ne pense pas que vous devriez regarder seulement un sprint en arrière.

### Step 2: Select Product Backlog Items

### Étape 2 : Sélectionner les items du _product backlog_

Armed with an average velocity, team members select the top items from the product backlog. They grab items up to or equal to the average velocity.

Muni de la vélocité moyenne, les membres de l’équipe sélectionnent les items présents en tête du _product backlog_. Ils prennent les items jusqu’à concurrence de la vélocité moyenne.

At this point, velocity-driven planning in the strictest sense is finished. Rather than taking an hour or two per week of the sprint, sprint planning is done in a matter of seconds. As quickly as the team can add up to their average velocity, they’re done.

À ce point, la planification pilotée par la vélocité est terminée au sens strict. Plutôt que prendre une heure ou deux par semaine de sprint, la planification du sprint se fait en quelques secondes. C’est aussi rapide, que de faire l’addition jusqu’à obtenir la vélocité moyenne et après c’est fini.

### Step 3: Identify Tasks (Optional)

### Étape 3 : Identifier les tâches (optionnel)

Most teams who favor velocity-driven sprint planning realize that planning a sprint in a few seconds is probably insufficient. And so many will add in this third step of identifying the tasks to be performed.

La plupart des équipes qui préfèrent la planification de sprint pilotée par la vélocité réalisent que planifier un sprint en quelques secondes est probablement insuffisant. Et beaucoup d’entre elles y ajouteront cette troisième étape pour identifier les tâches à réaliser.

To do this, team members discuss each of the product backlog items that have been selected for the sprint and attempt to identify the key steps necessary in delivering each product backlog item. Teams can’t possibly think of everything so they instead make a good faith effort to think of all they can.

Pour faire ça, les membres de l’équipe discutent de chaque item du _product backlog_ sélectionné pour le sprint et tentent d’identifier les étapes clés nécessaires pour livrer chacun d’eux. Les équipes ne peuvent pas raisonnablement penser à tout donc à la place elles s’emploient en toute bonne foi à penser à toutes les possibilités . 

After having identified most of the tasks that will ultimately be necessary, team members look at the selected product backlog item and the tasks for each, and decide if the sprint seems full. They may conclude that the sprint is overfilled or insufficiently filled and add or drop product backlog items. At this point, some teams are done and they conclude sprint planning with a set of selected product backlog items and a list of the tasks to deliver them. Some teams proceed though to a final step:

Après avoir identifié la plupart des tâches qui devraient être nécessaires, les membres de l’équipe regardent les items du _product backlog_ sélectionnés et les tâches correspondantes, et décident si le sprint semble complètement remplit. Ils peuvent conclure que le sprint est trop remplit ou insuffisamment remplit et ajouter ou abandonner des items du _product backlog_. À partir de ce point, certaines équipes auront fini et concluent la planification du sprint avec un ensemble d’items du _product backlog_ sélectionnés et une liste de tâches pour les livrer. Néanmoins certaines équipes passent par une dernière étape :

### Step 4: Estimate the Tasks (Optional)

### Étape 4 : Estimer les tâches (optionnel)

With a nice list of tasks in front of them, some teams decide to go ahead and estimate those tasks in hours, as an aid in helping them decide if they’ve selected the right amount of work.

Avec une belle liste de tâches devant elles, certaines équipes décident de continuer et d’estimer ces tâches en heures, en guise de guide pour les aider à savoir si elles ont sélectionné la bonne quantité de travail à faire.

In next week’s post, I’ll [describe an alternative approach, commitment-driven sprint planning](). And after that, I’ll share some recommendations.

Dans mon prochain article, je [décrirai une approche alternative, la planification de sprint piloté par l’engagement]()[^1]. Et après cela, je partagerai avec vous quelques recommandations

[^1]: traduction à venir - Ndt
---  
Auteur : [Mike Cohn](https://www.mountaingoatsoftware.com/company/about-mike-cohn)  
Source : [Velocity-Driven Sprint Planning](https://www.mountaingoatsoftware.com/blog/velocity-driven-sprint-planning)  
Date de parution originale : 21 Octobre 2014  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 07/09/2016

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

  
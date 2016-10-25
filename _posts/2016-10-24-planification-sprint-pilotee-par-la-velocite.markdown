---
layout: post
title:  "Planification de sprint pilotée par la vélocité"
date:   2016-10-25 00:00:01
published: true
categories: 
- scrum
- planification
---

Il existe généralement deux approches pour planifier les sprints : la planification pilotée par la vélocité et la planification pilotée par l’engagement. Au cours des trois prochains articles, je décrirai chacune de ces approches, et j’expliquerai laquelle je préfère et pourquoi.

<div align="right" style="float:right; padding-left:30px" >
  <img title="Vélocité" src="{{ site.url }}assets/mountain_goat/velocity.jpg" />
</div>

La planification de sprint pilotée par la vélocité étant la plus facile à décrire, nous commencerons par celle-là. La planification de sprint pilotée par la vélocité est basée sur l’hypothèse que la quantité de travail qu’une équipe accomplira au prochain sprint sera à peu près équivalente à ce qu’elle a faite aux sprints précédents. Cette hypothèse est tout à fait valable.

Bien sûr cela suppose des choses telles que : l’équipe est à effectif constant, l’équipe travaille sur des choses similaires de sprint en sprint, la longueur des sprints est identique, et ainsi de suite. Généralement, chacune de ces suppositions est correcte et leurs violations sont facilement identifiables, c’est-à-dire que lorsque l’équipe change le nombre de jours ouvrés de 10 à 9 en raison de jours fériés, l’équipe le sait à l’avance.

Les étapes de la planification de sprint pilotée par la vélocité sont les suivantes :

1 - Déterminer la vélocité moyenne de l’équipe dans le temps.
2 -  Sélectionner un nombre d’items du _product backlog_ équivalent à cette vélocité.

Certaines équipes s’arrêtent ici. D’autres équipes ajoutent cette étape supplémentaire :

3 - Identifier les tâches correspondantes aux _user stories_ sélectionnées et voir si cela correspond à la bonne quantité de travail.

Et certaines équipes iront encore plus loin pour :

4 - Estimer les tâches et voir si la quantité de travail est dans la droite ligne des sprints précédents.

Regardons en détails chacune de ces étapes

### Étape 1. Déterminer la vélocité moyenne de l’équipe

La première étape dans la planification de sprint pilotée par la vélocité est de déterminer la vélocité moyenne de l’équipe. Certaines équipes regardent uniquement la dernière vélocité. Leur logique étant que le dernier sprint est le meilleur indicateur de la quantité qui sera réalisée au prochain sprint. Bien que cela soit tout à fait correct, je préfère regarder en arrière sur une plus longue période à condition que l’équipe en ait gardé la trace.

Je préfère habituellement calculer la moyenne sur les huit derniers sprints. Je trouve que cela permet d’avoir une assez bonne prédiction du futur. Il est certain que je ne prendrai pas la moyenne sur les 10 dernières années. Savoir à quelle vitesse a pu aller une équipe pendant l’Administration Bush n’est pas du tout pertinent et n’a aucun rapport avec la vélocité de l’équipe aujourd’hui. Mais, de manière similaire, si vous avez gardé la trace de ce qui s’est passé, je ne pense pas que vous devriez regarder uniquement un sprint en arrière.

### Étape 2 : Sélectionner les items du _product backlog_

Munis de la vélocité moyenne, les membres de l’équipe sélectionnent les items présents en tête du _product backlog_. Ils prennent un nombre d’items équivalents ou jusqu’à concurrence de la valeur de la vélocité moyenne.

À ce point, la planification pilotée par la vélocité est terminée au sens strict. Plutôt que prendre une heure ou deux par semaine de sprint, la planification du sprint se fait en quelques secondes. C’est aussi rapide, que de faire l’addition jusqu’à obtenir la vélocité moyenne et après c’est fini.

### Étape 3 : Identifier les tâches (optionnel)

La plupart des équipes qui préfèrent la planification de sprint pilotée par la vélocité ont bien conscience que planifier un sprint en quelques secondes est probablement insuffisant. Et beaucoup d’entre elles y ajouteront alors cette troisième étape pour identifier les tâches à réaliser.

Pour faire ça, les membres de l’équipe discutent de chaque item du _product backlog_ sélectionné pour le sprint et tentent d’identifier les étapes clés nécessaires pour livrer chacun d’eux. Les équipes ne peuvent pas raisonnablement penser à tout donc à la place elles s’emploient en toute bonne foi à y réfléchir autant qu’elles peuvent. 

Après avoir identifié la plupart des tâches qui devraient être nécessaires, les membres de l’équipe regardent les items du _product backlog_ sélectionnés et les tâches correspondantes, et décident si le sprint semble complètement remplit. Ils peuvent conclure que le sprint est trop remplit ou insuffisamment remplit et ajouter ou abandonner des items du _product backlog_. À partir de là, certaines équipes auront fini et concluent la planification du sprint avec un ensemble d’items du _product backlog_ sélectionnés et une liste de tâches pour les livrer. Néanmoins certaines équipes passent par une dernière étape :

### Étape 4 : Estimer les tâches (optionnel)

Avec une belle liste de tâches devant elles, certaines équipes décident de continuer et d’estimer ces tâches en heures, en guise de guide pour les aider à savoir si elles ont sélectionné la bonne quantité de travail à faire.

Dans mon prochain article, je [décrirai une approche alternative, la planification de sprint piloté par l’engagement]() [^1]. Et après cela, je partagerai avec vous quelques recommandations  

[^1]: traduction à venir - Ndt  

---  
Auteur : [Mike Cohn](https://www.mountaingoatsoftware.com/company/about-mike-cohn)  
Source : [Velocity-Driven Sprint Planning](https://www.mountaingoatsoftware.com/blog/velocity-driven-sprint-planning)  
Date de parution originale : 21 Octobre 2014  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 25/10/2016

---

Copyright ©1998-2016 Mountain Goat Software. All Rights Reserved.

---

{% include share_buttons.html %}

  
---
layout: post
title:  "Anomalies, corrections et demandes de supports - c’est bien trop petit pour une user story"
date:   2016-03-14 10:26:55
published: true
tags:
- user stories
---

_Bien qu’elles doivent être gérées tout aussi efficacement durant le sprint, certaines choses s’avèrent trop petites pour faire l’objet d’une **user story**. Je propose donc d’utiliser une taxonomie simple permettant de les classifier et de les gérer._

Grâce à un vocabulaire adapté pour ces petites choses, Scrum devient plus facile au quotidien, car cela permet à l’équipe ayant adopté ce type de conventions de travail de savoir comment gérer chacune d’entre elles

## Anomalies

Il existe un seul type d’anomalies : l’anomalie. Il n’existe pas d’anomalies de priorité haute, toutes ont une priorité haute, et plus haute que les _user stories_. Sur le tableau, les anomalies ont un couloir au-dessus de ceux réservés pour les _user stories_.

Ceci dit, il est de la plus haute importance d’avoir une définition très stricte de ce qu’est une anomalie. Il s’agit d’une anomalie si et seulement si l’un des critères ci-après s’applique :

* Une information est corrompue ou détruite en raison d’erreurs de raisonnement dans le logiciel
* L’usabilité est si mauvaise qu’elle force l’utilisateur à saisir de mauvaises informations, provoquant ainsi la corruption d’informations
* Il s’agit d’une faille de sécurité menaçant de corrompre l’information

Le dénominateur commun est corruption de l’information. Et après tout, c’est bien ce que nous faisons : de la technologie de l’information.

Une fois que vous avez identifié une anomalie, mettez-la donc en haut de votre planning. La rapidité avec laquelle vous réagissez face à un tel type de changement de priorité sera entièrement de votre ressort mais si votre processus fonctionne, le surlendemain elle n’y sera plus.

La première chose à faire par rapport à des anomalies est d’écrire un test qui les met sous la lumière des projecteurs. Je ne dis pas cela parce que je fais du TDD [^1], mais parce que vous voudrez bien avoir un test qui d’une manière ou d’une autre qui vous permettra d’être en confiance pour dire que l’anomalie est résolue. Une chose pire qu’une anomalie, est une anomalie qui revient !

Si l’anomalie vous empêche de livrer de nouvelles fonctionnalités, alors arrêtez tout d’abord de produire des anomalies. Un sprint bourré de correctifs ne livre aucune valeur métier à moins que vous ne considériez que récupérer un colis piégé soit d’une quelconque valeur.

Si vous aimez vraiment beaucoup les anomalies, faites-en la collection-dans un suivi d’anomalie. Mais dans tous les cas, dénombrez-les afin de savoir s’il y a quelque chose à faire pour régler ça.

## Corrections

Les corrections concernent des choses infimes comme des fautes de grammaire ou d’orthographe dans une interface utilisateur. Aucune information n’est corrompue dans ce cas mais cela ne vous montre pas non plus sous votre meilleur jour. Ennuyant est le mot qui vient à l’esprit. Toutefois, vous ne pouvez pas raisonnablement rédiger une _story_ pour régler ce genre de choses. “En tant que professeur de mathématiques, je veux que la question posée dans la boîte de dialogue soit écrite correctement afin de ne pas avoir une crise cardiaque”.

Les corrections possèdent aussi leur propre rubrique sur le tableau. Je vous suggère de prendre quelques corrections à faire lorsque vous aurez terminé une _story_ et avant d’enchaîner sur la suivante. Elles sont souvent peu consommatrices de ressources et vous donnent un sentiment rapide de satisfaction.

Vous devriez compter aussi le nombre de corrections. Si vous en avez beaucoup, pensez à prendre en considération l’optimisation de votre processus. Est-ce qu’il y a du laxisme quelque part ou un manque de communication entre les personnes ? Est-ce qu’il y a une source commune à certaines de ces erreurs ?

## Support

Les problèmes de support arrivent lorsque le système fonctionne comme prévu mais qu’un besoin pour quelque chose existe tout de même. Par exemple des tableaux de bords disponibles uniquement en écrivant du SQL à la main ou expliquer à une équipe externe un point d’intégration.

Le support peut être délicat à prioriser. Généralement le besoin métier est assez imminent et sa valeur métier évidente, ce qui requière donc une grande attention. Sans  oublier qu’il y a des _user stories_ à gérer et bien évidemment, le PO à mettre dans la boucle.

Si vous avez trop de problèmes de support, vous devez les analyser et trouver comment en réduire le nombre. À nouveau, dénombrez et visualisez.

## En résumé

Ce genre de petites choses peuvent être assez frustrantes et prennent quelques fois beaucoup de temps pour s’en occuper. En les classant, en les visualisant et en gardant à jour des statistiques, cela devient plus facile de vivre avec.

[^1]: TDD - Test Driven Development ou Développement piloté par les tests, est une technique de développement - pour plus d’informations reportez-vous à cette [article d’introduction](https://fr.wikipedia.org/wiki/Test_driven_development) sur Wikipedia.

---  
Auteur : [Per Lundholm](https://www.crisp.se/konsulter/per-lundholm)  
Source : [Too small for a user story – bugs, fixes and support](http://blog.crisp.se/2015/03/24/perlundholm/too-small-for-a-user-story-bugs-fixes-and-support)  
Date de parution originale : 24 Mars 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 14/03/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

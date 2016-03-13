---
layout: post
title:  "Anomalies, corrections et demandes de supports - pour une user story, c’est beaucoup trop petit"
date:   2016-03-14 10:26:55
published: true
categories: 
- user-stories
---

_Some things are too small for the overhead of a user story, still they must be handled during the sprint effectively. I suggest a small taxonomy to classify them and also what to do with them._

_Bien qu’elles doivent être gérées tout aussi efficacement durant le sprint, certaines choses s’avèrent trop petites faire l’objet d’une **user story**. Je suggère donc d’utiliser une taxonomie succinte pour les classifier et les gérer._ 

With a vocabulary for small things daily Scrum becomes a lot easier as the team have working agreements on how to deal with each one of them.

Avec un vocabulaire adapté pour ces petites choses, Scrum devient plus facile au quotidien, l’équipe ayant adopté des conventions de travail lui permettant de savoir comment gérer chacune d’entre elles.

## Bugs

## Anomalies

Bugs are of one kind only: bug. There is no high priority bugs, all have the highest priority, higher than user stories. Bugs have a swim lane on the board above the ones meant for user stories.

Les anomalies sont d’un seul type : anomalie. Il n’existe pas d’anomalies de priorité haute, toutes ont une priorité haute, et plus haute que les _user stories_. Sur le tableau, les anomalies ont un couloir au-dessus de ceux réservés pour les _user stories_.

With that said, it is of paramount importance to have a very strict definition of what is a bug. It is only a bug if any of these applies:

Ceci dit, il est de la plus haute importance d’avoir une définition très stricte de ce qu’est une anomalie. Il s’agit d’une anomalie si et seulement si l’un des critères ci-après s’applique

* Information is corrupted or destroyed by logic errors in the software.
* Usability is so bad that it tricks the user into entering wrong information, thus making information corrupt.
* It is a security breach which threatens to corrupt information

* Une information est corrompue ou détruite en raison d’erreurs de raisonnement dans le logiciel
* L’usabilité est si mauvaise qu’elle force l’utilisateur à saisir de mauvaises informations, provoquant ainsi de la corruption d’informations
* Il s’agit d’une faille de sécurité menaçant de corrompre l’information

The common denominator is the corruption of information. After all, that’s is what we do, information technology.

Le dénominateur commun est une corruption de linformation. Après tout, c’est bien ce que nous faisons : de la technologie de l’information.

Once you have identified a bug, put it on the top of your planning board. How fast you react on such a change in the priority is up to you but if your process is working, the next day would be the latest.

Une fois que vous avez identifié une anomalie, mettez-la en haut de votre planning. La rapidité avec laquelle vous réagissez face à un tel type de changement de priorité est entièrement de votre ressort mais si votre processus fonctionne, le surlendemain elle n’y sera plus.

The first thing about bugs is to write a test that exposes them. I’m not saying that because I do TDD, you would like to have a test anyway so that you feel confident that the bug is fixed. The only thing worse than a bug, is a bug that comes back!

La première chose à faire par rapport à des anomalies est d’écrire un test qui les met sous la lumière des projecteurs. Je ne dis pas cela parce que je fais du TDD [^1], mais parce que vous voudrez bien avoir un test qui d’une manière ou d’une autre pour vous permettre d’être en confiance pour dire que l’anomalie est résolue. Une chose pire qu’une anomalie, est une anomalie qui revient !

If bugs stops you from delivering new features, first stop producing bugs. A sprint filled with bug fixes delivers zero business value, unless you consider getting a kidnapped person back as a kind of value delivery.

Si l’anomalie vous empêche de livrer de nouvelles fonctionnalités, alors arrêtez tout d’abord de produire des anomalies. Un sprint bourré de correctifs ne livre aucune valeur métier à moins que vous ne considériez que récupérer un colis piégé soit d’une quelconque valeur.

If you love bugs a lot, collect them in a bug tracker. But in either case, do count them to see if there something you need to follow up.

Si vous aimez vraiment beaucoup les anomalies, faites-en la collection-dans un suivi d’anomalie. Mais dans tous les cas, dénombrez-les afin de savoir s’il y a quelque chose à faire pour régler ça.

## Fixes

## Corrections

Fixes are small things like bad grammar or spelling in a user interface. No information is corrupted but it certainly does not make you look good. Annoying, is a word that comes to mind. Meanwhile, you can’t reasonably write a story that takes care of it. “As a teacher of mathematics, I want the question dialog be spelled correctly so that I don’t get a heart condition”.

Les corrections sont des choses infimes comme des fautes de grammaire ou d’orthographe dans une interface utilisateur. Aucune information n’est corrompue dans ce cas mais cela ne vous montre pas non plus sous votre meilleur jour. Ennuyant est le mot qui vient à l’esprit. Toutefois, vous ne pouvez pas raisonnablement rédiger une _story_ pour régler ce genre de choses. “En tant que professeur de mathématiques, je veux que la question posée dans la boîte de dialogue soit écrite correctement afin de ne pas avoir une crise cardiaque”.

Fixes go to the board as well, to their own spot. I suggest you grab fixes when you’re done with a story, before moving on to the next. They are often cheap and gives you a quick fix of satisfaction.

Les corrections possèdent aussi leur propre rubrique sur le tableau. Je vous suggère de prendre quelques corrections à faire lorsque vous avez terminé une _story_ et avant d’enchaîner sur la suivante. Elles sont souvent peu consommatrices de ressources et elles vous donnent un sentiment rapide de satisfaction.

You should count fixes too. If you have a lot of them, consider tuning your process. Is there a sloppy attitude somewhere or is there a lack of communication between people? Is there a common root cause to many of our fixes?

Vous devriez compter aussi le nombre de corrections. Si vous en avez beaucoup, pensez à prendre en considération l’optimisation de votre processus. Est-ce qu’il y a du laxisme quelque part ou un manque de communication entre les personnes ? Est-ce qu’il y a une source commune à certaines de ces erreurs ?

## Support

## Support

Support issues are when the system works as designed but there is still a need for something. E.g. database reports available only by writing custom SQL or explaining an integration point to an external party.

Les problèmes de support arrivent lorsque le système fonctionne comme prévu mais qu’un besoin pour quelque chose existe tout de même. Par exemple des tableaux de bords disponibles uniquement en écrivant du SQL à la main ou expliquer à une équipe externe un point d’intégration.

Support takes a delicate touch when prioritizing.  Usually the user need is imminent and the value obvious, thus requiring high attention. Still, there are user stories to handle. Of course, PO must be in the loop.

Le support peut être délicat à prioriser. Généralement le besoin métier est assez imminent et sa valeur métier évidente, ce qui requière donc une grande attention. Sans  oublier qu’il y a des _user stories_ à gérer. Et bien évidemment, le PO doit être mis dans la boucle.

If you have too many support issues, you need to analyze them and find ways to bring the number down.  Again, count and visualize.

Si vous avez trop de problèmes de support, vous devez les analyser et trouver comment en réduire le nombre. À nouveau, dénombrez et visualisez.

## Summary

## En résumé

Little things like these can be frustrating and sometimes take a long time to deal with. By classifying them, visualize and keeping statistics, it gets a bit easier to live with them.

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

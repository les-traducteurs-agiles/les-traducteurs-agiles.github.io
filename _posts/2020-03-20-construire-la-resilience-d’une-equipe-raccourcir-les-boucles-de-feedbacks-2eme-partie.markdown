---
layout: post
title:  "Construire la résilience d’une équipe : Raccourcir les boucles de feedbacks (2ème partie)"
date:   2020-03-31 00:00
published: true
tags:
- agile
- équipe
- feedback
- temps de traversée
- temps de cycle
---

Cette série aborde le sujet d'aider une équipe à créer un environnement moins fragile - plus résilient. La [1ère partie](http://www.les-traducteurs-agiles.org/2020/03/18/construire-la-resilience-d-une-equipe-travailler-ensemble-1ere-partie.html) évoquait le travail individuel. Cette partie traite du raccourcissement des boucles de retours d'informations (_feedback_)

Voici une brève description d'un problème évoqué récemment par un client : une Personne A avait inséré du code qui avait cassé une autre partie du système sans aucun rapport avec ce dernier. Je vais nommer cela « Plantage du moteur de recherche après insertion de code dans la partie courriel » (Oui, j'ai changé les noms de la fonctionnalité par d'autres parce que les noms n'ont que peu d'importance dans le fond.)

Les managers ne comprenaient pas. Ni l'équipe. Toutefois, ils avaient maintenant un problème de production à corriger.

Un seul retour d'informations était à leur disposition : le code inséré avait cassé une autre code « sans rapport » avec celui-ci. Il était temps de jeter un coup d'œil à leur boucle de feedback.

## Visualisez vos boucles de feedback

Chaque projet (ou chaque effort) que vous faites possède au moins une boucle de feedback. C'est celle que vous avez lorsque vous livrez quelque chose aux clients.

<div align="left" style="float:left; padding-right:30px" >
  <a href="{{ site.url }}assets/johanna/Lifecycle.serial.reality-fr.png"><img title="Différentes réalités d'un cycle de vie en série" src="{{ site.url }}assets/johanna/Lifecycle.serial.reality-fr.png" width="298px" height="207px"/></a></div>

Si vous utilisez une approche en cascade, vous avez probablement des boucles de feedbacks non désirées, comme dans cette image, « Plusieurs réalités possibles d'un cycle de vie en série ».

Plus vous livrez souvent en interne, plus vous aurez de feedbacks

Plus vous livrez souvent aux clients, plus vous obtenez des retours d'informations _validés_. Les problèmes de productions sont des retours d'informations validés.  Vous pourriez ne pas aimer ce type de retours d'informations, mais il s'agit tout de même de retours d'informations clients.

Dans ce cas précis, l'équipe projet n'avait pas de tests automatisés. L'équipe appelait les personnes du métier « product owners ». (Elles ne l'étaient pas, mais c'est là un problème différent). Ces personnes du métier exécutaient des tests manuels. Pire encore, ils ne testaient que les cas nominaux.

Les personnes du métier ne savaient pas comment tester les cas non nominaux susceptibles de donner des erreurs. Ils ne connaissaient pas assez les entrailles du produit pour chercher les interactions indésirables.

Et c'était pareil pour les développeurs. Les développeurs n'avaient pas de mécanismes de feebacks inclus dans leur code.

## Les tests automatisés, c'est du feedback

Il y a un quadrillion d'années, lorsque je codais pour gagner ma vie, j'écrivais mes tests après avoir codé. Je dois bien l'admettre.

J'étais même très bonne pour écrire des tests qui pouvaient ignorer mes erreurs. Oui, je testais tout à l'exception des endroits où j'avais fait des erreurs. Je devins très bonne à lire les _dumps_[^1] en hexadécimal ou en octal (selon le type de machine et le langage utilisé). (Il fût un temps où je pouvais lire les traces d'appels de la pile d'exécution en Fortran et de savoir exactement où je m'étais planté. Oh, ces bons vieux mauvais jours).

De nos jours, nous savons d'autres outils. Nous pouvons utiliser TDD, BDD, ATDD et obtenir des retours d'informations _avant_ d'écrire du code. Vous pouvez consultez les définitions à partir des liens ci-dessous :

* [Test-Driven Development](https://www.agilealliance.org/glossary/tdd/)
* [Behavior Driven Development](https://www.agilealliance.org/glossary/bdd)
* [Acceptance-Test Driven Development](https://www.agilealliance.org/glossary/atdd/)

Il se trouve que David Bernstein a écrit un livre que j'apprécie beaucoup, Beyond Legacy Code (disponible sur [Amazon](https://amzn.to/32URR5S) et [PragProg](https://pragprog.com/book/dblegacy/beyond-legacy-code)) qui décrit un ensemble de pratiques techniques facilement intégrables à votre processus de travail. (Vous pourriez également lire la version mise à jour de _Pragmatic Programmer_ ou tout autre livre sur le développement piloté par les tests disponible. Oh et puis flûte, lisez-les tous, apprenez et mettez en pratique.)

J'ai appris le développement piloté par les tests dans toutes ces formes après avoir arrêté d'écrire du code dans le cadre de ma vie professionnelle. Toutefois, j'utilise les idées des spécifications par l'exemple lorsque j'écris, même si j'écris en langage naturel (en Anglais).

Vous avez sans doute remarqué que je raconte souvent des histoires dans mes articles et dans mes livres. Il s'agit d'exemples. Je les utilise dans l'objectif de vous aider à prendre en compte le contexte et quand ce contexte s'applique ou ne s'applique pas à votre cas. De manière toute aussi importante, l'exemple permet d'ancrer dans le réel mes écrits et m'offre du feedback lorsque j'écris.

Je ne suis pas parfaite. Je suis sûr que lorsque je prends des chemins de traverse dans certains de mes articles de blogs cela vous laisse parfois un peu pantois. Même ainsi, les exemples m'aident à donner du feedback lorsque j'écris. Avec un peu de chance, cela vous permet de rester avec moi, même si j'avais pu prendre un chemin de traverse.

Cette équipe a décidé de visualiser ses boucles de feedback.

## Quelle est la durée de vos boucles de feedback ?

Vous pourriez imaginer que vos boucles de feedback sont plutôt courtes. Cela pourrait être le cas. Avez-vous mesuré votre chaîne de valeur pour voir vraiment quel est votre temps de cycle ? Vous pouvez en savoir plus sur la cartographie de la chaîne de valeur dans mon article [Measure Cycle Time, Not Velocity (VO)](https://www.jrothman.com/mpd/project-management/2019/09/measure-cycle-time-not-velocity/).

<div align="left" style="float:left; padding-right:30px" >
  <a href="{{ site.url }}assets/johanna/NonResilientTeamBeforeProblem-fr.png"><img title="Équipe non résiliente avant le problème" src="{{ site.url }}assets/johanna/NonResilientTeamBeforeProblem-fr.png" width="298px" height="167px"/></a></div>

Voici à quoi pouvait ressembler la cartographie de la chaîne de valeur de cette équipe pour une seule fonctionnalité. Elle n'avait pas encore découvert le problème dans cette chaîne de valeur.

Vous pouvez remarquer que le temps de réalisation de la fonctionnalité représente 1/4 du temps total où l'équipe a attendu.

Mais, trois jours après qu'elle ait inséré son code en « production », elle a découvert le problème « Plantage du moteur de recherche après insertion de code dans la partie courriel ».

<div align="left" style="float:left; padding-right:30px" >
  <a href="{{ site.url }}assets/johanna/NonResilientTeamAfterProblem-fr.png"><img title="Équipe non résiliente avant le problème" src="{{ site.url }}assets/johanna/NonResilientTeamAfterProblem-fr.png" width="300px" height="171px"/></a></div>

Lorsqu'elle a réalisé le problème avec cette insertion de code, elle a commencé à écrire des tests et faire des revues de code.

L'équipe pris 3,5 jours supplémentaires - en plus des 4+ jours précédents - pour terminer son travail.

Et tout le reste du travail à faire a été retardé par ces 3,5 jours.

Elle était vraiment bien en retard désormais. Tout ça, parce qu'elle n'avait pas des boucles de feedbacks suffisamment courtes.

## Des retours d'informations plus fréquents aident à construire la résilience

Plus vous obtenez des feedbacks fréquemment, plus vos actions deviennent résilientes. L'équipe a écrit les tests lorsqu'elle était sous pression, avec un problème de production à régler. Elle n'avait pas fait de revue de code avant de l'avoir sur les bras.

Les tests - et tout spécialement les petits tests faits de manière systématique - peuvent créer de la résilience dans une équipe. Même si vous ne travaillez pas [ensemble en tant qu'équipe (cf. 1ère partie)](http://www.les-traducteurs-agiles.org/2020/03/18/construire-la-resilience-d-une-equipe-travailler-ensemble-1ere-partie.html), les tests peuvent vous aider à construire la résilience.

Les tests offrent un support pour ce changement.

Voici comment j'en conçois le déroulement :

* Faites une petite quantité de travail
* Faites systématiquement des tests automatisés afin que vous sachiez comment vous pourrez modifier le code lorsque vous en aurez besoin. (Oui, il y a besoin de tests manuels, ces derniers prennent généralement bien plus de temps à être exécuter. Je parle ici de tests automatisés.)
* Mesurez le nombre de boucles de feedbacks que vous avez et leurs durées (prenez bien en considération le fait de mesurer votre temps de cycle)

Comment cette équipe s'en est-elle sortie ?

1. Tout d'abord, elle a utilisé des _user stories_ pour définir son travail
2. Elle a défini des critères d'acceptation pour faire de l'ATDD
3. Elle a utilisé (avec quelques réticences) une combinaison de TDD et de BDD. Tous les membres de l'équipe n'étaient pas d'accord sur ce qu'il fallait faire. Toutefois, ils ont commencé à écrire des tests en premier. Cela les a aidé avec la conception, pas avec le code.
4. Elle a mesuré son temps de cycle. Après un peu pratique, elle a géré son temps de cycle pour le faire passer en-dessous d'une journée.

Plus vous en faites en sorte de réduire vos boucles de feedback, plus vous renforcer la résilience de votre équipe.

La série :

* [Construire la résilience d'une équipe : travailler ensemble (1ère partie)](http://www.les-traducteurs-agiles.org/2020/03/19/construire-la-resilience-d-une-equipe-travailler-ensemble-1ere-partie.html)
* * [Construire la résilience d'une équipe : Raccourcir les boucles de feedbacks (2ème partie - traduction à venir)](http://www.les-traducteurs-agiles.org/2020/03/20/construire-la-resilience-d-une-equipe-raccourcir-les-boucles-de-feedbacks-2eme-partie.html)
* [Construire la résilience d'une équipe : Travailler « n'importe où » et « n'importe quand » (3ème partie - traduction à venir)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-work-anywhere-and-anytime-part-3/)
* [Construire la résilience d'une équipe en résumé (4ème partie - traduction à venir)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-summary-part-4/)

[^1]: NdT : Copie du contenu de tout ou partie d'une base de données ou de la mémoire d'une machine sous la forme d'un fichier à des fins d'analyse.  

---
Auteur : [Johanna Rothman](https://www.createadaptablelife.com/about)  
Source : [Build Team Resilience: Shorten Feedback Loops (Part 2)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-shorten-feedback-loops-part-2/)  
Date de parution originale : 05 Mars 2020  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 31/03/2020  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

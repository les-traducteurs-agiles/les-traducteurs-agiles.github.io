---
layout: post
title:  "LeSS - Coordination & Intégration"
date:   2017-01-09 00:01
published: true
tags:
- less
---

[<< Portail LeSS < Portail Framework](http://www.les-traducteurs-agiles.org/2016/12/28/less-portail-framework.html)

Scrum valorise une coordination et une intégration décentralisées plus qu'une coordination centralisée et contrôlée qu'on trouve dans la gestion de projet traditionnelle. La coordination et l'intégration LeSS se concentrent sur la façon de soutenir une coordination décentralisée tout en fournissant juste ce qu'il faut de de limites et de structure pour éviter le chaos.

## Juste parler

C'est probablement le meilleur moyen de coordonner les équipes entre elles. Chaque membre d'une équipe auto-gérée devrait être capable d'aller voir une autre équipe pour discuter d'un problème. Lorsqu'il y a un besoin de coordination, vous pouvez "juste en parler" avec l'autre équipe, décrocher le téléphone ou, dans le pire des cas, leur envoyer un mail. Vous n'avez pas besoin de passer par un mécanisme de coordination formel, officiel et généralement lent. Levez-vous et aller parler aux gens.

## Communiquer dans le Code

Les groupes LeSS adoptent [l'intégration continue (en)](http://less.works/less/technical-excellence/continuous-integration), ce qui signifie que tout le monde voit son code intégré dans le dépôt du référentiel central (les branches constituent une complication inutile qui devrait être évitée). Tous les membres des équipes produit se synchronisent plusieurs fois par jour avec le référentiel afin de bénéficier des modifications réalisées par les uns et les autres.

Donc, lorsque vous faites une mise à jour, passez deux minutes à parcourir les changements réalisés par les autres et regardez si cela concerne ce sur quoi vous êtes actuellement en train de travailler. Si c'est le cas, sentez-vous libre de vous lever et de "juste parler" pour synchroniser votre travail avec les autres !

## Envoyez des observateurs à la Mêlée quotidienne

Une méthode simple de coordination pour les équipes consiste à envoyer un représentant, pas le ScrumMaster, en tant qu'observateur silencieux à la Mêlée quotidienne des autres équipes qui travaillent sur des choses en rapport. Les observateurs reportent ensuite à leurs équipes afin qu'elles prennent des actions supplémentaires.

## Communautés de composant et mentors

Les personnes qui travaillent sur les mêmes composants au même moment doivent se connaître pour pouvoir poser des questions et faire la revue de code des uns et des autres. Faites-le en créant des [Communautés de Pratiques](http://www.les-traducteurs-agiles.org/2017/01/02/less-communautes.html) (CoPs) sur les composants, qu doivent communiquer via des listes de diffusion, le chat, des réunions occasionnelles et autres canaux collaboratifs à distance.

Ces communautés sont souvent organisées par un "mentor du composant" qui est généralement un membre de l'équipe feature ayant pris certaines responsabilités supplémentaires comme (1) être le formateur sur la façon dont le composant fonctionne, (2) suivre l'état de santé du composant sur le long-terme, (3) organiser une communauté de composant, (4) organiser des ateliers de conception et (5) les revues de code.

Un mentor de composant ne fait pas la revue de code pour donner son accord tant qu'on n'a pas fait un commit sur le code. Il est le formateur et l'organisateur / l'intendant au service du composant, il n'est donc PAS un portail ou une barrière.

Il peut y avoir plusieurs mentors pour un même composant, ceux-ci partagent leur travail et réduisent donc la dépendance à une seule personne.

Important ! ... Au-delà de soutenir la coordination, ces pratiques aident à maintenir et améliorer la qualité de la conception et du code d'un composant, et accroît l'apprentissage.

## Scrum de Scrums

Une mêlée de mêlées est une mêlée menée entre les équipes, typiquement deux ou trois fois par semaine.

Habituellement, le format ressemble à celui de la mêlée quotidienne :

* Qu'est-ce que mon équipe a réalisé d'intéressant pour les autres équipes ?
* Qu'est-ce que mon équipe va faire d'intéressant ?
* Quels sont les obstacles auxquels mon équipe fait face et que les autres équipes devraient connaître ou même aider à résoudre ?


Evidemment, vous êtes libre de faire évoluer ces questions.

Mise en garde : la demande de tenir une mêlée de mêlées peut être le signe de dépendances inutiles ou de problèmes de coordination causés par des groupes d'experts ou des équipes composants, ou par des équipes n'étant pas en mesure ou cherchant à identifier et partager leur travail.

La mêlée de mêlées ne fait pas partie de LeSS, et nous ne recommandons pas d'utiliser cette technique de coordination centralisée trop formelle. Cela dit, si cela fonctionne pour vous, n'arrêtez pas... et ne vous sentez pas obligé d'arrêter parce que vous adoptez LeSS.

## Réunions multi-équipes

Il est courant que des équipes ressentent le besoin de travailler en relation étroite alors que ce n'est pas le cas pour d'autres équipes. Pour celles qui travaillent en relation étroite, il est fréquent d'avoir plusieurs réunions LeSS inter-équipes. Quelques exemples :

* [Affinage du Backlog Produit](http://www.les-traducteurs-agiles.org/2018/01/26/less-l-affinage-du-backlog-produit.html) inter-équipes
* [Planification du sprint (partie 2)](http://www.les-traducteurs-agiles.org/2017/03/10/less-la-planification-du-sprint-2eme-partie.html) inter-équipes
* [Ateliers de conception (en)](http://less.works/less/technical-excellence/architecture-design.html) inter-équipes
* L'échange de membres lors des mêlées quotidiennes.


## Des voyageurs pour exploiter et casser les goulets d'étranglement et créer des compétences

Parfois, un groupe produit se repose sur quelques experts techniques expérimentés. Comment la connaissance de ces (rares) experts peut-elle être rendue disponible à toutes les équipes ? Ils peuvent devenir des voyageurs. À chaque sprint, ils rejoignent une équipe différente, et coachent en binômant, en animant des ateliers et des formations.

Bien que les voyageurs n'aient pas été créés spécifiquement pour créer de la coordination, ils créent ou renforcent un réseau élargi en rejoignant les différentes équipes, ce qui est exactement ce qu'il faut pour créer des canaux de coordination informelle. De plus, ils favorisent la cohérence des connaissances et des pratiques à travers les équipes, réalisant ainsi un objectif de coordination.

## Équipe organisatrice

Dans certains domaines, les features sont monstrueusement grandes. Lorsque vous découpez ces géants en plus petits éléments du Backlog Produit, cela peut nécessiter d'avoir plusieurs équipes travaillant étroitement ensemble, chacune séparément sur leurs éléments du Backlog Produit, pour créer une unique feature monstre.

Une autre technique, pour coordonner les équipes qui travaillent ensemble sur les éléments découpés qui se rapportent à une même grande feature, consiste à créer une équipe organisatrice. Une équipe organisatrice est une équipe feature ordinaire qui prend le lead sur la globalité d'une feature géante. En plus du travail de développement, cette équipe garde la trace de ce que les autres équipes font et les aide à se synchroniser. En résumé, elle organise la coordination transversale aux équipes qui travaillent sur la feature géante, en plus de son propre travail de développement.

Parfois, plusieurs équipes commencent à développer une feature géante au même moment. D'autres fois, l'équipe organisatrice commence toute seule pour préparer au plus tôt le transfert de connaissance et simplifier et rendre cohérente la conception. Après quelques sprints, d'autres équipes rejoignent l'équipe organisatrice. Dans ce cas, l'équipe organisatrice a la responsabilité de former les équipes qui les rejoignent pour les aider à apprendre ce qu'elle sait déjà.


---
Auteur : The LeSS Company B.V.  
Source : [Coordination & Integration - Large Scale Scrum (LeSS)](http://less.works/less/framework/coordination-and-integration.html)  

---
Traducteur : [Fabrice Aimetti](http://www.fabrice-aimetti.fr/)  
Date de traduction : 09/01/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

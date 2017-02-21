---
layout: post
title:  "Le modèle INVEST - I comme des _stories_ Indépendantes"
date:   2017-02-21 00:00:01
published: true
tags: 
- user stories
---

Le modèle [INVEST](http://www.les-traducteurs-agiles.org/story/2015/02/23/investissez-dans-de-bonnes-stories-et-dans-des-taches-smart.html) est un moyen mnémotechnique permettant de se rappeler des principales caractéristiques des _user stories_ et il commence par un **I** comme **Indépendant**.

Chacune des stories indépendante décrit un aspect différent des capacités d’un système. Elles sont plus facile à manier parce que chacune d’elle peut être (pour la plupart d’entre elles) comprise, suivie, implémentée, testée, etc.

Les approches de développement agile sont flexibles, elles sont plus aptes à poursuivre ce qui _a_ le plus de valeur aujourd’hui, et elles ne sont pas contraintes de suivre une conjecture vieille de 6 mois sur ce qui _devrait avoir_ de la valeur aujourd’hui. Des _stories_ indépendantes nous aident à faire en sorte à ce que cela soit vrai : plutôt qu’un gros bloc “à prendre ou à laisser”, elles nous permettent de nous focaliser sur les différents aspects d’un système.  

Nous aimerions que la description d’un système soit aussi cohérente et complète que possible. Des _stories_ indépendantes nous aide aussi là-dessus : en évitant de se chevaucher, les risques de contradiction entre _stories_ sont réduits, et la vérification pour voir si nous avons décrit tout ce dont nous avons besoin en est facilité.

> Trois types de dépendances existent : le chevauchement, l’ordonnancement et le confinement

Qu’est-ce qui fait que des _stories_ soient dépendantes plutôt qu’indépendantes ? Trois types de dépendances existent : le _chevauchement_ (indésirable), _l’ordonnancement_ (qui peut être contourné la plupart du temps), et le _confinement_ (quelques fois utile)

## Dépendance de chevauchement

Parmi toutes les formes de dépendances, le chevauchement en est la plus délicate. Imaginez cet ensemble de fonctions sous-jacentes :
* {A, B, C, D, E, F}

et dont les divers sous-ensembles sont couverts par les _stories_ suivantes :
* {A, B}
* {A, B, F}
* {B, C, D}
* {B, C, F}
* {B, E}
* {E, F}

Quel est le plus petit ensemble de _stories_ satisfaisant à la présence des fonctions {A, B, C, D, E, F} ? Et {A, B, C, E} ? Pouvons-nous les avoir et rien d’autre ?

Lorsque les _stories_ se chevauchent, il est assez difficile de savoir si tout le spectre d’un élément donné a bien été couvert au moins une fois et en même temps, une certaine confusion risque de se produire si nous voyons les choses apparaitre plus d’une fois.

> Des _stories_ qui se chevauchent génèrent de la confusion

Par exemple, considérons un système de messagerie électronique et les _stories_ suivantes : “L’utilisateur envoie et reçoit des messages” et “L’utilisateur envoie et répond à des messages” (La seule vue du mot “et” dans le titre d’une story devrait vous mettre la puce à l’oreille, mais il faudrait que vous ayez pu voir l’ensemble des _stories_ pour déterminer s’il y a vraiment un chevauchement entre elles). Pour réduire ce chevauchement, nous pouvons envisager les _stories_ différemment :

* L'utilisateur envoit un [nouveau] message
* L'utilisateur reçoit un message
* L'utilisateur répond à un message

(Notez bien que nous ne sommes pas concernés par des chevauchements “techniques” à ce niveau : il est plus que probable qu’envoyer et recevoir des messages peuvent avoir en commun un certain nombre de tâches techniques. La manière dont nous concevons le système ou que nous planifiions notre travail n’est pas notre préoccupation majeure lorsque nous essayons de comprendre le comportement du système.)

## Dépendance d’ordonnancement

Une seconde dépendance assez répandue est la dépendance d’ordonnancement : “cette story doit être implémentée avant celle-ci”.

> Des dépendances ordonnées compliquent les plans, mais il est possible généralement de les contourner.

Bien qu’aucune approche ne puisse le garantir, la dépendance d’ordonnancement est quelque chose généralement d’inoffensif la plupart du temps et qui peut être contourné. Il y a plusieurs raisons à cela :

1. Certaines dépendances d’ordonnancement découlent de la nature même du problème . Par exemple, une _story_ “l’utilisateur ré-expédie un message” suit naturellement “l’utilisateur envoie un message”. Même s’il y a une dépendance d’ordonnancement que nous ne pouvons pas supprimer, ce n’est pas grave car le métier aura tendance à planifier ces _stories_ de telle manière que cette dépendance sera naturelle et inoffensive.
2. Même si une dépendance d’ordonnancement existe, il y a seulement 50% de chance que la planification soit faite dans le “mauvais” ordre.
3. Nous pouvons trouver des manières plus intelligentes pour supprimer la plupart des dépendances d’ordonnancement.

Par exemple, un utilisateur pourrait avoir besoin d’un compte avant de pouvoir envoyer un message électronique. Cela pourrait nous amener à penser que nous devrions implémenter les _stories_ de gestion de compte d’abord (par exemple des stories comme “l’administrateur créé un compte”). À la place, nous pourrions intégrer (“coder en dur”) quelques comptes pour commencer. (Vous pouvez envisager cela comme du codage en dur ou bien y penser comme “la version la plus réduite qu’il soit de la gestion des comptes” ; d’une manière ou d’une autre, c’est beaucoup moins de boulot.)

Pourquoi choisir cette approche ? Parce que nous voulons explorer d’abord certaines zones et que nous prenons en compte à la fois la valeur et le risque. Du point de vue de la valeur, nous pouvons nous focaliser sur les parties que les clients valorisent le plus (pour qu’ils trouvent cela intéressant dès la première livraison). Du point de vue des risques, nous pouvons trouver intéressant de gérer les risques, de les envisager comme ayant une valeur négative. Dans notre exemple, nous pouvons considérer qu’une utilisabilité médiocre est un risque. Quelques comptes codés en dur pourraient s’avérer suffisants pour nous permettre d’explorer des problèmes potentiels d’utilisabilité.  

## Dépendances de confinement

Les dépendances de confinement arrivent lorsque nous organisons les _stories_ de manière hiérarchique : “cette _story_ contient ces autres _stories_”. Différents termes peuvent être utilisés par les équipes pour exprimer cette idée : vous pourriez entendre parler de “thèmes, d’épopées [^1] et de _stories_”, “fonctionnalités et _stories_”, “_stories_ et sous-_stories_”, etc. Une hiérarchie est un outil permettant d’organiser ; elle peut être formelle ou informelle.

> Une bonne organisation pour décrire un système est rarement la meilleure pour planifier son implémentation.

la plus grosse réserve au sujet d’une décomposition hiérarchique est bien qu’il puisse s’agir d’une stratégie utile pour organiser et comprendre un large ensemble de _stories_, cela n’en fait pas une bonne stratégie pour planifier. En effet, cela vous encourage à faire une planification de type “en profondeur d’abord” : gérer ce domaine d’abord, et lorsque cela est fini, de faire le domaine suivant. Mais il est peu probable en réalité que les _stories_ ayant le plus de valeur soient toutes dans le même domaine. Nous avons tout intérêt plutôt de créer d’abord une version minimale de l’ensemble du système, puis une version plus affinée ensuite (avec la fonctionnalité la plus importante qui suit), et ainsi de suite.

## Dernière ligne droite

Des _stories_ indépendantes nous aident à la fois du point de vue métier et du point de vue technique d’un projet. D’un point de vue métier, le projet se concentre sur les objectifs métiers à l’aide d’un modèle simple. D’un point de vue technique, des _stories_ techniques incitent à la réalisation d’une implémentation minimale, et renforcent les approches de conceptions minimisant et gérant l’implémentation des dépendances. 

[^1]: ou d’epics - pour ceux qui préfèrent le terme en vo - NdT

---
Auteur : [Bill Wake](http://xp123.com/about/)  
Source : [Independent Stories in the INVEST Model](http://xp123.com/articles/independent-stories-in-the-invest-model/)  
Date de parution originale : 8 Février 2012  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 21/02/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



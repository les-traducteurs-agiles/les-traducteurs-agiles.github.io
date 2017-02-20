---
layout: post
title:  "Le modèle INVEST - Les stories indépendantes"
date:   2017-02-20 00:00:01
published: true
tags: 
- user stories
---

The INVEST model is a reminder of the important characteristics of user stories, and it starts with I for Independent.

Le modèle [INVEST](http://www.les-traducteurs-agiles.org/story/2015/02/23/investissez-dans-de-bonnes-stories-et-dans-des-taches-smart.html) est un moyen mnémotechnique qui aide à se souvenir des principales caractéristiques des _user stories_. 
Il commence par un **I** comme **Indépendant**.

Independent stories each describe different aspects of a system's capabilities. They are easier to work with because each one can be (mostly) understood, tracked, implemented, tested, etc. on its own. 

Chacune des stories qui est indépendante décrit un aspect différent des capacités d’un système. Elles sont plus facile à manier parce que chacune peut être (pour la plupart) à part entière comprise, suivie, implémentée, testée, etc.

Agile software approaches are flexible, better able to pursue whatever _is_ most valuable today, not constrained to follow a 6-month old guess about what _would be_ most valuable today. Independent stories help make that true: rather than a "take it or leave it" lump, they let us focus on particular aspects of a system.

Les approches de développement agile sont flexibles, plus aptes à poursuivre ce qui _a_ le plus de valeur aujourd’hui, et non contraintes à suivre une conjecture vieille de 6 mois sur ce qui _devrait avoir_ de la valeur aujourd’hui. Des _stories_ indépendantes nous aident à faire en sorte à ce que cela soit vrai : plutôt qu’un gros bloc “à prendre ou à laisser”, elles nous permettent de nous focaliser sur les différents aspects particuliers d’un système.  

We would like a system's description to be consistent and complete. Independent stories help with that too: by avoiding overlap, they reduce places where descriptions contradict each other, and they make it easier to consider whether we've described everything we need.

Nous aimerions que la description d’un système soit cohérente et complète. Des _stories_ indépendantes nous aide aussi là-dessus : en évitant de se chevaucher, elles réduisent les occasions où les _stories_ peuvent se contredire les unes les autres, et elles facilitent la vérification pour voir si nous avons décrit tout ce dont nous avons besoin.

> Three common types of dependency: overlap, order, and containment

> Il y a trois types de dépendances : le chevauchement, l’ordre et le confinement

What makes stories dependent rather than independent? There are three common types of dependency: _overlap_ (undesirable), _order_ (mostly can be worked around), and _containment_ (sometimes helpful). 

Qu’est fait que des _stories_ soient dépendantes plutôt qu’indépendantes ? Il y a trois types de dépendances : le _chevauchement_ (indésirable), _l’ordonnancement_ (qui la plupart du temps peut être contourné), et le _confinement_ (quelques fois utiles)

## Overlap Dependency

## Dépendance de chevauchement

Overlap is the most painful form of dependency. Imagine a set of underlying capabilities:
* {A, B, C, D, E, F}

with stories that cover various subsets:
* {A, B}
* {A, B, F}
* {B, C, D}
* {B, C, F}
* {B, E}
* {E, F}

Le chevauchement est la forme la plus délicate de dépendances. Imaginez cet ensemble de capacités
* {A, B, C, D, E, F}

avec des _stories_ couvrant les divers sous-ensembles :
* {A, B}
* {A, B, F}
* {B, C, D}
* {B, C, F}
* {B, E}
* {E, F}

Quick: what's the smallest set of stories that ensure that capabilities {A, B, C, D, E, F} are present? What about {A, B, C, E}? Can we get those and nothing else?

Quel est le plus petit ensemble de _stories_ qui satisfont la présence des capacités {A, B, C, D, E, F} ? Et {A, B, C, E} ? Pouvons-nous avoir celles-ci et rien d’autres ?

When stories overlap, it's hard to ensure that everything is covered at least once, and we risk confusion when things are covered more than once. 

Lorsque les _stories_ se chevauchent, il est difficile de s’assurer que tout soit bien couvert au moins une fois et nous risquons d’avoir de la  confusion 

> Overlapping stories create confusion.

> Des _stories_ qui se chevauche génère de la confusion

For example, consider an email system with the stories "User sends and receives messages" and "User sends and replies to messages." (Just seeing the word "and" in a story title can make you suspicious, but you really have to consider multiple stories to know if there's overlap.) Both stories mention sending a message. We can partition the stories differently to reduce overlap:

Par exemple, considérons un système de messagerie électronique avec des _stories_ “L’utilisateur envoie et reçoit des messages” et “L’utilisateur envoie et répond à des messages” (La seule vue du mot “et” dans le titre d’une story devrait vous rendre suspicieux, mais il faudrait que vous ayezvous devriez vraiment jetez un œil à plusieurs _stories_ pour savoir  

* User sends [new] message
* User receives message
* User replies to message

* L'utilisateur envoit un [nouveau] message
* L'utilisateur reçoit un message
* L'utilisateur répond à un message

(Note that we're not concerned about "technical" overlap at this level: sending and replying to messages would presumably share a lot of technical tasks. How we design the system or schedule the work is not our primary concern when we're trying to understand the system's behavior.)

(Notez bien que nous ne sommes pas concernés pas des chevauchements “techniques” à ce niveau : il est plus que probable qu’envoyer et recevoir des messages pourraient avoir en commun un certain nombre de tâches techniques. La manière dont nous concevons le système ou que nous planifiions notre travail n’est pas notre préoccupation majeure lorsque nous essayons de comprendre le comportement du système.)

## Order Dependency

## Dépendance d’ordonnancement

A second common dependency is order dependency: "this story must be implemented before that one."

Une seconde dépendance assez répandue est la dépendance d’ordonnancement : “cette story doit être implémentée avant celle-ci”.

> Order dependencies complicate a plan, but we can usually eliminate them.

> Des dépendances ordonnées compliquent les plans, mais généralement il nous est possible de les éliminer.

While there's no approach that guarantees it, order dependency tends to be something that is mostly harmless and can be worked around. There are several reasons for that:

Bien qu’aucune approche ne puisse le garantir, la dépendance d’ordonnancement tend à être quelque chose d’inoffensif la plupart du temps et qui peut être contourné. Il y a plusieurs raisons à cela :

1. Some order dependencies flow from the nature of the problem. For example, a story "User re-sends a message" naturally follows "User sends message." Even if there is an order dependency we can't eliminate, it doesn't matter since the business will tend to schedule these stories in a way that reflects it. 
2. Even when a dependency exists, there's only a 50/50 chance we'll want to schedule things in the "wrong" order.
3. We can find clever ways to remove most of the order dependencies.

1. Certaines dépendances d’ordonnancement découlent de la nature du problème . Par exemple, une _story_ “l’utilisateur ré-expédie un message” suit naturellement “l’utilisateur envoie un message”. Même s’il y a une dépendance d’ordonnancement que nous ne pouvons pas supprimer, ce n’est pas grave car le métier aura tendance à planifier ces _stories_ de telle manière que cela le reflètera.
2. Même si une dépendance d’ordonnancement existe, il y a seulement 50% de chance que nous voudrons planifier les choses dans le “mauvais” ordre.
3. Nous pouvons trouver des manières plus intelligentes pour supprimer la plupart des dépendances d’ordonnancement.

For example, a user might need an account before they can send email. That might make us think we need to implement the account management stories first (stories like "Admin creates account"). Instead, we could build in ("hard-code") the initial accounts. (You might look at this as "hard-coding" or you might think of it as "the skinniest possible version of account management"; either way, it's a lot less work.)

Par exemple, un utilisateur pourrait avoir besoin d’un compte avant de pouvoir envoyer un message électronique. Cela pourrait nous amener à penser que nous devrions implémenter les _stories_ de gestion de compte d’abord (par exemple des stories comme “l’administrateur créé un compte”). À la place, nous pourrions intégrer (“coder en dur”) quelques comptes initiaux. (Vous pourriez considérer cela comme du codage en dur ou bien y penser comme “la version la plus réduite qu’il soit de la gestion des comptes” ; d’une manière ou d’une autre, c’est beaucoup moins de boulot.)

Why take that approach? Because we want to explore certain areas first. We consider both value and risk. On the value side, we may focus on the parts paying customers will value most (to attract them with an early delivery). On the risk side, we may find it important to address risks, thinking of them as negative value.  In our example, we may be concerned about poor usability as a risk. A few hard-coded accounts would be enough to let us explore the usability concerns. 

Pourquoi prendre cette approche ? Parce que nous voulons explorer d’abord certaines zones. Nous voulons considérer à la fois la valeur et le risque. Du côté valeur, nous pouvons focaliser sur les parties que les clients valorisent le plus (pour qu’ils trouvent cela intéressant dès la première livraison). Du côté risque, nous pouvons trouver intéressant de gérer les risques, de les envisager comme ayant une valeur négative. Dans notre exemple, nous pouvons considérer une facilité d’utilisation médiocre comme un risque. Quelques comptes codés en dur pourraient s’avérer suffisant pour nous permettre d’explorer ces problèmes potentiels de facilité d’utilisations.  

## Containment Dependency

## Dépendances de confinement

Containment dependency comes in when we organize stories hierarchically: "this story contains these others." Teams use different terms for this idea: you might hear talk of "themes, epics, and stories," "features and stories," "stories and sub-stories," etc. A hierarchy is an organizational tool; it can be used formally or informally. 

Les dépendances de confinement arrivent lorsque nous organisons les _stories_ hiérarchiquement : “cette _story_ contient ces autres _stories_”. Différents termes sont utilisés par les équipes pour exprimer cette idée : vous pourriez entendre parler de “thèmes, épopées et de _stories_”, “fonctionnalités et _stories_”, “_stories_ et sous-_stories_”, etc. Une hiérarchie est un outil permettant d’organiser ; il peut être formel ou informel.

> A good organization for describing a system is rarely the best organization for scheduling its implementation.

> Une bonne organisation pour décrire un système est rarement la meilleure pour planifier son implémentation.

The biggest caveat about a hierarchical decomposition is that while it's a helpful strategy for organizing and understanding a large set of stories, it doesn't make a good scheduling strategy. It can encourage you to do a "depth-first" schedule: address this area, and when it's done, go the next area. But really, it's unlikely that the most valuable stories will all be in a single area. Rather, we benefit from first creating a minimal version of the whole system, then a fancier version (with the next most important feature), and so on. 

la plus grosse réserve à propos de la décomposition hiérarchique est que bien que cela soit une stratégie utile pour organiser et comprendre un large ensemble de _stories_, cela n’en fait pas une bonne stratégie pour les planifier. Cela vous encourage à faire une planification de type “en profondeur d’abord” : gérer ce domaine d’abord, et lorsque cela est fini, de faire le domaine suivant. Mais il est peu probable en réalité que les _stories_ ayant le plus de valeur soient toutes dans le même domaine. Nous avons tout intérêt plutôt de créer d’abord une version minimale de l’ensemble du système, puis une version plus affinée ensuite (avec la fonctionnalité la plus importante qui suit), et ainsi de suite.

## Bottom Line

## Dernière ligne droite

Independent stories help both the business and technical sides of a project. From a business perspective, the project gets a simple model focused on the business goals, not over-constrained by technical dependencies. From a technical perspective, independent stories encourage a minimal implementation, and support design approaches that minimize and mange implementation dependencies. 

Les _stories_ importantes nous aident à la fois sur le côté métier et le côté technique d’un projet. D’une point de vue métier, le projet se concentre les objectifs métiers à l’aide d’un modèle simple. D’un point de vue technique, des _stories_ techniques encourage la réalisation d’une implémentation minimale, et renforce les approches de conceptions minimisant et gérant l’implémentation des dépendances. 

---
Auteur : [Bill Wake](http://xp123.com/about/)  
Source : [Independent Stories in the INVEST Model](http://xp123.com/articles/independent-stories-in-the-invest-model/)  
Date de parution originale : 8 Février 2012  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 19/12/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



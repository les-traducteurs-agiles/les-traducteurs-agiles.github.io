---
layout: post
title:  "Une user story est le titre d'un scénario alors qu'un cas d'utilisation est le contenu de plusieurs scénarios"
date:   2011-12-17 00:01
published: true
tags:
- user story
---

Information sur la dernière mise à jour : référence corrigée à l'article de Gerard Meszaros

* Pourquoi un corbeau est-il comme un secrétaire ?, demandait Lewis Caroll dans "De l'autre côté du miroir"


Parce que chacun commence par un 'e' (est la réponse consensuellement acceptée)

* Quelle est la différence entre une user story et un cas d'utilisation ?, demande presque tout le monde


-- un ange passe --(parce qu'il n'y a pas de réponse consensuellement acceptée)

Dans [Une user story est à un cas d'utilisation ce qu'une gazelle est à un gazoduc (discussion: Re: Une user story est à un cas d'utilisation ce qu'une gazelle est à un gazoduc](http://www.les-traducteurs-agiles.org/2011/12/15/une-user-story-est-a-un-cas-d-utilisation-ce-qu-une-gazelle-est-a-un-gazoduc.html), j’ai conclu par la réponse suivante :

> Après les trois premières lettres, ils n'ont rien en commun.

---

Jens Coldewey a écrit dans [son blog](http://coldewey.com/) qu'une user story est le titre d'un scénario. (Ce n'est pas parfaitement, ni obligatoirement, presque toujours cela, mais c'est vraiment très proche).

Cela amène à la réponse formelle suivante :

> Une user story est le titre d'un scénario, alors qu'un cas d'utilisation est le contenu de plusieurs scénarios.

Par conséquent, j'ai souvent été cité disant, "Une user story est une promesse pour une conversation", ... éludant ainsi la question " à propos de quoi ?" ... à laquelle il est répondu, "à propos du scénario dont c'est le titre !".

A propos, vous pourriez vouloir considérer, [Pourquoi je continue à utiliser les cas d'utilisation(discussion: Re: Pourquoi je continue à utiliser les cas d'utilisation](http://www.les-traducteurs-agiles.org/2011/12/11/pourquoi-je-continue-a-utiliser-les-cas-d-utilisations.html)

---

**Le Ver Plat Géant Qui A Mangé Calcutta** (3 février 2008)

(D'accord, cette ville ne s'appelle plus Calcutta, ils aiment l'écrire Kolkata, mais j'aime toujours Calcutta – elle a une histoire intéressante).

L'autre jour, Craig Larman m'a choqué en disant que les user stories étaient des fractales. Je savais déjà que les user stories étaient comme des vers plats ... coupez-les en deux et vous en aurez deux. Mais cela signifie seulement les rendre plus petits. Craig laissait entendre que vous pourriez les rendre plus gros (faites un zoom arrière sur une fractale et vous aurez encore une fractale ... faites un zoom arrière sur un ver plat (ou collez les ensemble) et vous aurez toujours deux vers plats).

Une remarque est que Craig aime écrire de vraiment grosses user stories, du genre prenant 3 ans et 2 000 personnes à implémenter.

Aussi, selon la distinction faite ci-dessus, il s'agirait juste d'écrire le nom d'un cas d'utilisation pour avoir ce même cas d'utilisation.

Toutefois, Craig va plus loin. Utilisant les Storyotypes de Gerard Meszaros comme base (non que Craig l'ait indiqué, c'est ma contextualisation de la recommandation de Craig), nous pouvons voir que Craig utilise d'énormes user stories pour même faire remonter les exigences non fonctionnelles sur une très grande échelle.
Je trouve cela intéressant et j'espère pouvoir faire des recherches sur le sujet. Attendez-vous à entendre parler davantage du Platus Helmins Gigantus avalant Tokyo ou attaquant NYC avec des exigences non fonctionnelles.

---

**15 décembre 2008** (essayant à nouveau à partir de la liste de diffusion Scrum, ce coup-ci)
\>\>\> D'un autre côté, si vous ignorez le concept de "complétude", l'approche du Cas d'Utilisation dégénère gentiment en Stories.
\>\> Non.
\> :-( as-tu le temps de dire autre chose que "Non." Ton livre était l'un des premiers que j'ai lu sur le sujet, je suis intéressé par ce que tu as à dire.

Trois caractéristiques distinguent un cas d'utilisation d'une user story ou d'une fonctionnalité.

1. Un cas d'utilisation a une intrigue. A l'inverse d'une "user story" (qui bizarrement, n'est pas une histoire du tout, parce qu'elle n'a pas d'intrigue), un cas d'utilisation raconte une histoire de quelqu'un utilisant le système pour réaliser un objectif quelconque. Cela signifie qu'il a plus d'une étape ...

2. Un cas d'utilisation décrit la boîte noire du comportement du système. C'est à dire, que les autres systèmes communiquent avec le système en cours de conception. Une user story ne le fait pas.

3. La différence la plus évidente est qu'un cas d'utilisation recueille des scénarios. Une user "story" (ahem à nouveau la partie 'histoire' d'une user story) indique seulement un scénario. Un cas d'utilisation ne peut se réduire à une user story parce qu'un cas d'utilisation a certainement ou presque deux portes de sortie, l'une où l'objectif de l'utilisateur est accompli et l'autre où l'objectif de l'utilisateur n'est pas accompli.

N'importe laquelle de ces trois caractéristiques fait qu'un cas d'utilisation ne se réduit pas à une user story.

Le cas d'utilisation a le mérite de montrer la taille et la forme du système lorsqu'il est assemblé, pour aider les rédacteurs à résoudre ce qui est peut être manquant ou pour être certain que des choses ne manquent pas, pour montrer le comportement général du système.

Les User (ahem) stories ou les fonctionnalités du produit sont des points utiles à développer dans les lots définis par les développeurs (comme Gerard l'avait fait remarqué).

Les grands bénéfices apportés par les cas d'utilisations sont pour le sponsor, l’utilisateur et le PO. Les développeurs ont montré une tendance ces dernières années à ne pas les aimer parce qu'ils ne montrent pas les travaux à mener par les développeurs.

Les user stories, les fonctionnalités et les éléments de backlog présentent la tendance inverse - ils montrent bien les travaux à mener, mais de manière flou le schéma général.

Il y a longtemps, j'en ai conclu que vous ne pourriez avoir les deux dans le même document (même si la story map de Jeff Patton en est proche), bien que je comprenne que les deux puissent être nécéssaires.

Personnellement, je travaille à partir des cas d'utilisations et fait le découpage dans ma tête ou avec des crayons. Gerard semble travailler à partir des user stories et les assemble ensemble en cas d'utilisation dans sa tête. La plupart des gens choisissent l’un des deux et ne se préoccupent pas d'apprendre l'autre.

Alistair


---
Auteur : [Alistair Cockburn](http://alistair.cockburn.us/Alistair)  
Source : [A user story is the title of one scenario whereas a use case is the contents of multiple scenarios](http://alistair.cockburn.us/A+user+story+is+the+title+of+one+scenario+whereas+a+use+case+is+the+contents+of+multiple+scenarios)  nbsp
Date de parution originale : 16 Janvier 2008  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 17/12/2011  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

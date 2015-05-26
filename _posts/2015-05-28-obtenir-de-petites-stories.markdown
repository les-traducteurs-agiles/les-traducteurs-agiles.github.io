---
layout: post
title:  "Obtenir de petites stories"
date:   2015-05-28 21:59:53
published: false
categories: 
- user stories
- pratique
---

In a thread about estimation in hours and whether it's a good idea (IMO it's not the best idea by far), this morning Robin Dymond tossed me this challenge:

Ce matin - dans un fil de discussion sur l’estimation en heures et notamment du fait, s’il s’agissait d’une bonne idée (à mon avis ce n’est pas une bonne idée) - Robin Dymond m’a lancé ce défi :


    You have advocated for years that teams should be able to slice stories to the point where they can complete a story in a day. My request is that you show the Agile community how to do that in writing and some exercises that use non trivial examples. I would appreciate learning more about how you do this.
    
    Pendant des années, vous avez promu que les équipes devaient être capable de découper les stories de telle façon qu'ils puissent réaliser une story en une journée. Ma demande est que vous montriez par écrit à la communauté agile comment le faire ainsi que quelques exercices de mise en pratique d'exemples non triviaux. J'apprécierai de pouvoir apprendre plus sur comment vous faites cela.

Here, off the cuff, is one reply:
Au pied levé, voici une réponse :

## Single Acceptance Test
## Un seul test d’acceptance

The most elegant way to do this that I know of is to consider acceptance tests for the feature. Then do them one at a time, simplest first. I first became aware of this idea from Neil Killick (one of the #NoEstimates guys), though I’d like to think I’d done it automatically a million times.

La manière la plus élégante de faire cela que je connaisse est d’étudier les tests d’acceptance de la fonctionnalité. Plus de les faire un par un, en commençant par le plus simple. La première fois que j’ai pris connaissance de cette idée est auprès de Neil Killick (un des gars de #NoEstimates), bien que j’aime à penser que j’ai déjà fait cela par le passé un million de fois de manière automatique.

But there is another fun way.
Mais il y a une autre manière plus amusante.

## One Dumb Idea
## Une idée bête

I’m often challenged to come up with something that could be done, even in a week, and that would look like the product. It’s rare that I can’t come up with something. But what happens next is what’s interesting. An example, from memory, cleaned up a bit to make the story clear at small expense to the facts:

Je suis souvent challenger pour trouver quelque chose qui pourrait être fait, même en une semaine, et qui ressemblerait au produit. Il est rare que je ne puisse pas trouver quelque chose. Mais ce qui arrive ensuite est intéressant. Un exemple de mémoire, très légèrement édulcoré pour rendre l’histoire plus claire :

Chet and I were visiting a cable TV company. Their challenge was about something they had already done, the old way: “What if our product was pay-per-view movies? The viewer has to be able to select any movie from a menu of them, watch the movie, pause it, wind it back, …” They went on and on. Then they said, “There’s no slice of that that could be done in a week.”

Chet et moi visitions une chaîne TV cablé. Leur défi était à propos de quelque chose qu’il avait déjà fait à l’ancienne : “Et si notre produit était des films à la demande ? Le téléspectateur devrait pouvoir sélectionner un film à partir d’un menu, de regarder le film, de le mettre en pause, de revenir en arrière, ...”. Et ils continuaient, et ils continuaient. Alors ils dirent, “Il n’y a rien de tout cela qui pourrait être fait en une semaine”.

We talked a bit. I asked, “At the beginning of this project, did you have the ability to play a movie over a channel?” They said that they did, because (of course) they had movie channels playing all the time.

Nous avons parlé un peu. J’ai demandé : “Au début de ce projet, aviez-vous la capacité de passer un film sur une chaîne ?”. Ils répondirent qu’ils pouvaient, parce que (bien sûr) ils avaient des chaînes en continue.

So I said, “What if the first slice is that you’re playing some movie on some secret channel, all the time, and if the viewer wants to watch it, he clicks that channel. That would nearly be done already.”

Alors j’ai répondu : “Et si le premier morceau était que vous puissiez passer un film sur une chaîne cachée en continue, et si le téléspectateur veut le regarder, il appuie sur cette chaîne. Ce serait déjà presque fait.”

Some of them hated that example. Some liked it. There were lots of objections to how one could imagine that as “done”. The objections were all about additional features of pay-per-view: “He doesn’t get to see the movie from the beginning.” “What if he wants a different movie?” “What if we don’t know his credit card?”

Certains d’entre eux détestèrent cet exemple. Certains aimèrent. Il y eu un tas d’objections sur comment quelqu’un pouvait imaginer cela comme quelque chose de “terminé”. Ces objections étaient toutes à propos de fonctionnalités supplémentaires pour le visionnage à la demande : “

Chet and I probably said a few times “Well, rewinding the movie is a new story,” or “Not switching to the secret channel without his credit card is a new story.” I remember that at one point we said "What if we started just using your boss's credit card for everyone?"

Il est probable que Chet et moi ayons dit un certain nombre de fois “Eh bien, remettre le film au début est une nouvelle story” ou “Ne pas changer vers la chaîne cachée sans carte de crédit est une nouvelle story”. Je me rappelle à un moment que nous avons dit “Et si nous démarrions en utilisant pour tous le monde la carte de crédit du patron seulement ?”.

Pretty soon — in minutes, not hours or days — some engineer in the room said “Well, that wouldn’t work, but what we could do is …” and described something they could have done.

Plus tard - quelques minutes après, pas des heures ni des jours - un ingénieur présent dans la pièce dit “Eh bien, ça ne marcherait pas, mais ce que nous pourrions faire serait ...” et de décrire quelque chose qu’ils pourraient faire.

That’s what always happens. Someone comes up with a stupid example of a story that could be done in a day or a week, whatever the then-current target is. That someone is usually me, because I am full of stupid ideas and I don’t mind putting them out there.

C’est ce qui arrive toujours. Quelqu’un vient avec un exemple stupide de story qui pourrait être faite en un jour ou en une semaine, quelque soit la cible alors désignée. Généralement, ce quelqu’un c’est moi, parce que j’ai la tête remplie d’idées stupides et que je n’ai aucun scrupule à les sortir. 

Suddenly things change. We’ve gone, in one step, from “impossible” to knowing a stupid, but possible, thing to do. The tone of the meeting changes, instantly, from “no way to do that” to improving the idea or bettering it.

Et tout à coup, les choses changent. En une seule étape, nous sommes partis de l’“impossible” pour aboutir à connaître une chose stupide à faire mais néanmoins possible. Le ton de la réunion changea immédiatement, de “aucune manière de faire cela” à perfectionner l’idée ou à l’améliorer.

Chet and I have done this, time and again, separately or together, in domains of all kinds. One dumb idea that could almost work is enough to switch the team from “can’t be done” to “yeah, but this would be a better way.”

Ensemble ou séparément, Chet et moi avons fait cela à maintes reprises dans toutes sortes de domaines. Une idée stupide qui pourrait presque marcher est suffisante pour basculer l’équipe de “cela ne peut pas marcher” à “ouais, cela pourrait être une meilleure façon de faire”.

## The Real World
## La vraie vie

Referring to Alistair Cockburn's "Elephant Carpaccio" exercise, Robin said:

Robin dit, en se référant à l’exercice du “carpaccio d’éléphant” d’Alistair Cockburn :

    I am familiar with Alistair's elephant carpaccio, however his exercise uses a calculator, and developers just don't think the example is applicable to their problems.

    Je suis familier du carpaccio d'éléphant d'Alistair, toutefois cet exercice utilise une calculatrice, et les développeurs pensent seulement que cet exemple n'est pas applicable à leurs problèmes. 

## They always think that
## Ils pensent toujours cela

A million examples, not in their domain, and they’ll still think that.

Un million d’exemples, pas dans leur domaine, et ils pensent toujours cela.

    Yes, but in the real world, we have to deliver every movie ever recorded, to anyone’s house, in real time, together with all the reviews from the major outlets, with or without surround sound, wide or narrow screen, 3D or flat, with subtitles in every known language including FORTRAN, color-enhanced to support red-green color blindness, using every major credit card plus any authorized Canadian grocery store coupons, with the naughty bits either covered or enhanced, with pause and zoom in available, in fast motion and slow motion as well as regular everyday motion, using no wires or cables of any kind, without emitting any electromagnetic radiation on any spectrum, delivering to any television, computer, tablet, phone, watch, or pinkie ring, at any location in the solar system, with zero delay. You can’t do that in the real world.
    
    Oui, mais dans le monde réel, nous devons livrer chacun des films enregistrés dans chacune des maisons en temps réel, avec toutes les critiques des magasins, avec ou sans le son surrond, écran large ou quatre-tiers, 3D ou non, avec les sous-titres dans toutes les langues connues y compris le FORTRAN, avec améliorations des couleurs pour le daltonisme, avec les cartes de crédits les plus répandues y compris les coupons de réductions des magasins canadiens accrédités, avec les parties indécentes floutées ou non, avec la possibilité de mettre en pause ou de zoomer, de mettre en accélérer ou au ralenti ainsi qu'à vitesse normale, sans fil ou avec des cables de toute sorte, sans aucune émission électromagnétique sur l'ensemble du spectre, en diffusant sur n'importe quelle télévision, ordinateur, tablette, téléphone, montre, ou chevalière à n'importe quel endroit du système solaire, immédiatement. Vous ne pouvez pas faire cela dans le monde réel.

Yeah, well, we just did. I doubt it took an hour.

Oui, eh bien, nous venons de le faire. Et je doute que cela nous ait pris une heure.

## Nonetheless
## Néanmoins

All you need is a stupid idea, or one acceptance test. I’d typically start trying to get one story that a PO could imagine was nearly “end to end”, that can be done in a week. A day probably isn’t something the team can do right out of the box.

Tout ce dont vous avez besoin est une idée stupide, ou un test d’acceptance. Généralement, je commence par essayer d’avoir une story qu’un PO pourrait presque imaginer “de bout en bout”, qui peut être faite en une semaine. Pour une équipe, un jour est insuffisant pour faire quelque chose fonctionnant immédiatement.

Or is it? In our CSD class, we do a real application and we run 90 minute Sprints. The teams deliver multiple stories in those Sprints. Not the first Sprint, mind you. :)

Ou pas ? Dans notre formation CSD (Certified Scrum Developper - Développeur scrum certifié - NdT), nous faisons une vraie application avec des sprints de 90 minutes. Les équipes livrent plusieurs stories dans ces sprints. Pas lors du premier sprint, je vous rassure. :)

## Yabbut ...
## OuaisMé...

Robin, of course, seemed to be asking for a more comprehensive compendium of ways to slice stories. I think he just wanted me to go away for a while. It might be fun to generate a whole list of examples. They would all have the same characteristics, though. It seems like you have to sit with the team and talk with them, or at least get them to talk among themselves.

Bien sûr, Robin semble plaider pour un compendium plus exhaustif des façons de découper les stories. Je pense qu’il voulait juste que je m’en aille un instant. Il pourrait être amusant de faire toute la liste possible d’exemples. Même s’ils auraient tous les mêmes caractéristiques. Il semble que vous deviez vous asseoir avec l’équipe et parler avec eux, ou du moins les faire suffisamment parler entre eux.

My way requires someone to have a dumb idea, which isn't that hard, but it also requires them to say it, which is harder. And -- I'm just guessing here -- they have to be respected enough, or enough of a stranger, to get the idea discussed instead of dismissed out of hand.

Ma manière exige que quelqu’un ait une idée idiote, ce qui n’est pas si difficile, mais qui exige aussi que quelqu’un le dise, ce qui est plus dur. Et -- je me demande juste -- ils doivent être suffisamment respectés, ou suffisamment respectueux d’un étranger, pour que l’idée soit discutée plutôt qu’écartée d’un revers de la main.

Neil's way, doing a single acceptance test, might be better. I'll know when I've tried it a few times. My way is more fun, though. I'm sure of that.

La manière de Neil, de faire un simple test d’acceptance, peut être meilleure. Je le sais pour l’avoir essayé quelques fois. Même si ma manière est plus amusante; Je suis sûr de cela.

---
Auteur : [Ron Jeffries](http://ronjeffries.com/about.html)  
Source : [Getting small stories](http://xprogramming.com/articles/getting-small-stories/)  
Date de parution originale : 7 octobre 2014  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 28/05/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



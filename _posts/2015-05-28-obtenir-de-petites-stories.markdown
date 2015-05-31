---
layout: post
title:  "Obtenir de petites stories"
date:   2015-05-28 21:59:53
published: true
categories: 
- user stories
- pratique
---

Ce matin - dans un fil de discussion où nous débattions de savoir si c’était une bonne idée de faire des estimations en heures (et à mon avis ce n’est pas une bonne idée) - Robin Dymond m’a lancé ce défi :

      Pendant des années, vous avez prôné que les équipes devraient être capables de 
    découper les stories de telle façon qu'elles puissent être développées en une 
    journée. 
    Je souhaiterais que vous le montriez par écrit à la communauté agile avec des 
    exercices et des exemples non triviaux. J'aimerai en apprendre plus sur la 
    manière dont vous vous y prenez.

Au pied levé, voici une réponse :

## Un seul test d’acceptance

La manière la plus élégante de faire que je connaisse est d’étudier les tests d’acceptance pour la fonctionnalité. Plus de les faire un par un, en commençant par le plus simple. La première fois que j’ai eu connaissance de cette idée est auprès de Neil Killick (un des gars de #NoEstimates), bien que j’aime à penser que j’ai déjà fait cela  un million de fois par le passé inconsciemment.

Mais il y a une autre manière plus amusante.

## Une idée bête

Je suis souvent mis au défi de trouver quelque chose qui pourrait être fait, même en une semaine, et qui ressemblerait au produit. Il est rare que je ne puisse pas trouver quelque chose. Mais ce qui arrive ensuite est intéressant. Voici de mémoire, un exemple très légèrement revu et modifié pour rendre l’histoire plus compréhensible :

Chet et moi visitions une chaîne TV du cable. Leur défi concernait quelque chose qu’ils avaient déjà fait “à l’ancienne” : “Et si notre produit était des films à la demande ? Le téléspectateur devrait pouvoir sélectionner un film à partir d’un menu, de regarder le film, de le mettre en pause, de revenir en arrière, ...”. Et ils continuaient, et ils continuaient. Puis ils dirent, “Rien de tout ça ne pourrait être fait en une semaine”.

Nous avons discuté un peu. J’ai demandé : “Au début de ce projet, aviez-vous la capacité de passer un film sur une chaîne ?”. Ils répondirent qu’ils pouvaient, parce que (bien sûr) ils avaient des chaînes diffusant en continu.

Alors j’ai répondu : “Et si la première tranche consistait à ce que vous puissiez passer un film sur une chaîne cachée en continu, et si le téléspectateur veut le regarder, il passe sur cette chaîne. Ce serait presque déjà fait.”

Certains ont détesté cet exemple. D’autres ont adoré. Il y eu un tas d’objections demandant comment quelqu’un pouvait imaginer ça comme étant quelque chose de “fini”. Ces objections portaient toutes sur des fonctionnalités supplémentaires pour le visionnage à la demande : “Il ne pourra pas voir le film depuis le début.”, “Et s’il veut voir un autre film ?”, “Et si nous ne connaissons pas sa carte de crédit ?”.

Il est probable que Chet et moi ayons dit un certain nombre de fois “Eh bien, remettre le film au début est une nouvelle story” ou “Ne pas pouvoir changer vers la chaîne cachée sans carte de crédit est une nouvelle story”. Je me rappelle à un moment que nous avons dit “Et si pour l’ensemble des téléspectateurs, nous commencions en utilisant seulement la carte de crédit du patron ?”.

Plus tard - quelques minutes après, pas des heures ni des jours - un ingénieur présent dans la pièce dit “Eh bien, ça ne marcherait pas, mais ce que nous pourrions faire serait ...” et de décrire quelque chose qu’ils pourraient faire.

C’est ce qui arrive tout le temps. Quelqu’un arrive avec un exemple stupide de story, quelque soit le sujet en question, qui pourrait être faite en un jour ou en une semaine. Généralement, ce quelqu’un c’est moi, parce que j’ai la tête remplie d’idées stupides et que je n’ai aucun scrupule à les sortir. 

Et tout à coup, les choses changent. En une seule étape, nous passons d’“impossible” à une chose stupide mais néanmoins faisable. Le ton de la réunion change immédiatement, nous passons de “impossible de faire cela” à perfectionner l’idée ou à l’améliorer.

Ensemble ou séparément, Chet et moi avons déjà fait ça à maintes reprises dans toutes sortes de domaines. Tout à coup, une idée stupide pouvant presque marcher devient suffisante pour faire basculer l’équipe de “ça ne peut pas marcher” à “ouais, mais ça serait mieux de faire comme ça ”.

## La vraie vie

En se référant à l’exercice du “carpaccio d’éléphant” d’Alistair Cockburn, Robin dit alors :

    Je connais bien le carpaccio d'éléphant d'Alistair, mais cet exercice utilise 
    une calculatrice, et généralement les développeurs ne pensent pas que cet 
    exemple soit applicable à leurs problèmes. 

## Ils pensent toujours ça

Un million d’exemples, pas dans leur domaine, et ils pensent toujours cela.

      Oui, mais dans le monde réel, nous devons livrer chacun des films existants 
    depuis les débuts de l'histoire du cinéma dans toutes les maisons en temps 
    réel, avec toutes les critiques de film des majors, avec ou sans le son 
    surround, écran large ou quatre-tiers, 3D ou non, avec les sous-titres dans 
    toutes les langues connues y compris le FORTRAN, avec amélioration des 
    couleurs pour le daltonisme, en prenant en charge les cartes de crédits les 
    plus répandues y compris les coupons de réductions des magasins canadiens
    accrédités, avec les parties indécentes floutées ou non, avec la possibilité
    de mettre en pause ou de zoomer, de mettre en accélérer ou au ralenti ainsi 
    qu'à vitesse normale, sans fil ou avec des cables de toute sorte, sans 
    aucune émission électromagnétique sur l'ensemble du spectre, en diffusant 
    sur n'importe quelle télévision, ordinateur, tablette, téléphone, montre, ou
    chevalière à n'importe quel endroit du système solaire, immédiatement. 
    Vous ne pouvez pas faire cela dans le monde réel.

Ouais, eh ben, nous venons bien de le faire. Et je doute que cela nous ait pris une heure.

## Néanmoins

Tout ce dont vous avez besoin est d’une idée stupide, ou d’un test d’acceptance. Généralement, je commence par essayer d’avoir une story qu’un PO pourrait presque imaginer “de bout en bout”, qui peut être développée en une semaine. Pour une équipe, un jour est insuffisant pour faire quelque chose fonctionnant immédiatement.

Ou pas ? Dans notre formation CSD (Certified Scrum Developper - Développeur scrum certifié - NdT), nous faisons une vraie application avec des sprints de 90 minutes. Les équipes livrent plusieurs stories dans ces sprints. Pas lors du premier sprint, je vous rassure. :)

## OuaisMé...

Bien sûr, Robin semble demander un recueil plus exhaustif des façons de découper les stories. Je pense qu’il voulait juste que je m’éloigne un instant du fil de discussion. Il pourrait être amusant de faire toute la liste possible des exemples. Même s’ils auront tous les mêmes caractéristiques. Il semble que vous deviez vous asseoir avec l’équipe et parler avec elle, ou du moins faire suffisamment parler les personnes de l’équipe entre elles.

Ma manière exige que quelqu’un ait une idée idiote, ce qui n’est pas si difficile, mais qui exige aussi que quelqu’un la dise, ce qui est plus dur. Et -- je m’interroge juste -- les personnes de l’équipe doivent être suffisamment respectées par un - ou suffisamment respectueuses d’un - étranger, pour que l’idée soit discutée plutôt qu’écartée d’un revers de la main.

La manière de Neil, de faire un simple test d’acceptance, pourrait être meilleure. Je le sais pour l’avoir essayé quelques fois. Cependant ma manière est plus amusante. Et je suis sûr de ça.

---
Auteur : [Ron Jeffries](http://ronjeffries.com/about.html)  
Source : [Getting small stories](http://xprogramming.com/articles/getting-small-stories/)  
Date de parution originale : 7 octobre 2014  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 31/05/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



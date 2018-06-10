---
layout: post
title:  "Pourquoi je continue à utiliser les cas d'utilisations"
date:   2011-12-11 00:01
published: true
tags:
- exigences
- cas d'utilisations
---

XP a pratiquement banni les cas d'utilisations, les remplaçant par "user stories" phonétiquement semblable (voir [Une user story est au cas d'utilisation ce qu'une gazelle est à un gazoduc(discussion: Re: Une user story est au cas d'utilisation ce qu'une gazelle est à un gazoduc)](http://www.les-traducteurs-agiles.org/2011/12/15/une-user-story-est-a-un-cas-d-utilisation-ce-qu-une-gazelle-est-a-un-gazoduc.html)), et les zélotes agiles ont été heureux de jeter les cas d'utilisations à la poubelle (avec les responsables de projets, les estimations, les planifications et les architectures). Scrum a fait de même, utilisant le "product backlog" à la place des "user stories". Néanmoins en passant du temps sur des projets, je n'arrête pas de passer dans des organisations souffrant de trois problèmes particuliers, réels, douleureux et coûteux.

1. Les users stories et les éléments de backlog ne donnent pas aux concepteurs un contexte à partir duquel travailler - quand un utilisateur fait ceci, alors quel est le contexte de leur opération, quel est l'objectif élargi à ce moment précis ?

2. Les users stories et les éléments de backlog ne donnent pas à l'équipe du projet un sens de "complétude" - ce que je n'arrête pas de trouver, est que l'équipe propose/estime les projets à (par exemple) 270 story points, et dès qu'ils commencent à travailler, ce nombre ne cesse de croître, sans limite apparente. Les développeurs sont déprimés et les sponsors en sont également déprimés. Quelle est la taille du projet, réellement ?

3. En relation avec la complétude, les user stories et les éléments de backlog ne donnent pas un mécanisme assez fiable pour regarder vers l'avenir, à la difficulté du travail à venir (en principe, ils pourraient, mais ils ne le font pas en pratique) - je n'arrête pas d'entendre cette complainte, "Nous posons une question à notre client (le product owner) et il/elle met 2 semaines à nous répondre. Nous devons avoir la mauvaise personne pour ce rôle.” Non, ils n'ont pas la mauvaise personne, ils ont un process cassé - certains types de questions prennent du temps pour faire des recherches dans les différents départements et groupes d'utilisateurs pour savoir ce qui est correct, et avoir une réponse partagée par la majorité d'entre eux. Regardant avec curiosité l'ensemble des conditions d'extension dans un cas d'utilisation, les analystes peuvent piger quelles sont celles qui seront faciles et celles qui poseront difficultés, et en fonction organiser leur recherche. Les user stories et les éléments de backlog n'ont pas une granularité définie assez tôt pour cette détermination - les conditions d'extension sont généralement détectées en milieu de sprint, lorsqu'il est trop tard.

Les cas d'utilisations sont, en effet, plus lourds et plus difficiles que les user stories ou les éléments de backlogs, mais ils apportent la valeur de ce poids supplémentaire. Comme un non-Einstein disait : "Faire les choses aussi simples que possible, mais pas plus simple." (L'attribution à Einstein a été semble-t-il discréditée.)

En particulier, les cas d'utilisations résolvent ces trois problèmes.

J'ai testé ceci ces 3 dernières années - j'entre et demande, "Dans votre/vos projet(s) agile(s), avez-vous par hasard souffert de l'une de ces trois choses ?" ... puis j'énonce les trois ... Plus fort même que je l'imaginais, il n'y a pas eu une seule organisation où j'ai posé cette question et qui n'ait pas dit : "Oh, Oui, et Comment !"

En d'autres mots, une utilisation naïve des user stories et des éléments de backlog peuvent provoquer des dégâts réels et très coûteux aux entreprises. Coûteux est mauvais.

Le plus récent, un cadre me disait à propos de la "livraison" d'un projet Scrum, qu'au moment de l'acceptation, il avait été découvert qu'il y avait toute une série de bénéficiaires du système dont les besoins n'avaient pas été identifiés du tout. Cette entreprise était face à la rédaction d'un contrat au forfait, les bénéficiaires n'étant pas certains de faire confiance à l’entreprise pour livrer un logiciel complet et utile.

Très coûteux, très mauvais. Le temps passé à la rédaction des cas d'utilisations et à la réalisation de recherche des exigences, aurait été récupéré largement, dans ce cas.

Voici 5 raisons pourquoi je continue d'écrire des cas d'utilisations ([les miens (discussion: Re: Structurer les cas d'utilisations avec des objectifs)](http://alistair.cockburn.us/Structuring+use+cases+with+goals) bien sûr :-)

1. La liste des objectifs fournit à la Direction le plus petit résumé possible de ce que le système apportera au métier et aux utilisateurs. Cela apporte aussi un squelette de planification de projet, à utiliser pour élaborer les prémisses des priorités, estimations, affectation de l'équipe et du timing. C'est la première partie de la question de la complétude.

2. Le scénario nominal de chaque cas d'utilisation apportent à toutes les personnes impliquées une vision commune de ce que le système fera basiquement, et aussi quelques fois plus important, de ce qu'il ne fera pas. Il fournit le contexte pour chaque élément d'exigence, un contexte qui est très difficile à obtenir ailleurs.

3. Les conditions d'extension de chaque cas d'utilisation fournissent aux analystes métiers un cadre pour rechercher toutes les petites, insignifiantes choses qui prennent quelques fois jusqu'à 80% du budget et temps de développement. Il fournit un mécanisme pour regarder vers l'avenir, afin que le client / product owner / analyste métier puisse déceler ces problématiques qui prennent du temps pour obtenir des réponses. Ces problématiques peuvent et devraient être mises au début du calendrier, afin que les réponses puissent être prêtes lorsque l'équipe de développement se réunira pour travailler dessus. Les conditions d'extension des cas d'utilisation sont la deuxième partie de la question de la complétude.

4. Les fragments du scénario d'extension du cas d'utilisation fournissent les réponses aux questions métiers détaillées épineuses posées par les développeurs : "Que sommes-nous supposés faire dans ce cas ?" (à laquelle, il est ordinairement répondu par : "Je ne sais pas, je n'ai jamais pensé à ce cas.") En d'autres mots, c'est un cadre de réflexion / documentation correspondant à la formulation si...alors...sinon qui aide les développeurs à réfléchir aux problématiques exposées. Sauf que ceci est fait au moment de l'étude, non à celui du développement

5. Le cas d'extension complet défini montre que les analystes ont considéré, à travers les besoins de chaque utilisateur, chaque objectif vis-à-vis du système, et de chaque variante métier concernée. C'est la dernière partie de la question de la complétude (Et oui, en effet, je me suis assis et j'ai parcouru 240 cas d'utilisation avec une cliente, à la fin de quoi, je me suis tourné vers elle et je lui ai demandé : "Et c'est tout ?" Elle a répondu, Oui, et nous l'avons construit, livré, nous avons été payés, et dix ans plus tard, il est toujours utilisé.)

Il y a plusieurs parties délicates pour les personnes utilisant les cas d'utilisations tels que je les décris :

* Il est vraiment facile de penser que tous les cas d'utilisations doivent être écrits à l'avance, quand, en fait, la rédaction devrait s'étaler durant toute la vie du projet. La partie "réflexion" ici est de déterminer combien devrait être écrits à l'avance pour avoir l'estimation du projet dans une zone de confiance, et quelle partie pourrait être différée pour une étude juste-à-temps.

* Ces jours-ci, les durées des itérations/sprints sont si courtes qu'il n'est pas commode d'implémenter un cas d'utilisation entier ne serait-ce que dans une seule d'entre elles. Cela signifie que du travail complémentaire est nécessaire, pour créer des user stories ou des éléments de backlog pour chaque cas d'utilisation, tracer que chacune d'elle a été développée, et s'assurer que l'ensemble des user stories ou des éléments de backlog ont effectivement livrés le sous-ensemble des cas d'utilisations pour cette livraison particulière.

* Écrire de bons cas d'utilisations (ou tout autre exigence(s)) exige de la réflexion, de la communication, et de nouveau de la réflexion. Il est plus facile d'écrire uniquement des user story sur des cartes et de laisser exploser le projet plus tard.

Si vous ne le pensez pas, trouvez une nouveau métier. Le développement logiciel exige de la réflexion, à tous les niveaux.

Si vous avez une histoire à propos de l’un de ces trois problèmes dans votre organisation, racontez-nous votre petite histoire sur la page "Discussions".

s. Pour approfondir le sujet :

* [Partie : précision, exactitude, pertinence, tolérance, conception objet à géométrie variable.](http://alistair.cockburn.us/Parts%3A+precision%2C+accuracy%2C+relevance%2C+tolerance%2C+scale+in+object+design)

* [Une user story est à un cas d'utilisation ce qu'une gazelle est à un gazoduc(discussion: Re: Une user story est à un cas d'utilisation ce qu'une gazelle est à un gazoduc)](http://www.les-traducteurs-agiles.org/2011/12/15/une-user-story-est-a-un-cas-d-utilisation-ce-qu-une-gazelle-est-a-un-gazoduc.html).

* [Cas d'utilisation agiles (Écrire des cas d'utilisation efficaces va dans le sens du Développement Logiciel agile) 180 (discussion: Re: Cas d'utilisation agiles (Écrire des cas d'utilisation efficaces va dans le sens du Développement Logiciel Agile)) 180)](http://alistair.cockburn.us/Agile+Use+Cases+%28Writing+Effective+Use+Cases+meets+Agile+Software+Development%29+180)

P.S. : Je sais que j'ai dit ces choses plusieurs fois ces dernières années, je les ai présentées, et j'avais pensé les avoir écrites. Mais cela ne semblait pas être le cas. Je suis content d'avoir eu la chance de réparer cet oubli.


---
Auteur : [Alistair Cockburn](http://alistair.cockburn.us/Alistair)
Source : [Why I still use use cases](http://alistair.cockburn.us/Why+I+still+use+use+cases)  
Date de parution originale : 09 Janvier 2008  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Relecteur : [Fabrice Aimetti](http://www.fabrice-aimetti.fr/)  
Date de traduction : 11/12/2011  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

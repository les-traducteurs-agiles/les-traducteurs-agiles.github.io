---
layout: post
title:  "Questions/Réponses à propos de la vélocité 3ème partie"
date:   2019-04-04 00:01
published: true
tags:
- vélocité
---

Dans la [2ème article](http://www.les-traducteurs-agiles.org/2019/01/29/questions-reponses-a-propos-de-la-velocite-2eme-partie.html) de cette série, nous avons parlé de la vélocité et de cette ligne (implicite) qui est de faciliter les choses pour le travail à faire plutôt que mettre encore plus de pression. Notre personnage « A » se posait la question si les _unités_ utilisées lors des estimations pourraient être d'une aide quelconque et qui, bien sûr, ne le sont pas.

Nous reprenons à partir de ce moment-là cette semaine avec ce petit extrait d'une discussion qui abordent quelques idées importantes :

> A: Then how can I get my 30-point velocity?
> B: What if there isn't a way? Maybe you need to need less?
> A: But the schedule....!
> B: The schedule is made up. How long it takes is real.

> A: Alors comment est-ce que je peux faire pour obtenir mes 30 points de vélocité ?
> B: Et s'il n'y avait aucune manière d'y arriver ? Peut être devriez-vous être moins exigeant ?
> A: Mais et le calendrier … !
> B: Le calendrier c'est quelque chose d'abstrait construit de toute pièces. La durée que cela prend de faire les choses c'est la réalité.

Software estimates are often wrong.

Les estimations en informatique sont souvent fausses.

Quite often they're off by over 200% on specific items. There is a very good reason for that, and that is that we aren't given uniform standardized work items and a standardized process. Nor can we be. If the feature the client wants has been written already, we don't write it again.

Assez souvent, elles s'avèrent inexactes d'environ 200 % sur des items spécifiques. Il y a une très bonne raison pour cela : les éléments fournis ne sont ni uniformes ni standardisés et le processus n'est pas standardisé non plus. Nous ne pouvons pas l'être non plus. Si la fonctionnalité souhaitée par le client a déjà été écrite, nous n'allons pas l'écrire à nouveau.

Software developers don't repeat thesmelves. Each problem and each solution is (a little bit) unique.

Les développeurs n'aiment pas se répéter. Chaque problème et chaque solution est (un tant soit peu) unique.

As such, each estimate includes not only effort but also a risk (of breaking something) and uncertainty (need to learn something).

Par conséquence, chaque estimation comporte non seulement l'effort à fournir mais aussi le risque (de casser quelque chose) et l'incertitude (le besoin d'apprendre quelque chose).

![diagramme](https://1.bp.blogspot.com/-paUyH-vNRI4/W1s552F1GDI/AAAAAAAAp-g/l1Phff-NAGc_SFEdi-gH9BeEvv9WuERngCLcBGAs/s1600/Screenshot%2B2018-07-27%2B10.26.16.png)

![diagramme](assets/tim_ottinger/incertitude-risque-effort.png)

* How long will it take you to learn how to do something you've not done before?
* What are the chances that adding this new feature will damage performance, suck memory, or complicate deployment?
* Have we discovered every "touch point" or is there some screen or report or calculation that needs to be modified because of the new data or procedure introduced by this change?
* What is the likelihood of some other unintentional or unforeseen consequences, perhaps due to different configuration options?
* Can we easily understand the code that we will have to be changing, or will it take considerable effort to unravel the original intent and comprehend all the side effects?

* Comment de bien cela va vous prendre pour apprendre comment faire quelque chose que vous n'avez jamais fait ?
* Quelles sont les chances pour qu'en ajoutant cette nouvelle fonctionnalité impactera négativement la performance de l'application, siphonera la mémoire ou compliquera le déploiement ?
* Quelle est la probabilité de voir arriver d'autres conséquences inattendues ou accidentelles, qui seront dues peut être à des options différentes de configuration.
* Pouvons-nous facilement comprendre le code que nous allons devoir modifier, ou est-ce que va nous demander des efforts considérables pour déchiffrer l'intention originelle et appréhender tous les effets de bord.

The **risk** element piles up greater and greater as a system grows. All new functionality, and especially functionality 'shoehorned' into place (quick and dirty hacks "to get it done fast") will increase the chance that something bad may happen in some dark corner of the code. Projects slow down over time due to this.

Le facteur **risque** va grimper de plus en plus au fur et à mesure que le système grandit. Toutes les fonctionnalités supplémentaires et tout spécifiquement les fonctionnalités 'implémentées au chausse-pieds' (avec des bidouillages vite faits mal faits "pour que ce soit fait rapidement") vont augmenter les chances que quelque chose se passe mal quelque part dans un coin obscur du code. Un certain nombres de projets dérapent à cause de cela.

When systems grow, and there is insufficient automated testing, then the ability of a developer to recognize that a new change has caused breakage is limited.

Lorsque les systèmes grandissent et que le nombre de tests automatisés est insuffisant, alors la capacité d'un développeur de prendre conscience qu'un changement récent ait provoqué un problème s'avère limitée.

Many software shops do a poor job of mitigating technical risks, and often blame them on "not having good enough programmers" when breakages inevitably occur.

Un certain nombre de boîtes informatiques font mal leur boulot en ce qui concerne la limitation des risques techniques, et prennent comme prétexte « de ne pas avoir d'assez bons développeurs » lorsque des problèmes arrivent inévitablement.

Sometimes more stories are done than expected because the risks didn't materialize and the learning was easier than anticipated.

Il arrive parfois que davantage de _stories_ soient faites que prévues parce que les risques ne se sont pas matérialisés ou que l'apprentissage a été plus facile que prévu.

Other times, unexpected risks materialize and stories blow up to several times their original estimate. But the same amount of work is being done every week.

À d'autres moments, des risques inattendus arrivent et la durée de réalisation des _stories_ peut exploser par rapport à leurs estimations d'origine. Mais la quantité de travail faite chaque semaine reste inchangée.

Estimates are made up. They were to someone's best guess about the amount of learning, the amount of typing, and the amount of risk that a story entails. Still, they can be off by 250% or more.

Des estimations ont été faites. Elles représentaient la meilleure conjecture qu'ait pu faire quelqu'un sur la quantité d'apprentissage, la quantité de code, et la quantité de risque qu'une _story_ génère. Malgré tout, elles peuvent être en dehors des clous de près de 250 % voire plus.

_**Schedules**_ tend to be based on _**estimates**_, although quite often this is done backward so that the estimates are based on the schedule.  

_**Les plannings**_ ont tendance à être basés sur les **estimations**, même si assez souvent cela est fait rétrospectivement afin que les estimations soient basées sur le planning.

The problem statement "we need 30 points per sprint" suggests that the original schedule and estimate were made based on a desire to have a particular thing finished by a particular time, believing that a high rate of accomplishment would be possible.

L'énoncé du problème « nous avons besoin de 30 points par sprint » suggère que le planning d'origine et l'estimation ont été faite sur la base du désir qu'une chose particulière soit terminé à un moment particulier, avec la croyance qu'un haut taux d'accomplissement serait possible.

Here, where the rubber meets the road, the actual work is not happening as fast as the original scheduler hoped that it would. This leaves the manager in a tough spot since the actual rate of completion is about 2/3rds the anticipated/hoped rate of completion.

Mais, là où le bât blesse, c'est que le vrai travail ne se déroule pas aussi vite qu'on aurait pu l'espérer dans le planning d'origine. Cela laisse le manager dans une situation délicate étant donné que taux réel de réalisation est environ des 2/3 du taux anticipé/espéré de réalisation.

There is a very real risk that a full 1/3 of the project cannot be completed on time.

Il y a un vrai risque que 1/3 du projet ne puisse être terminé dans les temps.

A smart software manager understands this, and so prioritizes so that the most important features are built early on and delivered soon. That way, when work has to be descoped, it is the least important work being dropped.

Un responsable informatique intelligent comprend bien tout cela, et il va par conséquent priorisé les fonctionnalités les plus importantes à faire d'abord afin de les livrer au plus tôt. De cette manière, lorsque du travail doit sortir du périmètre, ce sera les choses les moins importantes qui seront abandonnées.

This means not only sacrificing some stories but possibly the less-interesting parts of every story (cf Story Mapping and Example Mapping, Walking Skeletons, Evolutionary Design, etc).

Cela signifie non seulement de sacrifier certaines _stories_ mais potentiellement les parties les moins intéressantes de chaque _story_ (cf Story Mapping, la cartographie des _stories_ ; Example Mapping, la cartographie des exemples ; Walking Skeletons, les squelettes ambulants ; Evolutionary Design, la conception évolutionnaire etc).

A smart team will find -- through feedback -- which parts of the project should not be built at all. Often people over-specify and over-design. Sometimes the presence of a simple solution reduces the need for a comprehensive one.  This is built into the agile manifesto (called "simplicity", defined as "maximizing the amount of work not done") and is crucial to all agile methods.

Une équipe intelligente trouvera -- à travers des retours d'informations -- quelles parties du projet ne devraient pas être faites. Souvent les gens sur-spécifient et sur-conçoivent. Certaines fois la présence d'une solution simple réduit le besoin d'une solution globale. Cela fait partie intégrante du manifeste agile (sous la dénomination de « simplicité », et définie comme étant « l’art de minimiser la quantité de travail inutile »)

If we can need less, we can deliver sooner.
If we can prioritize well, we can sacrifice lower-value work.

Si nous avons besoin de moins, nous pouvons livrer plus tôt.
Si nous pouvons bien prioriser, nous pouvons sacrifier des choses ayant peu de valeur.

_Feedback from customers_ improves our prioritization and our ability to descope intelligently but requires us to release code to them early and often.

_Les retours d'informations des clients_ améliorent notre priorisation et notre capacité à sortir des éléments du périmètre intelligemment mais cela nous demande de leur livrer du code le plus tôt et le plus souvent possible.

If developers are pushed to provide brute-force, quick-n-dirty solutions then it increases the cost of change due to more difficulty researching changes and more difficulty spotting breakages.

Si les développeurs sont poussés à livrer des solutions brutes, vite fait et mal ficelées alors cela augmentent le coût du changement en raison de difficultés plus grandes pour rechercher les changements et à repérer les problèmes.

With enough risk pushed into the code, it may become intractable. The team may have to stop producing new features to clean it up. Nobody wants that. It is faster to write clean code with good automated tests to being with than to end up spending 80% of developers' time cleaning up messes and defects.

Avec tous ces risques poussés dans le code, ce dernier peut devenir ingérable. L'équipe peut être amenée à devoir arrêter de produire de nouvelles fonctionnalités pour le nettoyer. Personne ne veut ça. Il est plus rapide d'écrire du code propre avec de bons tests automatisés plutôt que de finir à passer 80 % du temps des développeurs à nettoyer le bordel et les anomalies.

Which again brings us to the hard truth in this installment:

Ce qui nous amène à nouveau à la dure vérité de cet article :

How long it actually takes is real. Estimates are made up.

La durée que cela prend de faire les choses c'est la réalité. Les estimations sont une construction.

Blaming reality for not matching fantasy isn't useful, and blaming people for making up unrealistic schedules is not helpful. We are where we are. We have to move forward.

Blâmer la réalité de ne pas correspondre à la fiction c'est inutile, et blâmer les gens de faire des plannings irréalistes n'est d'aucune aide. Nous sommes là où nous en sommes. Nous devons aller de l'avant.

It leaves us with a bit of optimistic pessimism: if this work cannot be fully completed, what is the best possible release we can make given the resources, time, and scope at hand?

Cela nous laisse avec un arrière-goût de pessimisme optimiste : si ce travail ne peut pas être réalisé complètement, quel est la meilleure livraison possible que nous pouvons faire étant donné les ressources, le temps et le périmètre disponible ?

See you back here for [Part IV](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-iv.html).

Rendez-vous [ici](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-iv.html) pour la 4ème partie

---
Auteur : Tim Ottinger
Source : [Q&A on Velocity, Part III](https://agileotter.blogspot.com/2018/07/q-on-velocity-part-ii.html)  nbsp
Date de parution originale : 27 juillet 2018  nbsp

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  nbsp
Date de traduction : jj/mm/yyyy  nbsp

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

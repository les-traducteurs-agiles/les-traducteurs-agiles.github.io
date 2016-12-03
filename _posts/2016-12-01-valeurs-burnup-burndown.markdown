---
layout: post
title:  "Quelle valeur donnez-vous aux graphiques de burndown et de burnup ? "
date:   2016-12-03 00:00:01
published: true
categories: 
- scrum
- dark scrum
---

I met a team recently who was concerned about their velocity. They were always “too late” according to their manager.

Récemment, j’ai rencontré une équipe qui était préoccupée à propos sa vélocité. D’après leur patron, elle était toujours “en retard”. 

I asked them what they measured and how. They measured the burndown for each iteration. They calculated the number of points they could claim for each story. Why? Because they didn’t always finish the stories they “committed” to for each iteration.

J’ai donc demandé aux membres de l’équipe ce qu’ils mesuraient et comment. Ils m’ont répondu qu’à chaque itération, ils mesuraient le _burndown_ et plus précisément le nombre de points qu’ils pouvaient revendiquer de chaque story. Pourquoi ? Parce les stories sur lesquelles ils s’“engageaient” à chaque itération n’étaient pas toujours terminés par l’équipe.

This is what their burndown chart looked like.

<div align="left" style="float:left; padding-right:30px" >
  <img title="Nombre de points de stories restantes" src="{{ site.url }}assets/johanna/Burndown.StoryPoints.jpg" />
</div>

Voici à quoi leur graphique de _burndown_ pouvait ressembler.

A burndown chart measures what you have finished. If you look at their burndown, you can see there are times when not much is done. Then, near the end of the iteration, they finish more. However, they don’t finish “everything” before they run out of time.

Un graphique de _burndown_ mesure ce que vous avez terminé. Si vous regardez leur _burndown_, vous pouvez voir qu’il y a des moments où il n’y a pas grand chose de fait. Puis, vers la fin de l’itération, il s’avère que davantage de stories sont terminées. Toutefois, l’équipe ne finit pas “tout” avant de se trouver à court de temps.

An iteration is a timebox, by definition. In this case, having to “declare victory” and assess what they were doing should have helped them. But, when this team saw the burndown, two interesting things happened. They beat themselves up for not finishing. And, when they didn’t finish everything, they didn’t always do a retrospective. In addition, the product owner often took the unfinished work and added it to the next iteration’s work. Yes, added, not replaced. That meant they never caught up.

Par définition, une itération est une période de temps fixe. Dans ce cas, “crier victoire” et évaluer ce qu’ils faisaient auraient dû les aider[^1]. Mais, lorsque l’équipe a vu le _burdown_, deux choses intéressantes se sont produites. Les membres de l’équipe se sont disputés entre eux parce qu’ils n’avaient pas tout fini. Et même lorsque l’équipe ne peut pas tout terminer, elle ne fait pas forcément de rétrospective. Et en plus, le _product owner_ avait pour habitude de prendre le travail non terminé et de le rajouter au travail à faire pour la prochaine itération. Oui, rajouté et non à la place de. Ce qui signifie que l’équipe ne pouvait jamais y arriver..

They tried this burndown chart next, to see if they could meet their ideal.

<div align="left" style="float:left; padding-right:30px" >
  <img title="Nombre de points de stories restantes avec droite idéale" src="{{ site.url }}assets/johanna/Burndownwithidealline.jpg" />
</div>

Par la suite, les membres de l’équipe ont essayé ce type de graphique de _burndown_ pour voir s’ils pouvaient rejoindre la droite idéale.

They realized they were “late,” off the ideal line from Day 2. They felt worse about themselves.

Dès le deuxième jour, ils ont réalisés qu’ils étaient “en retard” par rapport à la droite idéale et ils se sont sentis très mal.

They stopped doing retrospectives, which meant they had no idea why they were “late.”

Ils ont arrêtés de faire des rétrospectives, ce qui signifie qu’ils n’avaient aucune idée sur le pourquoi ils étaient “en retard”.

A burndown emphasizes what you have completed. A burndown with the “ideal” line emphasizes what you have done and what you “should” be doing. I have used story points here. You could look at story points against time, looking at the available hours or people days or something like that.

Un _burndown_ met l’accent sur ce que vous avez réalisé. Un _burndown_ avec une droite idéale met l’accent sur ce que vous avez fait et sur ce que vous “devriez” être en train de faire. Ici, j’ai utiliser des points de story. Vous pourriez faire un graphique des points de story par rapport au temps, en regardant les heures disponibles ou les jours/hommes ou un autre truc du même genre.

For me, a burndown is interesting, but not actionable. Think about what happens when you take a trip. You plug your destination into your favorite GPS (or app), and it calculates how much longer it will take to get to your destination. You know you have driven some number of miles, but to be honest, that’s done. What’s interesting to you is what you have remaining. That’s what a burnup chart helps you see.

Pour moi, un  _burndown_ est intéressant mais n’est pas actionnable. Pensez à ce que faites quand vous préparez un voyage. Vous saisissez votre destination dans votre GPS préféré (ou dans une app) et il calcule le temps que cela prendra pour arriver à votre destination. Lorsque vous conduisez ensuite, vous voyez le nombre de kilomètres parcourus, mais bon pour être honnête, voilà - c’est fait. Ce qui vous intéresse, c’est ce qui reste à faire. C’est ce qu’un graphique de  _burnup_ vous aide à voir.

For me, a burnup is a way to see what we have accomplished and what’s remaining. I can learn more from a burnup than I can from a burndown. That’s me. Here’s a burnup of the same data:

Pour moi, un _burnup_ est une manière de voir ce que nous avons accompli et ce qu’il reste. Je peux en apprendre plus d’un _burnup_ que je ne le peux d’un _burndown_. C’est mon point de vue. Voici donc un _burnup_ réalisé à partir des mêmes données que pour le _burndown_.

I made these charts from exactly the same data. Yet, I have a different feeling when I see the burnups.

<div align="left" style="float:left; padding-right:30px" >
  <img title="Nombre de points de stories finies" src="{{ site.url }}assets/johanna/StoryPointBurnup.jpg" />
</div>

J’ai fait ces graphiques exactement avec les mêmes données. Toutefois, j’ai un ressenti différent quand je vois des _burnups_.

When I see the Story points Done without the ideal line, I see a hockey stick. It’s not as bad a stick as the image in [Is the Cost of Continuous Integration Worth the Value on Your Program?, Part 1](http://www.jrothman.com/mpd/program-management/2011/12/is-the-cost-of-continuous-integration-worth-the-value-on-your-program-part-1/), and it’s still a significant hockey stick.

Quand j’observe ce nombre points de stories finies sans droite idéale, j’y vois une crosse de hockey. Ce n’est pas aussi mauvais qu’une courbe en forme du bâton telle que l’on peut la voir dans l’article [Is the Cost of Continuous Integration Worth the Value on Your Program?, Part 1](http://www.jrothman.com/mpd/program-management/2011/12/is-the-cost-of-continuous-integration-worth-the-value-on-your-program-part-1/)[^2] mais ça reste une crosse de hockey significative.

When I see this burnup, I can tell by Day 3 that we are “behind” from where we want to be. By Day 5, I know we cannot “make up” the time. As any team member, I can raise this as an impediment in the daily standup. If I am a leader of any sort, I will put this on my list to discuss in the retrospective, if not problem-solve before.

<div align="left" style="float:left; padding-right:30px" >
  <img title="Nombre de points de stories finies avec droite idéale" src="{{ site.url }}assets/johanna/StoryPointBurnupwithIdealLine.jpg" />
</div>

Quand je vois ce _burnup_, je peux dire qu’à partir du jour 3, nous sommes “largués” par rapport à là où nous voudrions être. Au jour 5, je sais que nous pouvons pas “rattraper” à temps. Comme tout personne membre de l’équipe, je peux signaler cela comme étant un obstacle lors de la mêlée quotidienne. Si je suis un responsable - peu importe le domaine - , je mettrai cela sur ma liste d’éléments à aborder pour la rétrospective, si cela n’est pas résolu d’ici là.

Maybe that’s just the way my mind works. I like seeing where we are headed and what it will take to get there. I’m interested in what we’ve done, but that’s in the past. I can’t address the past except to retrospect. I can address the future and say, “Is there something we can do now to help us accomplish what we thought we could in this timebox?”

Peut être, est-ce simplement la manière dont mon cerveau fonctionne. J’aime voir là où nous allons et le temps que cela va nous prendre pour y aller. Cela m’intéresse de savoir ce que nous avons pu faire, mais c’est le passé. Je ne peux pas m’occuper du passé si ce n’est pour faire une rétrospective. Par contre, je peux m’occuper du futur et dire “Est-ce qu’il y a quelque chose que nous pouvons faire aujourd’hui pour nous aider à accomplir ce que nous pensions pouvoir faire pendant cette période de temps ?” 

George Dinwiddie has a great article on burndown charts: [Feel the Burn: Getting the Most out of Burndown Charts](http://idiacomputing.com/pub/BetterSoftware-BurnCharts.pdf).

George Dinwiddie a écrit un grand article au sujet des graphiques de _burndown_ : [Feel the Burn: Getting the Most out of Burndown Charts](http://idiacomputing.com/pub/BetterSoftware-BurnCharts.pdf)[^2].

Oh, and the team I discussed earlier? They decided they were trying to cram too much into an iteration. They made their stories smaller. That put more pressure on their product owner, but then they realized lack of PO time was an impediment. They thought they were to blame with a burndown. They saw their data more easily with a burnup. Maybe we all had a mind-meld going on.

Oh, et l’équipe dont je parlais tout à l’heure ? Eh bien, elle a  décidé qu’elle essayait d’en mettre trop dans une itération. Elle a fait des stories plus petites. Ce qui a mis plus de pression sur son _product owner_ mais elle a alors réalisé que le manque de disponibilité du PO était un obstacle. Elle a pensé qu’elle serait plus mise sur le grill avec un _burndown_ alors qu’avec un _burnup_ la lecture des données était plus aisée. Peut-être que nous avons eu la même idée en même temps.

It doesn’t matter which chart you generate. It matters how the chart makes you feel: what action will you take from  your chart? If it’s not prompting you to act early, maybe you need a different chart. One project truism is: You cannot “make up” time. You can choose actions based on what your data tells you. Can you hear your data?

Peu importe le graphique que vous générez. Ce qui compte c’est qu’est-ce qu’il vous fait ressentir : quelle type d’action allez-vous prendre à partir des informations présentes sur votre graphique ? S’il ne vous fait réagir au plus vite, peut-être avez-vous besoin d’un autre type de graphique. Une vérité évidente pour tout projet est : vous ne pouvez pas “rattraper” le temps. Vous pouvez choisir de faire telle ou telle action à partir de ce que peuvent vous dire vos données. Pouvez-vous entendre vos données ?


[^1]: célébrer une petite victoire, ça fait toujours bien - NdT
[^2]: en vo, article non traduit - NdT

---
Auteur : [Johanna Rothman](http://www.jrothman.com/about/)  
Source : [Value of Burndown and Burnup Charts](http://www.jrothman.com/mpd/project-management/2016/02/value-of-burndown-and-burnup-charts/)  
Date de parution originale : 02 Février 2016  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 03/12/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}


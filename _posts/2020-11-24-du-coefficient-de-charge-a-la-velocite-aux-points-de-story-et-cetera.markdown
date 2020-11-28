---
layout: post
title:  "Du coefficient de charge à la vélocité aux points de story au décomptage de story au temps de traversée au …"
date:   2020-11-24 08:42
published: false
tags:
- vélocité
---

> ## The problem is that we’re over-optimistic

> Le problème c'est que nous sommes trop optimistes

The problem is that when we estimate how long it will take us to build something, we tend to be over-optimistic. We tend not to take into account all the interruptions and overheads of the typical work day nor the inevitable complications that show up on any “straightforward” task.

Le problème c'est que lorsque nous estimons la durée du temps que cela va nous prendre pour faire quelque chose, nous avons tendance à être trop optimistes. Nous avons tendance à ne pas prendre en compte toutes les interruptions et le fait d'avoir du boulot par-dessus la tête comme cela peut être le cas dans journée de travail classique ni les inévitables complications qui peuvent surgir sur une tâche « simple ».

I don’t remember anyone ever referencing this in the early days of Extreme Programming, but this is essentially the optimism bias that leads to the [planning fallacy](https://en.wikipedia.org/wiki/Planning_fallacy), proposed by Daniel Kahneman and Amos Tversky in 1979.

Je ne me rappelle pas que quelqu'un l'ait dit dans les premiers temps d'Extreme Programming, mais il s'agit en fait d'un biais cognitif qui conduit aux douces [illusions de la planification](https://en.wikipedia.org/wiki/Planning_fallacy) tel que présenté par DDaniel Kahneman et Amos Tversky en 1979.

## This led to the idea of [Load Factor](http://c2.com/cgi/wiki?LoadFactor)

## Cela nous conduit à l'idée du [Coefficient de charge (vo)](http://c2.com/cgi/wiki?LoadFactor)

We estimated each task in Perfect Engineering Days or Ideal Days(no interruptions, perfect flow) and then we multiplied by a Load Factor (originally 2.5, eventually most teams started with 3) to determine a more likely duration in real days. In essence, we assumed that everything would take around 3x longer than we thought.

Nous avons estimé chaque tâche en jour parfait d'ingénierie ou jour idéal (aucune interruption, flux parfait) puis nous multiplions cela par le coefficient de charge (à l'origine 2,5 ; la plupart des équipes utilisent 3 pour commencer) pour déterminer une durée qui se rapproche le plus d'une durée en jours réels.

Over multiple iterations, we could refine Load Factor to better reflect the actual data from the team. In the teams I was on, it usually ended up being 2.something.

Au fur et à mesure des multiples itérations, nous pouvons affiner le coefficient de charge pour mieux refléter la réalité de l'équipe. Dans les équipes dont j'ai fait partie, cela tournait généralement autour de 2 et des brouettes.

The problem was over-optimism. The solution was Load Factor. It roughly worked.

Le problème était le trop d'optimisme; La solution fût le coefficient de charge. Cela marchait grosso modo.

## Yesterday’s Weather is simpler than Load Factor

## La météo de la veille est plus simple que le coefficient de charge

But wait. What if you could make this simpler? Instead of multiplying by Load Factor, just observe how many Ideal Days you did every iteration (aka observe the [Project Velocity](http://c2.com/cgi/wiki?ProjectVelocity)). Each iteration, you simply committed to what you completed in the last iteration. This was known as [Yesterday’s Weather](http://c2.com/cgi/wiki?YesterdaysWeather).

Mais attendez une minute. Et si nous pouvions faire plus simple ? Et si au lieu de multiplier par un coefficient de charge, nous observons simplement le nombre de jours idéaux faits lors de chaque itération (alias la [vélocité du projet (vo)](http://c2.com/cgi/wiki?ProjectVelocity)). À chaque itération vous vous engagez simplement par rapport à ce que vous été en mesure de faire à la dernière itération. Cette approche est connue sous le nom de [météo de la veille (vo)](http://c2.com/cgi/wiki?YesterdaysWeather).

Velocity is the inverse of Load Factor and is simpler to understand. The practice of using Yesterday’s Weather to shape commitment theoretically gave the team a breather after tough iterations. In my experience, Yesterday’s Weather tended to be more of a guide than a rule.

La vélocité est l'inverse du coefficient de charge et elle est plus simple à comprendre. La pratique de l'utilisation de la météo de la veille pour formuler son engagement donne théoriquement à l'équipe un répit après des itérations difficiles. D'après mon expérience, on se sert de la météo de la veille plutôt comme d'un guide plutôt que comme une règle absolue à suivre.

The problem was still over-optimism. The simpler solution was Velocity and Yesterday’s Weather. It roughly worked.

Le problème par contre c'est que nous sommes toujours trop optimistes. La solution de vélocité et de la météo de veille est plus simple. Et ça marche grosso modo.

## I’d rather not get into why real days aren’t the same as ideal days…

## Je ne devrais pas dire pourquoi les jours réels ne sont pas la même chose que les jours idéaux …

Even back when people were using Load Factor, there would always be managers who would be challenging why the Ideal Days were not equivalent to Real Days. To attempt to sidestep this discussion, many teams chose to adopt arbitrary size units (_e.g._, [Gummi Bears](http://c2.com/cgi/wiki?GummiBearsOfComplexity), [Nebulous Units of Time](http://c2.com/cgi/wiki?NebulousUnitOfTime), etc.). Eventually, most teams stabilised around the term [Story Points](http://c2.com/cgi/wiki?StoryPoints) as more palatable to most environments.

Même lorsque les gens utilisaient le coefficient de charge, il y avait toujours des managers qui venaient à la charge en demandant pourquoi les jours idéaux n'étaient équivalents aux jours réels. Pour tenter d'esquiver cette discussion, un certain nombre d'équipes ont choisi d'adopter des unités arbitraires de mesures (par exemple en [Gummi Bears (vo)[^1] ](http://c2.com/cgi/wiki?GummiBearsOfComplexity), [Nebulous Units of Time (vo)[^2]](http://c2.com/cgi/wiki?NebulousUnitOfTime), etc.). Et finalement, la plupart des équipes ont fini par utilisé le terme de [points de story](http://c2.com/cgi/wiki?StoryPoints) comme étant le plus satisfaisait dans la plupart des cas.

I also believe that around this time, people were arguing that relative estimation was easier for humans than absolute estimation. That is, it’s easier for you to say these two tasks are roughly comparable than to say how long each task will take in days.

Je crois aussi qu'à ce moment-là, les gens affirmaient qu'il était plus facile pour le commun des mortels de faire des estimations relatives plutôt qu'absolue. Ceci dit, il est plus facile de dire que deux tâcjhes sont à peu près comparable que de dire la durée en jours que chaque tâche prendra.

[Planning Poker](https://en.wikipedia.org/wiki/Planning_poker) became popular but the fastest way to do Story Point estimation that I’m aware of is [Swimlane Sizing](http://theagilepirate.net/archives/109).

La pratique du [planning poker] est devenue populaire même si la manière de faire une estimation en point de story que je connaisse est celle du [Swimlane Sizing (vo)[^3]](http://theagilepirate.net/archives/109).

The problem was still over-optimism, but we also had the problem of over-optimism of managers and the difficulty of estimating. The solution was switching to Story Points. It roughly worked.

Le problème était toujours que nous étions trop optimistes, mais nous avions aussi le problème des managers trop optimistes et de la difficulté quant à estimer. La solution a été de changer d'approche pour utiliser les points de story. Cela a marché grosso modo.

## Just count the Stories

## Compter simplement le nombre de stories

When you break down work into Stories that are roughly 1–5 Story Points, you’ll begin to notice that they average out to 2.something. Many teams started to notice this and thought: “Instead of using Story Points, why don’t we just count Stories instead?”

Lorsque vous décomposez le travail à faire en stories qui font grosso modo entre 1 et 5 points de story, vous commencerez à remarquer qu'elles auront tendance à tourner autour de 2 et des brouettes. Beaucoup d'équipes ont commencé à remarquer cela et à penser : « Et si à la place d'utiliser les points de story, pourquoi ne nous compterions pas simplement le nombre de stories à la place ? »

The problem is still over-optimism and the difficulty of estimating. The solution is counting stories. It roughly works.

Le problème c'est que nous étions toujours trop optimistes and qu'il était toujours difficile d'estimer. La solution a été de compter les stories. Cela fonctionne grosso modo.

## Why are we grouping everything into big projects?

## Pourquoi avons-nous tendance à tout regrouper dans de gros projets ?

One of the key target attributes of a User Story is that it can be delivered independently. If that is actually the case, why are we grouping them together? Instead of asking how many Stories will get delivered after a period of time, why not ask, when will this Story be delivered? If we collect data on the start-to-done lead times of Stories, we can then use this data to estimate a range for when any particular story will get done. We can even do this for different Story sizes if necessary.

Un des éléments-clés d'une user story est que nous pouvons la livré de manière indépendante les unes des autres. Et si c'est bien le cas, pourquoi les regroupons-nous ensemble ? À la place de nous poser la question du nombre de stories que nous pourrions livrer dans une période de temps donnée, pourquoi pas plutôt nous poser la question, à quel moment cette story peut être livré ? Si nous récupérons des données les temps de traversée des stories de leur date de début à leur date de fin, nous pourrions utiliser ces données pour estimer une fourchette du moment à partir de quand une story pourrait être terminée; Nous pouvons même faire cela pour différentes tailles de story si c'est nécessaire.

The problem is still over-optimism and the difficulty of estimation. The solution is measuring start-to-done lead time to support estimation. It roughly works.

Le problème du trop d'optimisme et la difficulté pour estimer demeure. La solution pour aider à estimer consiste à mesurer le temps de traversée du début à la fin. Cela marche grosso modo.

[^1]: en petits nounours (les bonbons)  
[^2]: unité temporelle nébuleuse  
[^3]: estimation en couloir

---
Auteur : [Jason Yip](https://jchyip.medium.com/about)  
Source : [From “Load Factor” to “Velocity” to “Story Points” to “Counting Stories” to “Lead Time” to …](https://jchyip.medium.com/from-load-factor-to-velocity-to-story-points-to-counting-stories-to-lead-time-to-5f261707c76c)  
Date de parution originale : 29 Février 2016  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 28/11/2020  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

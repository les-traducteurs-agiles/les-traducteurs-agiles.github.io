---
layout: post
title:  "Du coefficient de charge à la vélocité aux points de story au décomptage de story au temps de traversée au …"
date:   2020-11-29 00:00
published: true
tags:
- vélocité
- temps de traversée
---

> #### Le problème c'est que nous sommes trop optimistes

Le problème c'est que, lorsque nous estimons la durée du temps que cela va nous prendre pour faire quelque chose, nous avons tendance à être trop optimistes. Nous avons tendance à ne pas prendre en compte ni toutes les interruptions et d'être déjà débordé comme cela peut nous arriver dans une journée de travail ordinaire ni les inévitables complications qui peuvent surgir sur une tâche « simple ».

Je ne me rappelle pas que quelqu'un l'ait dit dans les premiers temps d'Extreme Programming, mais il s'agit en fait d'un biais cognitif qui nous conduit tout droit aux douces [illusions de la planification](https://en.wikipedia.org/wiki/Planning_fallacy) comme a pu le présenté Daniel Kahneman et Amos Tversky en 1979.

## Cela nous a conduit à l'idée du [Coefficient de charge (vo)](http://c2.com/cgi/wiki?LoadFactor)

Nous avons estimé chaque tâche en jour parfait d'ingénierie ou jour idéal (aucune interruption, flux parfait) puis nous les avons multipliées avec un coefficient de charge (à l'origine 2,5 ; la plupart des équipes utilisent 3 pour commencer) pour déterminer une durée qui se rapproche le plus d'une durée en jours réels. En substance, nous avons pris comme postulat que tout va prendre 3 fois plus de temps que ce que nous avons pu imaginer.

Au fur et à mesure des itérations, nous aurions pu affiner le coefficient de charge pour mieux refléter la réalité quotidienne de l'équipe. Dans les équipes dont j'ai fait partie, cela tournait généralement autour de 2.

Le problème était le trop d'optimisme. La solution fût le coefficient de charge. Cela marchait grosso modo.

## La météo de la veille est plus simple que le coefficient de charge

Mais attendez une minute. Et si nous pouvions faire plus simple ? Et si au lieu de multiplier par un coefficient de charge, nous observions simplement le nombre de jours idéaux faits lors de chaque itération (alias la [vélocité du projet (vo)](http://c2.com/cgi/wiki?ProjectVelocity)). À chaque itération vous vous engagez simplement par rapport à ce que vous été en mesure de faire à la dernière itération. Cette approche s'appelait la [météo de la veille (vo)](http://c2.com/cgi/wiki?YesterdaysWeather).

La vélocité est le contraire du coefficient de charge et s'avère bien plus simple à comprendre. La pratique de l'utilisation de la météo de la veille permet de structurer l'engagement pour l'itération à venir et permet en théorie, du moins, de donner à l'équipe un répit après des itérations difficiles. D'après mon expérience, la météo de la veille est plutôt un guide qu'une règle absolue à suivre.

Le problème par contre c'est que nous sommes restés encore trop optimistes. La solution de vélocité et de la météo de veille s'est avérée plus simple. En gros, ça a marché.

## Je ne préfère ne pas entrer dans les détails sur pourquoi les jours réels ne sont pas la même chose que les jours idéaux …

Même lorsque les gens utilisaient le coefficient de charge, il y avait toujours des managers qui venaient à la charge en demandant pourquoi les jours idéaux n'étaient équivalents aux jours réels. Pour tenter d'esquiver cette discussion, un certain nombre d'équipes ont choisi d'adopter des unités arbitraires de mesures (par exemple en [Gummi Bears [vo]](http://c2.com/cgi/wiki?GummiBearsOfComplexity)[^1], en [Nebulous Units of Time [vo]](http://c2.com/cgi/wiki?NebulousUnitOfTime)[^2], etc.). La plupart d'entre elles ont fini par adopter le terme de [points de story](http://c2.com/cgi/wiki?StoryPoints) comme étant le plus adéquate dans la plupart des cas.

Je crois aussi qu'à cette période-là, les gens soutenaient qu'il était plus facile pour le commun des mortels de faire des estimations relatives plutôt qu'absolue. Quoi qu'il en soit, il est plus facile de dire que deux tâches sont à peu près comparables que de dire la durée en jours que chacune prendra.

La pratique du [planning poker](https://fr.wikipedia.org/wiki/Planning_poker) est devenue populaire même si la manière de faire une estimation en point de story la plus rapide que je connaisse est celle du [Swimlane Sizing (vo)](http://theagilepirate.net/archives/109)[^3].

Le problème c'est que nous sommes restés encore trop optimistes, mais nous avons aussi eu le problème de managers trop optimistes et de la difficulté pour estimer. La solution a été de changer d'approche pour utiliser les points de story. En gros, ça a marché.

## Compter simplement le nombre de stories

Lorsque vous décomposez le travail à faire en stories qui font grosso modo entre 1 et 5 points de story, vous commencerez à remarquer qu'elles auront tendance à tourner autour de 2. Beaucoup d'équipes ont commencé à remarquer cela et à penser : « Et si à la place d'utiliser les points de story, pourquoi ne pas compter simplement le nombre de stories ? »

Le problème c'est que nous sommes toujours trop optimistes et qu'il reste difficile d'estimer. La solution est de compter les stories. En gros ça fonctionne.

## Pourquoi avons-nous tendance à tout regrouper dans de gros projets ?

Un des éléments-clés d'une user story, c'est qu'il est possible de la livrer indépendamment d'une autre story. Et si c'est bien le cas, pourquoi les regroupons-nous ensemble ? À la place de nous poser la question du nombre de stories que nous pourrions livrer dans une période de temps donnée, pourquoi ne pas plutôt nous poser la question, à quel moment cette story peut-elle être livré ? Si nous récupérons les données sur les temps de traversée des stories de leur date de début à leur date de fin, nous pourrions utiliser ces données pour estimer une fourchette du moment à partir duquel une story pourrait être terminée. Nous pouvons même faire cela pour différentes tailles de story si cela s'avère nécessaire.

Le problème du trop d'optimisme et la difficulté pour estimer demeure. La solution pour aider à estimer consiste à mesurer le temps de traversée du début à la fin. En gros, ça marche.

[^1]: en petits nounours (les bonbons) - Miam (NdT)  
[^2]: unité temporelle nébuleuse  
[^3]: estimation en couloir

---
Auteur : [Jason Yip](https://jchyip.medium.com/about)  
Source : [From “Load Factor” to “Velocity” to “Story Points” to “Counting Stories” to “Lead Time” to …](https://jchyip.medium.com/from-load-factor-to-velocity-to-story-points-to-counting-stories-to-lead-time-to-5f261707c76c)  
Date de parution originale : 29 Février 2016  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 29/11/2020  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

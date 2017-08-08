---
layout: post
title:  "Le modèle INVEST - E comme stories Estimables"
date:   2017-04-25 00:00:01
published: true
tags: 
- user stories
---

**Estimable** stories can be estimated: some judgment made about their size, cost, or time to deliver. (We might wish for the term _estimatable_, but it’s not in my dictionary, and I’m not fond enough of estimating to coin it.)

Des stories **estimables** peuvent être estimées : qu’il s’agisse de la taille, du coût ou de la durée de réalisation (Nous aurions pu vouloir utiliser le terme _estimabilité_ [^1] , mais il n’existe pas dans mon dictionnaire, et je n’aime pas assez les estimations pour le revendiquer.)

To be estimable, stories have to be understood well enough, and be stable enough, that we can put useful bounds on our guesses.

Pour qu’elles soient estimables, les stories doivent être suffisamment comprises, suffisamment stables afin que nos suppositions puissent rester dans des limites sensées. 

_A note of caution: Estimability is the most-abused aspect of INVEST (that is, the most energy spent for the least value). If I could re-pick, we’d have “E = External”; see the discussion under “[V for Valuable](http://xp123.com/articles/valuable-stories-in-the-invest-model/)”._

_Petit message d’avertissement : l’estimabilité est l’aspect le plus mal compris du modèle INVEST (c’est-à-dire celui ayant le rapport énergie dépensée / valeur le moins intéressant). Si je devais choisir à nouveau, nous aurions “E = Externe” ; pour plus d’informations voir [V pour ayant de la valeur](http://www.les-traducteurs-agiles.org/2017/04/25/le-modele-invest-pour-des-stories-de-valeur.html)._

##Why We Like Estimates

## Pourquoi nous aimons les estimations

Why do we want estimates? Usually it’s for planning, to give us an idea of the cost and/or time to do some work. Estimates help us make decisions about cost versus value.

Pourquoi voulons-nous faire des estimations ? Généralement, nous les voulons dans un but de planification, pour nous donner une idée du coût et/ou du temps nécessaire pour faire le travail. Les estimations nous aident à prendre des décisions coût / valeur.

When my car gets worked on, I want to know if it’s going to cost me $15 or $10K, because I’ll act differently depending on the cost. I might use these guidelines:

Lorsque qu’il y a des travaux sur ma voiture, je veux savoir si cela va me coûter 15€ ou 10 000 €, parce que selon le coût, ma décision ne sera pas la même. Je pourrais prendre ma décision en fonction des critères suivants :

* < $50: just do it
* $50-$300: get the work done but whine to my friends later
* $300-$5000: get another opinion; explore options; defer if possible
* $5000+: go car shopping

* < 50€ : pas besoin de tergiverser, je fais faire les travaux
* 50€ - 300€ : je fais faire les travaux, mais je parlerai de cette mésaventure à mes amis
* 300€ - 5 000€ : je vais solliciter un autre avis ; chercher des alternatives ; retarder les travaux si possible
* 5 000€ + : je vais m’acheter une nouvelle voiture

Life often demands some level of estimation, but don’t ignore delivery or value to focus too much on cost alone.

Dans la vie, il est souvent nécessaire d’avoir un certain degré d’estimation, mais il faut également ne pas ignorer ce qui doit être livré ou sa valeur pour ne pas trop se focaliser uniquement sur le coût.

We’ll go through facts and factors affecting estimates; at the end I’ll argue for as light an estimation approach as possible.

Dans cet article, nous aborderons les faits et les facteurs ayant un impact sur les estimations ; à la fin, je vous donnerai mes arguments en faveur d’une approche aussi légère que possible concernant les estimations

## Face Reality: An Estimate is a Guess

## Voir la réalité en face : une estimation est une supposition

If a story were already completed, the cost, time taken, etc. would be (could be?) known quantities.

Si une story était déjà terminée, son coût, sa durée, etc. seraient (pourraient être) des éléments connues.

We’d really like to know those values in advance, to help us in planning, staffing, etc.

Nous aimerions vraiment connaître ces éléments à l’avance pour nous aider à planifier, recruter, etc.

Since we can’t know, we mix analysis and intuition to create a guess, which could be a single number, a range, or a probability distribution. (It doesn’t matter whether it’s points or days, Fibonacci or t-shirt sizes, etc.)

Étant donné que nous ne les connaissons pas, nous mélangeons analyse et intuition pour faire une supposition, qui peut être un simple nombre, un intervalle, ou une distribution probabiliste. (Il n’est pas important que ce soit des points, des jours, un chiffre ou un nombre issu de la suite de Fibonacci, ou une taille de t-shirt, etc.)

When we decide how accurate our estimates must be, we’re making an economic tradeoff since it costs more to create estimates with tighter error bounds.

Quand nous décidons du degré de précision auquel nos estimations doivent être, nous faisons un compromis économique car cela coûte plus cher de faire des estimations avec des marges d’erreur plus réduites.

## How Are Estimates Made?

## Comment sont faites les estimations ?

There are several approaches, often used in combination:

Il existe plusieurs approches, souvent combinées entre elles :

* **Expert Opinion AKA Gut Feel AKA [SWAG](http://en.wikipedia.org/wiki/Scientific_Wild-Ass_Guess)**: Ask someone to make a judgment, taking into account everything they know and believe. Every estimation method boils down to this at some point.

* **L’avis d’expert _alias_ le ressenti personnel _alias_ [SWAG](http://en.wikipedia.org/wiki/Scientific_Wild-Ass_Guess)[^1]** : Demander à quelqu’un d’émettre un jugement, en prenant en compte tout ce qu’il sait et tout ce qu’il croit. À un moment ou un autre, n’importe quelle méthode d’estimation passe par là.

* **Analogy**: Estimate based on something with similar characteristics. (“Last time, a new report took 2 days; this one has similar complexity, so let’s say 2 days.”)

* **Analogie** : Estimation basée sur quelque chose ayant des caractéristiques similaires. (“La dernière fois, il nous a fallut deux jours pour faire un nouveau rapport ; celui-ci est d’un niveau de complexité similaire, disons 2 jours pour lui alors.”)

* **Decomposition AKA Divide and Conquer AKA Disaggregation**: Break the item into smaller parts, and estimate the cost of each part — plus the oft-forgotten cost of re-combining the parts.

* **Décomposition _alias_ Diviser et conquérir _alias_ Désaggréation** : Scindez l’item en plus petites parties, et estimez le coût de chacune de ces parties - ajoutez-y le coût régulièrement oublié de la recomposition des parties.

* **Formula**: Apply a formula to some attributes of the problem, solution, or situation. (Examples: Function Points, COCOMO.)

* **Formule** : Elle consiste en l’application d’une formule à certains éléments du problème, de la solution ou du contexte. (Exemples : points de fonction, COCOMO[^2]

    Challenges:
  * formulas’ parameters require tuning based on historical data (which may not exist)
  * formulas require judgment about which formulas apply
  * formulas tend to presume the problem or solution is well-enough understood to assess the concrete parts

    Défis à surmonter lors de l’utilisation de formules :
  * certains éléments des paramètres des formules devront être affinés en fonction des données historiques (qui peuvent ne pas exister).
  * il sera nécessaire de faire preuve de jugeotte lorsqu’il s’agira de choisir d’utiliser telle ou telle formule
  * le fait que les formules aient tendance à présupposer le problème ou la solution de telle ou telle manière est un phénomène suffisamment bien connu pour que les différentes éléments de la formule soient contrôlés.

* **Work Sample**: Implement a subset of the system, and base estimates on that experience. Iterative and incremental approaches provide this ongoing opportunity.

* **Échantillon** : Implémentez une sous-partie du système, et basez vos estimations sur cette expérience. Les approches itératives et incrémentales se révèlent tout à fait adaptées.

* **Buffer AKA Fudge Factor**: Multiply (and/or add to) an estimate to account for unknowns, excessive optimism, forgotten work, overheads, or intangible factors. For example: “Add 20%”, “Multiply by 3”, or “Add 2 extra months at the end”.

* **Tampon _alias_ facteur arbitraire** : Multipliez (et/ou ajouter) une estimation à un facteur arbitraire pour prendre en compte l’inconnu, l’optimisme excessif, un travail oublié ou tout autre élément intangible. Par exemple : “Ajouter 20%”, “Multipliez par 3”, ou “Ajouter 2 mois supplémentaire à la fin”.

## Why Is It Hard to Estimate?

## Pourquoi est-ce difficile d’estimer ?

Stories are difficult to estimate because of the unknowns. After all, the whole process is an attempt to derive a “known” (cost, time, …) from something unknowable (“exactly what will the future bring?”).

Les stories sont difficiles à estimer à cause de ce qui est inconnu. Après tout, l’ensemble du processus d’estimation est une tentative d’aller vers quelque chose de connu (coût, durée, …) à partir de quelque chose d’inconnu (“de manière littérale, qu’est ce le futur va nous apporter”).

Software development has so many unknowns:

Le développement logiciel recèle de nombreuses inconnues.

* **The Domain**: When we don’t know the domain, it’s easier to have misunderstandings with our customer, and it can be harder to have deep insights into better solutions.

* **Le domaine** : Quand nous ne connaissons pas le domaine, les occasions d’incompréhensions avec notre client sont plus nombreuses, et il est plus difficile d’avoir une bonne vision des solutions les plus adaptées.

* **Level of Innovation**: We may be operating in a domain where we need to do things we have never done before; perhaps nobody has.

* **Niveau d’innovation** : Il se peut que nous soyons dans un domaine où nous devrons travailler sur des choses que nous n’avons jamais vues ; ou sur lesquelles personne n’a jamais travaillé.

* **The Details of a Story**: We often want to estimate a story before it is fully understood; we may have to predict the effects of complicated business rules and constraints that aren’t yet articulated or even anticipated.

* **Les détails de la story** : Nous voulons souvent estimer une story avant que nous soyons en mesure de la comprendre tout à fait ; nous pouvons avoir à prédire les effets de règles métiers et de contraintes compliquées qui ne sont ni complètement articulées ni même anticipées.

* **The Relationship to Other Stories**: Some stories can be easier or harder depending on the other stories that will be implemented.

* **La relation avec d’autres stories** : Certaines stories peuvent être plus faciles ou plus difficiles à estimer en fonction des autres stories qui seront implémentées.

* **The Team**: Even if we have the same people as the last project, and the team stays stable throughout the project, people change over time. It’s even harder with a new team.

* **L’équipe** : Même si nous disposons des mêmes personnes que lors du précédent projet, et que l’équipe reste stable tout au long du projet, les gens changent avec le temps. C’est encore plus dur avec une équipe nouvelle.

* **Technology**: We may know some of the technology we’ll use in a large project, but it’s rare to know it all up-front. Thus our estimates have to account for learning time.

* **Technologie** : Peut être connaissons-nous la technologie que nous serons amené à utiliser pour le prochain projet, mais il est rare de tout savoir à l’avance. Par conséquent, nous estimations devront prendre en compte ce temps d’apprentissage.

* **The Approach to the Solution**: We may not yet know how we intend to solve the problem.

* **L’approche de la solution** : Il se peut que nous ne sachions même pas comment nous allons aborder le problème.

* **The Relationship to Existing Code**: We may not know whether we’ll be working in a habitable section of the existing solution.

* **La relation avec le code existant** : Il se peut que nous ne sachions pas si nous allons travailler sur une partie habitable du code existant.

* **The Rate of Change**: We may need to estimate not just “What is the story now?” but also “What will it be by the end?”

* **Le taux de changement** : Il se peut que nous ayons à estimer non seulement le “Quelle est la story maintenant ?” mais aussi “Comment sera-t-elle à la fin ?”

* **Dysfunctional Games**: In some environments, estimates are valued mostly as a tool for political power-plays; objective estimates may have little use. (There’s plenty to say about estimates vs. commitments, schedule chicken, and many other abuses but I’ll save that for another time.)

* **Jeux dysfonctionnels** : Dans certains environnements, les estimations sont perçues essentiellement comme des outils dans des jeux de pouvoirs politiques ; dans ce cas, les estimations objectives ne sont que de peu d’utilité; (Il y aurait beaucoup à dire sur estimations vs. engagements, le planning de la poule mouillée, et encore beaucoup d’autres choses dont je parlerai une autre fois.)

* **Overhead**: External factors affect estimates. If we multi-task or get pulled off to side projects, things will take longer.

* **Débordé** : Les facteurs externes impactent les estimations. Si nous travaillons sur plusieurs choses simultanément ou si nous sommes mis sur des projets annexes, les choses prendront plus de temps.

Sitting in a planning meeting for a day or a week and ginning up a feeling of commitment won’t overcome these challenges.

S’assoir à une réunion de planification pendant une journée ou une semaine et se faire extorquer un sentiment d’engagement ne permettront pas de surmonter aucun des défis mentionnés ci-dessus.

## Flaws In Estimating

## Des failles dans l’estimation // des biais

We tend to speak as if estimates are concrete and passive: “Given this story, what is the estimate?”

Nous avons tendance à parler comme si les estimations étaient concrètes et à la voix passive : “Étant donné que … cette story, quelle est l’estimation ?”

But it’s not that simple:

Mais ce n’est pas si simple :

* “[N for Negotiable](http://xp123.com/articles/negotiable-stories-in-the-invest-model/)” suggests that flexibility in stories is beneficial: flexible stories help us find bargains with the most value for their cost. But the more variation you allow, the harder it is to estimate.

* Dans le modèle INVEST, le [N pour négociable](http://www.les-traducteurs-agiles.org/2017/03/12/le-modele-invest-les-stories-negociables.html) suggère que la flexibilité des stories est bénéfique : des stories flexibles nous aident à trouver des marges de négociation nous permettant de tirer un maximum valeur par rapport au coût. Mais plus vous vous autorisé de variation, plus la storie sera difficile à estimer.

* “[I for Independent](http://xp123.com/articles/independent-stories-in-the-invest-model/)” suggests that we create stories that can be independently estimated and implemented. While this is mostly true, it is a simplification of reality: sometimes the cost of a story depends on the order of implementation or on what else is implemented. It may be hard to capture that in estimates.

* Le [I pour indépendante](http://www.les-traducteurs-agiles.org/2017/02/21/le-modele-invest-les-stories-independantes.html) suggère que nous créons des stories qui peuvent être estimées et implémentées indépendamment. Bien que cela s’avère exactdans la plupart des cas, c’est une simplification de la réalité : quelque fois le coût d’une story dépend de l’ordre de l’implémentation ou ce sur la chose implémentée. Cela peut être difficile à cerner dans les estimations. 

* Factors that make it hard to estimate are **not stable over time**. So even if you’re able to take all those factors into account, you also have to account for their instability.

* Les facteurs qui rendent les estimations difficiles à réaliser ne sont **pas toujours stables dans le temps**. Même si vous êtes capables de prendre tous ces facteurs en compte, vous devez aussi prendre en compte leur instabilité.

Is estimating hopeless? If you think estimation is a simple process that will yield an exact (and correct!) number, then you are on a futile quest. If you just need enough information from estimates to guide decisions, you can usually get that.

Faire des estimations est-il sans espoir ? Si vous pensez que l’estimation est un processus simple qui amène à un nombre exact (et correct !), alors votre quête s’avère futile. Si vous avez seulement besoin d’assez d’informations de la part des estimations pour guider vos décisions, vous aurez généralement ce dont nous avons discuté précédemment.

Some projects need detailed estimates, and are willing to spend what it takes to get them. In general, though, Tom DeMarco has it right: “Strict control is something that matters a lot on relatively useless projects and much less on useful projects.”

Certains projets ont besoin d’estimations détaillées, et sont prêt à prendre le temps nécessaire pour les avoir. En général, toutefois, Tom DeMarco nous dit que : “Un contrôle strict est quelque chose qui compte énormément pour des projets relativement futiles et beaucoup moins sur les projets utiles.”

Where does that leave things? The best way is to use as light an estimation process as you can tolerate.

Où est-ce que cela nous mène ? La meilleure solution est d’utiliser un processus d’estimation tellement léger que vous pourrez le tolérer. 

We’ll explore three approaches: counting stories, historical estimates, and rough order of magnitude estimates.

Nous explorerons trois approches : compter les stories, les estimations basées sur des données historiques, et les estimations basées sur un ordre de grandeur approximatif

## Simple Estimates: Count the Stories

## Estimations simples : compter les stories

More than ten years ago, Don Wells proposed a very simple approach: “Just count the stories.”

Il y a plus de dix maintenant, Don Wells a proposé une approche très simple : “Simplement compter les stories”

Here’s a thought experiment:

Voici un petite expérience :

* Take a bunch of numbers representing the true sizes of stories

* Prenez quelques nombres représentant la tailles réelle des stories

* Take a random sample

* Prenez un échantillon de stories au hasard

* The average of the sample is an approximation of the average of the original set, so use that average as the estimate of the size of every story (“Call it a 1”)

* La moyenne de l’échantillon est une approximation de la moyenne de l’ensemble pris à l’origine, utilisez alors cette moyenne comme estimation pour chaque story (“appelez la un 1”)

* The estimate for the total is the number of stories times the sample average

* L’estimation au total sera le nombre de stories multiplié par la moyenne de l’échantillon

What could make this not work?

Pourquoi est-ce que cela ne pourrait pas marcher ?

* If stories are highly inter-dependent, and the order they’re done in makes a dramatic difference to their size, the first step is void since there’s no such thing as the “true” size.

* Si les stories sont très interdépendantes, et que l’ordre dans lequel elles sont réalisées fait une réelle différence par rapport à leur taille, la première étape est alors vide de sens car la taille “réelle” n’existera pas.

* If you cherry-pick easy or hard stories rather than a random set, you will bias the estimate.

* Si vous choisissez des stories faciles ou difficiles au lieu de le faire aléatoirement, vous allez biaiser l’estimation

* If your ability to make progress shifts over time, the estimates will diverge. (Agile teams try to reduce that risk with refactoring, testing, and simple design.)

* Si votre capacité à avancer fluctue avec le temps, les estimations divergerons. (Les équipes agiles essayent de réduire ce risque avec du _refactoring_, des test, et une conception simple.)

I’ve seen several teams use a simple approach: they figure out a line between “small enough to understand and implement” and “too big”, then require that stories accepted for implementation be in the former range.

J’ai vu plusieurs équipes utiliser une approche simple : elles ont pu déterminer une ligne entre des stories “suffisamment petites à comprendre et à implémenter” et “trop grosses”, ont exigé par la suite que les stories acceptées en vue d’une prochaine implémentation soient de la 1ère catégorie.

## Historical Estimates (ala Kanban)

## Estimations basées sur des données historiques (à la Kanban)

For many teams, the size of stories is not the driving factor in how long a story takes to deliver. Rather, work-in-progress (WIP) is the challenge: a new story has to wait in line behind a lot of existing work.

Pour beaucoup d’équipes, la taille des stories n’est pas le facteur essentiel pour déterminer la durée de réalisation d’une story. Le travail en cours (TEC) est le principal défi : une nouvelle story doit attendre derrière tout un tas de travail déjà présent.

A good measure is total lead time (also known as cycle time or various other names): how long from order to delivery. Kanban approaches often use this measure, but other methods can too.

Un bon indicateur est la durée totale de traversée (connu aussi sous le nom de temps de cycle ou aussi sous d’autres noms) : quelle durée de la commande à la livraison. Les approches Kanban utilisent souvent cette mesure, mais d’autres méthodes peuvent le faire aussi.

If we track history, we can measure the cycle times and look for patterns. If we see that the average story takes 10 days to deliver and that 95% of the stories take 22 or fewer days to deliver, we get a fairly good picture of the time to deliver the next story.

Si nous enregistrons les données au fur et à mesure, nous pouvons mesurer les temps de cycle et rechercher des modèles statistiques. Si nous voyons qu’une story prend en moyenne 10 jours à être livrée et que 95% des stories prennent 22 jours ou moins à être livrées, nous aurons une image plutôt fidèle de la durée à livrer pour la prochaine story.

This moves the estimation question from “How big is this?” to “How soon can I get it?”

Cela change la question de l’estimation de “Quelle est sa taille ?” à “Quand est-ce que je pourrais l’avoir ?”

When WIP is high, it is the dominant factor in delivery performance; as WIP approaches 0, the size of the individual item becomes significant.

Lorsque le TEC est haut, c’est le facteur dominant dans la performance de la livraison ; lorsque le TEC approche de 0, la taille d’un item à titre individuel devient alors significatif.

## Rough Order of Magnitude

## Un ordre de grandeur approximatif

A rough order of magnitude estimate just tries to guess the time unit: hours, days, weeks, months, years.

L’estimation sur un ordre de grandeur approximatif essayent seulement de deviner l’unité de temps : heures, jours, semaines, mois, années.

You might use such estimates like this:

Nous pourrions utiliser ce type d’estimations de la manière suivante :

* Explore risk, value, and options

* Explorer le risque, la valeur et les alternatives

* Make rough order of magnitude estimates

* Faire des estimations sur un ordre de grandeur approximatif

* Focus first on what it takes to create a minimal but useful version of the most important stories

* Se focaliser d’abord sur ce qu’il faut pour créer une version minimale mais utile des stories les plus importantes

* From there, decide how and how far to carry forward by negotiating to balance competing interests

* À partir de là, décider comment et jusqu’à quel point aller en négociant pour équilibrer les intérêts divergents

* Be open to learning along the way

* Être ouvert pour apprendre tout le long

## Conclusion

## Conclusion

Stories are estimable when we can make a good-enough prediction of time, cost, or other attributes we care about.

Les stories sont estimables lorsque nous pouvons faire une prédiction suffisamment fiable de la durée, du coût ou de tout autre attribut qui nous semble important. 

We looked at approaches to estimation and key factors that influence estimates.

Nous avons examiné différentes approches des estimations et les éléments clés qui influencent les estimations.

Estimation does not have to be a heavy-weight and painful process. Try the lighter ways to work with estimates: counting stories, historical estimates, and/or rough order of magnitude estimates.

Il n’est pas obligatoire que le processus d’estimation soit lourd et pénible. Essayez donc des manières de faire des estimations plus légères : comptage de stories, estimations basées sur des données historiques, et ou des estimations selon un ordre de grandeur approximatif.

Whatever approach you take, spend as little as you can to get good-enough estimates.

Quelque soit l’approche que vous choisirez, prenez juste ce qu’il faut de temps pour avoir des estimations suffisamment bonnes.

[^1]: NdT - estimatable - néologisme inventé par l’auteur - traduit par estimabilité - autre néologisme

[^2]: NdT - SWAG ou Scientific wild-ass guess, terme venant des États-Unis en langage familier indiquant un avis approximatif donné par un expert d’un domaine particulier

[^3]: NdT - COCOMO ou COnstructive COst MOdel est une méthode d’estimation conçu par Barry Boehm. Pour en savoir, consultez cet [article](https://fr.wikipedia.org/wiki/Constructive_Cost_Model) sur Wikipedia.

---
Auteur : [Bill Wake](http://xp123.com/about/)  
Source : [Estimable Stories in the INVEST Model](http://xp123.com/articles/estimable-stories-in-the-invest-model/)  
Date de parution originale : 01 Mars 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 08/08/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



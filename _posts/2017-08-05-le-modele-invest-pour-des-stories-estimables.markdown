---
layout: post
title:  "Le modèle INVEST - E comme stories Estimables"
date:   2017-08-08 00:00:01
published: true
tags: 
- user stories
---

Des stories **estimables** peuvent être estimées : qu’il s’agisse de la taille, du coût ou de la durée de réalisation (Nous aurions pu vouloir utiliser le terme _estimatibilité_ [^1] , mais il n’existe pas dans mon dictionnaire, et je ne suis pas assez fan des estimations pour l’inventer.)

Pour qu’elles soient estimables, les stories doivent être suffisamment comprises, suffisamment stables pour que nos suppositions puissent rester dans des limites raisonnables. 

_Message d’avertissement : l’estimabilité est l’aspect le plus mal compris du modèle INVEST (c’est-à-dire celui ayant le rapport énergie dépensée / valeur le moins intéressant). Si je devais choisir à nouveau une signification à lettre E d’INVEST, nous aurions “E = Externe” ; pour plus d’informations voir [V pour des stories ayant de la Valeur](http://www.les-traducteurs-agiles.org/2017/04/25/le-modele-invest-pour-des-stories-de-valeur.html)._

## Pourquoi nous aimons les estimations

Pourquoi voulons-nous faire des estimations ? Généralement, nous voulons faire des estimations dans un but de planification, pour nous donner une idée du coût et/ou du temps nécessaire pour faire un quelconque travail. Les estimations nous aident à prendre des décisions coût vs. valeur.

Lorsque qu’il y a des travaux à faire sur ma voiture, je veux savoir si cela va me coûter 15€ ou 10 000€, parce que selon le coût, ma décision ne sera pas la même. Je pourrais prendre ma décision en fonction des critères suivants :

* < 50€ : pas besoin de tergiverser, je fais faire les travaux
* 50€ - 300€ : je fais faire les travaux, mais je parlerai de cette mésaventure à mes amis
* 300€ - 5 000€ : je vais solliciter un autre avis ; chercher des alternatives ; retarder les travaux si possible
* 5 000€ + : je vais m’acheter une nouvelle voiture

Dans la vie, il est souvent nécessaire de faire un certain niveau d’estimation, mais il faut également ne pas ignorer ce qui doit être livré ou sa valeur afin de ne pas trop se focaliser uniquement sur le coût.

Dans cet article, nous aborderons les faits et les facteurs ayant un impact sur les estimations ; à la fin, je vous donnerai mes arguments en faveur d’une approche aussi légère que possible concernant les estimations

## Voir la réalité en face : une estimation est une supposition

Si une story était déjà terminée, son coût, sa durée, etc. seraient (pourraient être) des éléments déjà connus.

Nous aimerions donc vraiment connaître ces éléments à l’avance pour nous aider à planifier, recruter, etc.

Étant donné que nous ne les connaissons pas, nous mélangeons analyse et intuition pour faire une supposition, qui peut être un simple nombre, un intervalle, ou une distribution probabiliste. (Il n’est pas important que ce soit des points, des jours, un chiffre ou un nombre issu de la suite de Fibonacci, ou une taille de t-shirt, etc.)

Quand nous décidons du degré de précision souhaité pour nos estimations, nous faisons un arbitrage économique car plus nous voulons faire des estimations avec des marges d’erreur réduites plus cela coûte cher.

## Comment sont faites les estimations ?

Il existe plusieurs approches, qui sont souvent combinées entre elles :

* **L’avis d’expert _alias_ le ressenti personnel _alias_ SWAG[^2]** : Demander à quelqu’un d’émettre un jugement, en prenant en compte tout ce qu’il sait et tout ce qu’il croit. À un moment ou un autre, n’importe quelle méthode d’estimation passera par là.

* **Par analogie** : Estimation basée sur quelque chose ayant des caractéristiques similaires. (“La dernière fois, il nous a fallut deux jours pour faire un nouveau rapport ; celui-ci est d’un niveau de complexité similaire, disons 2 jours pour lui alors.”)

* **Par décomposition _alias_ Diviser et conquérir _alias_ Désaggréation** : Scindez l’item en plus petites parties, et estimez le coût de chacune de ces parties - ajoutez-y le coût de la recomposition des parties qui est régulièrement oublié.

* **Par utilisation d’une formule** : Elle consiste en l’application d’une formule à certains éléments du problème, de la solution ou du contexte. (Exemples : points de fonction, COCOMO[^3]

    L’utilisation de formules impliquent quelques défis supplémentaires à surmonter:
  * certains paramètres des formules devront être affinés en fonction des données historiques (qui peuvent peut être ne pas exister).
  * il sera nécessaire de faire preuve de jugeotte lorsqu’il s’agira de choisir d’utiliser telle ou telle formule
  * le fait que les formules aient tendance à présupposer le problème ou la solution de telle ou telle manière est un phénomène suffisamment bien connu pour que les différentes éléments de la formule fassent l’objet d’un contrôle.

* **Par l’utilisation d’un échantillon** : Implémentez une sous-partie du système, et basez vos estimations sur cette expérience d’implémentation. Les approches itératives et incrémentales se révèlent tout à fait adaptées.

* **Avec un tampon _alias_ facteur arbitraire** : Multipliez (et/ou ajouter) une estimation à un facteur arbitraire pour prendre en compte l’inconnu, l’optimisme excessif, un travail oublié ou tout autre élément intangible. Par exemple : “Ajouter 20%”, “Multipliez par 3”, ou “Ajouter 2 mois supplémentaire à la fin”.

## Pourquoi est-ce difficile d’estimer ?

Les stories sont difficiles à estimer à cause de ce qui est inconnu. Après tout, l’ensemble du processus d’estimation est bien une tentative d’aller vers quelque chose de connu (coût, durée, …) à partir de quelque chose d’inconnu (“de manière littérale, qu’est ce le futur va nous apporter”).

Le développement logiciel recèle de nombreuses inconnues.

* **Le domaine** : Quand nous ne connaissons pas le domaine, les occasions d’incompréhensions avec notre client sont plus nombreuses, et il est plus difficile d’avoir une bonne vision des solutions qui seraient les plus adaptées.

* **Le niveau d’innovation** : Il se peut que nous soyons dans un domaine où nous devrons travailler sur des choses que nous n’avons jamais vues ; ou sur lesquelles personne n’a encore jamais travaillé.

* **Les détails de la story** : Nous voulons souvent estimer une story avant que nous soyons en mesure de la comprendre tout à fait ; nous pouvons avoir à prédire les effets de règles métiers et de contraintes compliquées qui ne sont ni complètement articulées ni même anticipées.

* **La relation avec d’autres stories** : Certaines stories peuvent être plus faciles ou plus difficiles à estimer en fonction des autres stories qui seront implémentées.

* **L’équipe** : Même si nous disposons des mêmes personnes que lors du précédent projet, et que l’équipe reste stable tout au long du projet, les gens changent avec le temps. C’est d’autant plus dur avec une équipe nouvelle.

* **La technologie** : Peut être connaissons-nous la technologie que nous serons amené à utiliser pour le prochain projet, mais il est rare de tout savoir à l’avance. Par conséquent, nous estimations devront prendre en compte ce temps d’apprentissage.

* **L’approche de la solution** : Il se peut que nous ne sachions même pas comment nous allons solutionner le problème.

* **La relation avec le code existant** : Il se peut que nous ne sachions pas si nous allons travailler sur une partie habitable du code existant.

* **Le taux de changement** : Il se peut que nous ayons à estimer non seulement le “Quelle est la story maintenant ?” mais aussi “Comment sera-t-elle à la fin ?”

* **Les jeux dysfonctionnels** : Dans certains environnements, les estimations sont perçues essentiellement comme des outils dans des jeux de pouvoirs politiques ; dans ce cas, les estimations objectives ne sont que de peu d’utilité. (Il y aurait beaucoup à dire sur estimations vs. engagements, le planning de la poule mouillée, et encore beaucoup d’autres choses dont je parlerai une autre fois.)

* **Débordé** : Les facteurs externes impactent les estimations. Si nous travaillons sur plusieurs choses simultanément ou si nous sommes mis sur des projets annexes, les choses prendront plus de temps.

S’asseoir à une réunion de planification pendant une journée ou une semaine et se faire extorquer un sentiment d’engagement ne permettront pas de surmonter aucun des défis mentionnés ci-dessus.

## Estimations biaisées

Nous avons tendance à parler comme si les estimations étaient concrètes et passive : “Étant donné que … cette story, quelle est l’estimation ?”

Mais ce n’est pas si simple :

* Dans le modèle INVEST, le [N pour négociable](http://www.les-traducteurs-agiles.org/2017/03/12/le-modele-invest-les-stories-negociables.html) suggère que la flexibilité des stories est bénéfique : des stories flexibles nous aident à trouver des marges de négociation nous permettant de tirer un maximum valeur par rapport au coût. Mais plus vous vous autorisez de variation, plus la storie sera difficile à estimer.

* Le [I pour indépendante](http://www.les-traducteurs-agiles.org/2017/02/21/le-modele-invest-les-stories-independantes.html) suggère que nous créons des stories qui peuvent être estimées et implémentées indépendamment. Bien que cela s’avère exact dans la plupart des cas, c’est une simplification de la réalité : quelque fois le coût d’une story dépend de l’ordre de l’implémentation ou sur la chose implémentée. Cela peut être difficile à cerner dans les estimations. 

* Les facteurs qui rendent les estimations difficiles à réaliser ne sont **pas toujours stables dans le temps**. Même si vous êtes capables de prendre tous ces facteurs en compte, vous devez aussi prendre en compte leur instabilité.

Faire des estimations est-il sans espoir ? Si vous pensez que l’estimation est un processus simple qui amène à un nombre exact (et correct !), alors votre quête s’avère futile. Si vous avez seulement besoin d’assez d’informations de la part des estimations pour guider vos décisions, vous obtiendrez généralement ce dont nous avons discuté jusqu’à présent.

Certains projets ont besoin d’estimations détaillées, et sont prêt à prendre le temps nécessaire pour les avoir. En général, toutefois, Tom DeMarco nous dit que : “Un contrôle strict est quelque chose qui compte beaucoup pour des projets relativement futiles et beaucoup moins sur des projets utiles.”

Où est-ce que cela nous mène ? La meilleure solution est d’utiliser un processus d’estimation tellement léger que vous serez en mesure de le tolérer. 

Nous explorerons trois approches : le comptage de stories, les estimations basées sur des données historiques, et les estimations basées sur un ordre de grandeur approximatif

## Estimations simples : le comptage de stories

Il y a plus de dix maintenant, Don Wells a proposé une approche très simple : “Simplement compter les stories”

Voici un petite expérience :

* Prenez quelques nombres représentant la tailles réelle de stories

* Prenez un échantillon de stories au hasard

* La moyenne de l’échantillon est une approximation de la moyenne de l’ensemble pris à l’origine, utilisez alors cette moyenne comme estimation de base pour chaque story (“appelez la un 1”)

* L’estimation au total sera le nombre de stories multiplié par la moyenne de l’échantillon

Pourquoi est-ce que cela ne pourrait pas marcher ?

* Si les stories sont très interdépendantes, et que l’ordre dans lequel elles sont réalisées fait une réelle différence par rapport à leur taille, la première étape est alors vide de sens car la taille “réelle” n’existe pas.

* Si vous choisissez des stories faciles ou difficiles au lieu de le faire aléatoirement, vous allez biaiser l’estimation

* Si votre capacité à avancer fluctue avec le temps, les estimations divergerons. (Les équipes agiles essayent de réduire ce risque avec du _refactoring_, des test, et une conception simple.)

J’ai vu plusieurs équipes utiliser une approche simple : elles ont pu déterminer une ligne entre des stories “suffisamment petites à comprendre et à implémenter” et “trop grosses”, ont exigé par la suite que les stories acceptées en vue d’une prochaine implémentation soient de la 1ère catégorie.

## Estimations basées sur des données historiques (à la Kanban[^4])

Pour beaucoup d’équipes, la taille des stories n’est pas le facteur essentiel pour déterminer la durée de réalisation d’une story. Le travail en cours (TEC) est le principal défi : une nouvelle story doit attendre derrière tout un tas de travail déjà présent.

Un bon indicateur est la durée totale de traversée (connu aussi sous le nom de temps de cycle ou aussi sous d’autres noms) : quelle durée de la commande à la livraison. Les approches Kanban utilisent souvent cette mesure, mais d’autres méthodes peuvent le faire aussi.

Si nous faisons un suivi, nous pouvons mesurer les temps de cycle et rechercher des modèles statistiques. Si nous voyons qu’une story prend en moyenne 10 jours à être livrée et que 95% des stories prennent 22 jours ou moins à être livrées, nous aurons une image plutôt fidèle de la durée à livrer pour la prochaine story.

Cela change la question de l’estimation de “De quelle taille est une story ?” à “À partir de quand pourrais-je en disposer ?”

Lorsque le TEC est haut, c’est le facteur dominant dans la performance de la livraison ; lorsque le TEC approche de 0, la taille d’un item à titre individuel devient alors significatif.

## Un ordre de grandeur approximatif

L’estimation sur un ordre de grandeur approximatif essayent seulement de deviner l’unité de temps : heures, jours, semaines, mois, années.

Nous pourrions utiliser ce type d’estimations de la manière suivante :

* Explorer le risque, la valeur et les alternatives

* Faire des estimations sur un ordre de grandeur approximatif

* Se focaliser d’abord sur ce qu’il faut pour créer une version minimale mais utile des stories les plus importantes

* À partir de là, décider comment et jusqu’à quel point aller en négociant pour équilibrer les différents intérêts divergents

* Être ouvert pour apprendre tout le long

## Conclusion

Les stories sont estimables lorsque nous pouvons faire une prédiction suffisamment fiable de la durée, du coût ou de tout autre attribut qui nous semble important. 

Nous avons examiné différentes approches des estimations et les éléments clés qui influencent les estimations.

Il n’est pas obligatoire que le processus d’estimation soit lourd et pénible. Essayez donc des manières de faire des estimations plus légères : comptage de stories, estimations basées sur des données historiques, et ou des estimations selon un ordre de grandeur approximatif.

Quelque soit l’approche que vous choisirez, prenez juste ce qu’il faut de temps et pas plus, pour avoir des estimations juste suffisantes.

[^1]: NdT - estimatable - néologisme inventé par l’auteur - traduit par estimatibilité - autre néologisme ce coup-ci inventé par le traducteur

[^2]: NdT - SWAG ou Scientific wild-ass guess, terme venant des États-Unis en langage familier indiquant un avis approximatif donné par un expert d’un domaine particulier

[^3]: NdT - COCOMO ou COnstructive COst MOdel est une méthode d’estimation conçu par Barry Boehm. Pour en savoir, consultez cet [article](https://fr.wikipedia.org/wiki/Constructive_Cost_Model) sur Wikipedia.

[^4]: NdT - presque en français dans le texte original

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



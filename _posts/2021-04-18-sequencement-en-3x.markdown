---
layout: post
title:  "Le séquencement en 3X"
date:   2021-04-26 10:03
published: true
tags:
- 3X
---

![Les séquencements]({{ site.url }}assets/kent_beck/3X-sequencing.png)

Cet article fait partie de la série [3X - Quelques sujets de comparaison entre Exploration, Expansion et Extraction](http://www.les-traducteurs-agiles.org/2021/04/18/3x-quelques-sujets-de-comparaison-entre-exploration-expansion-et-extraction.html).

Mort, impôts et séquencement[^1]. Vous allez faire quelque chose maintenant et tout le reste plus tard (même si le quelque chose que vous faites maintenant c'est rien). Comment décidez-vous ce que vous allez faire maintenant et ce que vous reportez à plus tard ?

Les estimations en terme de coûts et de bénéfices sont l'un des facteurs pouvant influencer le séquencement. Tel que cela est décrit dans les [estimations en 3X](http://www.les-traducteurs-agiles.org/2021/04/20/les-estimations-en-3x.html), l'utilité des estimations est variable selon les différentes phases. En l'absence d'estimations, comment faites-vous pour choisir ?

## Exploration

La mauvaise nouvelle c'est que durant l'exploration, nous n'avons pas les informations dont nous avons besoin pour pouvoir séquencer de manière optimale nos décisions. La bonne nouvelle c'est que ce séquencement n'a pas d'importance en soi. On ne sait pas quand se produit une réussite, la surprise est totale. Nous allons jeter les dés jusqu'à ce que nous obtenions un double six. Quoi de plus semblable qu’un jet de dés si ce n’est un autre jet de dés.

Nous devons nous poser une question cruciale lorsque nous sommes en phase d'exploration : quelle est la proportion d'effort devrions-nous consacrer en terme d'expérimentation et quelle est celle à consacrer pour rendre l'expérimentation moins cher. Autrement dit, en tournant cela sous la forme d'une question sur le séquencement : dois-je expérimenter sur autre chose ou dois-je optimiser l'expérimentation ?

Une bonne heuristique pour faire un choix et séquencer correctement est d'optimiser certains aspects de l'expérimentation lorsqu'elle devient fastidieuse. J'appelle cela le développement piloté par la frustration.

## Expansion

La mauvaise nouvelle à propos du séquencement en phase d'expansion c'est que si vous le ratez, vous échouerez. La marge d'erreur est très faible. Vous êtes en train d'essayer d'éliminer les goulots d'étranglements juste avant qu'ils ne ruinent votre produit.

La bonne nouvelle c'est que ces décisions de séquencement sont pour la plupart entre vos mains. Vous êtes en train d'essayer de faire fléchir la courbe de l'offre — en deçà de la limite haute à ne pas atteindre — et de faire fléchir la courbe de la demande afin qu'elles ne croisent pas dans un futur proche. Une fois que vous avez fait ça, vous faites face au prochain goulot d'étranglement. Et une fois qu'il n'y a plus de goulot d'étranglement à l'horizon, vous vous retrouvez en phase d'extraction où vous _pouvez_ enfin prendre des décisions de séquencement sur la base d'informations fiables.  

![Les séquencements]({{ site.url }}assets/kent_beck/3X-sequencing-2-fr.png)

_Expansion : un foutu goulot d'étranglement l'un après l'autre_

## Extraction

En extraction, vous avez des estimations fiables des coûts et des bénéfices. Vous triez les tâches à faire par zone d'intérêt[^2], en y ajoutant un peu d'aléatoire pour éviter un minimum local[^3] et vous prenez ce qui vient ensuite.

Une heuristique est de faire en sorte que les tâches restent de petites tailles. En phase d'extraction, vous avez beaucoup à perdre, donc il faut éviter de faire de gros changements. De petites tâches sont plus faciles à estimer, et il est plus facile d'en détecter une qui se passe mal.

## Conclusion

L'erreur en terme de séquencement est d'être obsédé par des décisions de séquencement qui ne valent rien ou qui ne peuvent pas être basées sur des données. Toute cette énergie serait bien mieux employée en expérimentant ou en améliorant l'expérimentation.

[^1]: La partie de la phrase « Mort, taxe » fait référence à une citation célèbre attribuée généralement à Benjamin Franklin. Pour en savoir plus, vous pouvez vous référer à cet [article](https://en.wikipedia.org/wiki/Death_and_taxes_(idiom)) sur Wikipedia. - NdT

[^2]: Une région d'intérêt (ou ROI en anglais, pour region of interest et non return on investment) est un sous-ensemble d'un jeu de données généralement d'une image. L'auteur l'applique ici aux graphiques évoqués plus haut - NdT

[^3]: Imaginez une courbe ayant des hauts et des bas. Le « bas » le plus petit sur l'ensemble de la courbe est dit « minimum global » et les autres de moindre importance sont dit « minimum local ». L'auteur applique cette notion aux graphiques évoqués plus haut - NdT

---
Auteur : [Kent Beck](https://medium.com/@kentbeck_7670/about)  
Source : [Sequencing in 3X](https://www.facebook.com/notes/kent-beck/sequencing-in-3x/1243615332337995)  
Date de parution originale : 201x  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Relecture : [Cidalia De Bastos](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 26/04/2021  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

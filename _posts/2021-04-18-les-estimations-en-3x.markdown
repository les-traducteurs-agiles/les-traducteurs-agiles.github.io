---
layout: post
title:  "Les estimations en 3X"
date:   2021-04-20 00:01
published: true
tags:
- 3X
---

![Les estimations]({{ site.url }}assets/kent_beck/3X-estimates.jpg)

Cet article fait partie de la série [3X - Quelques sujets de comparaison entre Exploration, Expansion et Extraction](http://www.les-traducteurs-agiles.org/2021/04/18/3x-quelques-sujets-de-comparaison-entre-exploration-expansion-et-extraction.html).

Si vous avez des ressources pour ainsi dire infinies, vous pouvez tout faire. Des ressources infinies éliminent le coût de l'opportunité. Dans notre univers, toutefois, les ressources sont en quantités finies. Tout ce que nous faisons implique la perte de quelque chose que nous ne ferons pas à la place.

Nos prises de décisions sont loin d'être toujours parfaites, les regrets nous poursuivent jusqu'à notre dernier souffle. Toutefois, nous pouvons faire mieux quelques fois en matière de prise de décision que de faire comme si nous jouions aux fléchettes. C'est là où les estimations rentrent en jeu.

Une estimation est un indicateur relatif à une ressource limitée qui sera utilisée dans un plan d'actions donné. Nous pourrions, par exemple, dans l'objectif de commercialiser un livre d'y passer deux mois de notre propre temps, ou de dépenser dix milles dollars, ou d'utiliser deux équivalents temps plein pendant un mois. Que la ressource finie soit du temps, du budget ou des personnes, nous souhaiterions savoir avant de commencer quelle quantité de cette ressource sera utilisée afin que nous puissions choisir en toute conscience notre plan d'actions.

Les estimations prennent en compte tout autant les bénéfices que les coûts. Les bénéfices estimés permettant de décider entre telle ou telle alternative. Les estimations des bénéfices tout autant que celles des coûts sont sujettes à une certaine volatilité, et restent aussi sujettes à une certaine forme de dépendance (A ou B pourrait ne pas être utile mais A & B ensemble sont formidables).

Les estimations se comportent différemment en exploration, expansion ou extraction. Ces différences, quelques fois contradictoires, expliquent en partie pourquoi les estimations en développement logiciel s'avèrent certaines fois difficiles .

## Exploration

Les estimations des bénéfices sont justes de l'autre côté de la fenêtre. L'essence même de l'exploration c'est que vous ne savez pas là où le succès va apparaître. Vous avez bien quelque intuition là dessus ou sinon vous ne seriez pas en train d'essayer une idée, mais certaines des idées les plus utiles sont celles qui ont été tentés par pure effronterie.  

Les estimations des coûts d'exploration sont davantage de l'ordre du défi que de la prédiction. « Je pense que je peux répondre à cette question pour X euros/heures/personnes», « Et si on faisait X/4 ? ». Cette économie relative au périmètre est ce qui rend l'exploration romantique. À la place de faire des estimations, utilisez plutôt des forfaits. « Une fois que nous aurons utilisé X euros/heures/personnes, nous considérerons ce point comme réglé et continuerons à avancer. »

You _can_ estimate in the large in exploration. Think of a startup selling equity for a round of funding. The amount of money may be based on some mythical “valuation”, but it’s really an estimate of how much exploration will cost times the probability of success times the value of success. You’d hate to run out of money/time/people just before succeeding, but you’d also hate to keep spending after failure is inevitable.

En exploration, vous _pouvez_ estimer dans les grandes lignes. Pensez à une _startup_ vendant des actions lors d'un tour de financement. Le montant financier peut être basé sur une « évaluation » quelque peu chimérique, mais il s'agit vraiment d'une estimation de combien l'exploration coûtera multipliée par la probabilité de succès multipliée par la la valeur du succès. Vous détesteriez être à court de budget/temps/personnes à un cheveu de réussir, mais vous détesteriez tout autant continuer à dépenser alors que l'échec s'avère inévitable.

## Expansion

In the expand phase you are seeing consistent growth. This makes it possible to estimate when you are going to run out of a resource, be it money, computers, or people. You can generally only see one bottleneck ahead. Whatever you’ve done to mitigate that bottleneck changes the location and form of the next bottleneck.

Dans la phase expansion vous chercher une croissance constante. C'est ce qui rend possible l'estimation lorsque vous allez être à court d'une ressource, que ce soit en terme budgétaire, de matériels informatiques, ou de personnes. Tout ce que vous pouvez voir généralement c'est le prochain goulot d'étranglement. Quoi que vous fassiez pour atténuer cela, ce goulot d'étranglement va changer d'endroit pour former le prochain goulot d'étranglement.

« Selon les projections, le 12 mai, nous n'aurons plus d'espace disque. », « Okay, faites ça, ça et ça pour avoir plus de disques et ça, ça et ça pour utiliser moins de disque. »  

Les estimations nous préviennent des problèmes en phase d'expansion. Si vous voyez certaines choses se dessiner que vous ne voulez pas qui se réalisent, comme des courbes dont vous ne voulez qu'elles se croisent, vous essayez de changer les choses, mais il se peut que les courbes s'obstinent à se croiser, alors il est temps d'invoquer le plan B.

Les estimations en terme de coût durant l'expansion ne sont généralement pas importantes. Souvenez-vous, vous avez tiré le ticket gagnant en phase d'exploration … à condition que vous soyez capable de chevaucher la fusée jusqu'en haut. Cela a du sens de cramer un peu de budget maintenant pour être sûr d'aller en orbite. (Par contre, cramer trop d'argent alors que la fusée s'écrase, c'est moins bon). Gardez donc un œil sur la totalité du budget disponible, mais ne vous souciez pas de chaque actions individuelles.

## Extraction

Les estimations deviennent utiles lors de la phase d'extraction. Vous avez désormais assez d'expérience en matière de coûts et de bénéfices pour être plus précis. Séquencer les tâches correctement créé de la valeur. Dans cette phase, vous voulez avant tout réaliser le meilleur retour sur investissement possible.

Les règles suivantes s'appliquent :

- Pratiquer et réfléchir sur ce que vous avez appris.
- Estimer des toutes petites choses, afin que les surprises restent toutes petites.
- Prêter attention lorsque les estimations deviennent bizarroïdes subitement . Vous êtes peut-être revenu en exploration.

## Conclusion

“Estimate Sometimes” lacks the sensible ring of “plan the work, work the plan” and fails as a rallying cry beside “No Estimates!”. However, that’s the whole point of 3X. Each phase requires its own approach. Estimates are just one example.

« Estimer parfois » s'écarte du point sensible « planifier le travail, exécuter le plan » et sans être pour autant le cri de ralliement de la bannière « No Estimates ! »[^1]. Toutefois, c'est tout l'intérêt de 3X. Chaque phase exige sa propre approche. Les estimations en sont justes un exemple.

[^1]: « No Estimates ! » est un courant dans le mouvement Agile pour lequel l'inutilité des estimations à priori sans élément de référence n'est plus à démontrer. Que si estimations il doit y avoir, elles doivent être sur la base de données historiques sur lesquelles s'appuyer. NdT

---
Auteur : [Kent Beck](https://medium.com/@kentbeck_7670/about)  
Source : [Estimates in 3X](https://www.facebook.com/notes/kent-beck/estimates-in-3x/1242012852498243)  
Date de parution originale : 201x  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)   
Date de traduction : 20/04/2021  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

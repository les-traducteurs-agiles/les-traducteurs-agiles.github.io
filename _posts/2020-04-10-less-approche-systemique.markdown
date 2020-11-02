---
layout: post
title:  "Less - Approche systémique"
date:   2020-11-01 00:00
published: true
tags:
- less
- à grande échelle
- approche systémique
---

# Approche systémique

> J'ai pris un cours de lecture rapide puis j'ai lu « Guerre et Paix » en vingt minutes. Cela parle de la Russie. —Woody Allen

« Quoi que nous fassions, le nombre d'anomalie dans notre _backlog_ reste identique. » nous a dit un jour un manager en évoquant un produit de près de 15 millions de lignes de code écrites en C et C++ et sur lequel plusieurs centaines de développeurs étaient en train de travailler. Que pouvait-il bien se passer ? L'approche systémique peut s'avérer utile dans ce cas comme dans d'autres. En petits groupes, les forces en présence peuvent rapidement être identifiées et comprises de manière informelle, mais dans le cadre du développement d'un gros produit ou de n'importe quel gros système, c'est difficile. Gerry Weinberg met en avant deux facteurs décisifs dans ce genre de situation :

> **Loi de Weinberg-Brooks** : De plus en plus de projets informatiques sont partis de travers après que le management ait pris des décisions basées sur des **modèles systémiques incorrects** plus que pour toutes autres combinaisons de causes.
>
> **Erreur de causalité** : Chaque effet a une cause … et nous pouvons dire desquelles il s'agit. [[Weinberg92]](http://www.amazon.fr/Quality-Software-Management-Systems-Thinking/dp/0932633226/ref=sr_1_1?ie=UTF8&qid=1413527418&sr=8-1&keywords=Quality+Software+Management%3A+Systems+Thinking)

Ces deux facteurs reflètent bien l'impact de nos **modèles mentaux** sur le système, un sujet que nous reverrons plus tard dans cette partie.

Les problèmes résultant de nos modèles mentaux et de nos postulats sont un point à traiter. Un autre point est l'adoption à grande échelle de Scrum, de l'approche lean et des principes agiles en dehors du domaine du développement. Ce point est aussi présent dans la gestion de produit, les budgets, les tests, la commercialisation, la gouvernance et la politique RH. En conséquence, dans les adoptions agiles à grande échelle, il est utile de se réunir avec des collègues et de _réfléchir en profondeur_ sur les modèles mentaux, les relations causales, les boucles de feedback et les mécanismes (ou les illusions) de contrôles dans un gros système qui va être sérieusement _pertubé_. L'approche systémique est l'un de ces outils de réflexion.

En 1958 la _Harvard Business Review_ a publié un article de Jay Forrestor, professeur au MIT Sloan School, qui a fait date [“Industrial Dynamics: A Major Breakthrough for Decision Makers,”](https://kupdf.com/download/industrial-dynamics-a-major-breakthrough-for-decision-makers_5902479bdc0d603940959ed5_pdf). Cet article a lancé le mouvement de l'approche systémique dans le domaine des formations en gestion d'entreprise et la MIT Sloan School of Management devint célèbre pour ses formations en **dynamique des systèmes**. Le terme de dynamique des systèmes est parfois utilisé comme synonyme de l'**approche systémique**, même si ce dernier est un terme beaucoup plus général.

Le MIT a également attiré d'autres chercheurs intéressés par la dynamique systémique tel que Peter Senge[^1].

En corrélation avec la loi de _Weinberg-Brook_, Jay Wright Forrester a montré que les décideurs à qui il avait été donné des modèles dynamiques de systèmes opérationnels et à qui il avait été demandé d'améliorer la performance opérationnelle, _n'avaient fait généralement qu'empirer les choses_ [[SKRRS94]](https://www.amazon.fr/guide-lorganisation-apprenante-d%C3%A9velopper-lintelligence/dp/2212568711/). Il en est ressorti d'ailleurs que la plupart des personnes évaluaient mal la manière dont il faut améliorer les systèmes, et appliquaient généralement leur « bon sens », en mettant en place des solutions de contournement qui n'apportent aucune amélioration systémique à long terme.

Pourquoi le comportement d'un groupe de développement de grande taille (autrement dit un système) n'est-il pas compris ou guidé de manière compétente ? La réponse réside, en partie, dans le comportement des systèmes stochastiques avec les files et les variabilités comme nous avons pu l'évoquer avec le principe LeSS de la [théorie des files d'attentes](http://www.les-traducteurs-agiles.org/2017/01/29/less-theorie-des-files-d-attente.html). Et c'est la même réponse qui est au cœur de la _théorie du contrôle_ : la plupart des systèmes d'intérêt - tel qu'un groupe de développement de produit - ont des boucles de feedback positives et négatives ainsi qu'un comportement non linéaire. Le comportement de ces systèmes défient nos intuitions les plus profondes. Et puis il y a la question secondaire des _gens_.

En résumé, les raisons expliquants l'incompétence à maîtriser ou à guider un gros systèmes sont (liste non exhaustive) :

* le manque de connaissance des dynamiques des systèmes, des boucles de feedback, du comportement non linéaire des systèmes, et des conséquences inattendues dans les systèmes sur le lieu de travail.

* la mauvaise compréhension des causes racines des problèmes (et de comment les trouver)

    * _les causes_, pas _la cause_ ; en approche systémique, nous savons que les causes des problèmes sont multiples, indirectes et dynamiques

* l'incapacité à savoir si ou pourquoi une solution de contournement ou une décision locale dégrade la performance globale opérationnelle.

En bref, nous n'utilisons pas l'approche systémique[^2].

Ces raisons sont la conséquence de l'intersection du management et de l'adoption à grande échelle des principes lean et agile. L'équipe de direction fait partie du système qui est perturbé ; si elle n'applique pas l'approche systémique, elle pourrait _vraiment_ le perturber - et pas de la bonne manière !

Les points-clés à retenir de l'approche systémique peuvent être résumé dans les [11 ’lois’](https://en.wikipedia.org/wiki/The_Fifth_Discipline#The_11_Laws_of_the_Fifth_Discipline) décrites dans la [Cinquième discipline](https://www.amazon.fr/cinqui%C3%A8me-discipline-organisations-apprenantes-dexemplaires-ebook/dp/B017WSYAHG)

* Les problèmes d'aujourd'hui viennent des ’solutions’ d'hier
* Plus vous poussez, plus le système pousse en retour
* Le comportement va d'abord empirer avant de s'améliorer
* La manière la plus facile de s'en sortir conduit souvent à faire quelques pas en arrière
* Le médicament peut être pire que la maladie
* Aller plus vite c'est aller plus lentement
* Les causes et les effets ne sont pas étroitement liés dans l'espace et le temps
* De petits changements peuvent produire de gros résultats … mais les zones où l'effet de levier est le plus important sont souvent les moins évidentes
* Vous pouvez avoir votre gâteau et le manger aussi … mais pas en une seule bouchée
* Couper un éléphant en deux ne produit pas deux petits éléphants
* Il n'y a aucun reproche à faire

La devise de Toyota en interne est [« Bien **réfléchir** permet d'avoir de bons produits »](http://www.toyota-global.com/company/toyota_traditions/quality/may_jun_2005.html). L'approche systémique est un ensemble d'outils de réflexion pour aider à :

* **à voir les dynamiques des systèmes** : une organisation de développement est un système de personnes et de règles avec de subtiles boucles de feedback et des conséquences inattendues

    * nous pouvons apprendre à voir et ainsi à améliorer le système avec des **diagrammes de boucles causales** réalisés lors d'un atelier

* **percevoir les modèles mentaux** - parmi les raisons derrière des décisions sous-optimales se trouvent des hypothèses erronées et des raisonnements incorrects

    * les diagrammes de boucles causales et les cinq pourquoi permettent de révéler cela

* **see local optimization**—another source of suboptimal decisions is **local optimization** , making the ‘best’ decision from the viewpoint of a person or department, rather than **global optimization** for the lean systems-level goal of _deliver value fast with high quality and high morale_ .

* **voir les optimisations locales** - une autre source de décisions sous-optimales est **l'optimisation locale**, autrement dit prendre la « meilleure » décision du point de vue d'une personne ou d'un département, au détriment d'une **optimisation globale** qui est l'objectif au niveau système _lean_ et qui consiste à pouvoir _livrer la plus grande valeur possible de très grande qualité avec un moral d'acier._

Cette présentation de l'approche systémique est faite autour des domaines suivants : Apprendre à voir (1) _les dynamiques des systèmes_, (2) _les modèles mentaux_, (3) _les causes racines_, et (4) _l'optimisation locale_.

## Voir les dynamiques des systèmes : Introduction

### Complexité statique versus complexité dynamique

La plupart d'entre nous, notamment les ingénieurs et les financiers, ont été formés pour maîtriser la **complexité de détails statiques** - en apprenant à analyser et à gérer l'information (exigences, analyses financières, …), à décomposer des structures complexes en structures simples, et ainsi de suite. C'est-à-dire, la complexité d'une information qui est par nature structurellement statique.

Pourquoi les gros systèmes informatiques ont-ils tendance à se dégrader malgré de plus en plus de temps passé sur les anomalies ? Qu'est-ce qui pourrait bien se passer si les États-Unis d'Amérique envahissait l'Irak ? Voir les dynamiques derrière ces questions implique d'analyser la **complexité des dynamiques** en jeu.

Au contraire d'une formation sur les détails statiques que la plupart d'entre nous avons suivie, peu d'entre nous ont reçu de formation sur l'étude des systèmes dynamiques et complexes[^3] et notamment dans le milieu professionnel. Peut-être parce que nous avons la croyance qu'il est suffisant de s'appuyer sur le bon sens en milieu professionnel. Jay Wright Forrester a démontré que le « bon sens » n'est pas suffisant dans des systèmes complexes et qu'il est possible de former des personnes pour leur permettre de mieux appréhender les **modèles de dynamiques des systèmes** en milieu professionnel en utilisant notamment des _diagrammes de flux_ [[Forrester61]](http://www.amazon.fr/Industrial-Dynamics-Jay-Wright-Forrester/dp/1614275335/ref=sr_1_1?ie=UTF8&qid=1413582840&sr=8-1&keywords=Industrial+Dynamics).

Les diagrammes de flux peuvent s'appliquer aussi bien aux flux matériels, financiers, d'informations, de stocks (n'importe quel type de stock quantitatif comme de l'argent ou des anomalies), aux conséquences des décisions et des politiques et des relations de causes à effet. Lorsque nous pensons aux diagrammes de flux, nous pensons souvent au seul _diagramme de boucle causale_ dédié aux relations de cause à effets et aux boucles de rétroaction dans un système [[Sterman00]](http://www.amazon.fr/Business-Dynamics-Systems-Thinking-Modeling/dp/0071179895). Il existe une grande variété d'autres diagrammes qui peuvent faire figurer les stocks (quels qu'ils soient), les liens de causalités, et les retards. Dans son ouvrage,  [[Weinberg92]](http://www.amazon.fr/Quality-Software-Management-Systems-Thinking/dp/0932633226/ref=sr_1_1?ie=UTF8&qid=1413527418&sr=8-1&keywords=Quality+Software+Management%3A+Systems+Thinking) Gerald Weinberg appelle cela un _diagramme d'effet_.

### La première loi de la réalisation d'un diagramme : nous modélisons pour avoir une conversation

Un outil très utile pour apprendre les dynamiques des systèmes est le diagramme de boucles causales - nous vous recommandons de l'utiliser sur un tableau blanc notamment lors des Rétrospectives Globales LeSS. Mais avant d'aller plus loin, voici la _première loi de réalisation d'un diagramme_.

> **La première valeur d'un diagramme c'est la discussion qui se déroule lors de la réalisation du diagramme - nous modélisons pour avoir une conversation.**

Lorsqu'un groupe se rassemble pour dessiner un diagramme de boucles causales sur un tableau blanc (« C'est l'acte de discuter et de réfléchir qui est le plus important lorsque nous dessinons », Valtech India.), la première valeur d'un diagramme c'est la conversation et la compréhension commune à laquelle les personnes arrivent lors de la création du modèle. Ce qu'il en résulte, à savoir un diagramme facile à comprendre est important pour rendre les idées et les modèles mentaux concrets et non ambigües (sur le tableau blanc) parce que les mots seuls peuvent être imprécis et mal compris. Toutefois, le diagramme est secondaire par rapport à ce avec quoi les gens repartent : ils ont appris quelque chose et ont revu leur compréhension du monde à travers une discussion.

![xgroup-cld-modeling.jpg]({{ site.url }}assets/less/xgroup-cld-modeling.jpg)

_Un atelier d'approche systémique : réalisation d'un diagramme de boucles causales à plusieurs - modéliser pour avoir une conversation._

_Trucs et astuces de pro pour modéliser_ : nous commençons par écrire sur des post-its les noms des _variables_, par exemple « vélocité des _features_ » ou « nombre d'anomalies ». Nous les plaçons ensuite sur le tableau blanc. Puis nous dessinons les liens de causalités entre les post-its. Il y aura (ou il devrait y avoir) beaucoup de réécriture, d'effaçage, de redessin lors de la session de modélisation. Le résultat le plus important d'une telle session est la _compréhension_ - il se peut qu'à l'issue de cet atelier, certains participants voudront prendre une photo du dessin du tableau blanc.

## Voir les dynamiques des systèmes : les diagrammes de boucles causales

Les diagrammes de boucles causales sont souvent utilisés en introduction à LeSS pour aider à voir les dynamiques de ce qu'il se passe lors du développement à grande échelle. Il est donc utile de comprendre ce type de diagrammes pour cette seule et unique raison. Et cela s'avèrera encore plus utile pour vous, si vous le faites avec vos collègues devant un tableau blanc. Vous modélisez pour avoir une conversation. Quand ? Plus probablement lors d'une rétrospective globale LeSS.

L'aspect pratique de cet exercice est bien plus important que ce qu'il peut paraître au premier abord. Notre conseil d'« être un pratiquant systémique » peut vous sembler vague et sans grand impact. Mais si vous et quatre de vos collègues prenez l'habitude de vous réunir devant un grand tableau blanc, en dessinant des diagrammes de boucles causales ensemble, alors vous arriverez à faire la connexion entre « _être_ un pratiquant systémique » avec « _faire_ de l'approche systémique ».

Les exemples suivants peuvent paraître aseptisés car présentés dans un livre. Mais imaginez-vous à côté d'un tableau blanc avec d'autres personnes dessinant ensemble des diagrammes au cours d'une conversation animée. C'est de cette manière-là que nous suggérons de ’faire’ de l'approche systémique.

### Notation et exemples

Les diagrammes de boucles causales contiennent beaucoup d'éléments ; les éléments suivants sont les plus communément utilisés et sont vus en détail tout au long du scénario qui va suivre

* variables
* liens de causalité
* effets opposés
* contraintes
* objectifs
* réactions ; solutions de contournement
* effets d'interaction
* effets extrêmes
* retards
* boucles de feedback positives

_Le scénario qui suit est un scénario simplifié pour une organisation spécifique. Il ne s'agit pas d'une généralisation._

**Les variables** - Les diagrammes de boucles causales comportent des _variables_ (ou des stocks) telle que la _vélocité (taux de livraison) des features logicielles_ et le _nombre d'anomalies_. Les variables ont une quantité mesurable.

![systems thinking-4.png]({{ site.url }}assets/less/xsystems-thinking-4-fr.png)

**Les liens de causalité** - Un élément peut avoir un effet sur un autre, comme par exemple si la vélocité des _features_ augmente alors le nombre d'anomalies augmente ; autrement dit, plus de code, plus d'anomalies.

![systems thinking-5.png]({{ site.url }}assets/less/xsystems-thinking-5-fr.png)

Il est temps désormais de se jeter à corps perdu dans la _loi de Weinberg-Brooks_ et dans la _causalité fallacieuse_. Il est facile de dessiner un diagramme, ça l'est moins de modéliser en faisant preuve de clairvoyance comme par exemple, la relation entre le _nombre de développeurs_ et la _vélocité des features_.

Toute relation de cause à effets est par nature obscure, même si les gens ont l'habitude de sauter sur la première conclusion venue comme par exemple plus de développeurs égale plus de vélocité. Ajouter des personnes tard au cours du développement peut _réduire_ la vélocité (il s'agit d'une composante de la « loi de Brooks » [Brooks95]). Ou, _davantage_ de mauvais développeurs pourrait vraiment vous ralentir. Il pourrait être objecté qu'_enlever_ des développeurs exécrables peut permettre _d'améliorer_ la vélocité.

![systems thinking-6.png]({{ site.url }}assets/less/xsystems-thinking-6-fr.png)

**Effets opposés** - L'effet d'un lien de causalité peut aller dans la même direction ou dans la direction opposée. Si A augmente alors B augmente ou vice versa. L'effet opposé se souligne à l'aide d'un 'O' sur la ligne. Supposons que les anomalies ralentissent grandement le système, réduisant la vélocité des nouvelles _features_ parce que les gens passent davantage de temps à corriger ou à trouver des solutions de contournement aux anomalies.

![systems thinking-7.png]({{ site.url }}assets/less/xsystems-thinking-7-fr.png)

**Contraintes** - À moins que vous ne trouviez des personnes prêtent à travailler gratuitement, il y a une contrainte sur le nombre de développeurs basé sur le budget disponible.

Les contraintes ne sont _pas_ des liens de causalité. Lorsque la montant du budget disponible augmente, ce n'est pas le cas du nombre de développeurs.

![systems thinking-8.png]({{ site.url }}assets/less/xsystems-thinking-8-fr.png)

**Buts et réactions** - Les personnes, les départements et les systèmes ont des buts, comme par exemple avoir une _vélocité des features plus élevée_. Les buts occasionnent souvent de la pression pour que les gens réagissent (ou agissent) dans l'intention de leur faire atteindre ce but. Mais étant donné qu'il y a la _causalité fallacieuse_ et la _loi de Weinberg-Brooks_ à laquelle il faut faire face, les gens devraient être prudents quant aux actions pertinentes à entreprendre. Voici un exemple de diagramme modélisant cela :

![systems thinking-9.png]({{ site.url }}assets/less/xsystems-thinking-9-fr.png)

Non seulement un but à atteindre avec une _récompense_ au bout engendre une pression à agir, mais cela créé aussi une pression à _faire semblant_ d'agir et à atteindre le but — les récompenses provoquent un **dysfonctionnement des indicateurs**. Le dysfonctionnement des indicateurs peut être proportionnel à la valeur perçue de la récompense parce que les personnes sont motivées pour avoir la récompense, non pour améliorer le système [[Austin96]](http://www.amazon.fr/Measuring-Managing-Performance-Organizations-Dorset-ebook/dp/B00DY3KQX6/ref=sr_1_1?ie=UTF8&qid=1413596674&sr=8-1&keywords=measuring+and+managing+performance+in+organizations). Remarquez bien comment et de quelle manière les récompenses peuvent dégrader la performance du système. De manière visuelle, les dynamiques d'un tel système pourrait être …

![systems thinking-10.png]({{ site.url }}assets/less/xsystems-thinking-10-fr.png)

Il est assez intéressant de voir que toutes ces dynamiques ont été ajoutées par l'introduction d'une récompense et qu'il n'y pas de connexion entre le haut et le bas de cette modélisation.

Il n'y a aucune garantie que la vélocité des features s'améliore ou même que l'on y travaille.

Enlever le système de récompense est une solution à la cause racine de ce dysfonctionnement. Une autre contremesure de surface est le principe et le comportement managériale _Aller voir_ (aller voir physiquement sur le lieu où le travail s'effectue) de l'approche lean.

![systems thinking-11.png]({{ site.url }}assets/less/xsystems-thinking-11-fr.png)

**Solutions de contournement** - Une solution payante à long terme pour atteindre une vélocité plus grande, mais qui n'est pas sans difficulté, consiste à : recruter des développeurs très qualifiés, faire davantage d'accompagnements et de formations, et à se séparer des moins bons éléments. L'alternative est ce que l'on appelle une _solution de contournement_, c'est ce que l'on met en place dans l'espoir d'atteindre l'objectif en moins de temps et avec moins d'effort. Parfois, une solution de contournement se révèle payante aussi bien dans le court terme que dans le long terme, renforçant par la-même le système. D'autres fois cela ne fonctionne pas … d'où l'expression « aller plus vite c'est aller plus lentement ». Par exemple, les gens peuvent _croire_ qu'augmenter le nombre de développeurs permet d'augmenter la vélocité des features. Et ils peuvent par conséquent être amenés à espérer qu'en recrutant davantage de développeurs cela permettra de résoudre plus vite et plus facilement le problème de vélocité. La mention ‘SC’ sur le diagramme ci-dessous indique une solution de contournement.

![systems thinking-12.png]({{ site.url }}assets/less/xsystems-thinking-12-fr.png)

**Effets d'interaction** - La capacité à embaucher est contraint à la capacité budgétaire. Une solution de longue haleine non sans difficulté est d'obtenir davantage de budget. Une solution de contournement possible est de recruter un _grand_ nombre de développeurs bon marché. Dans ce cas, le niveau du budget a un _effet d'interaction_ avec les autres boucles causales. Un budget peu élevé aura tendance à renforcer le taux de développeurs bon marché si la pression pour recruter augmente.

Nous pourrions dessiner simplement un lien de causalité (opposé) de _rentrée budgétaire_ à _taux de recrutement de développeurs bon marché_, mais cela voudrait simplement dire qu'avoir un budget moindre aurait pour conséquence de recruter davantage de développeurs bon marché. Mais ce n'est pas tout à fait ce que nous voulons dire ; ce que voulons montrer en fait, c'est l'effet d'interaction - c'est-à-dire qu'un effet A influence un _effet_ B. Cela se fait en montrant un lien de causalité heurtant un autre lien de causalité, par exemple en traçant une ligne de _rentrée budgétaire_ vers la ligne représentant la solution de contournement qui va vers _taux de recrutement de développeurs bon marché_.

![systems thinking-13.png]({{ site.url }}assets/less/xsystems-thinking-13-fr.png)

**Effets extrêmes** - Il nous est arrivé de travailler avec d'excellents développeurs très bon marché et avec d'autres hors de prix et très nuls, mais en moyenne, vous obtenez à hauteur de ce que vous payez - lorsque vous recrutez au moins disant, le niveau moyen en terme de compétences sera plus faible. Dans le diagramme ci-dessous, nous avons voulu montrer que l'impact du recrutement de personnes bon marché en rapport avec le _nombre de développeurs peu qualifiés_ à un impact sensiblement plus grand que la moyenne.

Pour montrer un _effet extrême_ sur un modèle, faites un trait épais comme vous pouvez voir ci-dessous :

![systems thinking-14.png]({{ site.url }}assets/less/xsystems-thinking-14-fr.png)

**Retards** - Un problème courant au niveau du recrutement dans un projet de développement logiciel concerne _l'erreur au niveau de la variance d'un développeur moyen_ ; autrement dit la croyance fausse que la variance d'un développeur à un autre (en terme de productivité, de qualité de code, etc.) est relativement faible. Toutefois, les études de la variance au sujet des développeurs montrent un rapport de 1 à 4 entre le 1er quartile et le dernier [[Prechelt00]](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.43.4788). C'est plutôt quelque chose de significatif. De même des études - en long et en large - du modèle COCOMO  montrent que la capacité du développement personnel est le facteur de loin le plus important quant à la productivité [[Boehm00]](http://www.amazon.com/Software-Cost-Estimation-Cocomo-II/dp/0130266922/ref=sr_1_1?ie=UTF8&qid=1413597244&sr=8-1&keywords=Software+Cost+Estimation+with+Cocomo+II). Et, en moyenne, il s'avère que les développeurs peu qualifiés font du code de mauvaise qualité (mauvaise conception) et de plus d'anomalies, ceci rajoute un autre frein au système.

Mais l'impact de ces effets ne sont pas visibles immédiatement. Par exemple, cela peut prendre un certain temps après un recrutement massif de développeurs peu qualifiés avant que les impacts négatifs ne se fassent sentir au niveau de la qualité du code ou de la conception. De manière similaire, la _baisse_ moyenne de la vélocité des features (en raison de l'impact important de la variance des développeurs évoqué plus haut) ne se verra pas immédiatement.

Pour montrer ces _effets à retardement_ dans le modèle, faites une double-ligne en travers de la ligne d'effet.

![systems thinking-15.png]({{ site.url }}assets/less/xsystems-thinking-15-fr.png)

Le retard a une influence intéressante sur le pouvoir _pédagogique_ ou correctif sur un système. Si un impact ou une conséquence inattendue est retardé suffisamment longtemps, personne n'en voit ni l'effet (qu'il soit bénéfique ou néfaste) ni sur la façon dont A influence B ou plus subtilement comment _A a influencé B qui a influencé A_.

Par conséquent, personne n'apprend de ses erreurs ni n'est en capacité de les corriger - que ce soit en terme de stratégie, d'actions d'encadrement, d'outils ou de quoi que ce soit. De la même manière, l'amélioration graduelle à travers l'application d'une démarche lean _kaizen_, peut prendre un certain temps ; de la patience et de la perspicacité sont nécessaires pour voir si et comment les choses s'améliorent.

**Boucles de feedback positives** - Les boucles de feedback négatives ou positives[^4] et les retards sont le point de départ pour une approche plus subtile d'un système - et de sa compréhension. Par exemple, de quelle manière une personne peut-elle devenir un meilleur développeur ? En partie, en bénéficiant du mentorat de très bons développeurs et en jetant un œil sur du très bon code. Mais il est impossible de trouver du bon code dans un endroit remplit de développeurs médiocres, il est impossible également d'y attirer ou de retenir le petit groupe de très bon développeurs qui pourraient prendre le rôle de mentors. Ils préfèrent largement aller travailler ailleurs.

Ce groupe de développeurs médiocres rentrent dans un cercle vicieux en raison d'un ensemble de _boucles de feedback positives_. Fort heureusement, ce cercle vicieux est assujeti aux contraintes du budget.

Malheureusement de plus en plus des très bons développeurs, ceux en capacité d'élaborer du très bon code et de faire du mentorat auprès des autres développeurs, partent. Par conséquent, il y a de moins en moins de code de qualité à regarder et à partir duquel il est possible d'en tirer des enseignements. Le pourcentage de développeurs médiocres augmente de plus en plus et la vélocité au niveau des features continue à chuter. Le code devient de plus en plus brouillon, difficile, avec pleins de bouts de code dupliqués à gauche et à droite, le tout de telle manière que la capacité d'implémenter des features décline. Étant donné que la vélocité des features continue de chuter, il y a davantage de pression pour recruter des développeurs très bon marché. Tout cela conduit à de multiples boucles de renforcement positives dans le système comme l'illustre l'exemple ci-dessous :

![systems thinking-16.png]({{ site.url }}assets/less/xsystems-thinking-16-fr.png)

_Astuce_ : Vous pouvez trouver des boucles de feedback positives en cherchant des cycles ayant un _nombre pair_ de relations. Vous en trouverez plusieurs exemples ci-dessus.

#### Conclusion

Le scénario donné à titre d'exemple est uniquement cela - un exemple. Une diagramme de boucle causale permet de visualiser la richesse de la dynamique dans le système dans un milieu professionnel. La meilleure manière de modéliser un tel système est de le faire en groupe face à un tableau blanc.

## Voir les modèles mentaux

Les précédents diagrammes de boucles causales reflètent les modèles mentaux de causalité des individus … qui peuvent s'avérer faux. Il est intéressant de remarquer que les modèles de causalité des individus sont influencés par la ponctualité (ou les retards) et la qualité des feedbacks dans le système.

Les « modèles mentaux » nous permettent d'améliorer nos compétences de méta-cognition pour voir et questionner nos propres postulats et l'enchaînement de nos raisonnements. Brûlons-nous des étapes de manière erronée ? Cette question implique aussi lorsque nous sommes en train de travailler avec des collègues de discuter avec eux (en s'enquérant plutôt qu'en reprochant) de leurs modèles mentaux.

_Voir_ les modèles mentaux n'est que la première étape ; les _changer_ constitue une seconde partie bien plus difficile. Cet art est bien au-delà du sujet de cette introduction, même si une adoption réussie de LeSS implique des changements en terme d'état d'esprit et de prise de conscience au sein de très nombreuses équipes.

Une astuce pour mieux _voir_ les modèles mentaux (croyances, échelle d'inférence, …) en jeu au niveau des dynamiques des systèmes est de poser les questions suivantes lors d'un atelier de modélisation puis de tracer les éléments de réponse au tableau blanc. « Parlons donc des hypothèses derrière ce modèle. Que _croyons_-nous ou tenons pour acquis en terme de faits et d'effets qui nous ont conduits ici ? »

Les éléments de réponse sont dessinés sur le tableau blanc. En voici un exemple :

![systems thinking-17.png]({{ site.url }}assets/less/xsystems-thinking-17-fr.png)

_Visualiser les postulats présents dans nos têtes … nos modèles mentaux._

### Exemple : La dynamique « Aller plus vite c'est aller plus lentement »

Dorénavant, avec notre vocabulaire enrichi des termes de solutions de contournement, de boucles de feedback positives et de modèles mentaux, il est fascinant de voir qu'il peut y avoir un semblant d'amélioration à court terme sur une variable donnée, mais que cela entraîne en même temps une _dégradation à retardement_ de cette même variable - d'où la dynamique « Aller plus vite c'est aller plus lentement ». Il s'agit d'une dynamique récurrente et d'une cause de vulnérabilité à terme. Voici un nouvel exemple illustrant cela :

_Histoire de Microsoft Word et de_ **_la boîte à outils secrète du développeur_** : Un exemple typique d'une ‘amélioration’ à court terme mais d'une dynamique de dégradation à long terme est le récit de la première livraison de Microsoft Word sur Windows [[Spolsky04]](http://www.amazon.com/Joel-Software-Occasionally-Developers-Designers/dp/1590593898/ref=sr_1_1?ie=UTF8&qid=1413597951&sr=8-1&keywords=Joel+on+Software). Le logiciel a été livré avec des _années_ de retard par rapport à la date prévue. Pourquoi ? _Parce que les managers ont essayé à tout prix de suivre le calendrier de départ et ont fait pression sur les développeurs pour le respecter_.

Cette histoire illustre pourquoi cet espoir illusoire de respecter une date souhaitée est bien identifié comme une source de gâchis dans l'approche lean. Dans le cas présent l'espoir illusoire consiste à insister (du moins apparemment) à suivre le calendrier, ce qui implique une idée fausse ou illusoire que les estimations ne sont pas de simples estimations mais des promesses, un mythe classique qui pousse à la dégradation d'un système.

[Le modèle qui suit](https://less.works/less/principles/systems-thinking.html#figure-1) _résume_ les dynamiques à l'œuvre lorsque des managers poussent leurs équipes à respecter à tout prix les calendriers prévisionnels, et pourquoi cette solution de contournement qui freine pourtant l'avancement des travaux semblent les faire aller plus vite à court terme mais en réalité _plus lentement_ à long terme. Par rapport à ce qui est décrit précédemment dans la dynamique de la pression du calendrier et la boîte à outils secrète, certaines dynamiques ont été omises intentionnellement sur ce schéma et sont visibles sur le schéma dynamiques avancées.

![systems thinking-18.png]({{ site.url }}assets/less/xsystems-thinking-18-fr.png)

_Dynamique de la pression sur le calendrier et de la boîte à outils secrète._

En solution de contournement, les managers de Microsoft ont exhorté, ont corrompu (à l'aide de primes potentielles), et ont menacé les développeurs de Word pour leur faire respecter le calendrier prévisionnel. En conséquence, les développeurs ont, de manière tout à fait prévisible, sorti leur **boîte à outils secrète de développeurs**, autrement dit tout un arsenal de pratiques pour pisser du code pourri (aucuns tests, aucunes revues, ignorance des anomalies connues, développement par copier-coller, mauvaise conception, …) pour développer visiblement plus vite. Vous voyez bien, les développeurs ont aussi des solutions de contournement pour régler leurs problèmes.

Vu de l'extérieur, ces tactiques ont fonctionné à merveille. Au fur et à mesure que les managers mettaient la pression sur les développeurs, les ‘features’ étaient développées de plus en plus vite grâce à l'utilisation de la boîte à outils secrète, ce qui a renforcé la croyance en quoi mettre la pression sur les développeurs était quelque chose d'utile. Mais cette apparente accélération a eu en fait un effet à retardement qui a rendu les choses plus lentes (c'est ce que nous allons voir par la suite). Étant donné que le management n'a pas été assez rapide à voir l'effet à retardement de la boîte à outils, et parce que les managers pensent qu'ils n'ont pas besoin d'aller regarder fréquemment en détails le code source ou qu'ils n'ont pas besoin d'être eux-mêmes des développeurs très expérimentés, ils n'ont rien appris de cette dynamique.

Le schéma ci-dessous illustre l'examen approfondie des dynamiques des systèmes montrant pourquoi les choses sont allées plus lentement à long terme et pourquoi le tout premier Word pour Windows a été livré des années en retard par rapport à la date souhaitée …

![systems thinking-19.png]({{ site.url }}assets/less/xsystems-thinking-19-fr.png)

_Dynamiques avancées de la pression sur le calendrier et de la boîte à outils secrète._

Naturellement, avoir une grande quantité de code de mauvaise qualité ralentie les choses. De manière beaucoup plus subtile, les développeurs ont _ignoré_ la liste croissante d'anomalies pour privilégier la production de nouvelles features. Cela a eu pour conséquence d'avoir un délai important entre la déclaration d'une anomalie et sa correction. Il s'avère que cela a fait augmenter de manière significative la variabilité et le temps nécessaire pour corriger une anomalie en raison des effets cumulatifs négatifs liés à la nature même d'une vieille anomalie (par exemple avec la mise en place des solutions de contournement et des couplages existants entre les fonctionnalités), de l'oubli du contexte détaillé par les développeurs en relation avec l'anomalie, ces derniers mettant par conséquent plus de temps à le redécouvrir, de l'accumulation continue de code de mauvaise qualité dans le même temps.

Le lecteur avisé remarquera également plusieurs boucles causales positives renforçant le cycle de dégradation ; il s'agit de l'une des raisons expliquant le retard pris sur plusieurs années pour livrer le produit.

Une solution ? L'approche lean avec les principes _Arrêter et corriger_ et _Aller voir_. _Premièrement_, plutôt que d'essayer d'aller plus vite lorsqu'il y a des problèmes, des managers-formateurs encouragent les gens à aller plus _lentement_ et à les inciter à apprendre les dynamiques des systèmes, les causes racines et à les corriger pour améliorer le _système_ du développement. En allant plus lentement, Toyota - les maîtres de l'approche lean - est devenue l'une des entreprises les plus rapides du monde. _Deuxièmement, les managers doivent _aller voir ce qui se passe sur le vrai lieu de travail_ pour apprendre ce qu'il se passe. Le _vrai lieu_ dans le développement logiciel c'est le code, ce qui implique que les managers de proximité sont des développeurs expérimentés qui évalueront le code fréquemment.

Les personnes de chez Microsoft n'ont réfléchi sur la situation que bien après la livraison. Lorsqu'ils ont fini par faire une rétrospective, cela a amené à une politique du _zéro défaut_, cela signifie que la première priorité était de corriger les anomalies connues dans le code en cours de développement afin d'aller vers du zéro anomalie ouverte dans la liste des anomalies avant d'écrire du code pour une nouvelle feature.

## Voir (et entendre) l'optimisation locale

« Chacun fait de son mieux, mais malgré tout le flux de production du système se dégrade.  Comment cela est-il possible ? ». Il s'agit du paradoxe de **l'optimisation locale** - autrement dit c'est lorsqu'une personne à titre individuel ou un responsable de département prend une décision d'un point de vue local ou dans son propre intérêt. Les personnes prenant ce type de décision _croient fréquemment qu'ils prennent la meilleure décision_, mais parce que ‘meilleure’ est ici synonyme d'optimisation locale, cela a pour résultat une sous-optimisation globale du flux du système. Ceci est le résultat d'une « mentalité de silo », d'incompréhension, de peur, de restrictions d'informations, de feedbacks à retardement, d'ignorance, de carriérisme, d'avarice et de bien d'autres _dysfonctionnements d'apprentissages organisationnels_.

Une petite équipe produit de 30 personnes n'a ni temps ni l'argent pour s'engager dans ce genre de non-sens ou de gâchis. Mais les grandes entreprises avec de grands groupes produit, des processus centralisés et des groupes outils, un « bureau de gestion de projet » centralisé, et ainsi de suite, semblent avoir élevé l'optimisation locale et le gâchis à une forme d'art. Les bureaucraties gouvernementales en sont bien sûr la quintessence. En conséquence, lorsque vous servez de guide dans une adoption agile à grande échelle, _voir_ (ou _entendre_) et s'occuper de l'optimisation locale est tout simplement quelque chose de vital.

Par exemple, les départements juridiques et sécurité mettent en place des politiques qui leurs semblent très importantes de leurs points de vue. Dans l'objectif de prévenir la perte de propriété intellectuelle, le département juridique peut décréter « il est interdit d'afficher tout type d'information sur les murs. ». Or, le département de la logistique soumis de son côté, à une pression de politique de réductions de coûts peut surenchérir en disant : « Il est important de s'assurer que nos murs ne soient ni sales ni abîmés ». Et ainsi s'arrête le management visuel qui est l'une des pratiques de l'approche lean (le management visuel se faisant habituellement sur les murs), et ils inhibent également une pratique d'innovation bien connue à savoir le travail de groupe devant un tableau blanc. Les juristes réussiront peut être à réduire la perte de propriété intellectuelle (ce qui en réalité devrait poser question), et les gens de la logistique réussiront à garder leurs murs propres - mais au prix d'inhiber le groupe de développement produit dans sa capacité d'innover et de collaborer. Finalement, l'entreprise se laissera distancer par la concurrence avec de moins en moins de propriété intellectuelle valant la peine d'être défendue parce que les outils permettant l'innovation et de livrer rapidement ont été bannis, mais les juristes auront rempli leur mandat vis-à-vis de la direction de « s'assurer que la propriété intellectuelle est protégée ». Et la police de la logistique aura nettoyé les murs. _Ils ont fait de leur mieux_.

Ce qui suit est extrait d'un vrai mail de la _POLICE DE LA LOGISTIQUE_ dans une organisation qui a banni le management visuel sur les murs. Pouvez-vous identifier les optimisations locales et les modèles mentaux qui sont derrière tout ça ?

> Les [bureaux à cloisons](https://fr.wikipedia.org/wiki/Bureau_%C3%A0_cloisons) peuvent être personnalisés. Mais tout ce qui visible au-dessus de la cloison ou qui perturbe l'harmonie de l'environnement de bureau est interdit.

Nous constatons aussi des optimisations locales dans les groupes centralisés dont le rôle est de choisir les logiciels pour les autres personnes de l'entreprise. La croyance la plus répandue relative à cette démarche est qu'il s'agit de ce qu'il y a de mieux pour réduire les coûts d'achats (curieusement ces mêmes groupes recommandent rarement les logiciels open source gratuits) ou ce qu'il y a de mieux pour accomplir une tâche compliquée ou ce qu'il y a de mieux pour l'accomplissement du travail d'un seul type de travailleur (même si _tout le monde_ est censé devoir utiliser l'outil), plutôt que de maximiser l'objectif de l'entreprise qui est d'avoir un système de flux de production de la valeur plus rapide pour les clients.

Dans les adoptions de Scrum ou des principes agiles à grande échelle, la plupart des problématiques de type « Oui, mais … » qui sont soulevées sont des exemples de sous-optimisations, comme par exemple « _Oui, mais … qu'en est-il des comptes-rendus auprès du management_ ? »  ou encore de manière plus générale « * Oui, mais … qu'en est-il de ... * ? ». Alors, les principes et les pratiques sont dévoyés, pour servir soit l'objectif de rendre compte soit n'importe quel autre objectif secondaire plutôt que suivre l'objectif d'optimiser le flux de valeur produite. De temps en temps, nous voyons des **optimisations locales dans certains cas rares ou extrêmes**. Par exemple, une entreprise doit choisir un outil centralisé répondant à un certain nombre de cas d'utilisations possibles dont un cas extrêmement rare ou complexe, la personne, en charge de faire ce choix, choisit un outil correspondant à un cas unique d'utilisation, sous-optimisant ainsi l'ensemble du système pour un cas représentant uniquement 5% des cas d'utilisation au lieu de l'optimiser pour la majorité des 95% des autres cas d'utilisations.

D'autres optimisations locales sont dues, quant à elles, à l'ignorance des nouvelles manières de travailler. C'est quelque chose de très répandue et tout spécialement dans les groupes produit à grande échelle. Par exemple, un jour nous avons aidé un groupe produit distribué à travers l'Europe à adopter d'une part Scrum et d'autre part la pratique de _l'intégration continue_ (CI) le tout sous la forme d'un système d'intégration continue dédié intégrant, compilant, testant automatiquement de manière continue le produit. Après quelques temps, un manager, que l'on pourrait qualifier de traditionnel, extérieur au groupe est venu inspecter ce qu'il se passait. Celui-ci a recommandé que les pratiques d'intégration devraient être changées en raison de l'absence de schéma d'intégration global permettant à un responsable d'intégration de faire manuellement l'intégration de l'ensemble du logiciel ; une absence de schéma pour la bonne raison qu'il n'y avait plus besoin de responsable d'intégration au sein de l'organisation. Il voulait ‘optimiser’ le travail d'un responsable d'intégration qui n'existait plus. Il était dans l'impossibilité de voir que la totalité de l'ancienne manière de faire les choses avait disparu avec l'intégration continue. Cette histoire se répéta dans l'ensemble des départements du groupe produit : il y a avait des optimisations locales partout autour des façons de faire existantes, tels que les tests manuels, le département d'architecture séparé des équipes, les équipes composants, etc. N'importe quel coach dont la tâche consistait à introduire Scrum à grande échelle au niveau de l'organisation avait une _montagne_ d'optimisations locales à penser à gérer.

Dans l'approche lean et dans les méthodes agiles, l'accent est mis sur les objectifs du système dans sa globalité : livrer de la valeur de grande qualité au plus vite tout en gardant le moral des équipes au plus haut - autrement dit une **optimisation globale**. Essayer de reconsidérer vos décisions à la lumière de cet objectif. Pour développer une culture de « l'optimisation du tout », remettez donc en cause toutes les décisions et les règles avec la question suivante :

> **Est-ce que cette décision ou cette règle se focalise sur le fait de livrer de la valeur au client externe au plus vite, ou se focalise-t-elle sur les intérêts d'un département, d'une personne, d'une pratique/règle interne, ou d'un cas rarissime ?**

Dans LeSS, le Product Owner est responsable pour choisir ces objectifs à haute valeur qui **pourrait mener à un produit potentiellement livrable (à la fin du Sprint) maximisant les impacts souhaités et réjouissant le client tout en maintenant un rythme soutenable et une haute qualité d'ingénierie**. Cet objectif explicite est destiné à orienter le système vers son optimisation globale plutôt que vers une optimisation qui ne serait que locale.

## Conclusion

En plus de devenir un pratiquant de l'approche systémique vous-même, encouragez donc les autres à en apprendre plus sur ce sujet. Nous vous suggérons d'essayer de rassembler quelques-uns de vos collègues autour d'un tableau blanc et d'y dessiner des diagrammes de boucles causales, afin que les architectes des systèmes et les pratiquants de l'approche systémique soient réunis en un seul endroit.

![systems thinking-20.png]({{ site.url }}assets/less/xsystems-thinking-20-fr.png)

_Séance d'approche systémique. Réalisation d'un diagramme de boucle cause à plusieurs mains dans l'objectif d'avoir une conversation._

## Lectures recommandées

* [_Hors de la Crise_](https://www.amazon.fr/Hors-crise-W-Edwards-Deming/dp/2717843930/) de W. Edwards Deming est un ouvrage de référence par, sans conteste, le plus connu des penseurs systémiques et des experts sur la qualité. Cet ouvrage commence par un objectif modeste : « l'objectif de ce livre est la transformation du style du management américain … ce qui exige de tout changer pour mettre en place une toute nouvelle structure. ». Deming prône un _Système de connaissances approfondies_ dans lequel les managers (1) reconnaissent qu'il y a un _système_, (2) qu'ils sont en mesure de comprendre les facteurs les plus répandus et les facteurs spéciaux de variations au sein du système (la théorie des files d'attente est liée à ce phénomène de variation), (3) qu'ils sont en mesure de comprendre que les connaissances sont limitées et qu'il y a des erreurs de raisonnements, et (4) que la psychologie et les recherches en sciences sociales jouent des rôles tout à fait crédibles dans l'objectif de comprendre que les règles régissants les comportements ou en lien avec la motivation des individus ne soient pas basés sur le seul « bon sens ». Le cœur de l'ouvrage tourne autour des célèbres _14 points pour le management_, y compris par exemple « _Éliminer le management par les objectifs. Éliminer le management par les nombres, par les objectifs par les nombres. Y substituer le leadership_»

* [_Industrial Dynamics_](https://www.amazon.fr/Industrial-Dynamics-Jay-Wright-Forrester/dp/1614275335/) de Jay Forrester est un classique du genre sur les dynamiques des systèmes, très bien écrit et très instructif. Même si cet ouvrage a été écrit au début des années 1960, il est toujours aussi pertinent aujourd'hui. Il va au-delà de la modélisation des causes à effets pour modéliser également le flux et les stocks d'informations, d'argent et de matériaux au sein d'un système. Le livre contient également une modélisation mathématique formelle de ces dynamiques, toutefois la lecture de cette dernière reste facultative quant à apprécier la qualité de l'ouvrage.

* Les ouvrages [_Quality Software Management: Systems Thinking_](https://www.amazon.fr/Quality-Software-Management-Systems-Thinking/dp/0932633226/) et [_An Introduction to General Systems Thinking_](https://www.amazon.fr/Introduction-General-Systems-Thinking-Weinberg/dp/0932633498/) de Gerald Weinberg sont intéressants. Il sont écrits du point de vue d'un consultant expérimenté en développement de systèmes.

* [_La cinquième discipline_](https://www.amazon.fr/cinqui%C3%A8me-discipline-Levier-organisations-apprenantes/dp/2212559372/) est un autre classique du genre qui prône que l'encadrement d'une entreprise devrait appliquer l'approche systémique (autrement dit la _cinquième_ discipline) ainsi que d'autres disciplines-clés toutes aussi importantes en vue d'obtenir une entreprise durable. Ces autres disciplines que les dirigeants devraient appliquer sont (1) une discipline personnelle, (2) une réflexion sur leurs propres croyances et raisonnements erronés, (3) la définition et la communication d'une vision partagée ayant du sens, et (4) la capacité des équipes à apprendre. Nous vous recommandons d'ignorer - du moins dans un premier temps pendant vos premières années de pratiques - le concept d'archétypes présenté dans le livre. Ce concept avait pour but d'être une aide à l'apprentissage de la cinquième discipline mais nous avons observé qu'il était soit une source de distraction soit qu'il intimidait les lecteurs quant à leur apprentissage et à l'application de la modélisation basique[^5] de dynamiques des systèmes. Les ‘archétypes’ ne font pas partie à l'origine des dynamiques des systèmes.

* [_La 5ème discipline - le guide de l'organisation apprenante_](https://www.amazon.fr/guide-lorganisation-apprenante-d%C3%A9velopper-lintelligence/dp/2212568711/) est une source extrêmement riche sur l'approche systèmique écrite du point de vue des pratiquants de cette approche et de consultants.

* Les écrits d'Argyris, Outnam, McLain et Schön sur les apprentissages organisationnels comme [_Action Science_](https://actiondesign.com/resources/readings/action-science) et [_Organizational Learning_](http://www.amazon.com/Organizational-Learning-Addison-Wesley-Organization-Development/dp/0201001748/ref=sr_1_11?ie=UTF8&qid=1413601940&sr=8-11&keywords=organizational+learning) abordent des concepts importants tels que la _double-boucle apprenante_ et le _dialogue grand-plaidoyer/grand-réquisitoire_.

* Les publications et les ressources de la _Society for Organizational Learning_](https://www.solonline.org/).


[^1]: _La cinquième discipline_ écrit par Senge sur l'approche systèmique et les organisations apprenantes a été nommé « l'un des livres les plus novateurs sur le management de ces 75 dernières années » par la _Harvard Business Review._ See** [Senge94].
[^2]: Une autre raison : Croire que plus de contrôle est possible qu'il ne l'est actuellement. La science de la complexité montre qu'il existe des limites en terme de prédiction et de contrôle des systèmes sociaux semi-chaotiques [Stacey07]. C'est une énorme boîte de Pandore qui restera enfermée dans ce livre.
[^3]: Macro économie, psychologie, sociologie et biologie sont des exemples d'exceptions parmi d'autres
[^4]: _Les boucles de feedback_ sont parfois utilisées dans ce livre dans le sens littéral du terme, plutôt dans le sens des dynamiques des systèmes
[^5]: ‘Basique’ ne signifie pas trivial ou facile à résoudre. Par exemple, les problématiques de ‘motivation’ et de ‘qualité’ sont des problématiques basiques mais elles ne sont pas faciles à résoudre.


---
Auteur : The LeSS Company B.V.  
Source : [Systems Thinking](https://less.works/less/principles/systems-thinking.html)  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 01/11/2020  
Relecteurs : Christophe Gesché, Fabrice Aimetti  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

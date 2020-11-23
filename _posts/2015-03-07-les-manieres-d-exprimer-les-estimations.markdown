---
layout: post
title:  "Les manières d'exprimer les estimations"
date:   2015-03-07 14:00
tags: estimation
---

La manière dont nous exprimons nos estimations influe à la fois sur la manière dont nous réfléchissons sur l'élément en cours d'estimation et sur la manière dont nos estimations sont perçues.  

## Une seule valeur

Assez souvent, lorsqu'une évaluation est demandée, les gens donneront une seule valeur. "Combien de temps cela prendra t-il ?" "Trois semaines". Si le niveau de confiance est suffisant, et les points de référence suffisamment alignés, alors une seule valeur peut être suffisante. Exprimer une estimation sous la forme d'une seule valeur peut laisser en suspens beaucoup de non-dit. Quelle confiance avons-nous dans cette valeur ? Si nous avons tort, quelle pourrait être la valeur réelle ?  

Nous nous retrouvons souvent dans la panade lorsqu'une personne donne une estimation avec un ensemble de suppositions, et qu'une autre personne l'entend avec un autre ensemble de suppositions. Je pourrai souligner que mon estimation de 2 jours pour une tâche est une estimation optimiste, en supposant qu'aucun problème caché ne surgisse. Vous pourriez l'entendre comme l'expression de la valeur la plus plausible possible avec la marge d'erreur la plus réduite. Lorsque les communications vont au-delà d'une personne à une autre, la probabilité d'incompréhension du contexte sur lequel se base ces suppositions augmente. Maintenant, si vous communiquez mes estimations à votre patron, il peut l'interpréter comme un engagement sur cette durée. Les mises en garde et les alertes tendent à s'effacer alors que la valeur est retenue.  

## Sur/Sous évaluer

Lorsque j'ai appris l'orientation chez les scouts, une des leçons était, lorsque vous cherchez votre chemin dans les bois avec une boussole, d'être sûr que vous allez bien d'un côté. De cette manière, lorsque vous trouverez la route, vous saurez dans quel sens aller. Si vous essayez d'aller directement vers la destination souhaitée, vous pourriez arriver n'importe où sur la route.

Vous pouvez utiliser la même philosophie lorsque vous faites des estimations. Estimer "pas plus de" ou "pas moins de" peut souvent donner assez d'informations pour savoir dans quel sens aller avec une seule estimation.

## Une seule valeur avec des marges d'erreurs

Dans certaines situations, donner une estimation minimale ou maximale peut ne pas être aussi pertinent qu'une valeur "la plus plausible". Nous pouvons indiquer la confiance que nous avons dans cette valeur avec des marges d'erreur. Ces marges d'erreurs pourraient être exprimées sous la forme de valeurs minimale et maximale spécifique, même si cela signifie que nous aurons 3 valeurs séparées à estimer. Je suis plus enclin à utiliser les pourcentages. J'ai souvent estimé le temps requis pour décrire vaguement les tâches avec des marges d'erreur de -50% et +100%. Cela semble déséquilibré à certaines personnes, mais cela semble plus raisonnable sur une échelle logarithmique. Cela correspond bien à l'épidémie d'estimations sur-optimistes (existante - NdT) dans le développement logiciel.

## Intervalle

Si vous allez estimer les valeurs minimales et maximales possibles, vous pourriez arriver à la conclusion que l'intervalle estimé est suffisant et que vous n'avez pas besoin de la valeur la plus plausible. Faites attention comment vous communiquez un intervalle d'estimation. Il est trop fréquent que le destinataire entende juste la borne qu'il préfère. J'ai vu des responsables se plaindre qu'une tâche estimée entre 2 et 4 semaines prenne 3 semaines, "mais vous aviez dit qu'elle pourrait être faite en 2 semaines.".

## Avec un niveau de confiance

Vous pouvez exprimer l'incertitude, d'une valeur d'estimation ou d'un intervalle d'estimation, avec un niveau de confiance. "Je suis certain à 95% que cette tâche sera terminée dans les 2 semaines.", "Il est sûr à 95% que ce boulot prendra de 1 à 3 semaines.".  

Quelques fois, un niveau de confiance élevé n'est pas ce que vous auriez préféré. Par exemple, lors de l'estimation des user stories pour déterminer la quantité de travail pouvant être réalisé dans un sprint Scrum, utiliser des estimations avec un niveau de confiance élevé aura comme résultat que vous prendrez moins de travail que vous n'auriez été tenter d'en prendre. Alors, en application de la loi de Parkinson, le travail s'étalera pour prendre tout le temps disponible. Dans une telle situation, je recommande d'estimer avec un niveau de confiance de 50%. Je dis aux personnes qu'elles devraient s'attendre, à long terme, à être à court en temps et de travail à peu près dans les mêmes proportions.  

J'ignore comment estimer des niveaux de confiance avec une précision suffisante. Je sais qu'estimer avec des modèles mathématiques peut vous donner un niveau de confiance calculé. Vous pouvez alors utilisez ce niveau de confiance pour prendre des décisions avec une précision chirurgicale basé sur les chances que l'estimation devienne vraie.  Tout ceci, est toutefois basé sur la fiabilité du modèle mathématique et sur la précision des données d'entrées.  

Les niveaux de confiance sont facilement incompris par la plupart des personnes. J'ai souvent entendu des gens se plaindre que le bulletin météo est imprécis parce qu'il prévoit 30% de chance de pluie et qu'il ne pleut pas.  

## Distribution de probabilités

Vous pouvez aller plus loin qu'avec un niveau de confiance, en spécifiant la distribution de probabilités pour que notre estimation nous donne la précision sur n'importe quel niveau de confiance souhaité. S'il s'agit d'une distribution gaussienne, par exemple, nous savons qu'il y a 50% de chance que l'effectif soit inférieure ou égale à la valeur médiane. Il y a 97,5% de chance que l'effectif soit à deux écarts-type au-dessus de la moyenne.  

Bien sûr, les mêmes mises en garde sur la fiabilité des modèles mathématiques et la précision des données d'entrées s'appliquent aux estimations exprimées sous la forme de fonctions de probabilités. Les données empiriques montrent qu'il est peu plausible que la distribution de probabilités du temps de réalisation pour un projet de développement logiciel d'être symétrique, et par conséquent, la distribution gaussienne est un piètre modèle. Cela conduit les gens à utiliser la distribution Weibull à la place, pour modéliser le fait que le temps de développement est sans doute plus long que plus court par rapport au temps médian. Le paramètre de forme, β, de la loi de Weibull a un effet majeur sur la forme de la distribution, et par conséquent sur sa fiabilité.  

## Mesures sans unité relatives à d'autres estimations

En réaction aux problèmes bien trop fréquents survenant lors de la fourniture d'estimations avec des unités de temps, les personnes choisissent certaines fois d'utiliser des mesures sans unité pour leurs estimations. Cela permet de faire une estimation relative entre des tâches comparables. "Cette tâche-ci et celle-là sont à peu près de la même taille.". L'estimation sans unité permet à l'estimation de "flotter" au sens littéral et d'être basée sur l'expérience passée. "Si nous avons pu faire 42 unités de travail la semaine dernière, nous espérons pouvoir accomplir 42 unités de travail cette semaine.". Si la vitesse de réalisation du travail varie, alors seul l'espérance (du nombre d'unités de travail réalisés - NdT) doit changer ; le travail n'a pas besoin d'être ré-estimé.  

La mesure sans unité la plus rencontrée actuellement semble être les points de story. Ils sont surnommées ainsi parce qu'ils représentent la "taille" d'une tranche fonctionnelle de travail appelée user story. Ils sont souvent réduits à la seule "suite modifiée de Fibonacci" pour représenter la perte de précision par rapport à l'augmentation de la taille de la story.  

L'esprit humain est une chose merveilleuse et subtile. Il semble devenir meilleur à estimer la taille d'une story par rapport à une autre lorsqu'il est libéré de la tyrannie des mesures du temps. J'ai remarqué que les équipes ayant un étalon de référence complètement arbitraire basé sur la taille ("Disons que cette petite story est un '2' et estimons les autres par rapport à celle-là") semble donner des estimations cohérentes plus rapidement que celles ayant un étalon de référence basé sur le temps ("Disons que cette story sera un '2' si elle prend 2 heures 'idéales' de travail").  

Malheureusement, il est souvent trop tentant pour quelqu'un, et tout particulièrement pour quelqu'un ayant suffisamment de pouvoir dans l'organisation, de ré-étalonner les points de story sur des unités de temps. Généralement, cela annule l'avantage d'utiliser une mesure sans unité, les personnes commençant à penser en terme d'heures à la place de points. C'est même encore pire lorsque l'étalonnage est fait en heures "idéales", car quelqu'un se plaindra un jour sûrement "Pourquoi les développeurs accomplissent seulement 5 heures de points de story par jour ?" <sigh>  

Les points de story sont encore maintenant exprimés sous la forme de nombre, et cela tente les gens de faire plus de calculs mathématiques que leur précision et détermination leur permet raisonnablement de supporter. Le niveau suivant dans l'abstraction des estimations est d'éliminer les nombres. Les gens utilisent beaucoup de choses à la place des nombres. Une des plus créatives est celle des animaux. La plus commune est peut être les tailles de T-shirts, XS, S, M, L, XL. Alors que vous pouvez supposez qu'une story à 10 points est le double d'une taille à 5 points, et 5 fois celle d'une à 2 points, vous ne pouvez pré-supposé d'une telle relation entre une petite (small), moyenne (medium) et grande (large) story. C'est un autre moyen de libérer l'esprit de ce qu'il pense qu'il devrait savoir, et de le laisser opérer à un niveau subconscient qui donne souvent de bien meilleurs résultats.  


## Qu'est-ce-que vous en pensez ?

Ai-je omis des manières utiles d'exprimer des estimations ? Ou d'autres manières, utiles ou pas, que les personnes ont tendance à utiliser ? Ai-je mal caractérisé certaines d'entre elles ? Merci de laisser un commentaire avec vos réflexions.

---
Auteur : [George Dinwiddie](http://blog.gdinwiddie.com/about/)  
Source : [Ways of expressing estimates](http://blog.gdinwiddie.com/2015/02/08/ways-of-expressing-estimates/)  
Date de parution originale : 08 Février 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 07/03/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

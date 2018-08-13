---
layout: post
title: "Est-ce que vous voulez de l’agilité de merde ?"
date:   2016-04-27 09:26:55
published: true
tags: 
- agile
---

Regardez ce graphique de VersionOne :

![Vous voulez quoi]({{ site.url }}assets/vous_voulez_quoi/vous-voulez-quoi.png)

L’un des plus gros problèmes avec un outil comme VersionOne est qu’il vous encourage à suivre des “métriques”. Est-ce que vous voulez de l’agilité de merde ? Eh bien, c’est comme ça que vous obtiendrez, du moins le plus souvent, de l’agilité de merde.

Bien sûr, il est important de savoir comment vous travaillez et d’essayer de s’améliorer. Oui, c’est sûr … sauf que … voilà, il y a de grandes chances qu’elles seront détournées. Je dis _seront_ et non pourraient. Même si vous essayez de ne pas détourner ces métriques, cela arrivera inéluctablement. Le proverbe “vous obtiendrez ce que vous mesurez” se vérifie toujours.

## Vélocité - 59 % des utilisateurs …

… suivent le nombre de points ? Les _stories_ auront tendance alors à être estimées avec un nombre de points plus élevé. Tout ce que vous aurez à faire sera de froncer légèrement les sourcils lorsque l’équipe ne fera que 24 points à la place des 30 points du dernier sprint, et devinez quoi, le nombre de points sera plus élevé la prochaine fois.

… suivent le nombre de stories ? Faites des stories plus petites et vous en obtiendrez plus.

… suivent le nombre de stories mais ne les scindent pas ? Testez un peu moins, refactorez un peu moins et vous en aurez plus.

## Burn Down / Burn Up d’itération ou de livraison - environ 50 %

Les burn down d’itération et de livraison sont importants pour savoir où vous en êtes. Lorsque vous voyez un virage se profiler à l’horizon, vous n’accélérez pas, vous ajustez votre conduite. C’est la même chose avec le burn down : utilisez-le pour décider quoi faire, pas pour accélérer.

Mettre la pression (sur l’équipe - NdT) au niveau du burn down aura comme conséquence d’avoir de plus petites stories (ce qui peut être une bonne chose), qu’il y aura moins de tests et de _refactoring_. Ce n’est pas une bonnes chose, cela va vous ralentir et engendrer plus d’anomalies. Vous voulez des anomalies ? C’est comme ça que vous en aurez.

## Stories planifiés vs réalisées - 35 %

Vous me mettez la pression parce que je pensais que nous aurions obtenu 10 stories et que nous n’en avons obtenu que 8 ? Qu’est-ce que je peux faire ? Je travaille déjà aussi dur et aussi bien que possible. Alors qu’est-ce que je peux faire ? Faire moins de travail, voilà ce que je peux faire. Mais c’est vous qui avez défini les stories, donc tout ce que je peux faire c’est moins de travail dans chaque story. Je peux les rendre un peu moins robustes, je peux tester un peu moins attentivement, je peux aussi laisser le code dans un état peu plus mauvais que je ne l’ai trouvé. Est-ce que vous voulez de ces choses-là ? Non, vous ne le voulez pas.

## Dates de livraisons planifiées vs réalisées - 29 %

Salut, de quoi osez-vous donc parler ? Une des valeurs _fondamentales_ du développement agile de logiciel est d’avoir un _logiciel opérationnel_. Scrum exige que vous ayez une version testée, intégrée, prête à livrer, avec toutes les fonctionnalités à jour, en main à la fin de _chaque_ sprint.

Si vous respectez ça, vous pourrez atteindre n’importe quelle date de livraison souhaitée. Vous pourriez l’atteindre avec un nombre réduit de fonctionnalités par rapport à celles imaginées à l’origine. En fait, vous _l’atteindrez_ sans aucun doute avec moins de fonctionnalités que vous ne l’avez imaginé, parce que ces fonctionnalités que vous avez imaginées ne valent pas le coup de se mettre en retard pour elles. Si vous avez ordonné les fonctionnalités par valeur décroissante, vous aurez 80 % à 90 % de valeurs de disponible bien avant la date de livraison.

Les bonnes équipes agiles livrent avant la date de livraison. Les équipes à la hauteur livrent à la date de livraison. Si vous ne pouvez pas livrer à la date de livraison, quelque chose va mal et vous auriez dû vous en apercevoir foutrement bien avant la date finale.

## Satisfaction client - 21 %

Waow, voici qu’au numéro 7, nous trouvons la satisfaction client. Génial. Bien sûr, c’est difficile à mesurer (à moins que vous ne livriez aux clients très fréquemment). Bien sûr, c’est un indicateur un peu à la ramasse (à moins que vous ne leur livriez très fréquemment). Et, cet indicateur mesure, bien sûr, la qualité de vos propres décisions métiers, mais peut-être que ce que vous devriez faire finalement c’est de blâmer les développeurs pour la piètre qualité de leurs propres décisions sur ce qu’il y a à faire.

Toutefois, c’est une métrique convenable, bien qu’elle puisse être difficile à mesurer et à gérer.

## Maintenant j’accélère …

Regardons un peu plus rapidement les éléments restants sur la liste de VersionOne :

Le _travail en cours_ est une bonne chose à regarder. S’il est élevé, le travail reste alors en attente et les gens ont tendance à changer de tâches. Et c’est comme ça que les choses ralentissent et que vous rajoutez plus d’anomalies, donc garder un TEC [^1] aussi bas que possible est une bonne chose. Utilisez le TEC comme d’un signal pour voir si vos équipes ne sont pas aussi pluri-disciplinaires qu’elles pourraient l’être.

Les indicateurs des _anomalies en production_ et des _anomalies dans le temps_ valent le coût d’être suivis. De bonnes équipes agiles livraient peut être 10% ou moins d’anomalies avant de devenir agiles. Si le nombre d’anomalies ne baissent pas lorsque vous devenez agiles, réfléchissez à envoyer vos équipes à des ateliers de pratiques agiles de développement logiciel comme le développement piloté par les tests et le _refactoring_. Si les anomalies montent en flèche, vos équipes doivent resserrer les boulons sur les tests et le _refactoring_. Une des causes typiques d’une piètre qualité est de mettre la pression pour aller plus vite. C’est pourquoi mesurer des choses comme la vélocité est presque toujours négative.

_Budget vs coût réel_ est un indicateur un peu étrange. Le budget d’une équipe de développement logiciel est dominé dans le temps par les salaires. La seule manière vous permettant de dépasser le budget sur un mois donné, toute proportion gardée sur le degré de dépassement, est en embauchant accidentellement plus de personnes que prévu. C’est une erreur de budget ou d’encadrement, et non un problème d’équipe. À moins que vous ne les envoyiez à trop de réunions à Aruba, il y a peu de chances que ce soit une métrique utile.

L’indicateur _résolution des anomalies_ est également étrange. Évitez les anomalies, ne les résolvez pas. Toutefois, si vous avez trop d’anomalies pendant que vous êtes en train de travailler au renforcement des tests en vue de diminuer le taux d’anomalies, alors regardez  la durée que cela prend à l’équipe pour résoudre les anomalies. Si la durée pour corriger les anomalies s’allonge, prenez en considération que vous ne priorisez peut-être pas correctement. Vous voulez que davantage d’anomalies soient corrigées ? Ajoutez donc dans le _backlog_ plus d’items de corrections d’anomalies.

Attendez, hein ? quoi ? Vous pensiez que le _product owner_ devrait seulement empiler de nouvelles stories et que l’équipe devrait corriger comme par magie les anomalies pendant son temps libre pantagruélique. Vous vous êtes trompé. En tant que _product owner_, votre boulot est de présenter à l’équipe tous les items du backlog sur lesquels reposent les fonctionnalités qui doivent être faites. D’un côté, les nouvelles fonctionnalités, de l’autre les corrections à apporter aux anciennes : c’est à vous de décider.

La seule chose positive concernant l’indicateur _précision de l’estimation_ est d’être à la 13ème place. Tout d’abord, vous ne voulez pas vraiment de la précision. Si l’équipe pouvait faire tout le boulot en moins de temps qu’il n’en faut pour l’estimer vous seriez heureux, même si cette estimation s’avère complètement imprécise. Par conséquent, toutes les estimations faites par l’équipe seront plus élevées et vous serez heureux. La précision de l’estimation est donc une métrique bidon.

De nos jours, les meilleurs équipes n’estiment plus du tout au niveau de la story. Elles découpent les stories, elles les font, elles les réalisent, elles les font fonctionner et elles les terminent, finis.

_Valeur métier livrée_ Super ! Enfin une bonne idée. C’est vraiment dommage qu’elle soit en numéro 14 de la liste. Comment améliorez-vous la valeur métier livrée ? Vous donnez à l’équipe du travail à faire qui a de la valeur. Comme votre idée la meilleure vaut probablement 100 fois plus que votre idée la plus mauvaise, réaliser les stories dans l’ordre des plus au moins importantes est bien le meilleur plan possible. Et au sujet des dates de livraison, reportez-vous aux paragraphes précédents.

_Suivi des heures individuelles par itération/semaine_. Est-ce que vous êtes vraiment sérieux ??? Pensez-vous vraiment que faire travailler les gens plus d’heures vous permettra de faire faire plus de travail à des niveaux de qualité acceptables ? Sortez d’ici, vous n’êtes pas assez qualifié pour utiliser le mot “Agile” sur votre CV. Non, sérieusement, barrez-vous de là.

Le _temps de cycle_, par contre, peut être utile. Combien de temps cela prend-il pour une story de sa prise en charge par l’équipe à sa réalisation ? Plus de deux jours ? Alors c’est qu’elle est probablement trop grosse ou insuffisamment comprise. Combien de temps cela prend-il de la spécification d’un besoin important à son arrivée dans les mains de l’équipe ? Vous avez alors un problème de priorité. À moins que la story ne soit pas vraiment importante. Considérez donc le flux réel de valeur partant de l’idée jusqu’au client. Quelle est la proportion revenant à l’équipe ? Quelle est la proportion pour le reste de l’entreprise ? Corrigez ce qui ne va pas.

Le _Taux de réussites/d’échecs des tests dans le temps_ peut sembler intéressant mais je pense qu’il s’agit là d’un faux problème. À moins que vous ne trainiez un énorme boulet d’anomalies dès le début, les tests devraient toujours être au vert et le nombre de tests dans le système devraient augmenter de manière linéaire en corrélation avec le nombre d’items du backlog. Si vous avez des tests au rouge pendant un certain temps, vous avez un problème. Utilisez donc ça comme d’un sujet de rétrospective, non comme d’un sujet de mesure d’équipe.

Le _changement de périmètre dans une livraison_ est intéressant. Mais cela semble suggérer que vous étiez supposé connaître à l’avance ce que vous deviez construire et que d’une manière ou d’une autre vous vous êtes trompé. Eh oui, bordel. Votre boulot en tant que _product owner_ est de livrer les items du backlog ayant le plus de valeur d’abord. Cela afin d’obtenir le plus grand retour possible sur le travail de l’équipe de semaine en semaine. Il ne s’agit pas de pomper à travers une liste fixe de choses à faire, et il ne s’agit pas de prévoir à l’avance, si ce n’est uniquement en termes très généraux, ce qui sera fait. Si vous suivez les changements de périmètre dans une livraison, alors surtout ne vous montrez pas à la prochaine conférence agile, à moins que vous ne vouliez que je vous arrache votre badge agile de votre t-shirt.

Le _diagramme de flux cumulatif_ pourrait être intéressant. Je suggèrerais de faire figurer à la fois le nombre de stories, qui devraient augmenter grosso modo de manière linéaire au fil du temps et la valeur, qui devrait lui diminuer (parce que vous faites les choses les plus importantes d’abord, vous vous souvenez ?). Si votre nombre de stories diminue, vous avez de quoi vous mettre sous la dent pour une prochaine rétrospective. En aucun cas, vous n’aurez matière pour comparer des équipes entre elles. Par contre, vous pourriez avoir matière pour comparer des idées de produits entre elles.

La _valeur gagnée_ est un indicateur répandu dans certaines grandes organisations. Elle est vue par certains comme d’un moyen utile pour comparer la quantité de travail fait dans le temps et le budget imparti. Je pense que cela fonctionne bien probablement pour construire un pont ou une route. Cet indicateur, demande toutefois d’avoir un plan détaillé à l’avance. Si vous avez un plan détaillé à l’avance, il y a peu de chance que vous fassiez vraiment de l’agilité, même si vous utilisez quelques techniques comme les sprints ou même du temps qui vous font croire que vous êtes agile.

En supposant un budget en personnel fixe, la valeur gagnée sera représentée généralement par une ligne droite par rapport au temps ou au budget. Cela suppose donc un accroissement linéaire de la “valeur”. Étant donné que vous prenez les items du backlog ayant le plus de valeur d’abord, votre valeur gagnée devrait être connue d’avance pendant toute la durée du projet. Et cela, si vous êtes bien entendu vraiment bon à la budgétisation du coût des fonctionnalités que vous ne construirez jamais. Il est toutefois possible d’estimer combien de temps cela prend pour construire un pont ou une route. (Ajoutez ici votre propre liste de construction de ponts et de routes ayant dépassé le budget). Il est quasiment impossible de budgéter combien de fonctionnalités d’un nouveau produit vous pouvez faire avec une nouvelle équipe. Il peut toutefois être possible de budgéter un produit qui soit similaire à un autre que vous venez juste de réaliser.

Vous avez peut être commencé à comprendre que je n’ai pas grand chose à cirer de la valeur gagnée. C’est vrai. Je connais une personne, qui elle, je pense y est plutôt bonne. Si vous voulez que je vous mette en contact avec elle, faites-le moi savoir. Mais à moins que vous ne soyez obligé par le règlement intérieur d’utiliser la valeur gagnée, ne l’utilisez pas, tout simplement.

La _rétention client_ est une idée sympa. Mais c’est un indicateur à la ramasse, difficile à mettre en relation avec vos décisions, et tout aussi peu utile qu’un autre indicateur client auquel vous pourriez penser.

L’_impact sur les ventes/revenus_ est aussi vraiment à la ramasse et difficile à mettre en relation avec chacune des décisions prises sur le produit. C’est certainement quelque chose à surveiller mais je ne vois vraiment pas comment il peut être en relation à l’agilité.

L’_utilisation du produit_ peut être un super indicateur. Je connais une entreprise qui, dans un contexte publicitaire, suit le nombre de clics sur chacune des fonctionnalités. Ils ont trouvé cela intéressant en pensant comment cela pouvait servir le domaine de la publicité. Et la plupart d’entre nous savons bien qu’il y a une fonctionnalité à laquelle nous aimerions bien échapper dans les applications que nous utilisons au quotidien. Donc si vous suivez l’utilisation à un niveau suffisamment fin et suffisamment proche de vos décisions, vous pourriez apprendre comment prendre de bonnes décisions.

##D’accord Ron, y’a t’il UNE métrique qui trouve grâce à tes yeux ?

Pour comparer une équipe à une autre ? Je n’aime pas beaucoup les métriques car comparer les équipes les unes aux autres c’est pire que comparer des pommes ou des oranges. Au moins les pommes et les oranges sont des fruits et qu’elles sont à peu près de forme ronde. Les équipes, pas vraiment. Néanmoins, je me rappelle d’une comparaison d’équipe qui a donné quelque chose de positif :

> À l’époque chez Atlas, lorsqu’ils existaient encore, il y avait plusieurs services informatiques qui faisaient quelque chose qui ressemblait à du scrum. La plupart des équipes avaient appris à faire de petites stories et cela les aidait bien, parce que de petites stories focalisent généralement mieux votre attention, vous aident à mieux sélectionner ce qui a de la valeur, et vous aident à voir comment vous vous débrouillez. Toutefois, une équipe, une espèce de département système, continuait à faire de grosses stories prenant des mois à aboutir. Quelques soient les conseils, cela n’y changeait rien.
>  
> Puis, Nathan McCoy, qui était en charge de toutes les équipes commença à montrer dans ses comptes-rendus mensuels, un simple graphe illustrant le nombre de stories faites par chaque équipe. Le responsable système y fit objection parce que cela montrait une mauvaise image de lui. Les autres équipes faisaient dix ou vingt choses, et lui pouvait n'en faire qu'une par mois. La conversation que me rapporta Nathan prit la tournure suivante :
>  
> Responsable : “Nathan, ce n’est pas juste. Tu montres seulement le nombre de stories et non pas leur taille.”  
> Nathan : "C'est vrai"  
> Responsable : "Mais ce n'est pas juste !"  
> Nathan : [silencieux]  
> Responsable : "Tous ce que j'ai à faire c'est de couper mes stories en petits morceaux et de livrer tous les mois."  
> Nathan : [silencieux, souriant]  
> Responsable : "Oh"

Il est à noter que des indicateurs comparatifs vont rentrer en conflit, donc vous devez faire très attention quand vous les mettez en place, parce qu’ils vont rentrer en conflit … d’une manière ou d’une autre.

##Toutefois, en interne de l’équipe …

Quand l’équipe choisit des métriques lui permettant de savoir comment elle se débrouille, je suis tout à fait partant. En voici quelques-unes que je trouve utile.

Un _graphique du nombre de tests par rapport au nombre de stories réalisées_ Cela donnera un rapide aperçu si l’équipe essaye d’aller trop vite.

_Dessinez une petite zone sur le tableau blanc_. Lorsqu’une partie du code a besoin d’amélioration, mettez une note adhésive dans ce carré. C’est une manière rapide pour l’équipe d’indiquer quand elle rencontre un code alambiqué. Vérifiez cette zone à chaque rétrospective. Foncez faire du refactoring lorsqu’elle commence à se remplir. Et il est important que la zone soit vraiment “petite”. Peut-être 30 cm de côté si vous utilisez des règles des notes adhésives de 7 cm de côté.

Un _graphique du nombre de tests d’acceptance écrits par rapport à ceux qui sont au vert_ J’ai déjà vu ce graphique montrer à une équipe que celle-ci avait effectivement des tests écrits mais qu’elle n’avait pas eu les réponses “correctes” à ceux-ci de la part de l’équipe du _product owner_. Vous pourriez donc le trouver utile.

La _vélocité_ en terme de stories faites est tout à fait valable. Elle montera et descendra et vous pourrez bien apprendre quelque chose si vous réfléchissez dessus. Toutefois, soyez très prudent : ne regardez pas l’effort d’un travailleur ou d’une équipe ou quoi que ce soit de ce genre. Mais lorsque la courbe de progression change, vous êtes en train d’observer _quelque chose_. Profitez de la rétrospective pour trouver ce que c’est.

Cet article, [de gros graphiques bien visibles](http://www.ronjeffries.com/xprog/articles/bigvisiblecharts/), paru il y a quelques temps, pourrait vous donner des idées. Aujourd’hui, je pourrais peut-être déceler des problèmes dans certains d’entre eux que je n’avais pas vu lorsque j’ai écris cet article à l’époque en 2004 et notamment sur leur mauvaise utilisation éventuelle.

De manière générale, soyez très prudent en essayant de mesurer une équipe avec des métriques. Utilisez des métriques pour suivre des choses que l’équipe devra regarder par la suite. En tout cas, vous ne devriez certainement pas du tout les utiliser pour comparer les équipes entre elles.

[^1]: TEC : travail en cours ou WIP (Work in progress) pour les lecteurs et lectrices préférant l’acronyme anglophone

---
Auteur : [Ron Jeffries](http://ronjeffries.com/about.html)  
Source : [Do you want Crappy Agile?](http://ronjeffries.com/articles/016-03/you-want/)  
Date de parution originale : 29 Mars 2016  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 27/04/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

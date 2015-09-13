---
layout: post
title:  "Les story points considérés comme dangereux - ou pourquoi le futur de l'estimation se situe vraiment dans notre passé ..."
date:   2015-09-13 21:00:55
published: true
categories: 
- estimation
---

Cet article est le pendant de la [conférence](http://www.sigs-datacom.de/oop2012/oop2012-eng/conference/sessiondetails.html?tx_mwconferences_pi1[showUid]=818&tx_mwconferences_pi1[anchor]=%23Ndo3&tx_mwconferences_pi1[s]=0) donnée par [@josephpelrine](https://twitter.com/josephpelrine) et moi-même lors de l'OOP 2012.

 <div align="right" style="float:right; padding-left:30px" >
  <img title="Nébuleuses" src="{{ site.url }}assets/points_story_dangereux/Stars_banner.jpg" />
</div>

Nous avons beaucoup à apprendre de nos ancêtres. Celui dont je veux parler plus particulièrement dans cet article est [Galilée](https://fr.wikipedia.org/wiki/Galil%C3%A9e_%28savant%29).
Galilée a été ce que nous appellerions aujourd'hui un technophile[^1]. Il aimait tout ce qui était techno et un jour, il lui fut présenté une technologie intéressante qu'il ne pouvait pas ignorer. Grâce à elle, il développa la technologie optique pour construire d'abord le téléscope et plus tard le microscope. Grâce à l'utilisation du télescope et d'autres approches, il en arriva à la découverte et à la défense d'une conception [héliocentrique](https://fr.wikipedia.org/wiki/H%C3%A9liocentrisme) de l'univers : la Terre n'était pas le centre de l'univers, mais tournait autour du Soleil.
Cette découverte ne provoqua pas de controverse jusqu'à ce que Galilée l'écrivit, discréditant de manière manifeste, la conception défendue par l'Église à cette époque. L'Église croyait et défendait la conception que l'univers était tout entier organisé autour de la Terre et que toute chose tournait autour de notre planète.
Nous savons maintenant que Galilée avait raison et que l'Église avait - comme souvent cela à tendance à être le cas avec les croyances - tort. De nos jours, nous disons de manière évidente que la Terre est ronde et tourne autour du Soleil. Ou est-ce que nous ...

[^1]: certains diraient geek - NdT

## La Flat Earth Society

En fait, il y a encore des gens autour (bizarre comme mot, hein ?) du globe qui ne croient même pas que la terre soit ronde !  Vous ne me croyez pas ? Alors regardez par vous même la [Flat Earth Society](https://fr.wikipedia.org/wiki/Flat_Earth_Society).

Le fait est que même aujourd'hui, il y a beaucoup de gens qui ont des croyances sur la manière dont réellement notre monde tourne. Ou nos projets dans le cas de cet article ...

## La soupe de l'estimation

Nous avons tous été confrontés à différentes techniques d'estimation que ce soit dans un projet agile ou traditionnel. En voici quelques unes qui me viennent tout de suite à l'esprit : estimation par un expert, estimation par consensus, analyse par point de fonction, etc ... Puis nous avons les techniques d'estimation du coût (par opposition à celui portant uniquement sur le temps ou la durée) : COCOMO, SDM, etc ... Et bien sûr, **le sujet de cet article : l'estimation en story points. Qu'ont en commun toutes ces techniques ? Elles regardent toutes vers le futur !**  
Pourquoi cette caractéristique est-elle importante ?

## La condition humaine

Ce n'est pas parce que prédire l'avenir est toujours difficile ! Nous, humains excellons à anticiper les évènements immédiats dans le monde physique, mais dans le monde du logiciel, ce que nous estimons, n'est ni immédiat, ni ne suit aucune des lois physiques que nous comprenons intuitivement !
Prenez l'exemple du gardien de but dans un match de football. Il peut facilement prédire comment une simple frappe propulsera le ballon vers les buts, et il pourra faire cela avec une assez bonne précision (comme le prouve les scores généralement bas des matchs de football aujourd'hui). Mais même au football, lorsque vous êtes face à un joueur comme [Maradona](http://fr.wikipedia.org/wiki/Diego_Maradona), ou [Beckham](http://fr.wikipedia.org/wiki/David_Beckham), ou [Cristiano Ronaldo](http://fr.wikipedia.org/wiki/Cristiano_Ronaldo), la trajectoire de la balle devient très difficile à prévoir. Certains physiciens ont passé un temps considérable  à analyser la trajectoire des coups francs de Beckham pour essayer de comprendre comment la balle se déplaçait et pourquoi. De manière évidente, un gardien de but n'a pas les ordinateurs ou le temps d'analyser la trajectoire des coups francs de Beckham, ce qui a permis à Beckham de marquer par conséquent un certain nombre de buts de cette manière. **Même au football, où des lois bien connues de la physique s'appliquent, il y a des fois où cela devient difficile de prédire le futur proche !**
C'est un fait indiscutable que nous, humains, sommes très mauvais à prédire le futur.
Mais ce n'est pas tout !

## C'est maintenant que les choses deviennent complexes

Dernièrement, et tout spécialement dans le domaine agile, nous avons trouvé un nouveau champ d'étude : les sciences de la complexité.
Il s'agit d'un champ d'étude qui essaye d'identifier les règles qui nous permettent de nous déplacer dans un monde où la causalité même (cause et effet) est remise en question.
Un exemple dont vous avez peut être entendu parler est l'effet papillon : "où un petit changement quelque part dans un système non linéaire peut avoir comme résultat des conséquences importances à un stade ultérieur". Les sciences de la complexité nous permettent d'accroître notre compréhension du développement logiciel sur la base des théories développées ces dernières années.
Scrum est le parfait exemple d'une méthode qui a utilisé la complexité pour s'inspirer et justifier son approche sur beaucoup des problèmes auxquels nous sommes habituellement confrontés dans le développement logiciel.
Scrum a utilisé "l'auto-organisation", et "l'émergence" comme concepts pour expliquer pourquoi l'approche Scrum fonctionne. Et voici le problème : il y a un piège.

## Pourquoi est-ce que c'est arrivé ?

Dans un environnement complexe, nous n'avons pas de causalité discernable !
Quelque fois cela est dû aux conséquences retardées de nos actions, d'ailleurs c'est tellement le cas que le plus souvent nous attribuons la causalité des évènements dans le passé alors qu'en fait il n'y a aucune relation de cause à effets (cohérence rétrospective). Mais dans le domaine de l'estimation, cela se manifeste d'une autre manière.
Afin que nous puissions estimer, nous devons supposer que la causalité existe (si je demande à Tom de faire une revue de code, alors Helen sera contente que je sois pro-actif et me donnera un bonus. N'est-ce pas ?) Le fait est : que dans un environnement complexe, la présomption de base est que l'existence d'une causalité discernable n'est pas valable ! **Sans causalité, l'hypothèse fondamentale justifiant l'estimation tombe à plat !**

## Résoudre le manque de cohérence interne de Scrum

Alors, quel est-il ? Avons-nous un environnement complexe dans le domaine du développement logiciel ou pas ? Si nous en avons un alors nous ne pouvons pas - en même temps - argumenter en faveur de l'estimation (et bâtir toute une religion dessus) ! À contrario, si nous ne sommes pas dans un environnement complexe nous ne pouvons pas alors proclamer que Scrum - avec son accent mis sur la résolution de problème dans un domaine complexe - puisse fonctionner !
**Alors, la question pour nous est la suivante : Est-ce que cette estimation basée sur des story points est-elle si importante au point d'être promue et citée dans toute la littérature scrum ?**
Heureusement, nous avons une alternative simple autorisant l'existence d'un environnement complexe et qui résout les mêmes problèmes que ceux pour lesquels les story points ont été conçus (mais qui eux ont échoués).

## L'autre moyen de prédire

L'alternative à l'estimation en story points est simple : compter seulement le nombre de stories que vous avez terminées (comme étant "finies") dans les itérations précédentes. Elles sont le meilleur indicateur d'une performance future ! Utilisez alors cette information pour prévoir les futures avancées. À la base le meilleur indicateur du futur est votre performance passée !
Est-ce vraiment aussi simple ? Pour tester cette approche, j'ai examiné les données de différents projets et j'ai essayé de répondre à quelques simples questions. 
 
## L'expérience

* Q1 : Existe-t-il une différence significative entre ce que les story points et le "nombre d'éléments" mesurent pour dire qu'ils ne mesurent pas la même chose ?
* Q2 : Laquelle de ces deux métriques est la plus stable ? Et qu'est-ce que cela signifie ?
* Q3 : Est-ce que ces métriques sont assez proches afin que la mesure de l'un (le nombre d'élément) soit équivalente à la mesure de l'autre (story points) ? 

J'ai examiné les données de 10 équipes différentes de 10 projets différents. Je ne faisais pas partie d'aucun de ces projets (j'ai récupéré ces données auprès des équipes directement ou par le biais de demandes d'informations à des listes de diffusion sur l'agilité). Un autre point à souligner est que ces données viennent d'entreprises de tailles différentes aussi bien que d'équipes de tailles différents et de projets différents.
Et voici ce que j'ai trouvé :

* Sur la question 1 : j'ai remarqué qu'il y avait une corrélation constante allant de moyenne à élevée entre l'estimation en story points et le simple dénombrement de stories terminées (0,755; 0,83; 0,92; 0,51(!); 0,88; 0,86; 0,70; 0,75; 0,88). Avec une corrélation si élevée, il est probable que les deux métriques représentent le signal d'une même information sous-jacente.
* Sur la question 2 : Les données normalisées (normalisées pour la durée d'un sprint ou d'une itération) ont la même valeur d'écart-type (tout aussi constante). Cela m'amène à conclure qu'il n'y a pas de différence significative de constance entre l'une ou l'autre de ces métriques. Même si en valeurs absolues les estimations en story points varient plus entre deux itérations que le nombre de stories terminées/finies.
* Sur la question 3 : Les deux métriques (les points de stories terminées par rapport au nombre de stories terminées) semblent mesurer la même chose. Donc ...

À partir de là, je me suis intéresser à l'analyse des arguments justifiant l'utilisation des story points, comme les données précédentes ne semblaient pas donner un avantage significatif pour l'utilisation des story points comme métrique. J'ai donc cherché une publication justifiant l'utilisation des story points et j'ai trouvé un ensemble d'arguments dans le livre "User Stories Applied" (page 87, 1ère édition) de Mike Cohn.

* Argument 1 :  L'utilisation des story points nous permet de changer d'avis lorsque nous avons une nouvelle information sur une story
* Argument 2 : L'utilisation des story points fonctionne à la fois pour les _epics_ et les stories plus petites
* Argument 3 : L'utilisation des story points ne prend pas beaucoup de temps
* Argument 4 : L'utilisation des story points donne des informations utiles sur notre progression et le travail restant à faire
* Argument 5 : L'utilisation des story points tolère une certain imprécision dans les estimations
* Argument 6 : L'utilisation des story points peut être utilisée pour planifier les livraisons

Est-ce que ces arguments tiennent ?

## Argument 1 : L'utilisation des story points nous permet de changer d'avis lorsque nous avons une nouvelle information sur une story

Même s'il n'y a pas d'explications sur ce que "changer d'avis" veut dire dans le livre, nous pouvons en déduire que l'objectif n'est pas de passer trop de temps à essayer d'être exact. La raison de ceci est, bien sûr, que si la story change de taille légèrement, il n'y a aucun impact sur l'estimation en story points, mais et si la story change radicalement de taille ?
Eh bien, vous voudriez probablement avoir à ce moment-là une nouvelle session d'estimations, ou vous voudriez scinder cette story en stories plus petites pour avoir une meilleure idée de sa taille et de son impact réel sur le projet.
D'un autre côté, si nous devions utiliser une simple métrique comme le nombre de stories terminées, nous serions capable d'évaluer immédiatement l'impact de nouveaux éléments dans l'avancée du projet.

<div align="right" style="float:right; padding-left:30px">
  <img title="Graphique" src="{{ site.url }}assets/points_story_dangereux/graphique_argument_1.png" />
</div>

Comme illustré dans le graphique, si nous avons un certain nombre de stories à terminer (80 dans notre exemple) et que brusquement 40 sont ajoutées dans notre backlog (à partir de la scission d'un _epic_ par exemple) nous pouvons voir facilement l'impact que cela peut avoir sur l'avancée de notre projet.
Dans ce cas, comme nous pouvons le voir à partir du graphique, la modification de la signification d'une story ou la division d'une grosse story en plus petites stories a un impact sur le projet et nous pouvons le voir directement sur le graphique.
Cela m'amène à conclure que **sur l'argument 1, les story points n'offrent aucun avantage sur le simple dénombrement du nombre d'éléments restant à finir**.

## Argument 2 : L'utilisation des story points fonctionne à la fois pour les _epics_ et pour les plus petites stories

Autoriser de grosses estimations pour des items dans le backlog (disons par exemple un _epic_ à 100 PS) aide à prendre en compte d'une certaine manière l'incertitude que de grosses quantités de travail représentent. Toutefois, la même incertitude existerait quelque soit la manière dont nous pourrions mesurer l'avancée. Le fait est que nous ne savons pas vraiment si un _epic_ (disons de 100 PS) est réellement équivalent à une somme équivalente d'un ensemble de user stories (100 stories de 1 PS). **Conclusion : il n'y a aucun ajout d'information significative en classifiant une story dans la catégorie des 100 PS** ce qui veut dire qu'appeler quelque chose un "_epic_" donne à peu près la même information que la classifier comme un _epic_ de 100 story points.

## Argument 3 : l'utilisation des story points ne prend pas beaucoup de temps

Pour avoir travailler avec des story points pendant plusieurs années, cela n'est pas mon expérience. Même si des progrès ont été faits par des personnes comme Ken Power (à Cisco) avec la [technique du regroupement en silence](http://fr.slideshare.net/kenpower/using-silent-grouping-to-size-user-stories-xp2011), le fait même que nous ayons besoin d'une technique de ce genre devrait remettre en cause toute idée qu'estimer en PS "ne prend pas beaucoup de temps". En fait, comme toute personne s'étant frottée à un projet non-trivial, le sait, cela peut prendre des jours de boulot d'estimer le backlog initial d'un projet de taille raisonnable.

## Argument 5 : L'utilisation des story points tolère une certaine imprécision dans les estimations 

Bien que vous puissiez discuter le fond-même de cet argument - même si le livre n'explique pas comment - il n'y a aucune donnée justifiant la croyance que les story points font cela mieux que compter le nombre de stories finies. En fait, nous pouvons argumenter que compter le nombre de stories est même plus indulgent sur les imprécisions (voir ci-dessous pour plus de détails là-dessus)

## Argument 6 : Les points de stories peuvent être utiliser pour planifier les livraisons

C'est plutôt exact. D'un autre côté, nous pouvons utiliser n'importe quelle technique d'estimation pour faire cela, donc par quel moyen les story points seraient-ils meilleurs dans ce cas particulier que n'importe quelle autre technique d'estimation ? De même, comme nous le verrons dans l'analyse de l'argument 4, compter le nombre de stories finies (et celles restant à finir) est une manière très efficace de planifier une livraison (soyez patient, un exemple arrive)

## Argument 4 : L'utilisation des story points donne des informations utiles sur notre avancée et le travail restant à faire 

Cet argument est vrai **si, et seulement si** vous avez estimé toutes vos stories dans le backlog et que vous avez répété le même processus pour chaque nouvelle story ajoutée dans le backlog. Même les stories, qui seront développées dans quelques mois ou même un an plus tard (pour de longs projets), devront être estimées ! Cette approche n'est pas très efficace (ce qui en fait contredit l'argument 3).
Baser votre avancée sur le nombre d'items réalisés à chaque sprint est plus rapide à calculer (nombre d'items dans votre _product backlog_ / vélocité du nombre d'items finies par sprint = nombre de sprints restants) et peut être utilisé pour donner des informations vitales sur l'avancée du projet. Voici un exemple réel.

## L'utilisation réelle d'une métrique plus simple pour mesurer l'avancement d'un projet 

Dans une entreprise dans laquelle je travaillais, nous avions un produit qui allait arriver sur le marché. Il n'était pas le "premier arrivé" ce qui veut dire que la barrière à franchir pour entrer sur le marché était assez élevée (du moins c'était ce que croyait la direction produit et commerciale).
Cela signifie qu'un effort significatif était fait pour arriver à un _product backlog_ cohérent. Le backlog était revu par les personnes des ventes et avant-ventes (technico-commercial). Toutes étaient d'accord, nous devions vraiment livrer environ 140 stories (pas des points, des stories) pour être compétitif. Comme nous n'étions pas les premiers sur le marché nous avions une petite fenêtre de tir. Rater cette fenêtre signifierait invalider le fait-même d'entrer sur le marché.
Donc, nous avons commencé le projet et lors du premier sprint nous avons réalisé 1 seule story (peut être s'agissait-il d'une grosse story -- la vérité est que je ne me souviens plus). Pire, dans la même période 20 stories supplémentaires furent ajoutées dans le _product backlog_. Comme on pouvait s'y attendre, la direction produit et commerciale a découvert quelques stories de plus qui étaient vraiment "indispensables" et qui ne pouvaient pas être mises de côté.

L'équipe gagnait en rapidité et au seconde sprint elle avait 8 stories de "finies". L'équipe était heureuse. En même temps le responsable produit et commercial donna son accord pour une version réduite du _product backlog_ et enleva environ 20 stories du backlog.
Après le troisième sprint l'équipe avait donc atteint les vélocités de 1 (au premier sprint), de 8 (au second) et de 8 (au troisième). Le quatrième sprint allait commencer et la pression était forte sur l'équipe et sur le responsable produit. Pendant la réunion de planification du sprint, l'équipe s'était engagée sur 15 nouvelles stories. C'était un bon chiffre, une vélocité de 15 ferait croire aux parties prenantes que le projet pourrait réellement livrer le produit demandé. L'équipe devrait garder une vélocité de 15 stories par sprint pendant 11 mois. Pourrait-elle y arriver ?

## L'apogée

Alors que le quatrième sprint démarrait, je fis un pari avec le responsable produit. Je lui ai demandé combien d'items il croyait que l'équipe pourrait réaliser et il dit 15 (exactement le même nombre auquel l'équipe s'était engagée). N'étant pas d'accord, je lui répondit 10. Combien d'items diriez-vous que l'équipe pu réaliser ?
Je pose cette question à tout le monde à chaque fois que je raconte cette histoire. J'ai eu différente réponses. À chaque fois, un 42 fuse de l'assemblée comme réponse possible (on s'y attend un peu étant donné le public auquel je parle habituellement), mais la plupart répondirent 8, 10, quelques-uns peuvent dire 15 (très peu), d'autres disent 2 (très peu). Le consensus semble tourné autour de 8-10.
Arrivé à ce moment-là, je demande aux personnes du public pourquoi elles diraient 8-10 au lieu de 15 comme le responsable produit de cette équipe lui le disait. À priori, le responsable produit connaissait mieux son équipe et le contexte, non ?
À la fin du quatrième sprint, l'équipe réalisa 10 items, qui même si c'était 20% de mieux que ce qu'elle avait réalisé les précédents sprints est tout de même très loin de la vélocité dont elle avait besoin pour faire de ce projet un succès. La direction réfléchit à la situation et décida clairement que la meilleure décision pour l'entreprise était d'abandonner le produit. 

## Le mythe des story points : brisé !

Cette entreprise a prit une décision extrêmement difficile basée sur des données, pas sur les spéculations des responsables projets, non basée sur une estimation fallacieuse utilisant une technique quelconque. De vraies données. Elle a regardé les données qui étaient disponibles et a décidé d'abandonner le projet 10 mois avant la livraison planifiée à l'origine. Ce projet avait une équipe d'environ 20 personnes. Abandonné, ce projet a fait économisé à l'entreprise 200 mois-homme d'investissement dans un produit qu'elle n'avait aucun espoir de pouvoir faire sortir à temps !
Nous avons évité un projet à marche forcée et nous avons été capable de nous concentrer sur d'autres produits plus importants pour l'avenir de l'entreprise. Produits, qui aujourd'hui, rapportent de l'argent de manière significative !  

## OK, je comprends votre point de vue, mais comment cette technique fonctionne-t-elle ?

La plupart des gens seront sceptiques à partir de maintenant (si vous avez lu jusqu'ici vous l'êtes probablement aussi). Aussi laissez-moi expliquer comment cela fonctionne.
N'estimez pas la taille d'une story au-delà de ce qui suit : lorsque vous faites de l'affinage de backlog ou une planification de sprint, posez-vous simplement la question : est-ce que cette story peut être réalisée en un sprint par une personne ? Dans la négative, scindez-la !
Pour des projets de taille plus importante, utilisez un niveau d'abstraction supplémentaire : les stories s'inscrivent dans des sprint, par conséquent, les _epics_ s'inscrivent dans des meta-sprints (un meta-sprint vaudra 4 sprints par exemple). Posez-vous la même question pour les _epics_ que celle que vous êtes posée pour les sprint (est-ce qu'une équipe peut implémenter cet _epic_ dans un demi meta-sprint, c'est-à-dire en 2 sprints ?) et scindez-le si nécessaire.

<div align="center">
  <img title="Graphique" src="{{ site.url }}assets/points_story_dangereux/median_story_size_graph.jpg" />
</div>

&nbsp;

En harmonisant en continu la taille de stories/_epics_, vous créez alors une distribution des tailles autour d'une médiane.

En partant d'une distribution normale des tailles des stories cela signifie que vous pouvez supposer l'estimation/l'avancée du projet **dans l'objectif de regarder vers le long terme** (rappelez-vous : cela s'applique seulement sur le long terme, c.à.d plus que 3 sprints dans le futur), **vous pouvez présumer que toutes les stories sont de la même taille**, et vous pouvez **par conséquent mesurer l'avancée du projet en mesurant le nombre d'items réalisés par sprint**.

## En conclusion

As with all techniques this one comes with a disclaimer: you may not see the same effects that I report in this post. That's fine. If that is the case please share the data you have with me and I'm happy to look at it.
My aim with this post is to demystify the estimation in Agile projects. The fact is: the data we have available (see above) does not allow us to accept any of the claims by Mike Cohn regarding the use of Story Points as a valid/useful estimation technique, therefore you are better off using a much simpler technique! Let me know if you find an even simpler one!

Comme pour toutes les autres techniques, celle-ci comporte un avertissement : vous pourriez ne pas voir les mêmes effets que ceux que j'ai pu rapporter dans cet article. C'est tout à fait possible. Si c'est le cas, je vous prie de bien vouloir partager vos données avec moi et je serai heureux de les examiner.
Mon objectif avec cet article est de demystifier l'estimation dans les projets agiles. Le fait est que : les données dont nous disposons (voir ci-dessus) ne nous permettent pas d'accepter les arguments de Mike Cohn sur l'utilisation des story points comme étant une technique valide ou utile, par conséquent vous feriez mieux d'utiliser une technique beaucoup plus simple ! Faites-moi savoir si vous en avez trouvé une encore plus simple !

Oh, et puis en passant : arrêter de perdre du temps à estimer un backlog sans fin. Il n'y a aucune preuve que cela vous aidera à prédire le futur mieux que simplement compter le nombre de stories "finies" !

## Comment appliquer le #NoEstimates [^2] pour améliorer l'estimation ? Voici comment ...

... en lisant ce [livre blanc](http://eepurl.com/TVCG1)

![livre blanc]({{ site.url }}assets/points_story_dangereux/livre_blanc.png")



&nbsp;  

[^2]: #NoEstimates est le mot-clé (hashtag) utilisé dans Twitter et qui est depuis le nom de ce mouvement de réflexion sur les estimations - NdT  

---
Auteur : [Vasco Duarte](https://plus.google.com/114992270681478709673)  
Source : [Story Points Considered Harmful - Or why the future of estimation is really in our past...](http://softwaredevelopmenttoday.blogspot.com.au/2012/01/story-points-considered-harmful-or-why.html)  
Date de parution originale : 25 Janvier 2012  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 13/09/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}


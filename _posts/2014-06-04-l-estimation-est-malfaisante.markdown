---
layout: post
title:  "L'estimation est malfaisante"
date:   2014-06-04 21:41:55
tags:
- estimation
- scrum
- xp
---
## Dépassez l'obsession de l'estimation

![Pretty image](http://a.pragprog.com/magazines/2013-02/images/iStock_000014698811Small__2j613e__.jpg)

> L'ignorance peut vous nuire, surtout lorsque vous vous êtes convaincu que vous la connaissiez.

L'application des valeurs, principes et pratiques agiles a apporté certaines améliorations à beaucoup d'équipes agiles - à la plupart des équipes agiles, je crois -.

Ces équipes font mieux pour prévoir le moment où elles auront terminé, et mieux pour terminer au moment où elles l'ont prévu. Elles décomposent les exigences dans un backlog, elles estiment la durée des items, et elles achèvent le contenu de ce backlog plutôt bien. Généralement, vers la fin du projet, elles sont plus proches d'avoir fini qu'elles ne l'étaient avant de devenir agiles.

Les équipes agiles décomposent et font souvent l'estimation de leur travail par période de quelques semaines. Généralement, elles font la plupart des choses qu'elles avaient prévues de faire pendant cette itération. Elles ont peu de retours d'anomalies, et se réunissent régulièrement pour essayer de s'améliorer.

Ces équipes sont plus transparentes, à la fois à l'intérieur de l'équipe, avec leur encadrement et avec les parties prenantes. Elles sont plus proches de livrer dans les délais qu'elles ne l'étaient auparavant. Elles ont moins d'anomalies à la livraison. Leur encadrement ressent qu'il a plus de contrôle sur ce qu'il se passe.

Les équipes appliquant les idées agiles en tirent toujours quelques améliorations. J'estime que l'amélioration globale due à Scrum - l'approche agile la plus populaire - est d'environ vingt pour cent par rapport à ce qu'elles faisaient avant.

Certaines équipes font beaucoup mieux, et nous parlerons de ce qu'elles font plus tard. Les équipes ayant de bons résultats, sans être mirifiques, sont ici notre principale préoccupation, parce qu'il y a certaines particularités à ce qu'elles font, des particularités qui les empêchent encore (de se réaliser - NdT).

Ces équipes sont meilleures qu'elles ne l'étaient, mais restent banales. Elles semblent avoir une préoccupation excessive pour un ou plusieurs des éléments suivants :

 * Finir un backlog prédéfini;
 * Livrer tout ce qui leur a été demandé pour une date donnée;
 * Estimer ce qu'elles peuvent faire toutes les deux semaines et tenir leurs promesses;
 * Améliorer la qualité de leurs estimations;
 * Expliquer les écarts entre les estimations et le réalisé;
 * Améliorer la vélocité, leur taux de réalisation de fonctionnalités.

En bref, ces équipes sont souvent préoccupées de manière excessive par l'estimation, et par se montrer à la hauteur de leurs estimations.

Ces préoccupations sont compréhensibles. L'expérience de la plupart des organisations avec le développement logiciel n'est pas bonne. Des promesses faites et non tenues. Des projets supposés être finis pour une certaine date glissent encore et encore, perdant un temps précieux et de l'argent. Quand les produits sont suffisamment finis pour être livrés, ils ne rencontrent pas la vision de ceux qui les ont demandés. Quand les utilisateurs commencent à l'utiliser, ils découvrent à ce qu'il semble être des omissions et des erreurs stupides.

Le développement logiciel a été plutôt une déception pour presque toutes les personnes qui ont pu croiser son chemin. C'est pourquoi nous lisons très régulièrement des choses comme la "crise logicielle".

Il semble alors assez naturel que nous demandions que les développeurs deviennent meilleurs à prévoir quand ils auront fini. Il est évident que nous utiliserons la transparence supplémentaire qu'offre les méthodes agiles pour garder un œil sur le développement et maintenir ainsi les développeurs sur des charbons ardents, afin d'être certains qu'ils feront ce qu'ils ont promis. Il est donc raisonnable de leur demander d'apprendre à mieux estimer et à apprendre à respecter ces estimations. Il est aussi de bon aloi de leur demander d'aller plus vite.

Cela semble naturel. Cela a du sens. C'est simplement raisonnable. C'est bien pensé. Le seul problème est que : c'est faux. C'est le genre de choses qui font qu'un projet agile est seulement vingt pour cent meilleure que ce qu'il était avant. Examinons pourquoi ceci nous entravent, et ce que nous pouvons faire à la place.

# Commençons avec toutes nos exigences sont fausses

Il fût enseigné à la plupart d'entre nous d'écrire toutes nos exigences au tout début du projet. Seulement, il y a là, trois choses fausses : "exigences", "au tout début", et "toutes". C'est au tout début du projet que nous en savons le moins sur celui-ci. C'est le pire moment possible pour prendre des décisions fermes sur ce que nous "exigeons".

Toute personne ayant jamais regardé une liste d'"exigences" a vu certains items qui étaient très importants, et d'autres qui n'étaient - eh bien - pas si importants. Pas si important dans le sens de 1% aussi important que les items les plus importants. Pas si important, comme des idées franchement mauvaises. Dans les listes d'exigences, il y a là de manière flagrante l'application de la règle des "80-20". L'essentiel de la valeur vient de la très petite sous-partie des soi-disant exigences. Par conséquent, les autres choses ne sont pas du tout des "exigences". Ce sont des idées, et certaines d'entre elles ne sont pas très bonnes. Comment pourraient elles-être bonnes ? Nous les avons eus avant que nous commencions le projet, lorsque nous en savions le moins.

Pire encore, lorsque nous écrivons nos "exigences", nous le faisons comme si c'était notre dernière chance de demander quoi que ce soit. Aussi, nous demandons tout ce à quoi nous pouvons penser, tout ce que nous pourrions avoir besoin. D'ailleurs, nous sommes sûr que nous n'aurons pas tout, alors autant demander le maximum avec l'espoir d'obtenir quelque chose, nous pouvons bien vivre avec ça.

# Estimer pour quand nous aurons fini est faux ; contraindre à répondre est pire

Alors nous demandons aux développeurs d'"estimer" pour quand ils auront fini tout ce boulot. Eux, aussi, connaissent moins le produit maintenant qu'ils ne le connaitront jamais, et ils ne comprennent pas très bien non plus la plupart des exigences. Mais ils font de leur mieux et ils arrivent avec une date. Est-ce que le métier accepte cette date ? Bien sûr que non ! Premièrement, parce que c'est seulement une estimation. Deuxièmement, parce que les développeurs se laissent clairement beaucoup de marge - ils le font toujours. Troisièmement, parce que cela ne correspond pas à quand nous le voulons. Nous le voulons plus tôt.

Alors nous renvoyons les estimations aux développeurs, nous faisons pression encore et encore jusqu'à ce que nous soyons certain que nous avons expurgé tout le trop-plein qu'ils avaient pu y mettre. Quelques fois, nous pouvons même leur dire quand ils doivent avoir terminer.

Quoiqu'il en soit, les développeurs quittent la pièce, la tête basse, sûrs et certains qu'une fois de plus, il leur a été demandé de faire l'impossible. Et le métier écrit la date : "les développeurs jurent qu'ils auront finis le 13 novembre à 12h25.".

Je suis quasiment certain que personne dans l'équipe ne croit en cette date. Si certaines personnes y croient, j'aimerai avoir l'occasion de parier avec eux sur cette date. Je suis quasiment certain que je conduirai bientôt une vraie Ferrari, parce que cette date n'est pas réaliste. Cette date est basée sur une liste d'exigences irréalistes, elle fait appel des estimations non fiables, à un moment d'ignorance absolue, par des gens qui sont toujours optimistes sur leurs propres capacités. Ces estimations ont été extirpées par des managers qui pensent qu'il faut être dur, et quelques fois elles ont été juste outrepassées par quelqu'un qui a fait une promesse irréfléchie à quelqu'un plus haut dans la chaîne alimentaire.

Pourtant, ça marche. Il suffit de maintenir la pression, et ils le feront du bon boulot.

Sauf qu'ils feront rarement du bon boulot, même dans un contexte agile. Regardons ce qui se passe.

# Les équipes agiles travaillent en itérations courtes ; ils prennent une quantité de travail qu'ils prévoient qu'ils pourront accomplir

Généralement, les processus agiles travaillent pendant des périodes de quelques semaines appelées itérations ou "sprints". A chaque itération, l'équipe travaillent avec leur "product owner" pour sélectionner le travail à accomplir pour la prochaine itération. Ils sont supposés choisir la quantité de travail qu'ils prévoient d'accomplir dans le temps imparti. L'élément important ici est "choisir".

Trop souvent, leur product owner, ou un membre de l'encadrement, exprime une déception sur la quantité sélectionnée, et les encourage, les presse, ou leur demande d'en prendre plus. "Les gens ont besoin d'objectifs à long terme", me disait une personne lorsque je lui demandais pourquoi ils faisaient comme cela.

Est-ce que cela vous surprend de savoir, que si une équipe reçoit une quantité de travail supplémentaire imposée et qu'elle ne pense pas pouvoir accomplir, elle échoue généralement ? Cela ne devrait pas être le cas. Est-ce que cela vous surprend qu'il soit fréquent, que seulement deux semaines après que quelqu'un leur ait donné du travail supplémentaire, que cette même personne exprime sa déception à l'équipe en lui disant qu'elle n'a pas "respecté sa promesse" ? Cela ne devrait pas être le cas.

# Ayant demandé l'impossible, l'encadrement demande de meilleures estimations

A la surprise de personne, débordée, l'équipe échoue. Quoi qu'il en soit, l'encadrement dit à l'équipe qu'elle doit améliorer ses estimations. Ce que l'encadrement veut vraiment dire c'est que les estimations sont des promesses - même pour des estimations forcées - et que l'équipe doit tenir ses "promesses", même si elle ne les a jamais faites. L'équipe accomplit tout ce qu'elle est en mesure d'accomplir. Alors l'encadrement essaye de forcer l'équipe à faire plus qu'elle ne peut faire, demendant à ce que l'équipe "devienne plus productive", ce qui signifie "aller plus vite, promettre plus, et le réaliser".

Les équipes à qui il est demandé de faire plus qu'elles ne peuvent faire diront, "Nous essaierons". Et elles essayent. Cela donne rarement de bons résultats. Afin d'être certains d'accomplir le travail, elles commenceront par tout surestimer. Dans l'objectif d'accomplir vite, elles amputeront des aspects importants du travail que vous ne pouvez pas voir. C'est un peu comme mettre la poussière sous le tapis. Elles feront un peu moins de tests que nécessaire. C'est OK, nous aurons ensuite un rapport d'anomalies et nous les corrigerons alors. Elles garderont le code un peu moins propre que nécessaire. C'est OK, nous nettoierons cela plus tard et cela ne nous retardera pas beaucoup.

Pourquoi devriez-vous vous en soucier ? Vous devriez vous en soucier, car les défauts n'apparaîtront pas avant la toute fin du projet, ou même après, une fois que le projet sera livré aux utilisateurs. Alors vous devrez faire le travail qui aurait déjà dû être fait pour faire fonctionner le code. Vous devriez vous en soucier car le code sera de pire en pire, le travail deviendra plus difficile et l'équipe ralentira. Et, le code s'empirant, de plus en plus de défauts se glisseront dedans.

Une livraison tardive du produit, moins riche en fonctionnalités, avec plus d'anomalies qu'il ne devrait en avoir, et plus coûteux à maintenir sera le résultat de tout cela.

"OK, Captain Négatif, ces choses sont de l'abus. Mais il y a des besoins légitimes pour des estimations et des prévisions, alors pourquoi ne pas râler contre les abus et mettre en avant les bons côtés ? "

"Quels sont ces bons côtés, alors ? J'ai oublié."

"Eh bien. Euh. Nous devons savoir combien de temps cela prendra pour que le projet soit prêt. Nous devons savoir combien il coûtera. Donc, nous devons estimer toutes les exigences et voir de combien de personnes nous aurons besoin, combien de temps, et combien cela coûtera. Alors nous saurons quand nous serons à court de temps et nous pourrons, euh, faire quelque chose.

"Et, euh. Nos équipes travaillent en itérations. Elles doivent savoir la quantité de travail qu'elles peuvent prendre en charge, et pour pouvoir faire cela, elles doivent estimer. Et évidemment, nous voulons qu'elles s'améliorent à déterminer combien de travail elles peuvent prendre en charge, alors nous comparerons leurs performances par rapport à leurs estimations et lorsqu'elles échoueront nous ferons en sorte qu'elles s'améliorent.

Le voici notre problème : cette pente est vraiment très glissante. Considérons d'abord le planning à long terme, et ensuite le planning à court terme.

Un des projets Agile à long terme les plus connus fût le projet de gestion de la paye C3 à Chrysler : le premier projet en Extreme Programming.

Un jour, je fus présent lors d'un échange entre Sue Unger, alors directrice des systèmes d'informations de Chrysler, la responsable la plus élevée dans la hiérarchie de la direction informatique que j'avais pu rencontrer, et l'équipe C3. Kent Beck venait justement d'expliquer comment nous travaillions en itérations de quelques semaines, réalisant tout ce que notre "cliente" Marie DeArment, nous demandait de faire. Mme Unger demanda "Comment saurai-je si vous êtes dans les clous ou pas ?"

Kent montra notre pile de carte de stories pour la gestion de la paye. "Voici toutes les choses que nous devons faire. Nous ajouterons des choses au fur et à mesure que nous les découvrirons, et nous enlèverons toutes celles qui ne doivent pas être faites. Nous vous demandons de venir nous voir tous les mois. Nous vous montrerons ces cartes, et nous vous montrerons combien auront été faites et combien resteront à faire. Si vous n'êtes pas satisfaite des progrès, nous arrêterons le projet."

Sue Unger, répondit "Je peux faire ça". Si elle peut faire cela, alors vous pouvez le faire aussi.

Le projet C3 étant un programme de gestion de la paye, et Marie, une experte dans ce domaine, elle savait exactement ce qu'il y avait à faire. L'équipe avait déjà travaillé sur un logiciel de paye, elle avait donc une bonne idée des besoins et de ce que cela impliquait. Même dans ce cas, nous ajoutions et enlevions des choses au fur et à mesure du projet, décalant du travail qui n'avait pas besoin d'être fait, et récupérant des nouveaux éléments en cours de chemin. Ce fût un des projets les mieux planifiés que j'ai jamais vu, même si, au moins un tiers des exigences furent ajoutées, supprimées, ou substantiellement modifiés.

Quoi qu'il en soit, l'équipe, et Mme Unger furent capable de dire si les choses allaient bien juste en regardant la pile de travail qui avait été faite, et la pile restant à faire.

Comme les étudiants en histoire Agile le savent, toutefois, le projet C3 ne fut pas entièrement un succès. Malgré la livraison d'un nombre de versions dans les temps, le projet fut annulé en fin de compte. Les raisons en furent largement politiques, mais clairement si le projet avait été parfait, cela ne serait pas arrivé. Cela nous pris quelques temps pour réaliser qu'il y avait une grande leçon cachée dans cette histoire.

L'objectif du projet C3 était de remplacer la totalité de la famille des programmes de gestion de la paye de Chrysler. Il ne faisait pas cela. Des années plus tard, le projet subséquent destiné à remplacer la totalité de la famille des programmes de gestion de la paye ne le faisait pas non plus. Nous réalisons maintenant ce qui aurait dû être fait.

Nous aurions dû remplacer les pièces cassées, une à la fois, les plus importantes d'abord.

L'idée fondamentale de faire une liste complète de tous les éléments de la paye, et de les réaliser était fausse.

Certaines parties des anciens programmes de la paye étaient corrects, et n'avaient pas besoin d'être remplacées. D'autres parties n'avaient aucun rapport avec la gestion de la paye. Certaines d'entre elles, comme les taxes, étaient considérées comme externes, et étaient traitées par des programmes externes. Mais d'autres parties étaient considérées comme faisant partie intégrante de la paye, et donc le nouveau système de paye ne pouvait être livré sans les inclure.

Ce n'était pas la bonne idée. Il y avait une idée bien meilleure, bien plus simple que nous n'avions pas vue. Il y avait des choses que Chrysler n'aimait pas dans la gestion de la paye existante. Cette partie-ci était trop lente. Cette partie-là était gérée différemment dans les différents systèmes de gestion de la paye. Cette autre partie était difficile à maintenir. Et ainsi de suite. Nous pensions que le boulot consistait à réaliser un nouveau vaste programme les regroupant tous. Faux.

Ce que nous aurions dû faire, ce que nous pourrions avoir fait, aurait été de régler les problèmes les uns après les autres, dans l'ordre dans lequel Marie et les autres personnes de la paye voulaient que nous les réglions, et déployer ces solutions dès lors qu'elles étaient prêtes. Certaines de ces solutions auraient été de garder un programme central, et certaines autres auraient été d'avoir des modules séparés. Par exemple, le flux global de la paye est essentiel, et il devrait être gérer avec précaution. À un certain point nous aurions dû organiser cela en ce que nous appelions "la ligne". Il n'est pas certain que nous aurions dû faire cela dès le début.

Les programmes de plan d'épargne de Chrysler était une autre partie qui avait besoin d'être travaillée. Les plans d'épargne étaient nombreux, complexes, et interagissaient les uns avec les autres. Nous aurions dû écrire un programme, ou une série de programmes, pour gérer cela. Ces programmes devaient interagir avec la ligne, mais ils ne devaient pas en faire partie.

Et ainsi de suite. Nous aurions pu travailler facilement sur ces problèmes quelques uns à la fois, car Chrysler avait besoin qu'ils soient réglés. Nous aurions pu déployer ces solutions aussitôt qu'elles fonctionnaient. Il aurait pu y avoir des problèmes pour qu'ils continuent à coopérer, à les garder maintenables, et ainsi de suite, mais nous avions déjà ces problèmes de toute façon, et des modules plus petits, indépendants auraient été la bonne manière de les gérer. Nous aurions pu même exécuter des modules séparés sur différentes machines, à différentes étapes du processus, pour des calculs, pour les processus de déboursement, et nous aurions certainement réalisé un programme plus modulaire, plus efficient.

Aurions nous fait cela, beaucoup de ce travail tournerait encore aujourd'hui et seulement certaines parties qui devaient vraiment être refaites l'auraient été.

La gestion de la paye C3, considérée pour être l'un des premiers succès - et des premiers échecs - de l'Agile, aurait pu probablement être beaucoup plus réussie, n'eût été la présomption que le boulot était de prédire quand tout serait fini, ou même de suivre et de projeter lorsque tout serait fini. Le boulot était de réunir une équipe pour résoudre les problèmes de l'organisation de la paye, et lorsque le retour sur investissement diminuerait, de partir. Certainement, nous aurions pu accomplir plus, et sans doute, tout cela et bien plus encore continuerait de fonctionner aujourd'hui.

Ce n'est pas l'idéal de penser à notre produit comme une longue liste de choses que nous devons faire. Ce n'est pas la meilleure idée que de prédire quand nous aurons fini, ou même de projeter quand nous aurons fini. Le manifeste agile exige des logiciels opérationnels. Prenez le problème qui vient, résolvez-le avec un logiciel opérationnel. Résolvez-le réellement, c'est-à-dire en mettant la solution dans les mains des personnes qui en ont besoin. Il ne s'agit pas de planification, de prédiction, et de projection. Il s'agit de choisir, de construire, et de livrer.

Bien sûr, il existe des bonnes manières d'utiliser l'estimation, et de la faire. En voici quelques-unes :

# De quelle taille est-il ce projet ?

Il semble qu'"ils" veulent souvent connaître combien de temps quelque chose va prendre, et combien cela va coûter. Mon point de vue est qu'"ils" ne savent même pas ce qu'ils veulent, donc bordel de merde, nous ne pouvons pas leur dire combien de temps cela va prendre. Quoi qu'il en soit, "ils" sont souvent puissants et ils ont l'argent dont nous avons besoin, alors nous devons répondre à leur question, bien que nous ne le puissions pas.

Bien entendu, si vous connaissez une manière d'estimer correctement la durée et le coût, allez-y et faites-le. Et pendant votre temps libre pantagruélique, faites-nous le plaisir de l'écrire pour nous autres (qui ne savons pas - NdT). Je vous en prie, mettez les histoires vraies de ce qu'il s'est réellement passés sur les projets que vous avez estimé de cette manière, y compris les changements survenus et les vies détruites. Pendant ce temps-là, nous continuerons notre bonhomme de chemin.

La plupart du temps, "ils" savent combien de personnes ils nous fourniront, ainsi que le délai impartit. Ils font ce mouvement de tête jusqu'à ce que nous donnions les "estimations" qu'ils ont en tête. Aussi nous devrions retourner la question. "Combien voulez-vous dépensez, et quand espérez-vous voir sortir le produit ?" Alors ils nous le diront, et nous déciderons si nous pouvons faire quelque chose de raisonnable avec ce budget. Si nous le pouvons, nous continuons. Si nous ne pouvons pas, nous déclinons poliment l'offre. Si nous avons décidé que nous ne pouvons pas, c'est que nous avons une estimation à l'esprit et nous devrions simplement l'énoncer. Franchement, c'est aussi valable que n'importe quoi d'autre auquel nous aurions pu arriver en utilisant une méthode plus complexe.

Si personne ne sait, et si personne n'a une idée, il y a de grandes chances que le projet soit trop vague et trop gros. Alors fuyez. Toutefois, si pour quelque raison que ce soit vous aimez vivre dangereusement en espérant créer un plan tout en descendant la paroi d'une falaise, voici quelque chose que vous pourriez essayer. Chet Hendrickson et moi-même l'appelons la "méthode des cinq cartes".

Considérons l'idée du produit et scindons la vision en cinq sujets majeurs. Chaque sujet devrait avoir un sens métier : ne scindez pas d'un point de vue technique. "Libraire en ligne" se scinde en, euh, peut-être "Avoir des infos sur un grand nombre de livres", "Chercher, trouver, et recommander des livres", "Commande et facturation", "Préparation de la commande et livraison", "Tableaux de bords et comptabilité". Qui sait ? Trouvez les vôtres.

Pouvez-vous estimer l'un des cinq sujets maintenant ? Vous pourriez déjà en connaître un rayon sur les commandes et avoir une idée claire du temps que cela prendra. Si c'est le cas, estimer ces items. Pour chaque item que vous ne pouvez pas estimer, scindez-le grosso modo en 5 idées plus petites. Peut-être "Chercher, trouver et recommander des livres" se transformera en, je ne sais pas, "Chercher par titre", "Chercher par auteur", "Chercher par similarité", "Chercher d'après les achats d'autres clients", "Chercher d'après les achats de ce client".

Eh bien ! Nous pouvons presque écrire le SQL pour la recherche par titre et l'auteur. Les achats d'un client ressemblent à une opération de jointure et ensuite à un simple résumé. La recherche par similarité semble encore assez floue. Et ainsi, nous estimons celles que nous comprenons, nous répétons, et scindons celles que nous ne comprenons pas.

Généralement, après quelques opérations de scissions, nous arrivons à des choses que nous pouvons estimer. Utiliser tous les moyens d'estimations que vous préférez.

Additionnez ensuite les nombres obtenus, multipliez par n'importe quel entier entre e et pi, et voici votre estimation. Ou bien utilisez vos propres formules magiques. Cela ne compte pas vraiment à vrai dire.

Cela ne compte pas à vrai dire parce que cela reste une estimation. Et c'est une estimation très peu fiable. D'ailleurs, c'est plutôt garanti qu'elle soit fausse. Mais elle pourrait être un point départ suffisant pour vous permettre de commencer, et notamment à commencer à faire des décisions à un niveau de maille plus fin sur ce qu'il faut faire ensuite et sur ce qu'il faut différer. Faites-le Agile, en produisant un système opérationnel une semaine sur deux. Peut-être que votre première version ne pourra gérer que quatre livres, aura un panier de commande trivial, facturera tout sur la carte de crédit de votre patron, et enverra un message électronique à James du service livraison en lui disant d'aller chez le libraire du coin acheter le livre, et de s'arrêter à la poste sur le chemin du retour au bureau.

Non, je suis sérieux. Pourquoi ne pas avoir un produit complet qui fera peu de choses au début, et puis ensuite de plus en plus ? Chaque fois que nous regarderons le produit, nous verrons quoi faire après.

# Combien de travail devrions-nous accepter ce coup-ci ?

Une équipe agile doit décider de la quantité de travail qu'elle accepte pour sa prochaine itération. Une manière de le faire est de regarder chaque élément de travail proposé et d'estimer combien de temps cela prendra pour le réaliser. Additionnez ces temps pour avoir un tour d'horizon rapide sur le backlog de l'itération proposé.

Cela peut être délicat d'additionner uniquement les temps. Aucune équipe ne peut travailler à la tâche huit heures par jours, vous devez donc décider comment ajuster. Une manière, est de suivre votre progression par rapport à vos estimations. Il pourrait être plus judicieux de considérer combien de temps vous passez réellement à travailler sur le sujet - c'est-à-dire, est-ce que cela vous prend vraiment quatre heures de travail pour le faire - et de considérer combien de temps s'est écoulé avant que vous ayez vos quatre heures dessus. Quelques fois cela peut prendre des jours d'avoir quatre heures de travail accompli.

Vous êtes sur une pente glissante ici, alors attention. Il sera tentant de demander aux personnes pourquoi il faut deux jours pour avoir quatre heures de travail accompli, et de demander aux personnes de travailler plus dur, plus vite et ainsi de suite. C'est le point culminant dont nous nous préoccupons ici. Gardez ces préoccupations et leurs impacts à l'intérieur de l'équipe.

Beaucoup d'idées existent sur comment estimer en utilisant quelque chose d'autre que la durée. Points, bonbons nounours, suite de Fibonacci, tailles de t-shirts. A l'origine, elles ont été inventés pour masquer l'aspect durée, afin que l'encadrement ne soit pas tenté de mal utiliser les estimations. (Je le sais : j'étais là quand elles ont été inventées. En fait, j'ai peut-être inventé la méthode des points. Si je l'ai fait, j'en suis désolé maintenant.)

Il y a une vraie bonne idée derrière ces méthodes, celle de comparer l'idée d'une fonctionnalité avec une autre et de réfléchir si elle est "grosse" ou "petite", et classifier ces fonctionnalités par groupe. Avec des mesures de durées que peuvent prendre des items similaires, une équipe peut apprendre à estimer assez rapidement et efficacement.

Rappelez-vous, pourtant... Nous faisons tout ceci pour décider combien de travail nous pouvons prendre en charge en une itération. Nous pourrions vouloir améliorer notre aptitude à faire cela, et bénéficier de la réflexion sur pourquoi ce que nous pensions être facile s'est révélé être difficile. Toutefois, à la fin de journée, les équipes en contemplant le travail (NdT : de la session d'estimation), discutent, se regardent les yeux dans les yeux et se disent "tout ça là", cela fait juste aussi bien que ceux qui passent du temps en numérologie. Mais souvent, elles font mieux, parce que le travail d'équipe et l'engagement sont plus puissants que du simple crachage de nombre.

Alors, quel est mon conseil ? En fait, il est assez simple. Il est probablement difficile à réaliser. Vous devez trouver votre propre voie, mais il y a deux voies valables vers lesquelles se diriger. La seconde étant bien meilleure que la première.

# Bonne, mais pas idéale : sélectionner votre date de livraison ; livrer chaque semaine entre maintenant et jusqu'à cette dernière

Les "grosses huiles" ont une date à l'esprit. Dans les rares cas où elles n'en ont pas, sélectionnez-en une vous-même. Choisissez-la assez tôt afin que nul ne devienne impatient en attendant la réalisation de votre projet. Comptez les personnes de votre équipe, et multipliez ce chiffre par le temps à votre disposition. Réfléchissez alors à ce que cela vous donnera avec cinq items majeurs. Si cela est nécessaire, scindez-les. Laissez-les assez vagues : vous aurez besoin de marge de manœuvre. Voilà ! Maintenant, vous avez un budget, complété par des estimations.

Maintenant, trouvez-vous un "client" ou un "product owner" qui pourra prendre les décisions sur ce qui pourra être fait ensuite et ce qui pourra être décalé. Travaillez en cycle très court. Deux semaines. Une semaine. Une fonctionnalité à la fois, en deux jours. Petite. Réalisez les fonctionnalités des plus aux moins importantes. À chaque fois qu'une fonctionnalité est faite, ou au moins une semaine sur deux, réalisez une version testée d'intégration du logiciel. Montrez-la à tout le monde. Si possible, mettez-la à disposition des utilisateurs qui en ont besoin. Si votre logiciel est destiné à sauver des vies, alors avec lui, sauvez quelques vies. Observez ce qui se passe. Prenez-le en compte pour la suite.

Désormais, vous livrez un produit complet une semaine sur deux. Lorsque la date butoir arrivera, il s'agira juste d'une autre livraison. Si tout le monde est satisfait, et ils devraient l'être, arrêtez. S'ils en veulent plus, vous serez prêts à en faire plus, une semaine sur deux.

# Dans l'idéal, évitez l'estimation, développez juste quelque chose maintenant

Pourquoi ne pas commencez chaque produit avec une simple expérience ? Est-ce que nous pensons que c'est assez simple ? Prenez un vrai visionnaire de produit, comme un product owner, et faites-le s'assoir avec quelques développeurs pendant une semaine ou deux pour élaborer quelque chose. Demandez-vous, alors, s'il faut continuer. Est-ce qu'il s'agit d'un gros projet, prenant sans doute six mois ou un an ? Alors construisez-le pendant quelques cycles d'itérations de deux semaines. Examinez où vous en êtes. Si c'est bon, poursuivez. Si ce n'est pas bon, arrêtez.

Sérieusement. Mettez une personne qui comprend le problème avec les personnes qui savent comment résoudre les problèmes, et solutionnez les problèmes dans l'ordre qui semblent être le plus important. Livrez tout ce que vous avez fait immédiatement. Observez ce que les utilisateurs disent, et observez ce que le marché dit. Ajustez en conséquence.

Existe t'il des "problèmes" avec cette approche ? Sûrement. Vous devez être très bon pour faire ça. Vous devez avoir quelqu'un qui aura la bonne intuition sur ce qui est demandé, et une équipe qui pourra le construire rapidement, à un niveau de qualité suffisant pour le donner aux utilisateurs rapidement. Et vous devez savoir comment construire un logiciel qui sera assez souple et malléable pour évoluer facilement au besoin. La partie technique est bien comprise. La partie de la prise de décision - du côté client - ne l'est pas, mais l'attendre ne la rendra pas meilleure. Sortez le produit et observez ce qu'il se passe.

Cette approche raccourcit tous les cycles qui retardent l'obtention de valeur. Elle raccourcit les lignes de communication entre les personnes qui veulent des choses et celles qui les réalisent. Elle raccourcit les lignes de communication entre les personnes qui créent des choses et celles qui les utilisent. Prenez les idées les plus importantes, réalisez-les rapidement et livrez-les.

Oui, c'est dur de le faire. C'est pourquoi c'est mieux. Arrêtez d'estimer. Commencez à livrer.

<p>&nbsp;</p>  

---
<p>&nbsp;</p>  
> Ron Jeffries a développé des logiciels depuis plus longtemps que depuis la naissance de la plupart des gens vivants actuellement. Il est titulaire de diplômes supérieurs en mathématiques et en informatique, obtenus bien avant l'invention des entiers négatifs. Ses équipes ont construits des systèmes d'exploitations, des compilateurs, des systèmes de bases de données relationnelles, et une grande variété d'applications. Les logiciels de Ron ont généré un revenu d'environ un demi milliard de dollars, bien qu'il se demande pourquoi il n'a pas vu la couleur d'un seul billet.
> Envoyez vos commentaires à l'auteur ou venez discuter de l'article sur le forum du magazine.
<p>&nbsp;</p>  

---
Auteur : [Ron Jeffries](http://www.xprogramming.com/)  
Source : [Estimation is Evil](http://pragprog.com/magazines/2013-02/estimation-is-evil)  
Date de parution originale : Février 2013  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 02/06/2014  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

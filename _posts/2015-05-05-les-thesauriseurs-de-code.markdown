---
layout: post
title:  "Les thésauriseurs de code"
date:   2015-05-05 22:00:53
categories: equipe développement refactoring
---
Avez-vous déjà vu un épisode de _Hoarders_ (Thésauriseurs [^1] [^2] en VF - NdT), ou un documentaire à propos d'un thésauriseur ? Des émissions de ce genre étaient assez populaires il y a quelques années. Elles montraient une tragédie, et un phénomène bien trop fréquent de personnes ayant perdu le contrôle sur leur espace de vie en le remplissant de tellement de bazar qu'il ne leur reste plus de place pour vivre.

Ces personnes remplissent leurs maisons de tellement de choses que tout ce qu'il reste ce sont des passages sombres, étroits, circulant à travers des piles allant du sol au plafond, de saloperies, de déchets, de déjections d'animaux, de linges sales, et d'autres choses que l'on peut encore moins mentionner. Le volume de chaque pièce est pris par des saloperies. Le compteur électrique, les tables et les meubles sont invisibles, enterrés en-dessous. Les déchets s'empilent aussi dans les chambres et les salles de bain.  Il n'y aucune place pour se déplacer. Aucune place pour manger. Aucune place pour dormir. Aucune place pour vivre. Il y a même eu des cas où des cadavres ont été retrouvées sous des piles de déchets et de détritus.

Et pourtant, chaque jour, ces thésauriseurs pitoyables apportent une nouvelle quantité de saloperies dans leurs maisons. Et ils les empilent tout en haut des tours des anciennes saloperies. Quelques fois ces tours tanguent, tremblent et tombent -- bloquant les passages étroits qui ont été taillés dans les montagnes de détritus.

Cherchez sur internet pour "Thésauriseurs" (Hoarders pour le nom de l'émission - NdT) si vous n'avez vu aucune de ces émissions ; et préparez-vous à être dégouté.

Si vous avez déjà vu une émission de ce genre, peut-être vous êtes vous demander comment quelqu'un pouvait vivre comme cela -- comment quelqu'un pouvait _choisir_ de vivre comme cela. Mais pensez-y. Ce n'est pas si difficile à comprendre. C'est facile de penser que toutes ces "affaires" que vous apportez dans votre maison apporte de la valeur à votre vie. Après tout, ce sont de nouvelles affaires. De nouveaux habits. De nouveaux appareils. De nouveaux meubles. De nouveaux livres. C'est un _bien_ ! Et un bien a de la valeur. Alors c'est facile de penser : "Plus il y a d'affaires, mieux c'est".

Il est aussi facile de croire qu'_acquérir_ de nouvelles affaires est plus important que mettre de l'ordre dans de vielles affaires.  Après tout, mettre de l'ordre dans de vieilles affaires n'apportent pas de valeur. C'est acquérir de nouvelles affaires qui comptent. Donc, tout temps libre, efforts ou énergie disponibles seront consacrés à l'acquisition de nouvelles affaires. Mettre de l'ordre dans les vieilles affaires est un gaspillage. 

Enfin, une fois que le désordre à commencer à s'installer, il est facile de penser qu'il n'y aucun espoir que cela puisse être remis en ordre. Vous concluez rapidement qu'il est inutile de nettoyer quoi que soit parce que les efforts d'une journée, d'une semaine et même d'un mois seront insuffisants. Pour citer _le Chat chapeauté_  du Dr. Seuss : "... ce désordre est si important, et si imposant et si grand, que nous ne pouvons rien ramasser. Il n'y a rien à y faire !".

##Code

Maintenant bien sûr vous réalisez que je parle de code. Cela me fait penser que la mentalité qui créé des systèmes encombrés et touffus est une mentalité de thésauriseur. Cela me fait penser également que le résultat est le même : un environnement malsain, impossible à vivre et à y travailler. Mais regardons point par point le raisonnement.

Avez-vous déjà été un _thésauriseur de code_ ? Avez-vous déjà travailler sur un projet qui a été construit par des _thésauriseurs de code_ ? Vous êtes vous déjà aventuré dans des passages encombrés du sol au plafond alors vous essayez d'ajouter une nouvelle fonctionnalité ou de corriger une vieille anomalie ? Est-ce que les piles de saloperies tanguent, tremblent et menacent de s'effondrer et de bloquer votre chemin ? Est-ce qu'il y a des sections entières de code dans lesquels vous n'osez pas vous aventurez ? Est-ce que la structure du système est invisible et enterrée sous des piles de nouvelles fonctionnalités et de code mort ?

Croyez-vous qu'ajoutez de la valeur signifie ajouter des nouvelles fonctionnalités. Croyez-vous qu'avoir de nouvelles fonctionnalités est plus important que mettre de l'ordre dans de vieilles fonctionnalités ? Croyez que l'effort consacré à nettoyer un vieux système est un gaspillage ? Avez-vous abandonné tout effort de nettoyer parce que vous savez que vous n'avez pas le temps de faire quoi que ce soit dans ce bordel ? Si vous répondez positivement, vous êtes un thésauriseur de code ; et votre vie professionnelle est un bordel sans nom.  

Nous avons un nom pour ce résultat. Nous l'appelons _code hérité_. Et ce terme même nous remplit de dégoût et de désespoir.

##Héritages

Qui doit nettoyer ce bordel horrible lorsque les thésauriseurs meurent ? Qui doit louer  les camions poubelles pour évacuer les centaines de tonnes de déchets ? Qui doit faire appel à une équipe de gestion des matières dangereuses pour désinfecter la maison ? Qui doit faire appel à une équipe de nettoyage pour frotter, nettoyer, peindre et réparer la maison ? Les enfants bien sûr. Ou si ce n'est pas les enfants, la communauté alors. L'héritage que laisse un thésauriseur est un héritage de saloperies, de déchets, de saleté, et un effort incommensurable est exigé pour que tout soit nettoyé. Du vivant du thésauriseur, son legs empire de jour en jour.

Mais il n'est obligatoire que les héritages se passent comme cela. En effet, la plupart des gens aspirent à laisser un héritage de _mieux_. La plupart des gens veulent laisser quelque chose derrière eux qui rend la vie meilleure pour ceux qui suivent. En effet, pour la majorité des personnes, c'est l'oeuvre constante de toute une vie que d'améliorer ce qu'ils laisseront derrière eux, leur héritage. 

Un _vrai_ héritage _s'améliore_ avec le temps.

##S'améliorer avec le temps ?

Et n'est-ce pas ce que font les humains ? Est-ce que les humains ne rendent pas les choses meilleures avec le temps ? Si vous avez dans le garage une voiture ancienne que vous êtes en train de retaper, n'espérez-vous pas que son état s'améliore de plus en plus chaque jour ? Si vous êtes en train de peindre une peinture, n'attendez-vous pas que la peinture soit de mieux en mieux avec le temps ?

Pouvez-vous imaginer embaucher un artiste, un mécanicien, un ingénieur, un docteur, un avocat ou qui que ce soit, dont le fruit du travail serait de pire en pire au fur et à mesure qu'ils y travaillent ? Comment rendre les choses de pire en pire, jour après jour, peut être le comportement d'un professionnel ? Comment cela peut-il être le comportement d'un développeur ? 

Une équipe professionnelle de développeurs rend son code meilleur chaque jour. La qualité du code s'améliore avec le temps. C'est comme cela que vous savez qu'ils sont professionnels. Les professionnels rendent les choses meilleures avec le temps. Le code hérité laissé par des professionnels sera plus propre, et l'ancien code sera plus propre parce qu'il a fait l'objet d'une longue attention par ces professionnels.

Rendez-vous le code meilleur chaque jour ? Ou laissez-vous chaque jour le code devenir pire que la veille ? 

Est-ce que votre travail laisse un héritage de valeur, ou ne faites-vous que bâtir un foutoir monstrueux que quelqu'un d'autre devra nettoyer ?

---
[^1]: source Larousse : [Thésauriseur](http://www.larousse.fr/dictionnaires/francais/th%C3%A9sauriseur/77856?q=th%C3%A9sauriseur#76938) : Personne qui thésaurise, qui amasse de l'argent.      

[^2]: source Larousse : [Thésauriser](http://www.larousse.fr/dictionnaires/francais/th%C3%A9sauriser/77855) : Mettre de l'argent de côté sans le dépenser ni le faire fructifier. (et par extension au code dans le présent article - NdT)

[Robert Martin (Uncle Bob)](http://www.8thlight.com/team/uncle-bob) est un maître artisan. Depuis 1970, c'est un auteur primé, un conférencier renommé et l'informaticien geek suprême.

---
Auteur : [Uncle Bob](http://www.8thlight.com/team/uncle-bob)  
Source : [Code Hoarders](http://blog.8thlight.com/uncle-bob/2014/04/03/Code-Hoarders.html)  
Date de parution originale : 03 Avril 2014  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 19/06/2014  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

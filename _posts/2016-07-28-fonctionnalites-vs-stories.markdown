---
layout: post
title:  "Fonctionnalités vs. stories"
date:   2016-08-09 00:00:01
published: true
categories: 
- agile
---

 Je réalise que, jusqu’à aujourd’hui, la différence entre fonctionnalités et _stories_ n’était pas clair dans mon esprit et qu’il s’agit d’une différence fondamentale. Une fonctionnalité est un groupe de _stories_ liées donnant un ensemble de fonctions que les utilisateurs finaux s’attendent à avoir toutes ensemble à la fois. Par exemple, redimensionner un tableau de type en-ligne[^1] est une fonctionnalité (remarque : ceci représente la possibilité de redimensionner les colonnes et les lignes dans des tableaux - essayez donc dans Word[^2]). Dans un premier temps, vous aurez probablement une seule _story_ pour le redimensionnement des tableaux de type en-ligne, mais cela devrait s’avérer à être trop gros à estimer. Par conséquent vous allez la scinder en trois _stories_, redimensionnement des colonnes, redimensionnement des lignes et redimensionnement du tableau lui-même. 

Nous avons maintenant trois _stories_ - trois choses différentes à développer qui ajouteront de la valeur au produit et qui pourront être faites relativement rapidement (nous pensons que la plus grosse de ces _stories_ devrait prendre une journée à développer). Il y a de la valeur à être capable de redimensionner les colonnes mais pas en ce qui concerne les lignes ou le tableau lui-même - le redimensionnement des colonnes permet aux utilisateurs de distribuer l’espace entre les colonnes plus facilement afin que le tableau ait un aspect plus joli. Cela couvre 90% des cas d’utilisation de redimensionnement de ce type de tableau - les personnes redimensionnent rarement l’ensemble du tableau ou la hauteur des lignes, généralement ils veulent juste faire en sorte que la largeur des colonnes soient ajustées au mieux aux données présentes à l’intérieur. En dépit de cela, livrer cette seule _story_ aux utilisateurs provoquerait de la confusion et des plaintes au support parce que cette livraison entraîne une attente dans l’esprit des utilisateurs de pouvoir redimensionner les tableaux alors ils se demandent pourquoi ils ne peuvent pas redimensionner les lignes ou le tableau ?

La fonctionnalité, c’est les trois _stories_ réunies ensemble, et c’est la capacité à pouvoir livrer sans entraîner de confusion chez nos utilisateurs, nous voulons vraiment être certain que ces trois _stories_ seront terminées avant la livraison - toutefois nous pouvons toujours la livrer à nos utilisateurs internes dans le cadre du programme “tiens-mets-toi-çà-sous-la-dent” ou aux beta testeurs avant que nous ayons les trois, il y a donc une certaine valeur à faire une seule de ces trois _stories_.

Il y a deux avantages clés à scinder les fonctionnalités de cette manière. Tout d’abord, cela rend l’estimation plus facile et plus précise - les choses qui prennent du temps ont tendance à être difficile à estimer. Deuxièmement, cela nous permet de suivre plus précisément nos progrès sur la fonctionnalité. Une des premières règles de suivi de l’avancée d’un projet est que vous ne devez suivre que les tâches terminées et non les tâches terminées partiellement car les personnes ne sont vraiment pas bonnes pour estimer quand est-ce qu’ils auront terminés.  Avec des _stories_ de taille réduite vous pouvez suivre l’avancée du projet simplement en vous basant sur le nombre de _stories_ terminées sans perdre en précision.

Scindez les _stories_ reste toutefois quelque chose d’assez difficile parce que vous devez être certain qu’elles continuent à avoir de la valeur. Récemment, nous avons eu une _story_ dont l’objectif était de développer une panneau de propriétés quelconque qui devait faire partie intégrante d’une boîte de dialogue plus importante. Malheureusement, nous avons livré la _story_ du panneau avant la _story_ sur la boîte de dialogue, nous avions donc développer un panneau que l’utilisateur n’était pas capable d’accéder. Ce fût même pire, nous avons perdu du temps à créer une boîte de dialogue juste pour ce panneau parce que nous pensions qu’il était nécessaire - nous aurions dû remarquer le peu de valeur de cette _story_ et poser la question au client avant de commencer - nous aurions probablement fais d’abord la _story_ de la création de la boîte de dialogue, donnant ainsi immédiatement de la valeur pour la _story_ du panneau.

[^1]: type de tableau à base de CSS dans une page web - pour plus d’informations à ce sujet, veuillez consulter cette [page](http://www.yoyodesign.org/doc/w3c/css2/tables.html) ou [celle-ci](http://www.yoyodesign.org/doc/w3c/css2/visuren.html#inline-level) - NdT

[^2]: ou dans votre traitement de texte préféré - NdT

---  
Auteur : [Adrian Sutton](https://www.symphonious.net/about-me/)  
Source : [Features vs Stories](https://www.symphonious.net/2006/05/18/features-vs-stories/)  
Date de parution originale : 18 Mai 2006  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 09/08/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

 
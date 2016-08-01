---
layout: post
title:  "Features vs. stories"
date:   2016-07-31 00:00:01
published: false
categories: 
- story
---

 I realized today that I hadn't made explicit the difference in my mind between _features_ and _stories_ and it's an important difference. Essentially, a _feature_ is a group of _stories_ that are related and deliver a package of functionality that end users would generally expect to get all at once. For instance, inline table resizing is a _feature_ (note: this is the ability to drag to resize tables, rows and columns – try it in Word). In the first pass, you'd probably have a single story for inline resizing of tables, but it would be too big to estimate. So you break it down into three _stories_, resize columns, resize rows and resize the table itself.
 
 Je réalise aujourd’hui que jusqu’à aujourd’hui, la différence entre les _features_ et les _stories_ n’était pas clair dans mon esprit et qu’il s’agit d’une différence importante. Une _feature_ est un groupe de _stories_ liées donnant un ensemble de fonctionnalités que les utilisateurs finaux s’attendent à avoir toutes ensemble à la fois. Par exemple, redimensionner une tableau de type en-ligne[^1] est une _feature_ (remarque : ceci représente la possibilité de redimensionner les colonnes et les lignes dans des tableaux - essayez donc dans Word). Au premier passage, vous aurez probablement une seule story pour le redimensionnement des tableaux de type en-ligne, mais cela devrait s’avérer à être trop gros à estimer. Par conséquent vous allez la scinder en trois _stories_, redimensionnement des colonnes, redimensionnement des lignes et redimensionnement du tableau lui-même. 

[^1]: type de tableau à base de CSS dans une page web - pour plus d’informations à ce sujet, veuillez consulter cette [page](http://www.yoyodesign.org/doc/w3c/css2/tables.html) ou [celle-ci](http://www.yoyodesign.org/doc/w3c/css2/visuren.html#inline-level) 

Now we have three _stories_ – three things to develop which add value to the product and can be done fairly quickly (we're currently aiming for the biggest of our _stories_ to take a day). There is value in being able to resize columns but not rows or the table itself – it allows users to distribute space between columns more easily to make the table look good. In fact, it covers 90% of the use cases for inline table resizing – people rarely resize the overall table or the height of rows, usually they just want to make column widths fit the data better. Despite that, shipping just that story out to users would cause confusion and complaints to support because it sets up the expectation in user's minds that they can resize tables so why can't they resize the rows or the table?

Nous avons maintenant trois _stories_ - trois choses différentes à développer qui ajouteront de la valeur au produit et qui pourront être faites relativement rapidement (nous pensons que la plus grosse de ces _stories_ devrait prendre une journée à développer). Il y a de la valeur à être capable de redimensionner les colonnes mais pas en ce qui concerne les lignes ou le tableau lui-même - le redimensionnement des colonnes permet aux utilisateurs de distribuer l’espace entre les colonnes plus facilement afin que le tableau ait un aspect plus joli. Cela couvre 90% des cas d’utilisation de redimensionnement de ce type de tableau - les personnes redimensionnent rarement l’ensemble du tableau ou la hauteur des lignes, généralement ils veulent juste faire en sorte que la largeur des colonnes soient ajustées au mieux aux données présentes à l’intérieur. En dépit de cela, livrer cette unique story aux utilisateurs provoquerait de la confusion et des plaintes au support parce qu’elle entraîne comme attente dans l’esprit des utilisateurs qu’ils peuvent redimensionner les tableaux alors pourquoi ne peuvent-ils pas redimensionner les lignes ou le tableau ?

The _feature_ is all three _stories_ put together, and to be able to ship without confusing our users we really want to make sure all three _stories_ are completed before we ship – however we can still release to internal users as part of our dog-fooding program or to beta testers before we have all three, so there is value in doing just one of the _stories_.

La _feature_ c’est les trois _stories_ réunies ensemble, et c’est être capable de livrer sans entraîner de confusion chez nos utilisateurs car nous voulons vraiment être sûr que ces trois _stories_ seront terminées avant la livraison - toutefois nous pouvons toujours livrer à nos utilisateurs internes dans le cadre du programme tiens-mets-toi-sous-les-dents ou aux beta testeurs avant que nous ayons les trois, il y a donc de la valeur à faire une seule de ces trois _stories_.

There are two key advantages to breaking down _features_ like this. Firstly, it makes estimation easier and more accurate – things that take a long time tend to be very difficult to estimate. Secondly, it allows us to track progress on the _feature_ accurately. One of the first rules of tracking project progress is that you only ever track tasks complete, and not partial tasks because people are really bad at estimating how close to completion they are. With small _stories_ you can track progress just based on the number of complete _stories_ without losing too much accuracy.

Il y a deux avantages clés à scinder les _features_ de cette manière. Tout d’abord, cela rend l’estimation plus facile et plus précise - les choses qui prennent du temps ont tendance à être difficile à estimer. Deuxièmement, cela nous permet de suivre plus précisément nos progrès sur la _feature_. Une des premières règles de suivi de l’avancée d’un projet est que vous ne devez suivre que les tâches terminées et pas les tâches terminées partiellement car les personnes ne sont vraiment pas bonnes pour estimer quand est-ce qu’ils auront terminés.  Avec des _stories_ de taille réduite vous pouvez suivre l’avancée du projet simplement en vous basant sur le nombre de _stories_ terminées sans perdre de précision.

Breaking down _stories_ is pretty hard though because you have to make sure that they still deliver value. We had one story recently to develop a particular properties panel that would become part of a larger dialog. Unfortunately we were given the panel story before the overall dialog story so we developed a panel that the user couldn't possibly access. Worse still, we wasted time beginning to create a dialog just for that panel because we assumed it was required – we should have picked up on the lack of value in the story and asked the client about it before we started work – we probably would have done the create the dialog story first, thus making the panel story suddenly have value.

Scindez les _stories_ reste toutefois quelque chose d’assez difficile parce que vous devez être certain qu’elle continue à avoir de la valeur. Récemment, nous avons eu une storie dont l’objectif était de développer une panneau de propriétés assez particulier qui devrait faire partie intégrante d’une boîte de dialogue plus importante. Malheureusement, nous avons livré la story du panneau avant la story sur la boîte de dialogue, nous avions donc développer un panneau que l’utilisateur n’était pas en capacité d’accéder. C’est même pire, nous avons perdu du temps à créer une boîte de dialogue juste pour ce panneau parce que nous pensions qu’il était nécessaire - nous aurions dû remarquer le manque de valeur de cette story et poser la question au client avant de commencer - nous aurions probablement fais d’abord la story de la création de la boîte de dialogue, donnant ainsi immédiatement de la valeur à la story du panneau.

---  
Auteur : [Adrian Sutton](https://www.symphonious.net/about-me/)  
Source : [Features vs. Stories](https://www.symphonious.net/2006/05/18/features-vs-stories/)  
Date de parution originale : 18 Mai 2006  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 31/07/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

 
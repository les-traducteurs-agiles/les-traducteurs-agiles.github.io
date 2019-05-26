---
layout: post
title:  "Questions/Réponses à propos de la vélocité 4ème partie"
date:   2019-05-26 00:01
published: true
tags:
- vélocité
---

Lors de notre [dernier épisode](http://www.les-traducteurs-agiles.org/2019/04/08/questions-reponses-a-propos-de-la-velocite-3eme-partie.html), nous avons parlé de la vraie réalité et du contraste que cela peut avoir avec le côté artificiel des calendriers, des estimations et des promesses faites.

Aujourd'hui, nous allons regarder plus en profondeur l'un des éléments de cette dichotomie :

> A: Ce planning représente la meilleure hypothèse valable actuellement, mais il y a une vraie promesse qui se cache derrière celui-ci.  
> B: Comment cela peut-il affecter le rythme auquel les choses avancent ?  
> A: Est-il possible de mettre davantage de monde sur le projet ?  
> B: Peut-être, mais jetez donc un coup d'œil à la loi de Brook  

Ces plannings bien qu'artificiels ont un certain côté réel également. Dans cet échange, la personne A rappelle ce fait à la personne B.

Les promesses sont réelles. La confiance est réelle. Respecter ses promesses permet de créer, de maintenir et de favoriser la confiance. La vraie vie des organisations repose sur la confiance. Beaucoup de dirigeants d'entreprise (ainsi qu'un certain animal aquatique agile[^1]) ont parlé de cela et écrit à ce sujet en long et en large. L'un de mes auteurs préférés sur le sujet est Stephen M. R. Covey (connu également sous le nom de  "Covey le Second[^2]") avec son livre intitulé [« La vitesse de la confiance »](https://www.amazon.fr/Vitesse-Confiance-Stephen-M-R-Covey/dp/1633538168/). Les travaux de l'économiste [Ronald Coase](https://fr.wikipedia.org/wiki/Ronald_Coase) dans lesquels il explique le faible coût transactionnel de la confiance sont également très intéressants.

Toutefois, pour toutes ces raisons, la réalité ne fait pas ce que nous voulons qu'elle fasse. Les choses prennent toujours autant de temps.

C'est dur comme de la pierre.

Si nous étions en train d'installer une cloison sèche ou de poser la moquette, alors les travaux à mener seraient une combinaison de compétences et de pas mal d'effort. Nous pourrions embaucher plus d'ouvriers et nous pourrions terminer davantage de pièces en même temps. Nous pourrions même être en mesure de faire une pièce plus vite, selon la manière dont ils se débrouillent bien pour se coordonner.

Mais non. Là, c'est différent. La programmation est une suite d'enchainements logiques alimentée par d'autres enchainements logiques et qui va alimenter d'autres enchainement logiques. Les différentes parties ne sont pas aussi indépendantes que nous le pensons, et ne pas comprendre le contexte de manière plus large (et les défauts présents dans les différentes parties dans un contexte plus grand) engendrera des anomalies.

Un jour, j'ai changé un bout de code développé d'une mauvaise manière (en construisant des chaînes JSON par concaténation) pour le redévelopper en utilisant de manière plus propre une bibliothèque JSON, ce qui a eu comme conséquence de faire planter le système quelques temps. Quelques fois, le système dépend de la manière dont le travail a été fait -- même si c'est de mauvaise manière -- pour pouvoir fonctionner. Les choses s'emboîtent parfois de manière bizarre.

Ramener des développeurs qui ne connaissent pas la manière dont le code fonctionne n'aide pas. La programmation en groupe[^3] ou la programmation en binôme[^4] avec des gens qui en savent plus sur les différentes parties du code, ça aide. Ajouter des sachants à l'effort commun conduit à un meilleur résultat, mais cela ne fait pas nécessairement avancer le travail plus vite.

La [loi de Brook](https://fr.wikipedia.org/wiki/Loi_de_Brooks) résulte de l'observation qu'ajouter des personnes à un projet en retard ne fait que le retarder davantage. Cela a été étudié et documenté en long et en large, et quiconque voulant essayer de faire accélérer un projet en ajoutant des personnes devrait en être averti. Il n'est pas impossible de rajouter des personnes à un projet , mais rajouter tout un tas de nouvelles personnes qui ne connaissent pas le système ne fera que le rendre bien PLUS pire encore.

Ce sont ces vérités dérangeantes, qui nous obligent à chercher des alternatives prometteuses si nous voulons voir aboutir les travaux dans un délai réaliste.

Rejoignez-nous pour le [5ème épisode](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-v.html)

[^1]: le surnom de l'auteur est _Agile Otter_, la loutre agile - NdT
[^2]: Steven M. R. Covey surnommé le second a écrit « la vitesse de la confiance » et son père a écrit notamment « Les sept habitudes des gens efficaces » ainsi que « Le pouvoir de la confiance »
[^3]: _Mob programming_ pour celles ou ceux préférant le terme anglophone - NdT
[^4]: _Pair programming_ pour celles ou ceux préférant le terme anglophone - NdT

---
Auteur : Tim Ottinger  
Source : [Q and A on Velocity, Part IV](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-iv.html)  
Date de parution originale : 15 Octobre 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 26/05/2019  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

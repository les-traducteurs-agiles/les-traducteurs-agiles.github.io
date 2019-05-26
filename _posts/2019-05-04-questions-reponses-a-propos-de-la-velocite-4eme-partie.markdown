---
layout: post
title:  "Questions/Réponses à propos de la vélocité 4ème partie"
date:   2019-05-04 00:01
published: false
tags:
- vélocité
---

In our [last installment, part III](https://agileotter.blogspot.com/2018/07/q-and-on-velocity-part-iii.html), we talked about the reality of reality and contrasted that to the made-up-ness of schedules and estimates and promises.  

Lors de notre [dernier épisode](http://www.les-traducteurs-agiles.org/2019/04/08/questions-reponses-a-propos-de-la-velocite-3eme-partie.html), nous avons parlé de la réalité de la réalité et du contraste que cela peut avoir avec le côté artificielle des calendriers, des estimations et des promesses faites.

Today we take a deeper look into one element of that dichotomy:  

Aujourd'hui, nous allons regarder plus en profondeur l'un des éléments de cette dichotomie :

> A: The schedule is a best-guess, but there is a real promise behind it.  
> B: How does that affect the rate at which things can be done?  
> A: Can I put more people on it?  
> B: Maybe, but cf Brook's Law  

> A: Ce planning représente la meilleure hypothèse actuellement, mais on y voit une vraie promesse derrière celui-ci.  
> B: Comment cela peut-il affecter le rythme auquel les choses avancent ?  
> A: Est-il possible de mettre davantage de monde sur le projet ?  
> B: Peut-être, mais jetez donc un coup d'œil à la loi de Brook  

There is a reality to the made-up-ness of schedules, too. In this exchange, person A is reminding person B of the fact.  

Ces plannings bien qu'artificielles ont un certain côté réel également. Dans cet échange, la personne A rappelle ce fait à la personne B.

Promises are real. Trust is real. Keeping promises creates, sustains, and promotes trust. Real life organizations run on trust.  Plenty of business leaders (and one agile aquatic mammal) have spoken and written on this at length. One of my favorite authors on the subject is Stephen M. R. Covey (AKA "Covey the Lesser") with his book titled [The Speed Of Trust](https://www.amazon.com/SPEED-TRUST-Thing-Changes-Everything/dp/1416549005). Also, see economist[ Ronald Coase's](https://en.wikipedia.org/wiki/Ronald_Coase) work, where he explains the lower transactional costs of trust.  

Les promesses sont réelles. La confiance est réelle. Respecter ses promesses permet de créer, de maintenir et de favoriser la confiance. La vraie vie des organisations repose sur la confiance. Beaucoup de dirigeants d'entreprise (ainsi qu'un animal aquatique agile[^1]) ont parlé de cela et écrit à ce sujet en long et en large. L'un de mes auteurs préférés sur le sujet est Stephen M. R. Covey (connu également sous le nom de  "Covey le Second[^2]") avec son livre intitulé [La vitesse de la confiance](https://www.amazon.fr/Vitesse-Confiance-Stephen-M-R-Covey/dp/1633538168/). Le travail de l'économiste [Ronald Coase](https://fr.wikipedia.org/wiki/Ronald_Coase) dans lequel il explique le faible coût transactionnel de la confiance est également intéressant à regarder.

And yet, for all of this, reality doesn't do what we want it to do. Things still also take as long as they take.  

Toutefois, pour toutes ces raisons, la réalité ne fait pas ce que nous voulons qu'elle fasse. Les choses prennent toujours autant de temps.

Rock, meet hard place.  

C'est dur comme de la pierre.

If we were installing drywall or carpet, then the work would be partly skill and mostly effort. We could get more drywallers or more carpet-layers and we could do more rooms at the same time.  We might even be able to do one room at a time faster, provided on how well they coordinate.  

Si nous étions en train d'installer une cloison sèche ou de poser la moquette, alors les travaux à mener seraient une combinaison de compétences et de pas mal d'effort. Nous pourrions embaucher plus d'ouvriers et nous pourrions terminer davantage de pièces en même temps. Nous pourrions même être en mesure de faire une pièce plus vite, selon comment ils se débrouillent bien pour se coordonner.

But no. This is different. Programming is a chain of logic that is fed by and feeds into many other chains of logic. The parts are not as independent as we think, and not understanding the larger context (and the flaws in the parts in the larger context) will lead to many defects.  

Mais non. C'est différent. La programmation est un enchainement logique alimenté par d'autres enchainement logique et qui va alimenter d'autres enchainement logiques. Les parties ne sont pas aussi indépendantes que nous le pensons, et ne pas comprendre un contexte plus grand (et les ce qui ne va pas dans les différentes parties dans un contexte plus grand) engendrera des anomalies.

I once switched a bit of code from a bad way of doing work (building JSON strings by concatenation) to a more proper use of a JSON library, and took a system down for a little while. Sometimes the system depends on the work having been done the way it was -- the wrong way -- in order to function. Things stick together in a weird way.  

Un jour, j'ai changé un bout de code développé d'une mauvaise manière (en construisant des chaînes JSON par concaténation) pour le redévelopper en utilisant de manière plus propre une bibliothèque JSON, ce qui a eu comme conséquence de faire planter le système quelques temps. Quelques fois, le système dépend de la manière dont le travail a été fait -- la mauvaise manière -- pour pouvoir fonctionner. Les choses s'assemblent parfois de manière bizarres.

Bringing in developers who don't know the way that the code works doesn't help. Mob programming or pair programming with people who know more about the different parts of the code certainly does help. Adding knowledgeable people to the effort does lead to a better result, but doesn't necessarily make the work go faster.  

Ramener des développeurs qui ne connaissent pas la manière dont le code fonctionne n'aide pas. La programmation en groupe ou la programmation en binôme avec des gens qui en savent plus que les différentes parties du code, ça aide. Ajouter des sachants à l'effort commun mène à un meilleur résultat, mais cela ne fait pas nécessairement avancer le travail plus vite.

[Brooks' Law](https://en.wikipedia.org/wiki/Brooks%27s_law) is the observation that adding people to a late project makes it later. This has been studied and documented at length, and anyone wanting to try to accelerate a project by adding people should beware. It's not impossible to add people to a project, but often a flood of new workers who don't know the system will make it FAR worse.  

La loi de Brook résulte de l'observation qu'ajouter des personnes à un projet en retard ne fait que le retarder davantage. Cela a été étudié et documenté en long et en large, et quiconque voulant essayer de faire accélérer un projet en ajoutant des personnes devraient en être averti. Il n'est pas impossible de rajouter des personnes à un projet , mais rajouter un paquet de nouvelles personnes qui ne connaissent pas le système le rendront encore bien pire.

These are inconvenient truths, which press us to look into more promising alternatives if we want to see work delivered to an all-to-real schedule.  

Ce sont ces vérités dérangeantes, qui nous obligent à chercher des alternatives prometteuses si nous voulons voir aboutir les travaux dans un planning réaliste.

Follow us to [Part V](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-v.html)

Rejoignez-nous pour le [5ème épisode](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-v.html)

---
Auteur : Tim Ottinger  
Source : [Q and A on Velocity, Part IV](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-iv.html)  nbsp
Date de parution originale : 15 Octobre 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : jj/mm/yyyy  nbsp

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

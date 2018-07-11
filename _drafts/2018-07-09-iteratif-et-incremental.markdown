---
layout: post
title:  "Itératif et incrémental"
date:   2018-07-11 00:01
published: true
tags:
- agile
- dark scrum
---

> Il se pourrait un jour que j'écrive un livre s'appelant "Développement logiciel, voici comment je fais". Si cela arrive, cet article pourrait bien en faire partie.
>
> Quoi qu'il en soit, quelque chose sur Twitter m'a amené à penser que je devrais écrire quelques lignes sur les concepts du développement itératif et incrémental.  

Les approches de développement logiciel telles qu'Extreme Programming et Scrum peuvent être qualifiées d'itérative et incrémentale.

Un processus _**iteratif**_ est un processus dans lequel une série d'opérations est répétée de manière cyclique, avec l'intention de se rapprocher de plus en plus d'un certain résultat désiré. En mathématiques, par exemple, la méthode de Newton-Raphson est utilisée pour approximer les solutions d'équations algébriques. Il s'avère souvent difficile d'obtenir une solution directe à une équation : quelques fois, il se peut qu'aucun moyen d'y arriver directement existe. Mais souvent, il est possible de se rapprocher par approximation d'une solution, en essayant généralement une valeur, puis en essayant de manière répétitive cette valeur en vue d'obtenir une solution plus précise. Si le calcul de la nouvelle approximation s'avère plus facile que déterminer une solution directe, alors l'itération, en tant que telle, est digne d'intérêt.

Par analogie, des approches telles que XP et Scrum répètent un cycle simple d'activités, qui produit un nouvel incrément du produit à chaque cycle. Généralement, le cycle est réalisé dans un période de temps fixe, mais avoir une période de temps n'est pas nécessaire en tant que tel dans de l'itératif. Toutefois, XP et Scrum utilisent une période de temps fixe par itération, alors que des approches qui se focalisent plus sur un flux continu, comme Kanban, peuvent réaliser un cycle uniforme d'étapes, mais dans un "temps nécessaire" plutôt que dans une période de temps fixe.

XP appelle ce cycle de période de temps une "Itération", alors que Scrum l'appelle un "Sprint". Ces cycles eux-mêmes s'avèrent être similaires. Dans une période de temps d'une semaine ou deux, l'équipe planifie ce qu'elle accomplira dans cette période de temps. Elle fait les travaux, puis le passe en revue et réfléchit à comment améliorer les travaux, ainsi que la manière de travailler, puis c'est reparti pour un tour. Chaque itération du cycle est par conséquent similaire à la précédente, mais pas identique. Les travaux spécifiques changent, bien sûr, mais nous améliorons aussi la manière dont nous abordons le travail.

Et il est attendu de chaque itération qu'elle produise un "Incrément", opérationnel, testé, d'un logiciel utilisable qui soit en mesure de remplir davantage d'objectifs du produit que la fois précédente.

Une approche _**incrémentale**_ pour produire quelque chose peut être définie comme étant une approche permettant de produire davantage chaque fois. C'est un petit peu en contraste avec le concept d'approche itérative, qui est définie comme étant une approche permettant de produire une version améliorée en vue d'obtenir une solution cible. Une approche incrémentale produit quelque chose de nouveau en modifiant une ancienne.

Ces différentes idées, ensemble, définissent ce que des approches "Agile" telles que XP et Scrum font. Elles répètent un schéma cyclique d'action, produisant une nouvelle version du produit souhaité, en modifiant la version précédente. Généralement, ces changements consisteront en l'ajout d'une nouvelle fonctionnalité, parce que nous avons généralement besoin de plus d'une fonctionnalité dans un produit avant que les gens ne le trouvent utile.

La chose que nous produisons s'appelle l'Incrément, et nous allons en discuter en détails plus loin. Jetons donc un coup d'œil sur quelques points.

Premièrement, l'Incrément devrait toujours être testé intégralement et être opérationnel. La seule chose qui ferait qu'il ne serait "pas prêt à être livré" serait l'absence d'une fonctionnalité indispensable pour qu'il soit utile. De manière toute vraisembable, ce que nous devrions faire par la suite serait d'ajouter cette fonctionnalité. À part ce cas de figure, l'Incrément devrait être prêt à être livré. En fait, le meilleur là-dedans, c'est qu'il est prêt à être livré. L'idée ici c'est d'avoir une envie irrésistible de donner l'Incrément à quelqu'un pour qu'il l'utilise.

Deuxièmement, pendant que nous essayons généralement d'améliorer l'incrément en y ajoutant des fonctionnalités, cela ne signifie pas que nous n'enlevons rien ou que nous ne faisons aucun progrès visible. Une bonne utilisation de l'approche du développement incrémental est d'essayer des choses. Nous introduisons une fonctionnalité, nous laissons quelques personnes l'utiliser, et nous en tirons des leçons. Le prochain coup, nous pourrions enlever cette fonctionnalité, ou la manière dont elle rend service, et en mettre une autre à la place. D'une manière similaire, nous pourrions améliorer l'efficience ou une caractéristique moins visible du produit. L'idée, assez simple, est que nous l'améliorons à chaque fois.

Vous savez tout désormais. Les approches que nous préférons sont itératives, car elles consistent en des cycles courts de développement, qui se déroulent généralement d'une manière similaire, avec des améliorations. Elles sont incrémentales, car elles produisent un Incrément du produit chaque fois, chaque Incrément étant prêt à être livré, et meilleur que celui qui l'a précédé.

Itératif et incrémental : régulier, cohérent, produisant des résultats utilisables. C'est de cette manière que je fais du logiciel.

---
Auteur : [Ron Jeffries](http://ronjeffries.com/about.html)  
Source : [Iterative and Incremental](https://ronjeffries.com/articles/018-01ff/iter-incr/)  
Date de parution originale : 9 Juillet 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 11/07/2018  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

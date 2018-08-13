---
layout: post
title:  "Refactoring - Pas dans le backlog !"
date:   2014-09-25 22:20:55
tags:
- refactoring
- backlog
---
Récemment, il y a eu beaucoup d'agitations sur les listes de diffusion, et de questions lors de conférences, à propos de mettre les "stories" refactorées dans le backlog. C'est toujours une mauvaise idée même si la dette technique a augmenté. Voici pourquoi :

<div align="center">
    <img src="{{ site.url }}assets/refactoring_pas_dans_le_backlog/Ref01.jpg" />
</div>

Lorsque notre projet débute, le code est propre. Le terrain est bien entretenu, la vie est belle, nous avons le monde au creux de notre main. Tout est bien dans le meilleur des mondes.

<div align="center">
  <img src="{{ site.url }}assets/refactoring_pas_dans_le_backlog/Ref02.jpg" />
</div>

Nous pouvons construire des fonctionnalités en douceur et facilement, même si nous semblons prendre toujours quelques tours et détours. Les choses semblent assez propres, et de toute façon nous sommes assez pressés. Nous ne remarquons rien d'anormal et nous poursuivons rapidement notre chemin.

<div align="center">
  <img src="{{ site.url }}assets/refactoring_pas_dans_le_backlog/Ref03.jpg" />
</div>

Néanmoins, nous laissons ça et là quelques mauvaises herbes pousser sur notre terrain de code presque parfait. Mais, à part ça, il n'a pas l'air si mal.

<div align="center">
  <img src="{{ site.url }}assets/refactoring_pas_dans_le_backlog/Ref04.jpg" />
</div>

Au fur et à mesure que nous construisons, nous devons contourner des broussailles, ou  nous frayer un chemin à travers. Généralement, nous faisons un détour.

<div align="center">
  <img src="{{ site.url }}assets/refactoring_pas_dans_le_backlog/Ref05.jpg" />
</div>

Inévitablement, cela nous ralenti un peu. Afin de continuer à progresser rapidement, nous sommes encore moins attentif qu'avant, et bientôt d'autres mauvaises herbes ont poussées.

<div align="center">
  <img src="{{ site.url }}assets/refactoring_pas_dans_le_backlog/Ref06.jpg" />
</div>

Ces nouvelles broussailles, qui ont poussées par-dessus les anciennes, nous ralentissent encore plus. Nous réalisons qu'il y a un problème mais nous sommes trop pressés pour faire quoi que soit sur le sujet. Nous travaillons encore plus dur pour maintenir notre vélocité première.

<div align="center">
  <img src="{{ site.url }}assets/refactoring_pas_dans_le_backlog/Ref07.jpg" />
</div>

Bientôt, il semble que la moitié du code avec lequel nous devons travailler est encombré avec de mauvaises herbes, des broussailles, du sous-bois, et toutes sortes d'obstacles. Il pourrait même y avoir des vieilles canettes qui trainent et des affaires sales dans un coin. Et même quelques pièges.

<div align="center">
  <img src="{{ site.url }}assets/refactoring_pas_dans_le_backlog/Ref08.jpg" />
</div>

Chaque voyage à travers cette jungle impénétrable de code devient un long périple, pour contourner les sous-bois, et essayer d'éviter les pièges qui ont été laissés précédemment. Inévitablement, nous tombons dans certains d'entre eux et nous devons nous dégager un chemin vers la sortie. Nous allons encore plus lentement qu'auparavant. Les choses doivent changer !

<div align="center">
  <img src="{{ site.url }}assets/refactoring_pas_dans_le_backlog/Ref09.jpg" />
</div>

Nous voyons maintenant très nettement l'importance des problèmes, et nous voyons que nous pouvons pas faire une simple tonte sur notre terrain et que de toute façon cela ne sera d'aucune utilité. Nous avons beaucoup de refactoring à faire pour avoir de nouveau un terrain propre. Nous sommes tentés de demander du temps au product owner pour refactorer. Bien souvent, ce temps ne sera pas accordé : nous demandons du temps pour corriger ce que nous avons bousillé dans le passé. Et c'est certain, que personne ne nous laissera du temps pour nous en occuper.

<div align="center">
  <img src="{{ site.url }}assets/refactoring_pas_dans_le_backlog/Ref10.jpg" />
</div>

Si l'on nous donne le temps, nous n'obtiendrons pas un très bon résultat. Nous désherberons tout ce que nous voyons, autant que nous le pouvons dans le temps imparti, mais ce ne sera jamais suffisant. Il nous a fallu plusieurs semaines pour mettre le code dans cet état, et nous n'aurons certainement pas le même nombre de semaines pour le corriger.

Ce n'est pas la voie à suivre. Une grosse session de refactoring est difficile à vendre, et si c'est le cas, après une longue attente, elle nous rapporte moins que ce que nous aurions pu l'espérer. Ce n'est pas une bonne idée. Que devrions-nous faire ?

<div align="center">
  <img src="{{ site.url }}assets/refactoring_pas_dans_le_backlog/RefA1.jpg" />
</div>

C'est simple ! Nous prenons la fonctionnalité suivante qu'il nous est demandé d'implémenter, et à la place de contourner toutes les broussailles et les sous-bois, nous prenons le temps de débroussailler un chemin à travers certains. Peut-être ferons-nous un détour pour d'autres. Nous améliorons le code sur lequel nous travaillons, et ignorons le code sur lequel nous n'avons pas à travailler. Nous aurons un magnifique chemin dégagé pour une partie de notre travail. Il y a de fortes chances que nous passerons de nouveau par là : c'est ainsi que de le développement logiciel fonctionne.

Peut-être que cette fonctionnalité prendra un peu plus de temps à implémenter. Mais souvent, ce ne sera pas le cas, parce que ce nettoyage nous aidera ensuite avec la première fonctionnalité qui suivra ce chemin. Et bien sûr, cela aidera toutes les autres qui suivront par là aussi.

<div align="center">
  <img src="{{ site.url }}assets/refactoring_pas_dans_le_backlog/RefA2.jpg" />
</div>

Nettoyer, répéter. Avec chaque nouvelle fonctionnalité, nous nettoyons le code utilisé par cette fonctionnalité. Si nous avons continué à dégager le terrain, nous aurons investi un peu plus de temps que nécessaire, mais pas beaucoup plus - et bien souvent moins. Tout spécialement si le processus est continu, nous tirons de plus en plus de bénéfices de notre nettoyage, et les choses commencent à aller de plus en plus vite.

<div align="center">
  <img src="{{ site.url }}assets/refactoring_pas_dans_le_backlog/RefA3.jpg" />
</div>

Bientôt, souvent pendant le même sprint sur lequel nous avons commencé à nettoyer, nous trouvons qu'une fonctionnalité subséquente utilise une zone que nous venons juste de nettoyer. Tout de suite, nous commençons à tirer les bénéfices du refactoring incrementale. Si nous avions attendu de le faire dans un lot dédié, cela nous aurait demandé plus d'efforts, cela aurait retardé les bénéfices à encore plus tard, et certainement nous aurions gaspillé nos efforts à des endroits qui ne nous auraient rien rapporté.

Le travail se passe mieux, le code devient plus propre, et nous livrons plus de fonctionnalités que nous ne le pouvions le faire avant. Tout le monde y gagne.

C'est comme cela que vous le faites.

---
Auteur : [Ron Jeffries](http://www.xprogramming.com/)  
Source : [Refactoring - Not on the backlog!](http://xprogramming.com/articles/refactoring-not-on-the-backlog/)  
Date de parution originale : 29 juillet 2014  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 25/09/2014  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

---
layout: post
title:  "Questions/Réponses à propos de la vélocité - 8ème partie"
date:   2020-05-08 00:00
published: true
tags:
- vélocité
---

Dans notre [précédent article](http://www.les-traducteurs-agiles.org/2020/04/15/questions-reponses-a-propos-de-la-velocite-7eme-partie.html), nous avons discuté de faire de plus petites unités de travail et de ne pas en faire plus qu'il n'est nécessaire pour répondre au besoin de notre utilisateur final. De cette manière, nous terminons davantage de choses, nous les livrons plus rapidement, et nous développons moins de code inutile (étant donné que nous avons des retours d'informations réguliers de la part des utilisateurs).

Les fans du développement agile de logiciels reconnaîtront là l'un des concepts axiomatiques derrière agile basé sur des travaux beaucoup plus anciens comme le [développement itératif et incrémental (vo)](https://en.wikipedia.org/wiki/Iterative_and_incremental_development). Sans développement incrémental, itératif et sans retours d'informations, un processus quel qu'il soit aura du mal à se dire agile d'une quelconque manière.

Donc, reprenons la conversation à partir de là aujourd'hui.

> A : ... Mais, j'ai … nous avons obtenu 23 points aujourd'hui et les éléments sont de la même taille que ceux qui correspondaient à 1/19ème de sprint.  
> B : Il y a deux explications possibles.  
> A : Quelle est la première explication ?  
> B : C'est que l'équipe attribue un nombre de points supérieur pour un travail de taille identique, en un mot c'est : l'_inflation_.  
> A : Pourquoi feraient-ils cela ?

Les salariés dans une entreprise essayent de satisfaire constamment leurs patrons. Lorsque les entreprises mettent la pression sur les développeurs pour produire davantage de points, les développeurs commencent à trouver des biais pour faire monter le score du nombre de points. Il y a quelques exemples hilarants dans cet [article de Joshua Kerievsky](https://www.industriallogic.com/blog/stop-using-story-points/) sur les _story points_ publié sur le [blog](http://blog.industriallogic.com/) d'Industrial Logic. Certaines fois, c'est fait intentionnellement, mais pas toujours.

Lorsqu'une équipe a fait 8 points sur un sprint, une itération ou autre chose d'équivalent, et qu'elle est déçue, elle aura souvent tendance à regarder en arrière sur la semaine écoulée ; elle réalisera qu'elle a _sous-estimée_ certaines _stories_ qui étaient plus difficiles qu'elles ne paraissaient. Et c'est la raison pour laquelle le sprint a fait seulement 8 points alors qu'il aurait dû faire 15 points. En réaction à cela, elle fera des surestimations la prochaine fois. Ce genre d'inflation n'est pas fait dans l'intention de duper, mais pour mieux refléter la réalité et la vérité. Et désormais l'équipe est plus satisfaite de faire un sprint à 15 points avec la même quantité de travail accomplit.

L'interprétation faite par certaines personnes qu'il s'agit d'une certaine forme d'accélération n'est pas dans l'intention de l'équipe. Elle s'octroie simplement le crédit mérité pour le travail réellement effectué.

« Marquer des points » et « avoir des hauts scores » illustrent de manière très classique la [loi de Goodhart](https://fr.wikipedia.org/wiki/Loi_de_Goodhart). Un indicateur (d'un taux de réalisation) qui s'avère un indicateur raisonnable, une fois choisit comme objectif, cesse d'être un indicateur valide.

Vous entendrez certaines équipes de développement engagées dans des processus _à là_ scrum parler de travail "qui explose". C'est-à-dire « comme un ballon » et non « comme de la dynamite ». Comme par exemple pour une _story_ à qui l'on donne un petit 2, mais qui s'avère prendre la quasi-totalité du sprint parce qu'elle comporte tout un tas de risques et d'incertitudes que personne n'a vu.

Une _story_ peut avoir semblé simple : « ajouter un champ pour un code de réduction ». Le _product owner/manager_ ou le patron a peut-être dit : « cela ne devrait être qu'une _story_ a deux points ».

Cela semble facile. Cela devrait être facile à faire. Qu'est-ce qui pourrait être plus simple que ça ? Il s'agit d'un champ dans un formulaire et vous soustrayez une valeur d'un total.

Mais ce genre de choses sont rarement aussi simple. Le marketing et la comptabilité veulent tracer les remises, les dates d'expiration des réductions, les données à caractère démographiques liées à l'utilisation des réductions. Les réductions doivent apparaître sur la facture du client pour lui montrer qu'il a fait une bonne affaire (marketing !). Les remises doivent figurées sur les rapports de vente.

Il peut y avoir des tableaux de bord dédiés aux remises pour mesurer le succès des promotions. Il peut y avoir aussi des ramifications anti-fraudes.

Puis tout d'un coup quelqu'un décide qu'il devrait y avoir plusieurs codes de réductions et qu'ils devraient se combiner d'une certaine façon et pas d'une autre. Désormais l'expérience utilisateur doit redessiner le nouveau formulaire, et il y a des règles compliquées. Peut-être a t-on besoin d'un nouveau microservice ?

Mais c'était bien une _story_ a 3 points, n'est-ce pas ? Cela amène donc les questions suivantes :

* Pourquoi l'équipe a fait seulement 5 points à ce sprint ?
* Qu'est-ce qui se passe MAL chez elle ?
* Pourquoi ralentit-elle ?
* Qu'est-ce qui peut la motiver à aller plus vite ?
* L'équipe X a fait 50 points par rapport à cette équipe qui en a fait 5, pourquoi l'équipe X fait-elle 10 fois mieux ?
* Est-ce que cette équipe a besoin d'un plan d'amélioration des performances ?

Il s'agit là de **mauvaises questions**. Elles sont basées sur de mauvaises hypothèses et agir dans leurs sens ne fera qu'empirer les choses. Nous avons discuté précédemment de l'[espace de curiosité](http://www.les-traducteurs-agiles.org/2016/10/16/espace-de-curiosite.html) en relation avec la vélocité évoquée en [partie 6](http://www.les-traducteurs-agiles.org/2020/03/26/questions-reponses-a-propos-de-la-velocite-6eme-partie.html) que vous pourriez bien avoir envie d'aller relire désormais.

Enfin, la chose à comprendre à propos des équipes utilisant des temps impartis[^1] c'est que la même quantité de travail est faite chaque semaine (exception faite des absences, des réunions et des évènements pris sur le temps de l'entreprise). [La vélocité est la plupart du temps une illusion (vo)](https://agileotter.blogspot.com/2012/09/14-weird-observations-about-agile-team.html).

Réfléchissez donc à la loi de Goodhart, à l'espace de curiosité, aux _stories_ qui explosent et à l'inflation.

Puis revenez vous joindre à nous pour la [9ème partie (vo)](http://agileotter.blogspot.com/2019/08/q-and-on-velocity-part-ix.html).

[^1]: ou les timeboxes si vous préférez le terme anglo-saxon - NdT

---
Auteur : Tim Ottinger  
Source : [Q and A on velocity, Part VIII ](http://agileotter.blogspot.com/2018/12/q-and-on-velocity-part-viii.html)  
Date de parution originale : 19 Décembre 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 08/05/2020  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

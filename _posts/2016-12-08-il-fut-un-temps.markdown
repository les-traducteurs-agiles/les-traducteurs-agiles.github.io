---
layout: post
title:  "Il fût un temps …"
date:   2016-12-12 00:00:01
published: true
categories: 
- scrum
- dark scrum
---

> Il fût un temps où vous receviez une spec, où vous étiez mis sous pression par des gens qui vous disaient que vous deviez le faire en 6 mois, puis où vous étiez laissé à votre sort pendant 6 mois. Maintenant, ils viennent vous faire c** tous les p** de jours ! - Ron Jeffries (Twitter)

Avec [Dark Scrum](http://www.les-traducteurs-agiles.org/scrum/2016/11/20/dark-scrum.html), les développeurs ressentent exactement ce que décrit cette citation. Au moins, au bon vieux temps ils avaient le temps d’essayer de livrer ce qui était souhaité, avec seulement peut-être quelques rapports mensuels à fournir et quelques rodomontades occasionnelles, histoire de remonter le morale. Maintenant, on dirait que chaque planification de sprint, chaque revue de sprint, chaque rétrospective de sprint, et on atteint le summum, chaque mêlée quotidienne est une opportunité pour mettre à nu l’équipe pour voir comment elle bosse.

Scrum n’est vraiment pas comme ça, mais trop souvent, Scrum se transforme en Dark Scrum et le monde devient risqué pour les développeurs. Cette série d’articles aborde comment nous pouvons faire pour arranger cela.

Le fait est que Scrum (euh en fait Extreme Programming) est la meilleure manière de développer un logiciel que j’ai pu expérimenter.

Je fais du développement logiciel depuis plus d’un demi siècle, et par développer je veux vraiment dire programmer. Hier, j’ai travaillé sur un programme. Je programme presque tous les jours. Pas sur un truc aussi difficile que ce que vous et votre équipe êtes en train de travailler, mais suffisamment difficile tout de même. Et vraiment, sincèrement le cycle Scrum / XP fondamental qui suit, peut tout simplement être génial :

* Travailler activement avec le Client ou le Product Owner pour comprendre le problème
* Décider toutes les semaines ou toutes les deux semaines quoi faire ensuite
* Se mettre d’accord avec le Client sur des exemples concrets de ce qu’il y a à faire
* Faire le travail, se retrouver entre nous fréquemment pour être certain que nous sommes dans les clous
* Montrer à notre client et aux autres parties prenantes une version opérationnelle livrable de ce que nous avons toutes les semaines ou toutes les deux semaines
* Se retrouver toutes les semaines ou toutes les deux semaines pour examiner comment nous travaillons et trouver des manières de nous améliorer.

C’est vraiment quelque chose de bien. Ce cycle est la meilleure manière de travailler que j’ai pu expérimenter en un demi siècle de réalisation de logiciel. Lorsque nous pouvons montrer un vrai logiciel opérationnel à nos parties prenantes, les conversations peuvent changer de vagues explications et de vagues menaces à des choses plus productives sur ce qu’il faut faire ensuite et comment faire mieux. Oh, nous devons avoir des conversations, et nous devons savoir comment les orienter afin de parler de la réalité, et nous pouvons le faire, parce que nous avons une réalité - celle d’un logiciel opérationnel - à portée de la main pour discuter.

Cela signifie qu’il y a un certain nombre de choses où nous, développeurs, sommes devenus bon. Nous en parlerons de choses en profondeur tout au long de cette série d’articles. Ces choses sont notamment les suivantes :

* Comment retourner une conversation grâce à l’Incrément, si nous en avons un.
* À quoi doit ressembler un Incrément pour être un agent efficace du changement
* Comment orienter la planification vers des chemins plus sensés plutôt que dans un esprit “on fonce, on fait tout”
* Comment s’assurer que le Client et les développeurs soient sur la même longueur d’onde
* Comment réaliser une application opérationnelle et robuste dans le temps

… et plein d’autres choses encore. Nous itèrerons sur ces sujets tout au long de cette série, en explorant les idées dont nous avons besoin et comment y arriver. Mais pour l’instant …
Imaginons ce que nous pourrions faire.

Supposez qu’il y ait une manière quelconque, aussi magique soit-elle, de se mettre d’accord avec nos parties prenantes sur ce qu’il y a à faire le lundi, et qu’au vendredi, nous ayons entre les mains le fruit de notre meilleure compréhension, opérationnel, intégré, si propre et si fini qu’ils peuvent l’utiliser ou le livrer si elles le veulent. Si bien fignolé que la seule raison de ne pas livrer le produit est qu’il ne contient pas encore quelque chose d’important qu’elles n’ont pas encore demandé.

Imaginez que nous pourrions construire un logiciel de manière incrémentale, fonctionnalité par fonctionnalité, bien testé et bien intégré, prêt à être livré à volonté.

Maintenant bien sûr, nos parties prenantes pourraient toujours vouloir que nous en fassions plus, plus vite, avec de plus en plus de fonctionnalités. C’est leur boulot d’en vouloir plus. Et nous pourrions même leur répondre en toute sincérité :

> Nous allons aussi vite que possible. Nous nous rencontrons toutes les semaines pour essayer de trouver comment aller encore plus vite. Au jour d’aujourd’hui, voici ce que nous avons, et chaque semaine vous devez nous dire ce qui est important à vos yeux, et nous vous dirons en retour ce que nous pensons que nous pourrons accomplir. Une semaine plus tard, vous l’aurez entre vos mains. Aujourd’hui, cette version est entre vos mains. Elle est bien faite, testée, prête à être livrée. Vous pourriez la mettre en production si vous le voulez : voici une copie sur CD et une enveloppe. Le manuel mis à jour figure aussi sur le CD.

Les parties prenantes seraient vraiment aveugles pour ne pas comprendre comment ça fonctionne : dites-nous ce qui est le plus important, mettez-vous d’accord avec nous sur les éléments permettant de dire que ces besoins ont été remplis, allez ensuite en coulisse et venez voir le vendredi suivant ce que nous avons fait. Les parties prenantes seraient vraiment bêtes de ne pas voir suffisamment tôt que s’ils arrêtent leurs idées folles, ils pourraient avoir rapidement quelque chose entre les mains de leurs clients, résoudre leurs problèmes et rapporter de l’argent. Et nous serions tout disposer à les aider pour comprendre cela, au lieu de simplement de nous tenir la tête prêt à recevoir une nouvelle raclée.

Nous pourrions collaborer dans le but d’obtenir une livraison au plus tôt d’un meilleur produit. Nous pourrions devenir une véritable équipe de développement de produit plutôt d’un groupe de serfs que l’on apprécie seulement pour leur capacité à déplacer du fumier tous les jours.

Comment je le sais ? J’ai déjà vu ça plein de fois. J’ai vu arrivé cela assez souvent pour être certain que cela arrive fréquemment. De plus, si vous êtes coincés dans le cauchemar du Dark Scrum, changer la conversation est votre seul véritable espoir, plutôt que de changer de travail ou de profession. Et programmer peut être fun. Vous rappelez-vous quand programmer c’était fun ? Ça peut être fun à nouveau.

Au cœur de cela est l’Incrément. Autrement dit, le logiciel opérationnel testé que nous mettons au centre de la discussion de ce qui va être fait ensuite avant même les parties prenantes. Nous parlerons en profondeur tout au long de cette série d’article des manières spécifiques permettant d’obtenir l’Incrément. Mais vous avez déjà entendu parler de ces manières-là, et vous savez plutôt assez bien comment les faire. L’élément principal est de commencer à tirer profit de vos rétrospectives régulières pour voir ce qu’il y en travers du chemin pour livrer un véritable Incrément, et améliorer comment vous pourriez travailler de manière plus étroite.

Travaillez donc là-dessus. Je reviendrai avec quelques astuces bientôt. [Ou prenez contact](http://agilementoring.com/). J’essaierai de vous aider.

---
Auteur : [Ron Jeffries](http://ronjeffries.com/about.html)  
Source : [Time was …](http://ronjeffries.com/articles/016-09ff/time-was/)  
Date de parution originale : 05 Octobre 2016  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 12/12/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



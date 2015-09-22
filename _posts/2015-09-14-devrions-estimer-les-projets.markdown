---
layout: post
title:  "Devrions-nous estimer les projets ... en fait ?"
date:   2015-09-20 21:00:55
published: true
categories: 
- estimation
---

<div align="left" style="float:left; padding-left:30px" >
  <img title="Dés" src="{{ site.url }}assets/devrions_nous_estimer_les_projets/estimation-300x201.jpg" />
</div>

## Introduction

Après en "avoir eu l'intuition" pendant une année ou deux, et avoir passé plusieurs années à faire des estimations ou à travailler sur les estimations des autres, j'en suis finalement arrivé à la conclusion que l'utilisation de l'estimation sur tout type de projet est non seulement une perte de temps mais est réellement néfaste. 

Je suis tout à fait conscient que c'est une déclaration extrêmement polémique donc je vais essayer d'être aussi rigoureux que possible dans mon explication sur comment je suis arrivée à cette conclusion à travers une expérience, des données et sa validation.  
En effet, lorsqu'il y a quelques mois, j'ai lu [l'article de Vasco Duarte](http://www.les-traducteurs-agiles.org/estimation/2015/09/13/les-story-consideres-comme-dangereux.html), je l'ai vu "pointer"[^1] le bout de son nez (aucun jeu de mots là-dessus) mais j'ai aussi pesé les mérites de l'utilisation de l'estimation en story points dans l'objectif de :

[^1]: l'intuition - NdT

* Dimensionner au préalable un projet pour déterminer sa validité pour un budget ou une période donnés.
* Accroître la compréhension et la connaissance commune de l'équipe sur la base des discussions qui sont survenues lors d'une session de _planning poker_
* Permettre au PO de faire des arbitrages (basés sur le retour sur investissement) entre des stories de différentes tailles  
* Mesurer la vélocité de l'équipe
  * pour valider en continu le dimensionnement initial du projet en prévoyant l'adéquation du périmètre par rapport à une date d'une livraison de version donnée
  * pour permettre à l'équipe de mesurer et d'améliorer sa performance

## Pourquoi ne devrions-nous pas estimer ?

J'en suis arrivé depuis à la conclusion que certaines de ces choses n'ont pas besoin d'être faites du tout, et que d'autres peuvent être faites sans avoir besoin de les estimer (approximation) en aucune façon. Je voudrais maintenant faire valoir que, même si vous reconnaissez les limites de l'estimation et que vous utilisez des fourchettes, que vous prenez en compte l'incertitude, etc... , l'acte de l'estimation en lui-même est néfaste pour les raisons suivantes :

* **Les attentes sur la livraison de projets à périmètre "fixe" sont souvent (toujours ?) basées sur une estimation initiale du périmètre (supposé) et la durée que cela prendra pour livrer ce périmètre (une nouvelle supposition), et conduisent à des dysfonctionnements patents comme les marches forcées, une qualité médiocre, etc ...**

Si le budget est fixé, alors il n'y aucune manière de "dépasser le budget" afin de livrer le périmètre fixé. Toutefois "dépasser le budget" est un terme habituellement utilisé lorsque l'on parle de projets ayant échoués. Si votre budget est vraiment une contrainte alors vous livrerez seulement ce qui peut être livré. Les méthodes agiles veillent à que vous livriiez la plus forte valeur au métier.

_Quelques temps plus tôt, j'avais discuté avec un membre de l'équipe et il se plaignait de ressentir de la pression pour augmenter la vélocité. Je lui ai demandé d'où cette pression venait et il me répondit qu'elle provenait du fait que le projet puisse échouer si l'équipe n'était pas capable de livrer davantage de stories plus rapidement. En réalité, personne ne demandait spécifiquement à l'équipe de livrer plus, mais il y avait une pression implicite de le faire parce qu'elle savait que le budget s'épuisait. Cette façon de voir les choses provient d'années de projets mal financés, de marches forcées, de focalisation sur la productivité plutôt que sur la qualité et de projets qui ont été étouffés ou ayant échoués._

* **Demander aux équipes d'estimer la durée de leur travail (ou du nombre de points qu'elles livreront en un sprint ou pour une version, ce qui revient au même ...) a des connotations laissant entendre que leur travail est mesuré par une tierce partie (le responsable), créant un environnement de peur et de manipulation de chiffres pour refléter ce qui est désiré plutôt que pour ce qui est prévisible** 

Pour accroître la vélocité, l'équipe doit simplement surestimer les stories pour donner l'illusion de livrer plus. Ils ne le font peut être pas consciemment mais cela peut arriver inconsciemment. Le chef de projet leur fait alors une tape dans le dos, mais tout ce qui s'est passé c'est que la même quantité de logiciel fonctionnel "fini" a été livré. 

Le moment est venu d'avoir et d'utiliser de vraies données pour donner l'image de la progression réelle, qu'elle soit bonne ou mauvaise.

* **Nous ne devrions pas définir la totalité du périmètre initial, cela signifie que nous ne devrions pas estimer tout le périmètre initial, ce qui veut dire également que nous ne devrions pas définir notre date de livraison sur la base de notre périmètre**

Nous devrions fixer notre date pour la livraison de la version 1 et avoir l'objectif de réaliser le meilleur produit possible pour cette date (périmètre variable).

Dès que nous introduisons le mot "estimation", l'attitude par défaut est de penser à "combien de temps ce projet prendra ?" (même si cela n'a pas été demandé explicitement). Cela provoque en nous la prise en compte du périmètre et de la durée complète du projet (c'est tout à fait anti-agile et je n'expliquerai pas ici pourquoi il s'agit d'une mauvaise idée car il y a eu suffisamment d'écrits à ce sujet ailleurs)

## Comment déterminons-nous la taille d'un projet ?

Réponse courte - vous ne devriez pas. Si vous n'avez pas une date butoir ferme pour votre projet (par exemple le 1er jour du Grand Prix pour une application sur le Grand Prix), vous aurez un budget pour votre projet (fixé par le PMO ou par le client externe) à partir duquel vous pourrez déterminer une date butoir. La chose maline à faire est alors de planifier une version intermédiaire (disons à mi-chemin) où vous pourrez jauger de la façon  dont le projet se déroule sur la base de la mesure d'un logiciel qui fonctionne.

Par exemple, si votre budget vous permet d'avoir assez d'argent pour dix sprints de 2 semaines (avec une équipe dédiée à 100 %),  vous devriez supposer, de manière évidente, que votre date de mise en production sera dans un délai de 20 semaines. Mais l'objectif devrait être d'avoir un logiciel opérationnel en environnement de production dans un délai de 2 semaines (après le sprint 1). Vous devriez alors itérer sur le produit, permettre aux exigences (le périmètre) d'émerger et de donner la direction que le produit prendra, et prendre le temps de réexaminer après le sprint 5. 

Ces choses ne sont pas prévisibles initialement - l'estimation va vous balancer un périmètre gigantesque (les attentes) qui ne sera pas livré et qui génèrera un temps d'analyse inutile (argent) et de la pression.

## Comment l'équipe aura-t-elle une compréhension commune d'une story ?

C'est simple. Lorsqu'un élément est ajouté au-dessus du _product backlog_, l'équipe le discute lors du _sprint planning_ et le décompose si nécessaire. S'il n'a pas besoin d'être décomposé alors il est probable qu'il est déjà bien compris. S'il l'est alors l'acte de le décomposer nécessitera des discussions autour de l'implémentation qui faciliteront une compréhension commune.

En bref, l'équipe n'a pas besoin d'être dans une réunion d'estimation pour discuter et décomposer une story.

## Comment le PO prend-t-il des décisions d'arbitrage ?

Le PO doit probablement connaître le ROI d'une story lorsqu'il la présente à l'équipe pour qu'elle soit livrée. Afin de calculer le ROI, il doit connaître combien elle va coûter pour être livrée (sa durée).

À partir de là, une équipe estimerait l'item en utilisant les story points et ensuite le PO, armé de la vélocité de l'équipe, pourrait estimer le ROI de l'item. Mais sans les _story points_, comment cela peut il être accomplit ?

C'est là où le concept d'"estimation implicite" vient en jeu. Afin de créer la prédictibilité dans le flux de travail, l'équipe décomposera les stories juste-à-temps (lors du _sprint planning_) afin qu'elles soient grosso modo de la même taille. C'est là quelque chose qui arrive naturellement le long de la vie du projet. Avec le temps, la taille des stories se normalise parce que l'équipe veut naturellement des petits morceaux sur lesquels travailler pendant la courte période du sprint. Elle est habituée à livrer un certain nombre de stories, plus ou moins, dans un sprint.

Donc pour que le PO puisse chiffrer l'item, il doit juste demander à l'équipe si l'item est compris ou s'il doit être décomposé. Si le PO le considère comme ayant une priorité assez haute, il voudra le présenter au _sprint planning_ afin qu'il soit vu tout de suite, si bien sûr cela a un sens de faire ainsi. Le _sprint planning_ est le moment pour l'équipe de décomposer la story si nécessaire et de décider si elle peut être livrée pendant le sprint. Si elle peut, le coût de l'item est essentiellement les 2 semaines de salaires de l'équipe (en supposant que le déploiement en production soit fait à la fin du sprint  - un modèle de livraison continu peut améliorer la vitesse de mise sur le marché et le ROI, mais ceci est une discussion pour un autre jour).

Si l'item ne peut être livré pendant le sprint, le PO peut simplement regarder combien de stories ont été tirées d'un _epic_ et déterminer la probabilité d'être livré au prochain sprint ou au sprint d'après, en se basant sur la quantité de stories que l'équipe délivre habituellement. Cela me conduit naturellement vers le sujet de comment nous mesurons la vélocité en l'absence de _story points_.

## Comment mesurons-nous la vélocité ?

Désormais, je me déplace avec résolution sur le territoire de Duarte. La réponse est que nous comptons le nombre de stories plutôt que d'accumuler les _story points_, éliminant ainsi le besoin d'estimer. Comme je l'ai mentionné précédemment, les équipes décomposent les stories en plus petites ayant grosso modo la même taille, donc compter combien de stories sont livrées lors de chaque sprint donne ainsi une mesure de la vélocité satisfaisante. Si l'équipe livre habituellement 5 stories avec zéro défaut et ensuite un sprint avec 6 ou 7 stories ayant zéro défaut, c'est qu'une amélioration a été faite (en écartant la variance, qui existe bien quelque soit l'unité de mesure que vous utilisez pour la vélocité).

À cause de l'intuition dont j'ai parlé plus tôt, j'ai fait le suivi de la vélocité de mon équipe actuelle à la fois sous la forme du comptage de story et de points et j'ai fait des projections en utilisant les deux méthodes. Comme je l'avais suspecté (et comme [Duarte l'avait fait remarqué](http://www.les-traducteurs-agiles.org/estimation/2015/09/13/les-story-consideres-comme-dangereux.html) en s'appuyant sur tout un tas de données), le comptage de données donne une mesure tout aussi bonne, si ce n'est mieux, de l'avancée et de la prédictibilité que les story points ne l'auraient fait. Par conséquent, pourquoi perdre tout ce temps, cet argent, et ces efforts en sessions d'estimations et de calculs de vélocité ?

Alors que le comptage des story fonctionne bien pour la vélocité, je voudrais tout de même alerter de son utilisation ou de l'utilisation de toute autre mesure de la vélocité comme une manière de prévoir sur quand vous pouvez livrez. Vous devriez savoir quand vous êtes en train de livrer et seulement prévoir ce que vous pouvez livrer à cette date. Ne laissez pas la chance guider votre date de livraison, même si vous utilisez des données plutôt que des approximations pour prédire combien de stories pourront être finies.

Ce que vous pouvez faire, toutefois, est d'utiliser la vélocité pour aider le PO à comprendre les arbitrages du périmètre dans le backlog (_les données m'indiquent que l'équipe peut livrer 20 stories de plus avant la date de livraison, donc je voudrai être sûr que les 20 plus importantes soient en haut du backlog_).

## Conclusion

Cela m'a pris plusieurs années pour arriver à cette conclusion. Mais, si vous y pensez, les gens s'esclaffent et plaisantent tout le temps à propos des estimations. Tout le monde sait que ce sont des suppositions. Tout le monde sait qu'elles sont fausses. Toutefois nous continuons de les faire. Je crois qu'il est temps pour nous de reconnaître qu'il est plus sensé d'éliminer le risque et le coût de l'estimation complètement et d'utiliser uniquement des données empiriques (telles que Agile et Scrum le promeuvent) pour faire des prévisions.

Dans un monde sans la charge de l'estimation, l'équipe sera probablement plus heureuse et plus productive, l'inefficacité du temps passé à estimer plutôt que livrer un logiciel opérationnel sera éliminée et le PO aura des données réelles avec lesquelles prendre des décisions plutôt que faire, sous pression, des suppositions .

Pour résumer :

* N'estimez pas votre date de livraison - basez-la sur votre budget ou sur une date butoir ferme
* N'estimez pas le périmètre - permettez-le d'émerger afin de récolter les bénéfices de construire des produits avec agilité
* N'estimez pas explicitement les items du _product backlog_ (stories)
* Utilisez des données historiques (comptage des stories) pour prévoir la livraison du périmètre à une date donnée
* Utilisez l'estimation implicite en juste-à-temps (la décomposition de stories lors d'un _sprint planning_) et les données historiques pour estimer le coût (ROI) de livraison d'une story

Je n'aime pas supposer, mais je prédis que ne pas estimer vos projets rendra le succès beaucoup plus certain :) 

---
Auteur : [Neil Killick](https://plus.google.com/u/0/+NeilKillick/about)  
Source : [Should We Estimate Software Projects… At All?](http://neilkillick.com/2012/04/12/do-not-estimate-software-projects-at-all/)  
Date de parution originale : 12 Avril 2012  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Relecteur : [Sylvain Fraïssé](http://www.les-traducteurs-agiles.org/traducteurs/), [Baptiste Mathus](http://batmat.net/cv/fr.html)   
Date de traduction : 20/09/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}


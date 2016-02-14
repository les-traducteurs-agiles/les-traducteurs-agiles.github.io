---
layout: post
title:  "Est-ce qu’une spécification des exigences traditionnelles peut être convertie en user stories ?"
date:   2016-02-14 20:00:55
published: true
categories: 
- user-stories
---

Un certain nombre de projets gérés de manière traditionnelle débutent avec une spécification des exigences. Puis quelques fois il arrive pendant la vie d’un projet que la décision soit prise d’adopter une approche agile. Survient alors la question toute naturelle de savoir si une spécification des exigences peut servir de _product backlog_ pour ce projet nouvellement devenu agile. Certaines équipes envisagent d’aller jusqu’à procéder à la réécriture de la spécification des exigences sous la forme d’un _product backlog_ et de _user stories_. Regardons si cela est vraiment nécessaire

Mais avant d’aborder cette question, je veux clarifier le point sur ce que j’entends par spécification des exigences. Je trouve que ce type de document varie grandement d’une entreprise à une autre. En général, ce à quoi je pense dans ce cas cependant, c’est au document type remplit de déclaration du genre “Le système devrait ...”.

Même avec toutes sortes de documents d’exigences écrits de manière traditionnelle que vous pourriez imaginer, mes conseils devraient pouvoir continuer à s’appliquer. Cela est plus particulièrement le cas pour tout document ayant des listes d’exigences numérotées et imbriquées, peu importe que chaque affirmation soit vraiment écrite ou pas sous la forme de “le système devrait ...”

## Quelques inconvénients quant à l’utilisation d’une spécification en tant que _product backlog_.

Dans le développement agile d’un produit, le _product backlog_ sert à deux choses :

* Il sert de dépôt pour le travail à faire
* Il facilite la priorisation du travail

C’est-à-dire que le _product backlog_ indique à l’équipe ce qui doit être fait et qu’il peut être utilisé comme un outil de planification pour séquencer le travail. En contraste, une spécification traditionnelle des exigences gère uniquement la problèmatique de ce qui doit être fait sur le projet.

Il n’y aucune possibilité avec une spécification des exigences d’écrire des exigences pouvant être implémentées en un sprint ou priorisées. Écrire des exigences indépendantes est au mieux un objectif secondaire comme peut le montrer l’organisation hiérarchique de la plupart des documents de spécification des exigences, avec leurs exigences numérotées 1.0, 1.1, 1.1.1, et ainsi de suite.

Cela ne constitue pas un problème lorsqu’une spécification des exigences est considérée uniquement comme un document d’exigences. Mais lorsque les items à l’intérieur d’une spécification des exigences seront utilisées aussi comme items d’un _product backlog_ et donc priorisés, cela créera alors des problèmes.

Avec une spécification des exigences, il est souvent impossible pour une équipe de développer l’exigence 1.1.1 sans avoir à développer en parallèle la 1.1.2 et la 1.1.5. Ces dépendances ne facilitent pas le fait de prendre une _story_ à la fois dans un _product backlog_ en bonne et dûe forme.

Priorisés les sous-items d’une spécification des exigences c’est également difficile tout comme peut l’être l’identification d’un sous-ensemble de fonctionnalités pour créer un produit viable à minima.

Une spécification des exigences est juste bonne à être ... une spécification des exigences. Il est bon de dire ce que le système ou le produit doit faire. (La spécification des exigences échoue bien entendu sur tous les aspects agiles de l’émergence des exigences, de la collaboration, devla découverte et ainsi de suite. Je suppose que cela continuera à se produire dans le futur).

Mais une spécification des exigences n’est pas faite pour l’organisation, la priorisation et la planification du travail. Un _product backlog_ est utilisé pour tous ces aspects d’un projet agile.

## Mon conseil

En général, je ne recommande pas de prendre le temps de réécrire une spécification des exigences faite dans les règles de l’art. Réécrire une spécification des exigences sous la forme de _user stories_ et d’un _product backlog_ pourrait permettre de répondre aux problèmes que j’ai souligné précédemment. Mais, généralement cela ne vaut pas la peine de perdre du temps à réécrire les spécification des exigences en _user stories_.

Quelqu’un devra passer du temps à faire ça, et généralement cette personne pourrait passer son temps d’une meilleure manière. Je serais particulièrement réticent à réécrire une spécification des exigences surtout si d’autres co-équipiers sont bloqués dans leur propre boulot dans l’attente d’un _product backlog_ réécrit. 

Un ScrumMaster ou quelqu’un d’autre dans l’équipe devra trouver la manière de suivre l’avancée par rapport à la spécification des exigences et s’assurer que des exigences présentes ne passent pas à travers les mailles du filet. Avoir de l’aide auprès de l’assurance qualité pour valider que l’ensemble de la spécification des exigences est fait ou listé dans le _product backlog_ est fortement conseillé.

Une autre stratégie serait d’éduquer ceux impliqués dans la création des spécifications des exigences d’envisager de le faire d’une manière plus agile pour des projets futurs. Si vous pouvez faire cela, vous aiderez votre prochain projet à éviter les écueils liés à l’incompatibilité entre l’agilité et le fait de commencer avec un document de spécification des exigences.

## Qu’en pensez-vous ?

Joignez-vous à notre discussion et partagez avec nous votre avis  et vos expériences dans les commentaires ci-dessous [^1]. Avez-vous déjà travaillé sur un projet agile qui ait commencé avec une spécification traditionnelle des exigences ? Comment cela s’est-il passé ? Est-ce que cela aurait été différent si la spécification des exigences avait été réécrite sous la forme plus agile d’un _product backlog_ ?

[^1]: ou dans votre réseau social préféré, notre site étant dépourvu de commentaires - NdT

---
Auteur : [Mike Cohn](http://www.mountaingoatsoftware.com/company/about-mike-cohn)  
Source : [Can a Traditional SRS Be Converted into User Stories?](https://www.mountaingoatsoftware.com/blog/can-a-traditional-srs-be-converted-into-user-stories)  
Date de parution originale : 05 Janvier 2016  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 14/02/2016  

---

Copyright ©1998-2015 Mountain Goat Software. All Rights Reserved.

---

{% include share_buttons.html %}


---
layout: post
title:  "Est-ce qu’une spécification des exigences traditionnelles peut-elle être convertie en user stories ?"
date:   2016-02-11 21:00:55
published: true
categories: 
- user-stories
---

A lot of traditionally managed projects begin with a Software Requirements Specification (SRS). Then sometime during the project, a decision is made to adopt an agile approach. And so a natural question is whether the SRS can serve as the newly agile project's product backlog. Some teams contemplate going so far as rewriting the SRS into a product backlog with user stories. Let's consider whether that's necessary.

Beaucoup de projets gérés de manière traditionnelle débutent avec une spécification des exigences. Puis quelques fois il arrive pendant la vie d’un projet de prendre la décision d’adopter une approche agile. Survient alors la question toute naturelle de savoir si une spécification des exigences peut servir de _product backlog_ pour ce projet nouvellement agile. Certaines équipes envisage d’aller jusqu’à procéder à la réécriture de la spécification des exigences sous la forme d’un _product backlog_ et de _user stories_. Regardons si cela est vraiment nécessaire

But before taking up this question, I want to clarify what I mean by a Software Requirements Specification or SRS. I find this type of document to vary tremendously from company to company. In general, though, what I'm referring to is the typical document full of "The system shall ..." type statements.

Mais avant de prendre la question, je veux clarifier sur ce que j’entends par spécification des exigences. Je trouve que ce type de document varie grandement d’une entreprise à une autre. En général, ce à quoi je pense dans ce cas cependant c’est au document type remplit de déclaration du genre “Le système devrait ...”.

But you can imagine any sort of traditional requirements document and my advice should still apply. This is especially the case for any document with numbered and nested requirements statements, regardless of whether each statement is really written as "the system shall ..."

Mais vous pouvez imaginer toutes sortes de documents d’exigences tels que vous pouvez les trouver habituellement ; mes conseils devraient pouvoir continuer à s’appliquer. Cela est plus spécialement le cas pour tout document ayant des listes d’exigences numérotées et imbriquées, peut importe que chaque affirmation soit vraiment ou pas écrite sous la forme de “le système devrait ...”

## Some Drawbacks to Using the SRS as a Product Backlog

## Quelques inconvénients quant à l’utilisation de la spécification en tant que _product backlog_.

On an agile product, the product backlog serves two purposes:

Dans le développement agile d’un produit, le _product backlog_ sert à deux choses :

* It serves as a repository for the work to be done
* It facilitates prioritization of work

* Il sert de dépôt pour le travail à faire
* Il facilite la priorisation du travail

That is, the product backlog tells a team what needs to be done and can be used as a planning tool for sequencing the work. In contrast, a traditional SRS addresses only the issue of what is to be done on the project.

C’est-à-dire que le _product backlog indique à l’équipe ce qui doit être fait et qu’il peut être utilisé comme un outil de planification pour séquencer le travail. En contraste, une spécification traditionnelle des exigences gère uniquement la problèmatique de ce qui doit être fait sur le projet.

There is no attempt with an SRS to write requirements that can be implemented within a sprint or that are prioritized. Writing independent requirements is a minor goal at best, as shown by the hierarchical organization of most SRS documents, with their enumerated requirements such as 1.0, 1.1, 1.1.1, and so on.

Il n’y aucune possibilité avec une spécification des exigences d’écrire des exigences pouvant implémentées en un sprint ou priorisées. Écrire des exigences indépendantes est au mieux un objectif mineur comme peut le montrer l’organisation hiérarchique de la plupart des documents de spécification des exigences, avec leurs exigences numérotées 1.0, 1.1, 1.1.1, et ainsi de suite.

These are not problems when an SRS is evaluated purely as a requirements document. But when the items within an SRS will also be used as product backlog items and prioritized, it creates problems.

Cela ne constitue pas un problème lorsqu’une spécification des exigences est considéré uniquement comme un document d’exigences. Mais lorsque les items à l’intérieur d’une spécification des exigences seront utilisées aussi comme items d’un _product backlog_ et donc priorisés, cela créera alors des problèmes.

With an SRS, it is often impossible for a team to develop requirement 1.1.1 without concurrently developing 1.1.2 and 1.1.5. These dependencies make it not as easy as picking a story at a time from a well-crafted product backlog.

Avec une spécification des exigences, il est souvent impossible pour une équipe de développer l’exigence 1.1.1 sans avoir à développer en parallèle la 1.1.2 et la 1.1.5. Ces dépendances ne facilitent pas le fait de prendre une story à la fois dans un _product backlog_ en bon et dû forme.

Prioritizing sub-items on an SRS is also difficult, as is identifying a subset of features that creates a minimum viable product.

Priorisés les sous-items d’une spécification des exigences est également difficile tout comme peut l’être l’identification d’un sous-ensemble de fonctionnalités pour créer un produit viable à minima.

A Software Requirements Specification is good at being a requirements specification. It’s good at saying what a system or product is to do. (Of course, it misses out on all the agile aspects of emergent requirements, collaboration, discovery, and so on. I’m assuming these will still happen.)

Une spécification des exigences est juste bonne à être ... une spécification des exigences. Il est bon de dire ce que le système ou le produit doit faire. (Bien sûr, elle échoue sur tous les aspects agiles de l’émergence des exigences, de la collaboration, devla découverte et ainsi de suite. Je suppose que cela pourra toujours se produire dans le futur).

But an SRS is not good for planning, prioritizing and scheduling work. A product backlog is used for both of these purposes on an agile project.

Mais une spécification des exigences n’est pas faite pour l’organisation, la priorisation et la planification du travail. Un _product backlog_ est utilisé pour tout cela lors d’un projet agile.

## My Advice

## Mon conseil

In general, I do not recommend taking the time to rewrite a perfectly fine SRS. Rewriting the SRS into user stories and a nice product backlog could address the problems I’ve outlined. But, it is not usually worth the time required to rewrite an SRS into user stories.

En général, je ne recommande pas de prendre le temps de réécrire une spécification des exigences qui a été faite dans les règles de l’art. Réécrire une spécification des exigences sous la forme de _user stories_ et d’un _product backlog_ pourrait permettre de répondre aux problèmes que j’ai souligné précédemment. Mais, généralement cela ne vaut pas la peine de perdre du temps à réécrire les spécification des exigences en _user stories_.

Someone would have to spend time doing this, and usually that person could spend their time more profitably. I would be especially reluctant to rewrite an SRS if other teammates would be stalled in starting their own work while waiting for the rewritten product backlog.

Quelqu’un devrait passer du temps à faire ça, et généralement cette personne pourrait passer son temps d’une manière plus profitable. Je serais particulièrement réticent à réécrire une spécification des exigences surtout si d’autres co-équipiers étaient bloqués dans leur propre boulot dans l’attente d’un _product backlog_ réécrit. 

A ScrumMaster or someone on the team will have to find ways of tracking progress against the SRS and making sure requirements within it don’t fall through the cracks. Usually enlisting help from QA in validating that everything in an SRS is done or listed in the product backlog is a smart move.

Un ScrumMaster ou quelqu’un d’autre dans l’équipe devra trouver la manière de suivre l’avancée par rapport à la spécification des exigences et s’assurer que des exigences présentes ne passent pas à travers les mailles du filet. Avoir de l’aide auprès de l’assurance qualité pour valider que l’ensemble de la spécification des exigences est fait ou listé dans le _product backlog_ est stratégiquement avisé.

One additional important strategy would be educating those involved in creating SRS documents to consider doing so in a more agile-friendly manner for future projects. If you can do this, you’ll help your next project avoid the challenges created by a mismatch between agile and starting with an SRS document.

Une autre stratégie serait d’éduquer ceux impliqués dans la création des spécifications des exigences d’envisager de le faire d’une manière plus agile pour de futurs projets. Si vous pouvez faire cela, vous aiderez votre prochain projet à éviter les écueils crées par une incompatbilité entre l’agilité et le fait de commencer avec un document de spécification des exigences.

## What Do You Think?

## Qu’en pensez-vous ?

Please join the discussion and share your thoughts and experiences below. Have you worked on an agile project that started with a traditional SRS? How did it go? Would it have been different if the SRS had been rewritten as a more agile product backlog?

Joignez-vous à notre discussion et partagez avec nous votre avis  et vos expériences dans les commentaires ci-dessous [^1]. Avez-vous déjà travaillé sur un projet agile qui ait commencé avec une spécification traditionnelle des exigences ? Comment cela s’est-il passé ? Est-ce que cela aurait été différent si la spécification des exigences avait été réécrite sous la forme plus agile d’un _product backlog_ ?

[^1]: ou dans votre réseau social préféré, notre site étant dépourvu de commentaires - NdT

---
Auteur : [Mike Cohn](http://www.mountaingoatsoftware.com/company/about-mike-cohn)  
Source : [Can a Traditional SRS Be Converted into User Stories?](https://www.mountaingoatsoftware.com/blog/can-a-traditional-srs-be-converted-into-user-stories)  
Date de parution originale : 08 Décembre 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 11/02/2016  

---

Copyright ©1998-2015 Mountain Goat Software. All Rights Reserved.

---

{% include share_buttons.html %}


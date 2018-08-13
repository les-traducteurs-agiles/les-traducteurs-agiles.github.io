---
layout: post
title:  "INVESTissez dans de bonnes stories et dans des tâches SMART"
date:   2015-02-23 22:35:55
tags: story
---
> Les équipes XP ont à gérer des stories et des tâches. Les acronymes INVEST et SMART peuvent permettre aux équipes de se rappeler les bonnes caractéristiques de chacune.  

En XP, nous pensons aux exigences arrivant sous la forme de user stories. Il serait facile de confondre la carte de story pour la "totalité de la story", mais Ron Jeffries fait remarquer que les stories en XP sont composées de trois éléments : les cartes (le support physique), la conversation (la discussion qui les entoure), et la confirmation (les tests qui les vérifient).  

Un _sabir_ est une langage simplifié, utilisé généralement dans le commerce, permettant aux personnes qui ne peuvent pas communiquer dans leur langue maternelle de pouvoir néanmoins travailler ensemble. Les user stories fonctionnent un peu comme cela. Nous n'attendons pas des clients ou des utilisateurs qu'ils voient le système de la même manière que des développeurs ; les stories agissent comme un sabir à partir duquel les deux parties peuvent se mettre suffisamment d'accord pour travailler ensemble efficacement.  

Mais quelles sont les caractéristiques d'une bonne story ? L'acronyme "INVEST" peut vous rappeler ce que sont de bonnes stories :  

* I - Indépendante
* N - Négociable
* V - (de) Valeur
* E - Estimable
* S - [Suffisamment] petite (NdT - l'initiale de petite (traduction de Small) ne collait pas avec l'acronyme, il a fallu donc trouver un astuce pour conserver l'acronyme INVEST plus facilement à mémoriser que INVEPT)
* T - Testable

### Indépendante

Les stories sont plus faciles à travailler si elles sont _indépendantes_. C'est-à-dire, nous aimerions que les concepts, qu'elles portent, ne se chevauchent pas, et nous aimerions être capable de les planifier et de les implémenter dans n'importe quel ordre.  

Nous ne pouvons pas toujours y parvenir ; une fois de temps en temps, nous pouvons dire des choses comme "3 points pour le premier rapport, puis ensuite 1 point pour chacune des autres".  

### Négociable ... et négociée

Une bonne story est _négociable_. Ce n'est pas un contrat explicite pour des fonctionnalités ; les détails seront plutôt co-créés par le client et le développeur pendant le développement. Une bonne story capture l'essence, non les détails. Avec le temps, la carte pourra se voir ajouter des notes, des idées de tests et ainsi de suite, mais nous n'avons pas besoin de ceci pour prioriser ou planifier les stories.  

### (de) Valeur

Une story doit avoir de la _valeur_. Nous ne nous pré-occupons pas de la valeur pour n'importe qui ; elle doit avoir de la valeur pour le client. Les développeurs peuvent y avoir des intérêts (légitimes), mais ils doivent être exprimés de telle manière à ce que le client les perçoivent comme importants.  

C'est particulièrement un problème lors du découpage des stories. Pensez à une story dans sa globalité comme un gâteau ayant plusieurs couches, par exemple, une couche réseau, une couche persistence, une couche logique et une couche présentation. Lorsque nous découpons une story, nous servons uniquement une part de ce gâteau. Nous voulons donner au client l'essence de la totalité du gâteau, et la meilleure manière de le faire est de découper verticalement à travers les couches (du gâteau - NdT). Les développeurs ont souvent une inclination à travailler sur une seule couche à la fois (et de le faire "bien") ; mais une couche complète de base de données (par exemple) est de peu de valeur pour le client s'il n'y a pas de couche de présentation.  

Faire de chaque part, une part de valeur pour le client va dans le sens de la philosophie d'XP de payer-au-fur-et-à-mesure pour l'infrastructure.  

### Estimable

Une bonne story peut être _estimée_. Nous n'avons pas besoin d'une estimation exacte, mais juste assez pour aider le client à prioriser et à planifier l'implémentation de la story. Être estimable est en partie en fonction de la négociation, car il est difficile d'estimer une story que nous ne comprenons pas. C'est aussi en fonction de la taille : les grosses stories sont plus difficiles à estimer. Enfin, c'est en fonction de l'équipe : ce qui est facile à estimer variera en fonction de l'expérience de l'équipe. (Quelques fois une équipe peut avoir à découper une story en un "essai expérimental" (NdT - spike dans le texte original) (limité dans le temps) qui donnera à l'équipe assez d'information pour faire une estimation convenable, et le reste de la story implémentera réellement la fonctionnalité souhaitée.).  

### [Suffisamment] petite

Les bonnes stories tendent à être _petites_. Typiquement, les stories représentent au plus quelques semaines/hommes de travail. (Quelques équipes se restreignent à quelques jours/hommes de travail). Au-delà de cette taille, cela semble trop difficile de savoir ce qu'il y a dans le périmètre de la story. À la phrase, "cela me devrait me prendre plus d'un mois" (pour le faire - NdT) s'ajoute souvent implicitement, "comme je ne comprends pas tout ce que cela entraîne". Des stories plus petites tendent à avoir des estimations plus précises.  

Les descriptions de la story peuvent être courtes également (et les écrire sur une fiche cartonnée est un bon moyen d'y parvenir). Alistair Cockburn décrit les cartes comme d'un gage d'une conversation future. Rappelez-vous, les détails peuvent être élaborés au cours des conversations avec le client.  

### Testable

Une bonne story est testable. Rédiger une carte de story porte implicitement la promesse : "Je pourrais rédiger un test sur cette story car j'ai compris ce que je veux suffisamment bien". Plusieurs équipes ont indiqué qu'elles étaient plus productives en exigeant des tests utilisateur avant l'implémentation d'une story. La "testabilité" a toujours été la caractéristique des bonnes exigences ; écrire réellement les tests précocement nous permettent de savoir si l'objectif est atteint.  

Si un client ne sait pas comment tester quelque chose, cela peut indiquer que la story n'est pas suffisamment claire, ou qu'elle ne reflète pas quelque chose comme ayant de la valeur à leurs yeux, ou que le client a juste besoin d'aide pour tester.  

Une équipe peut traiter des exigences non fonctionnelles (telles que la performance et l'utilisabilité) comme des éléments qui doivent être testés. Savoir comment réaliser ces tests peut aider l'équipe à connaître ses vrais besoins.  

Pour toutes ces caractéristiques, le cycle de retours d'informations de propositions, d'estimations, et d'implémentations des stories aidera l'équipe à apprendre ce qu'elle doit connaître.  

## Tâches SMART

Voici un acronyme pour créer des objectifs efficaces : "SMART" (NdT - là aussi il a fallu ruser pour conserver l'acronyme SMART)

* S - Spécifique
* M - Mesurable
* A - réAlisable
* R - peRtinente
* T - Temps imparti

### Spécifique

Une tâche doit être suffisamment explicite pour être compréhensible par toutes les personnes impliquées. Cela permet d'éviter que les autres tâches ne se chevauchent, et de permettre aux personnes de comprendre si les tâches doivent s'ajouter à la story complète.  

### Mesurable

La mesure clé ici est, "pouvons-nous la marquer comme finie ?". L'équipe doit se mettre d'accord sur ce que cela signifie mais elle devrait inclure "fait ce qui était prévu qu'elle fasse", "les tests sont inclus", et "le code a été refactoré".  

### réAlisable

Le propriétaire de la tâche devrait s'attendre à être capable de réaliser la tâche. Les équipes XP ont comme règle que n'importe qui peut appeler à l'aide lorsqu'il en a besoin. ; cela inclus certainement s'assurer que les propriétaires de la tâche soient à la hauteur du travail à faire.  

### peRtinente

Chaque tâche devrait être pertinente, et contribue à la story en cours. Les stories sont découpées en tâches pour rendre service aux développeurs, mais le client devrait toujours s'attendre à ce que chaque tâche soit expliquée et justifiée.  

### Temps imparti

Une tâche devrait être (faite - NdT) dans un temps imparti : limitée à une durée spécifique. Il n'est pas obligatoire que cela soit une estimation formelle en heures ou en jours, mais il devrait être entendu que les personnes devraient savoir quand elles ont besoin d'aide. Si une tâche est plus difficile qu'escomptée, l'équipe doit savoir si elle doit découper la tâche, changer de joueurs, ou faire quelque chose pour faire en sorte que la tâche (et la story) soit réalisée.  

## Conclusion

Lorsque vous discutez des stories, écrivez des cartes, et découpez des stories, l'acronyme peut vous aider à vous rappeler des caractéristiques des bonnes stories. Lorsque vous créez un planning de tâches, appliquer l'acronyme SMART peut vous permettre d'améliorer vos tâches.  

[J'ai développé l'acronyme INVEST, et j'ai rédigé cet article en avril et en août 2003. Je remercie Mike Cohn pour ses encouragements et ses retours.]  

---
Auteur : [Bill Wake](http://xp123.com/about/)  
Source : [INVEST in Good Stories, and SMART Tasks](http://xp123.com/articles/invest-in-good-stories-and-smart-tasks/)  
Date de parution originale : 17 Août 2003  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 23/02/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

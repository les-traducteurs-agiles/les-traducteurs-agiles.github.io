---
layout: post
title:  "Le modèle INVEST - V comme stories ayant de la Valeur"
date:   2017-04-25 00:00:01
published: true
tags:
- user story
---

Parmi toutes les caractéristiques d’une bonne _story_ présentées dans le modèle [INVEST](http://www.les-traducteurs-agiles.org/story/2015/02/23/investissez-dans-de-bonnes-stories-et-dans-des-taches-smart.html), la “Valeur” est la plus facile à … euh … valoriser. Après tout, qui peut être contre la valeur ?

Jetons un coup d’œil aux points clés suivants :

* La valeur, c’est quoi ?
* L’importance de l’impact externe
* De la valeur pour qui ?

## La valeur, c’est quoi ?

La valeur dépend de ce que nous essayons d’accomplir. Pour qualifier la valeur, nous pouvons utiliser la bonne vieille formule connue sous l’acronyme ARECAS[^1] (mentionnée en 1977 par Gane & Sarson dans leur ouvrage [Structured Systems Analysis](http://www.amazon.com/exec/obidos/ASIN/0138545472/xp123com/), sans pour autant qu’ils en aient réclamé la paternité). ARECAS signifie :

* Augmenter les Recettes
* Éviter les Coûts
* Améliorer le Service

**Augmenter les recettes** : La seule présence de nouvelles fonctionnalités ou l’amélioration d’anciennes peuvent s’avérer suffisantes pour motiver un acheteur potentiel à payer davantage afin d’en disposer.

**Éviter les coûts** : Une part significative des logiciels qui sont écrits, le sont pour faire en sorte que quelqu’un puisse économiser de l’argent. Par exemple, supposons que vous écriviez un logiciel pour gérer un centre d’appel : chaque seconde gagnée sur une transaction peut signifier une diminution du nombre de télé-opérateurs de ce centre d’appel et donc potentiellement une source d’économie pour l’entreprise.

**Améliorer le service** : Une partie du travail de développement logiciel peut être destinée à améliorer l’existant. Prenons comme exemple Skype, le réseau de communication : l’amélioration de la qualité audio des appels n’est pas une nouvelle fonctionnalité, par contre elle a de la valeur (davantage de clients seront, par exemple, susceptibles de continuer à utiliser le service si la qualité de service est au rendez-vous).

ARECAS couvre plusieurs types de valeur, il en existe toutefois d’autres :

**Respecter les contraintes réglementaires** : Les autorités réglementaires peuvent demander à ce que nous ayons à gérer certaines choses (que nous le voulions ou pas). Par exemple, les entreprises de cartes de crédit doivent pouvoir gérer une liste “noire” de clients ne veulant pas recevoir de nouvelles sollicitations de leurs parts. Si l’entreprise n’offre pas cette possibilité avant une certaine date, les autorités pourraient ordonner la fermeture de l’entreprise.

**Se bâtir une réputation** : Nous pouvons faire un certain nombre de choses pour accroître notre présence sur le marché. Nous pourrions faire par exemple une version gratuite de démonstration de notre logiciel. Il s’agira en effet d’une manière indirecte en vue d’augmenter les recettes à plus ou moins brève échéance.

**Se créer des options** : Certaines choses peuvent nous donner plus de flexibilité pour le futur. Par exemple, nous pouvons investir pour être indépendant vis-à-vis des bases de données afin d’avoir la capacité de changer rapidement de base de données dans le futur. Le futur est incertain, avoir des options est une assurance en la matière.

**Produire de l’information** : Certaines fois, nous avons besoin d’avoir des informations plus pertinentes pour prendre la bonne décision. Par exemple, nous pourrions faire un test A/B pour savoir la couleur du bouton qui se vend le plus. Les expérimentations _à la ExtremeProgramming_ font également partie de cette catégorie.

**Construire une équipe** : D’autres fois, une fonctionnalité est choisie parce qu’elle aidera l’équipe à faire ou à apprendre quelque chose d’important qui pourra s’avérer utile dans un futur proche.

Plusieurs valeurs peuvent s’appliquer en même temps (il ne s’agit pas là non plus d’une liste exhaustive) et d’ailleurs nous devons faire arbitrer sur ces différentes valeurs lorsqu’il y en a plusieurs en jeu, ce qui ne facilite pas la prise de décisions.

## Valoriser l’impact extérieur

Un logiciel est conçu pour accomplir quelque chose dans le monde réel.

Nous nous appuierons pour cela sur une analyse somme toute classique : décrire le comportement du système comme si l’implémentation système était parfaite. Concentrons-nous sur les impacts du système sur le monde.

Cela nous permet de clarifier quelles sont les “vraies” _stories_ : elles commencent à l’extérieur du système et y rentrent, ou bien commencent à l’intérieur et en sortent.

Cela nous aide aussi à éviter deux écueils :

* les “_stories_” concernant la solution que nous utilisons (la technologie)
* les “_stories_” concernant les créateurs du système, ou ce qu’ils veulent.

Si nous cadrons les _stories_ afin que leur impact soit clair, les _product owners_ et les utilisateurs peuvent alors comprendre ce qu’apportent les _stories_, et faire les bons choix les concernant.

## De la valeur pour qui ?

Qui tirent les bénéfices du logiciel que nous créons ? (Pour pouvoir répondre à cette question, nous devons envisager quel rôle une personne est susceptible d’avoir parmi les rôles suivants - il s’agit là-aussi d’une liste non exhaustive -)

**Utilisateurs** : Le mot “utilisateur” n’est sans doute pas le meilleur terme, toutefois nous devrons vraiment parler des gens qui utilisent le logiciel. Certaines fois, il ne s’agit pas d’un utilisateur direct : dans un centre d’appel, le télé-opérateur du centre d’appel est l’utilisateur direct, et le client qui appelle est un utilisateur indirect.

**Acheteurs** : Les acheteurs sont responsables pour choisir et ouvrir les cordons de la bourse pour obtenir le logiciel. (Quelque fois, il peut s’agir de deux rôles séparés). Il arrive que les besoins des acheteurs ne soient pas exactement alignés sur ceux des utilisateurs. Par exemple, les télé-opérateurs du centre d’appel qui utilisent le logiciel peuvent vouloir ne pas faire l’objet d’un suivi par celui-ci, mais l’acheteur du système lui pourrait bien exiger cette possibilité.

**Organisations de développement** : Dans certains cas, les équipes de développement peuvent avoir aussi des besoins comme la conformité à des standards, l’utilisation de certains langages ou de certaines architectures, etc.

**Sponsors** : Les sponsors sont les personnes qui payent pour le développement du logiciel. Ils veulent du retour sur inverstissement que ce soit sous une forme ou sous une autre.

Il existe bien d’autres catégories de personnes qui peuvent tirer de la valeur du logiciel que nous développons. Une partie du boulot de l’équipe de développement est d’équilibrer les besoins des différentes parties prenantes.

## En résumé

Nous avons examiné ce que nous pouvions entendre par valeur : ARECAS (Accroître les Recettes, Éviter les Coûts, Améliorer le Service), ainsi que d’autres choses comme Respecter les contraintes réglementaires, Produire de l’information et Se créer des options.

Nous avons exploré brièvement l’idée que généralement de bonnes _stories_ parlent  de ce qu’il se passe à limite du système : les impacts du logiciel sur le monde.

Enfin, nous avons vu comment les différentes parties prenantes en tirent parti : utilisateurs, acheteurs, développeurs et sponsors.

La valeur est importante. En être déconnecté est étonnamment facile  ; il est donc essentiel de revenir à la compréhension de “Qu’est-ce que la valeur pour ce projet ?”

[^1]: pour les plus curieux, l’acronyme en vo est IRACIS pour Increase Revenue, Avoid Costs et Improve Service - NdT

---
Auteur : [Bill Wake](http://xp123.com/about/)  
Source : [Valuable Stories in the INVEST Model](http://xp123.com/articles/valuable-stories-in-the-invest-model/)  
Date de parution originale : 03 Janvier 2013  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 25/04/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

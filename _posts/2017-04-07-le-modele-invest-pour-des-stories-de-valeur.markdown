---
layout: post
title:  "Le modèle INVEST - V comme stories ayant de la Valeur"
date:   2017-04-25 00:00:01
published: true
tags: 
- user stories
---

Of all the attributes of the [INVEST](http://xp123.com/articles/invest-in-good-stories-and-smart-tasks/) model, "Valuable" is the easiest one to, well, value. Who is against value?

Parmi toutes les caractéristiques présentes dans le modèle [INVEST](http://www.les-traducteurs-agiles.org/story/2015/02/23/investissez-dans-de-bonnes-stories-et-dans-des-taches-smart.html) d’une bonne _story_, la “Valeur” est la plus facile à … eh bien … valoriser. Après tout, qui peut être contre la valeur ?

We'll look at these key aspects:

Jetons un coup d’œil aux éléments-clés suivants :

* What is value?
* The importance of external impact
* Value for whom?

* La valeur, c’est quoi ?
* L’importance de l’impact externe
* De la valeur pour qui ?

## What is Value?

## La valeur, c’est quoi ?

Value depends on what we're trying to achieve. One old formula is IRACIS. (Gane & Sarson mentioned it in 1977 in [Structured Systems Analysis](http://www.amazon.com/exec/obidos/ASIN/0138545472/xp123com/), and didn't claim it was original with them.) IRACIS means:

La valeur dépend de ce que nous essayons d’accomplir. Pour qualifier la valeur, nous pouvons utiliser la bonne vieille formule connue sous l’acronyme d’ARECAS[^1] (mentionnée en 1977 par Gane & Sarson dans leur ouvrage [Structured Systems Analysis](http://www.amazon.com/exec/obidos/ASIN/0138545472/xp123com/), sans pour autant qu’ils en aient réclamé la paternité). ARECAS signifie :

* Increase Revenue
* Avoid Costs
* Improve Service.

* Augmenter les Recettes
* Éviter les Coûts 
* Améliorer le Service

**Increase Revenue**: Add new features (or improve old ones) because somebody will pay more when they're present. 

**Augmenter les recettes** : La seule présence de nouvelles fonctionnalités ou l’amélioration d’anciennes peuvent s’avérer suffisantes pour motiver un acheteur potentiel à payer davantage pour les avoir.

**Avoid Costs**: Much software is written to help someone avoid spending money. For example, suppose you're writing software to support a call center: every second you save on a typical transaction means fewer total agents are needed, saving the company money. 

**Éviter les coûts** : Une part significative des logiciels qui sont écrits, le sont pour faire en sorte que quelqu’un puisse économiser de l’argent. Par exemple, supposons que vous écriviez un logiciel pour gérer un centre d’appel : chaque seconde gagnée sur une transaction peut signifier une diminution du nombre de télé-opérateurs de ce centre d’appel et donc potentiellement une source d’économie pour l’entreprise.

**Improve Service**: Some work is intended to improve existing capabilities. Consider Skype, the voice network: improving call quality is not a new feature, but it has value. (For example, more customers might stay with the service when call quality is higher.) 

**Améliorer le service** : Une partie du travail de développement logiciel peut être destinée à améliorer l’existant. Prenons comme exemple Skype, le réseau de communication : l’amélioration de la qualité audio des appels n’est pas une nouvelle fonctionnalité, par contre elle a de la valeur (davantage de clients seront, par exemple, susceptibles de continuer à utiliser le service si la qualité de service est au rendez-vous).

IRACIS covers several types of value, but there are others:

ARECAS couvre différentes types de valeur, il en existe toutefois d’autres :

**Meet Regulations**: The government may demand that we support certain capabilities (whether we want to or not). For example, credit card companies are required to support a "Do Not Call" list for customers who don't want new offers. If the company didn't provide the capability by a certain date, the government would shut down the company.

**Respecter les contraintes réglementaires** : Les autorités réglementaires peuvent demander à ce que nous ayons à gérer certaines choses (que nous le voulions ou pas). Par exemple, les entreprises de cartes de crédit doivent pouvoir gérer une liste “noire” de clients qui ne veulent pas recevoir de nouvelles sollicitations de leurs parts. Si l’entreprise n’offre pas cette possibilité avant une certaine date, les autorités pourraient ordonner la fermeture de l’entreprise.

**Build Reputation**: Some things are done to increase our visibility in the marketplace. An example might be producing a free demo version of packaged software, to improve its marketing. In effect, these are an indirect way to increase revenue.

**Se bâtir une réputation** : Nous pouvons faire un certain nombre de choses pour accroître notre présence sur le marché. Nous pourrions faire par exemple une version gratuite de démonstration de notre logiciel. Il s’agira en effet d’une manière indirecte en vue d’augmenter les recettes à plus ou moins brève échéance.

**Create Options**: Some things give us more flexibility in the future. For example, we may invest in database independence today, to give us the ability to quickly change databases in the future. The future is uncertain; options are insurance. 

**Se créer des options** : Certaines choses nous donnent plus de flexibilité pour le futur. Par exemple, nous pouvons investir pour être indépendant vis-à-vis des bases de données afin d’avoir la capacité de changer rapidement de base de données dans le futur. Le futur est incertain, avoir des options est une assurance en la matière.

**Generate Information**: Sometimes we need better information to help us make a good decision. For example, we might do an A-B test to tell us which color button sells more. XP-style spikes may fit this category as well.

**Produire de l’information** : Certaines fois, nous avons besoin d’avoir des informations plus pertinentes pour prendre la bonne décision. Par exemple, nous pourrions faire un test A/B pour savoir la couleur du bouton qui se vend le plus. Les expérimentations _à la ExtremeProgramming_ font également partie de cette catégorie. 

**Build Team**: Sometimes a feature is chosen because it will help the team successfully bond, or learn important to the future.

**Construire une équipe** : D’autres fois, une fonctionnalité est choisie parce qu’elle aidera l’équipe à faire ou à apprendre quelque chose d’important qui pourra s’avérer utile dans un futur proche.

Several of these values may apply at the same time. (There's nothing that makes this an exhaustive list, either.) Because multiple types of values are involved, making decisions is not easy: we have to trade across multiple dimensions. 

Plusieurs valeurs peuvent s’appliquer en même temps (cette liste n’étant pas exhaustive non plus) et d’ailleurs nous devons faire arbitrer sur ces différentes valeurs lorsqu’il y en a plusieurs en jeu, ce qui peut ne pas faciliter la prise de décisions. 

## Valuing External Impact

## Valoriser l’impact externe

Software is designed to accomplish something in the real world.

Un logiciel est conçu pour accomplir quelque chose dans le monde réel.

We'll lean on a classic analysis idea: describe the system's behavior as if the system is implemented with a perfect technology. Focus on the effects of the system in the world.

Nous nous appuierons pour cela sur une analyse somme toute classique : décrire le comportement du système comme si l’implémentation système était parfaite. Concentrons-nous sur les impacts du système sur le monde.

This helps clarify what are "real" stories: they start from outside the system and go in, or start inside and go outside. 

Cela nous permet de clarifier quelles sont les “vraies” _stories_ : elles commencent à l’extérieur du système et y rentrent, ou bien commencent à l’intérieur et en sortent.

This also helps us avoid two problems:

Cela nous aide aussi à éviter deux problèmes :

* "stories" that are about the solution we're using (the technology)
* "stories" that are about the creators of the system, or what they want

* les “_stories_” concernant la solution que nous utilisons (la technologie)
* “_stories_” concernant les créateurs du système, ou ce qu’ils veulent.

If we frame stories so their impact is clear, product owners and users can understand what the stories bring, and make good choices about them. 

Si nous cadrons les _stories_ afin que leur impact soit clair, les _product owners_ et les utilisateurs peuvent alors comprendre ce qu’apportent les _stories_, et faire les bons choix les concernant.

## Value for Whom?

## De la valeur pour qui ?

Who gets the benefit of the software we create? (One person can fill several of these roles, and this is not an exhaustive list.)

Qui tirent les bénéfices du logiciel que nous créons ? (Une personne peut remplir plusieurs des rôles suivants - liste non exhaustive -)

**Users**: The word "User" isn't the best, but we really are talking about the people who use the software. Sometimes the user may be indirect: with a call center, the agent is the direct user, and the customer talking to them is indirect. 

**Utilisateurs** : Le mot “utilisateur” n’est sans doute pas le meilleur terme, toutefois nous devrons vraiment parler des gens qui utilisent le logiciel. Certaines fois, il ne s’agit pas d’un utilisateur direct : dans un centre d’appel, le télé-opérateur du centre d’appel est l’utilisateur direct, et le client qui appelle est un utilisateur indirect. 

**Purchasers**: Purchasers are responsible for choosing and paying for the software. (Sometimes even these are separate roles.) Purchasers' needs often do not fully align with those of users. For example, the agents using call center software may not want to be monitored, but the purchaser of the system may require that capability.

**Acheteurs** : Les acheteurs sont responsables pour choisir et ouvrir les cordons de la bourse pour le logiciel. (Quelque fois, il s’agit de deux rôles séparés). Il arrive que les besoins des acheteurs ne soient pas exactement alignés sur ceux des utilisateurs. Par exemple, les télé-opérateurs du centre d’appel qui utilisent le logiciel peuvent vouloir ne pas être surveillés par celui-ci, mais l’acheteur du système lui pourrait bien exiger cette possibilité. 

**Development Organizations**: In some cases, the development organization has needs that are reflected in things like compliance to standards, use of default languages and architectures, and so on.

**Organisations de développement** : Dans certains cas, les équipes de développement peuvent avoir aussi des besoins comme la conformité à des standards, l’utilisation de certains langages ou de certaines architectures, etc.

**Sponsors**: Sponsors are the people paying for the software being developed. They want some return on their investment. 

**Sponsors** : Les sponsors sont les personnes qui payent pour le développement du logiciel. Ils veulent du retour sur inverstissement que ce soit sous une forme ou sous une autre.

There can be other kinds of people who get value from software we develop. Part of the job of a development team is balancing the needs of various stakeholders.

Il existe bien d’autres catégories de personnes qui peuvent tirer de la valeur du logiciel que nous développons. Une partie du boulot de l’équipe de développement est d’équilibrer les besoins des différentes parties prenantes.

## Summary

## En résumé

We looked at what values is: IRACIS (Increase Revenue, Avoid Costs, Improve Service), as well as other things including Meeting Regulations, Generating Information, and Creating Options. 

Nous avons examiné ce que nous pouvons entendre par valeur : ARECAS (Accroître les Recettes, Éviter les Coûts, Améliorer le Service), ainsi que d’autres choses comme Respecter les contraintes réglementaires, Produire de l’information et Se créer des options. 

We briefly explored the idea that good stories usually talk about what happens on the edge of the system: the effects of the software in the world.

Nous avons exploré brièvement l’idée que généralement de bonnes _stories_ parlent  de ce qu’il se passe à limite du système : les impacts du logiciel sur le monde.

Finally, we considered how various stakeholders benefit: users, purchasers, development organizations, and sponsors.

Enfin, nous avons vu comment les différentes parties prenantes en tirent parti : utilisateurs, acheteurs, développeurs et sponsors.

Value is important. It's surprisingly easy to get disconnected from it, so returning to the understanding of "What is value for this project?" is critical.

La valeur est importante. En être déconnecté est étonnamment facile  ; il est donc vital de revenir à la compréhension “Qu’est-ce que la valeur pour ce projet ?”

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



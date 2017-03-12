---
layout: post
title:  "Le modèle INVEST - N comme stories Négociables"
date:   2017-03-12 00:00:01
published: true
tags: 
- user stories
---

In the INVEST model for user stories, N is for Negotiable (and Negotiated). Negotiable hints at several important things about stories:

Dans le modèle INVEST, le **N** signifie **Négociable** (et **Négocié**). Par Négociable, plusieurs choses importantes sur les _stories_ sont sous-entendues.

* The importance of collaboration
* Evolutionary design
* Response to change

* L’importance de la collaboration
* La conception évolutive
* La réponse au changement

## Collaboration

## La collaboration

Why do firms exist? Why isn't everything done by individuals interacting in a marketplace? Nobel-prize winner Ronald Coase gave this answer: firms reduce the friction of working together. 

Pourquoi les entreprises existent-elles ? Pourquoi est-ce que tout ce qui est fait par des individus ne se négocie-il pas directement sur une place de marché ? Le prix Nobel d’économie Ronald Coase a donné la réponse suivante : “parce que les entreprises permettent de réduire la friction du travailler ensemble”.

Working with individuals has costs: you have to find someone to work with, negotiate a contract, monitor performance carefully–and all these have a higher overhead compared to working with someone in the same firm. In effect, a company creates a zone where people can act in a higher-trust way (which often yields better results at a lower cost). 

Travailler avec des individus distincts a un coût : vous devez trouver quelqu’un avec qui travailler, négocier un contrat, surveiller minutieusement ce qu’il fait - et tout cela présente des frais généraux supérieurs au fait de travailler avec quelqu’un au sein d’une même entreprise. En effet, une entreprise créée une zone dans laquelle les personnes peuvent interagir à un niveau de confiance plus élevée (ce qui conduit souvent à de meilleurs résultats à moindre coût). 

The same dynamic, of course, plays out in software teams; teams that can act from trust and goodwill expect better results. Negotiable features take advantage of that trust: people can work together, share ideas, and jointly own the result. 

C’est cette même dynamique qui est ici en jeu, bien sûr, dans les équipes de développement logiciel ; les équipes qui peuvent agir en toute confiance et qui font preuve de bonne volonté ont normalement de bien meilleurs résultats. Et les fonctionnalités Négociables tirent avantage de ce climat de confiance : les gens travaillent ensemble, partagent des idées et s’approprient ensemble le résultat.

## Evolutionary Design

## La conception évolutive

High-level stories, written from the perspective of the actors that use the system, define capabilities of the system without over-constraining the implementation approach. This reflects a classic goal for requirements: specify what, not how. (Admittedly, the motto is better-loved than the practice.)

Les stories à grosses mailles, écrites du point de vue des acteurs qui utilisent le système, définissent les capacités du système sans mettre de contraintes trop fortes sur l’approche de l’implémentation. On retrouve là un objectif classique des exigences : spécifier le quoi, pas le comment (c’est du moins ce que l’on dit en théorie car en pratique …).

Consider an example: an online bookstore. (This is a company that sells stories and information printed onto pieces of paper, in a package known as a "book.") This system may have a requirement "Fulfillment sends book and receipt." At this level, we've specified our need but haven't committed to a  particular approach. Several implementations are possible:

Prenons un exemple : une librairie en ligne. (Autrement dit une entreprise qui vend des histoires et des informations imprimées sur des feuilles de papier, rassemblées en un volume communément appelé un “livre”). Dans cet exemple, une exigence du système pourrait être “la bonne exécution d’une commande suppose l’envoi du livre et du récapitulatif de la commande”. À ce niveau, nous avons spécifié notre besoin mais nous n’avons rien indiqué de particulier concernant telle ou telle approche. Plusieurs implémentations sont possibles :

* A fulfillment clerk gets a note telling which items to send, picks them off the shelf, writes a receipt by hand, packages everything, and takes the accumulated packages to the delivery store every day.

* Après avoir reçu une information lui indiquant quels articles sont à envoyer, un employé les prends dans un rayon, écrit le récapitulatif de la commande de manière manuscrite, les emballent puis amènent quotidiennement tous les paquets au magasin

* The system generates a list of items to package, sorted by (warehouse) aisle and customer. A clerk takes this "pick list" and pushes a cart through the warehouse, picking up the items called for. A different clerk prints labels and receipts, packages the items, and leaves them where a shipper will pick them up. 

* Le système génère une liste d’articles à préparer, triés par allée (au sens d’allées d’entrepôt) et par client. Un employé prend cette liste et pousse un chariot dans les allées de l’entrepôt et prends les articles demandés. Un autre employé imprime étiquettes et récapitulatif, emballe les articles et les laisse à un livreur qui viendra les chercher.

* Items are pre-packaged and stored on smart shelves (related to the routing systems used for baggage at large airports). The shelves send the item to a labeler machine, which sends them to a sorter that crates them by zip code, for the shipper to pick up. 

* Les articles sont pré-emballés et placés sur des casiers intelligents (à l’identique des systèmes de convoyages utilisés pour les bagages dans les gros aéroports). Les casiers amènent l’article à une étiqueteuse qui l’envoie à une trieuse qui les trie par code postal afin que le livreur puisse les prendre en charge.

Each of these approaches fulfills the requirement. (They vary in their non-functional characteristics, cost, etc.)

Toutes ces approches répondent au besoin. (Elles varient de par leurs caractéristiques non fonctionnelles, leurs coûts, etc.).

By keeping the story at a higher level, we leave room to negotiate: to work out a solution that takes everything into account as best we can. We can create a path that lets us evolve our solution, from basic to advanced form. 

En faisant en sorte que la _story_ reste à un niveau grosse maille, celo nous laisse de la marge pour négocier : et trouver une solution qui puisse tout prendre en compte en faisant de notre mieux. Nous pouvons créer un chemin qui nous permettra de faire grandir notre solution de sa forme la plus basique à la plus avancée.

## Feedback

## Retour d’information

Waterfall development is sometimes described as "throw it over the wall": create a "perfect" description of a solution, feed it to one team for design, another for implementation, another for testing, and so on, with no real feedback between teams. But this approach assumes that you can not only correctly identify problems and solutions, but also communicate these in exactly the right way to trigger the right behavior in others. 

Le développement dans une approche classique dite en cascade est décrite quelque fois comme “jeter tout par-dessus le mur” : faire une description “parfaite” de la solution, la donner à une équipe pour qu’elle fasse sa conception, une autre pour l’implémentation, encore une autre pour le test, et ainsi de suite, et ceci sans aucuns réels retours d’informations entre les équipes. Mais cette approche suppose que non seulement vous êtes mesure d’identifier correctement les problèmes et les solutions, mais aussi de les communiquer de la bonne manière pour que cela déclenche le comportement attendu chez les autres. 

Some projects can work with this approach, or at least come close enough. But others are addressing "wicked problems" where any solution affects the perceived requirements in unpredictable ways. Our only hope in these situations is to intervene in some way, get feedback, and go from there.

Certains projets peuvent bien fonctionner avec cette approche ou du moins fonctionner pour le mieux. Mais d’autres se voient amener à gérer de “vicieux problèmes” dans lesquelles n’importe laquelle des solutions a des impacts sur la perception des besoins de manière imprévisible. Notre seul espoir dans ce cas est d’intervenir d’une manière ou d’une autre, d’obtenir des retours d’informations, et de partir de là.

Some teams can (or try to) create a big static backlog at the start of a project, then measure burndown until those items are all done. But this doesn't work well when feedback is needed.

Certaines équipes peuvent (ou essayent) de créer un gros _backlog_ statique au démarrage du projet, puis de mesurer le _burndown_ jusqu’à ce que tous les items soient terminés.  Mais cela ne fonctionne pas bien lorsqu’il est nécessaire d’avoir des retours d’informations.

---

Negotiable stories help even in ambiguous situations; we can work with high-level descriptions early, and build details as we go. By starting with stories at a high level, expanding details as necessary, and leaving room to adjust as we learn more, we can more easily evolve to a solution that balances all our needs.

Les _stories_ Négociables peuvent même être utile dans les situations ambigües ; nous pouvons travailler au plus tôt d’abord avec des descriptions très grosses mailles, et détailler au fur et à mesure que nous avançons. En commençant avec des _stories_ à grosses mailles, en détaillant lorsque cela est nécessaire, et en se laissant de la marge pour ajuster au fur et à mesure que nous en apprenons plus, nous pouvons plus facilement évoluer vers une solution en concordance avec tous nos besoins.

---
Auteur : [Bill Wake](http://xp123.com/about/)  
Source : [Independent Stories in the INVEST Model](http://xp123.com/articles/negotiable-stories-in-the-invest-model/)  
Date de parution originale : 20 Août 2012  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 12/03/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



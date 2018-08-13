---
layout: post
title:  "Le modèle INVEST - N comme stories Négociables"
date:   2017-03-12 00:00:01
published: true
tags:
- user story
---

Le **N** dans le modèle INVEST signifie **Négociable** (et **Négocié**). Par Négociable, plusieurs choses importantes sur les _stories_ sont sous-entendues :

* L’importance de la collaboration
* La conception évolutive
* La réponse au changement

## Collaboration

Pourquoi les entreprises existent-elles ? Pourquoi est-ce que tout ce qui est fait par des individus ne se négocie-t-il pas directement sur une place de marché ? La réponse suivante fut donnée par Le prix Nobel d’économie Ronald Coase : “parce que les entreprises permettent de réduire la friction du travailler ensemble”.

Travailler avec des individus distincts a un coût : vous devez trouver quelqu’un avec qui travailler, négocier un contrat, surveiller minutieusement ce qu’il fait - et tout cela présente des frais généraux supérieurs au fait de travailler avec quelqu’un au sein d’une même entreprise. En effet, une entreprise créée une zone dans laquelle les personnes peuvent interagir à un niveau de confiance plus élevée (ce qui conduit souvent à de meilleurs résultats à moindre coût).

C’est cette même dynamique qui est ici en jeu, bien sûr, dans les équipes de développement logiciel ; les équipes qui peuvent agir en toute confiance et qui font preuve de bonne volonté ont normalement de bien meilleurs résultats. Et les fonctionnalités Négociables tirent avantage de ce climat de confiance : les gens travaillent ensemble, partagent des idées et s’approprient ensemble le résultat.

## Conception évolutive

Les stories à grosses mailles, écrites du point de vue des acteurs qui utilisent le système, définissent les capacités du système sans mettre toutefois des contraintes trop fortes sur l’approche de l’implémentation. On retrouve là un objectif classique des exigences : spécifier le quoi, pas le comment (c’est du moins ce que l’on dit en théorie car en pratique …).

Prenons un exemple : une librairie en ligne. (Autrement dit une entreprise qui vend des histoires et des informations imprimées sur des feuilles de papier, rassemblées en un volume communément appelé un “livre”). Dans cet exemple, une exigence du système pourrait être “la bonne exécution d’une commande suppose l’envoi du livre et du récapitulatif de la commande”. À ce niveau, nous avons spécifié notre besoin mais nous n’avons rien indiqué de particulier concernant telle ou telle approche. Plusieurs implémentations sont possibles :

* Après avoir reçu une information lui indiquant quels articles sont à envoyer, un employé les prends dans un rayon, écrit le récapitulatif de la commande de manière manuscrite, les emballent puis amènent quotidiennement tous les paquets au magasin.

* Le système génère une liste d’articles à préparer, triée par allée (au sens d’allées d’entrepôt) et par client. Un employé prend cette liste et pousse un chariot dans les allées de l’entrepôt et prends les articles demandés. Un autre employé imprime étiquettes et récapitulatifs, emballe les articles et les laisse à un livreur qui viendra les chercher.

* Les articles sont pré-emballés et placés sur des casiers intelligents (à l’identique des systèmes de convoyages utilisés pour les bagages dans les gros aéroports). Les casiers amènent l’article à une étiqueteuse qui l’envoie à une trieuse qui les trie par code postal afin que le livreur puisse les prendre en charge.

Toutes ces approches répondent au besoin. (Elles varient de part leurs caractéristiques non fonctionnelles, leurs coûts, etc.).

En faisant en sorte que la _story_ reste à un niveau grosse maille, celo nous laisse de la marge pour négocier : et trouver une solution qui puisse tout prendre en compte en faisant de notre mieux. Nous pouvons créer un chemin qui nous permettra de faire grandir notre solution de sa forme la plus basique à la plus avancée.

## Retour d’information

Le développement dans une approche classique dite en cascade est décrite quelque fois comme “jeter tout par-dessus le mur” : faire une description “parfaite” de la solution, la donner à une équipe pour qu’elle fasse sa conception, une autre pour l’implémentation, encore une autre pour les tests, et ainsi de suite, et ceci sans aucuns réels retours d’informations entre les équipes. Mais cette approche suppose que non seulement vous soyez en mesure d’identifier correctement les problèmes et les solutions, mais aussi de les communiquer de la bonne manière pour que cela déclenche le comportement attendu chez les autres.

Certains projets peuvent bien fonctionner avec cette approche ou du moins fonctionner au mieux. Mais d’autres doivent gérer de “vicieux problèmes” dans lesquelles n’importe laquelle des solutions a des impacts sur la perception des besoins de manière imprévisible. Notre seul espoir dans ce cas est d’intervenir d’une manière ou d’une autre, d’obtenir des retours d’informations, et de (re)partir de là.

Certaines équipes peuvent (ou essayent) de créer un gros _backlog_ statique au démarrage du projet, puis de mesurer le _burndown_ jusqu’à ce que tous les items soient terminés.  Mais cela ne fonctionne pas bien lorsqu’il est nécessaire d’avoir des retours d’informations.

---

Les _stories_ Négociables peuvent même être utiles dans des situations ambigües ; nous pouvons travailler au plus tôt d’abord avec des descriptions très grosses mailles, et détailler au fur et à mesure que nous avançons. En commençant avec des _stories_ à grosses mailles, en détaillant lorsque cela est nécessaire, et en se laissant de la marge pour ajuster au fur et à mesure que nous en apprenons plus, nous pouvons plus facilement évoluer vers une solution en concordance avec tous nos besoins.

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

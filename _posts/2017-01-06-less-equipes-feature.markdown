---
layout: post
title:  "LeSS - Équipes Feature"
date:   2017-01-06 00:01
published: true
tags:
- LeSS
---

[<< Portail LeSS < Portail Structure](http://www.les-traducteurs-agiles.org/2016/12/26/less-portail-structure.html)

Une équipe feature, comme illustrée dans le schéma ci-dessous, est une équipe pérenne, pluridisciplinaire, transversale aux composants, qui finit de bout-en-bout plusieurs features client, une à la fois.

![feature team]({{ site.url }}assets/less/feature-team_fr.png)

Les caractéristiques d'une équipe feature sont énumérées ci-dessous :

* pérenne, les membres de l'équipe restent ensemble et forment un "noyau dur" pour encore plus de performance ; l'équipe réalise de nouvelles fonctionnalités au fil de l'eau
* pluridisciplinaires et multi-composantes
* idéalement, colocalisée
* travaille sur une feature centrée sur le client et de bout en bout, en passant à travers tous les composants et toutes les disciplines (analyse, programmation, tests, ...)
* composée de spécialistes se généralisant
* dans Scrum, habituellement 7 ± 2 personnes.


La mise en oeuvre de pratiques d'ingénierie modernes, en particulier l'intégration continue, est essentielle lorsque vous choisissez d'être une équipe feature. L'intégration continue facilite la propriété collective du code, ce qui est nécessaire lorsque plusieurs équipes travaillent en même temps sur les mêmes composants.

Un malentendu fréquent : chaque membre d'une équipe feature doit connaître l'ensemble du système. Pas forcément, parce que :

* L'équipe entière, et non chaque membre, doit avoir les compétences pour mettre en œuvre l'ensemble de la feature centrée sur le client. Il s'agit notamment de la connaissance des composants et de compétences fonctionnelles tels que les tests, la conception centrée utilisateur ou la programmation. Mais au sein de l'équipe, les gens continuent à être spécialisés ... de préférence dans de multiples domaines.
* Les features ne sont pas réparties au hasard sur des équipes features. Les connaissances et compétences actuelles d'une équipe sont prises en compte pour décider quelle équipe va travailler sur quelles features.


Dans une organisation basée sur des équipes feature, lorsque la spécialisation devient une contrainte... l'apprentissage commence.

**Une organisation basée sur des équipes feature exploite les avantages de la vitessegénérée par la spécialisation, ceci tant que la cartographie des exigences correspond aux compétences des équipes.**

**Mais lorsque les exigences ne correspondent pas aux compétences des équipes,l'apprentissage est "forcé", rompant ainsi la contrainte de sur-spécialisation.**

Les compétences d'une équipe feature s'équilibrent entre spécialisation et flexibilité.

## Équipes feature vs composant

Le tableau et le schéma qui suivent mettent en évidence les différences entre les équipes feature et les équipes composants plus traditionnelles.

![Équipes feature vs composant]({{ site.url }}assets/less/LeSS-Equipes-feature-vs-composant.png)

![composant vs équipes feature]({{ site.url }}assets/less/component-vs-feature-teams_fr.png)

Le tableau et le schéma qui suivent mettent en évidence les différences entre les équipes feature et les équipes projet ou groupes de feature conventionnels.

![équipe feature vs groupe de features conventionnels]({{ site.url }}assets/less/feature-team-vs-project-feature-groups.png)

La majorité des défauts des équipes composant sont explorés dans le chapitre "Feature Teams" du livre "Scaling Lean & Agile Development" ; le schéma suivant en résume quelques-uns.

![défauts des équipes composant]({{ site.url }}assets/less/component-teams-drawbacks.png)

Ce qu'on ne voit pas parfois, c'est que la structure d'une équipe composant renforce le développement séquentiel (modèle de la « cascade » ou cycle en V) en générant beaucoup de files d'attente, des tâches de taille variable, des niveaux élevés de TAF (NdT : Travail à Faire ~ WIP), de nombreux intermédiaires, une augmentation du multitâches et l'affectation partielle des ressources.

## Choisir des équipes composant ou des équipes feature ?

Une organisation basée uniquement sur des équipes feature est idéale d'un point de vue valeur ajoutée livrée et souplesse. Valeur et souplesse ne sont cependant pas les seuls critères pour construire une organisation, et de nombreuses organisations finissent par conséquent en mode hybride, plus particulièrement pendant la transition des équipes composant vers des équipes feature. Attention : les modèles hybrides ont les inconvénients des deux mondes et peuvent donc être... douloureux.

Un motif fréquemment exprimé en faveur d'une organisation hybride est la nécessité de construire des infrastructures, des composants réutilisables, ou de nettoyer le code écrit au sein des équipes composant. Mais ces activités peuvent aussi être réalisées par une organisation basée sur des équipes purement feature, sans établir d'équipes composant permanentes. Comment ? En ajoutant les besoins d'infrastructure, de composants réutilisables ou de travail de nettoyage dans le Backlog Produit et en le donnant tel quel à une équipe feature existante comme s'il s'agissait de feature centrée client. L'équipe feature réalise ces travaux pendant un certain temps, aussi longtemps que le Product Owner le permet, puis retourne au développement de features centrées client.

## Évoluer vers des équipes feature

Différentes organisations exigent différentes stratégies de transition lors du passage d'équipes composant à des équipes feature. Nous avons l'expérience de nombreuses stratégies qui ont marché... et échoué dans un contexte différent. Une stratégie de transition sécurisée, mais lente, consiste à établir une seule équipe feature au sein de l'organisation basée sur des équipes composant. Une fois que cette équipe fonctionne bien, une deuxième équipe feature est formée. Cela continue progressivement selon un rythme adapté à l'organisation. Ceci est illustré dans le schéma qui suit.

![Transition des équipes composants]({{ site.url }}assets/less/transition-component-teams-slow_fr.png)

## Lectures conseillées :

* Introduction aux Équipes Feature. Cet article apparaît initialement comme le [Feature Team Primer (fr)]({{ site.url }}assets/fabrice_aimetti/feature_team_primer_fr.pdf)
* Le chapitre Feature Teams du livre [Scaling Agile & Lean Development](https://www.amazon.com/Scaling-Lean-Agile-Development-Organizational/dp/0321480961). Cette analyse de 60 pages des équipes composant et feature est aussi disponible en ligne.
* [Dynamics of Software Development par Jim McCarthy](https://www.amazon.com/Dynamics-Software-Development-Jim-McCarthy/dp/1556158238). Initialement publié en 1995 et republié en 2008. Le livre de Jim est un véritable classique sur le développement logiciel. En 1995, il mettait en avant les équipes feature. Le reste du livre est rempli de conseils pertinents concernant le développement logiciel.
* "XP and Large Distributed Software Projects" par Karlsson et Andersson. Cet article sur le développement agile à grande échelle a été publié très tôt dans Extreme Programming Perspectives. C'est un article pertinent et sous-estimé décrivant la forte relation entre les équipes feature et l'intégration continue.
* ["How Do Committees Invent?" par Mel Conway](http://www.melconway.com/research/committees.html). Cet article a 40 ans et est toujours aussi pertinent aujourd'hui comme il y a 40 ans. Il est disponible sur le site de l'auteur [www.melconway.com](http://www.melconway.com/).


---
Auteur : The LeSS Company B.V.  
Source : [Feature Teams - Large Scale Scrum (LeSS)](http://less.works/less/structure/feature-teams.html)  

---
Traducteur : [Fabrice Aimetti](http://www.fabrice-aimetti.fr/)  
Date de traduction : 06/01/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

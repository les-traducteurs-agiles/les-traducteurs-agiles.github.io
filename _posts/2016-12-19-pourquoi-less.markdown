---
layout: post
title:  "Pourquoi LeSS ?"
date:   2016-12-19 00:01
published: true
tags:
- LeSS
---

[<< Portail LeSS < Portail Framework](http://www.les-traducteurs-agiles.org/2016/12/28/less-portail-framework.html)

Le développement traditionnel selon un cycle de de vie séquentiel ne fonctionne pas assez bien. Il ne fonctionne pas bien pour générer les efforts nécessaires au développement d'un produit, qu'il soit petit ou gros. Depuis 2001, le développement Agile, et Scrum en particulier, ont révolutionné le développement logiciel, mais lorsqu'on pose la question de comment décliner le développement Agile sur de grands groupes de personnes, la plupart des gens répondent "ne le faites pas" ou "utilisez juste une petite équipe" ou encore "faites du Scrum au niveau de l'équipe". Aucune de ces réponses n'est particulièrement aidante, et même s'il est vrai qu'il vaut mieux ne pas ajouter de personnes pour produire l'effort de développement, il est également vrai que le développement de produit à une large échelle ne va pas disparaître, nous devons donc découvrir des moyens de le faire correctement.

Nous ([Craig](https://less.works/profiles/craig-larman) et [Bas](https://less.works/profiles/bas-vodde)) sommes impliqués dans le développement logiciel depuis longtemps, dans toutes sortes de rôles dans le développement traditionnel selon un cycle de vie séquentiel, que ce soit avec Unified Process (UP), CMMi, etc. Aucun ne nous a _convenu_. Scrum, par contre, nous allait bien pour le développement avec une seule équipe. La question qui s'est ensuite posée a été de savoir "Comment mettre à l'échelle Scrum sans perdre de sa force ?".

## LeSS, c'est Scrum mis à l'échelle

Quelle est la force de Scrum ? Il n'est pas facile de répondre à cette question. Bien sûr, les concepts et les principes qui sont à la base de Scrum, tels que la [Transparence (fr)](http://www.les-traducteurs-agiles.org/2016/12/23/less-transparence.html), le [Contrôle du Processus Empirique (fr)](http://www.les-traducteurs-agiles.org/2016/12/24/less-controle-du-processus-empirique.html), le Développement itératif et les [Équipes auto-gérées (fr)](http://www.les-traducteurs-agiles.org/2016/12/19/less-auto-gestion.html) sont critiques. Ces principes ont gravité autour de Scrum pendant un certain temps, mais leur prise en compte n'explique pas pour autant le succès de Scrum. Après de multiples discussions, nous en avons conclu que :

_Scrum se situe à l'endroit idéal entre les principes abstraits et les pratiques concrètes._

Aussi, pour garantir que [Scrum à grande échelle reste du Scrum (fr)](http://www.les-traducteurs-agiles.org/2016/12/25/less-scrum-a-grande-echelle-reste-du-scrum.html), nous aurons besoin de trouver le même type d'équilibre, nous serons alors capable de dire que :

_Pour les groupes de grande taille, LeSS se situe à l'endroit idéalentre des éléments concrets et définis et un contrôle de processus empirique._

Ce qui nous a conduit à prendre certaines décisions :

* **LeSS doit rester simple.**
    Lorsqu'on met à l'échelle, on a tendance à ajouter des rôles, des artefacts, des processus, etc. Ceci doit être évité afin qu'un processus puisse émerger de manière empirique au sein du groupe produit. La plupart des frameworks de mise à l'échelle tombe dans le piège de fournir un processus prédéfini. Avec LeSS, nous souhaitons éviter ce piège.
* **LeSS c'est Scrum mis à l'échelle.**
    Au lieu de considérer Scrum comme un élément de base pour un framework à l'échelle, nous devons regarder chaque élément de Scrum et nous demander "A quoi sert-il ?" puis "Si nous avons plus d'une équipe, comment pouvons-nous atteindre le même objectif sur une échelle plus grande ?".
* **Mettre à l'échelle plutôt que décliner à petite échelle.**
    Un concept habituel dans le développement de processus est de définir un framework global et universel, puis de le décliner à petite échelle en fonction du contexte. Cela ne fonctionne pas bien parce que les gens supposent que tout est nécessaire dans leur contexte spécifique. Cette hypothèse mène souvent à la création de processus surdimensionnés. LeSS doit être minimaliste. Nous sommes conscients que la mise à l'échelle demandera "davantage" de choses mais au lieu de "polluer" LeSS avec des éléments optionnels, nous avons identifié un framework différent, [LeSS Huge (fr)](http://www.les-traducteurs-agiles.org/2016/12/26/less-portail-less-huge.html).


## Vue d'ensemble de LeSS

La façon dont nous envisageons LeSS est très bien décrite dans l'image ci-dessous :

![Vue d'ensemble de LeSS]({{ site.url }}assets/less/xless-complete-picture_fr.png)

## LeSS se base sur l'expérimentation

Dans nos deux premiers livres, [Scaling Agile and Lean Development](https://www.amazon.com/Scaling-Lean-Agile-Development-Organizational/dp/0321480961) et [Practices for Scaling Agile and Lean Development](https://www.amazon.com/Practices-Scaling-Lean-Agile-Development/dp/0321636406), nous avons conçu Scrum à l'échelle comme un ensemble d'expériences menées selon le principe suivant :

_Les meilleures pratiques n'existent pas. Il y a uniquement des pratiques qui sont bonnes dans un certain contexte._

Les deux livres sont donc remplis d'expériences que nous avons menées. Nous vous conseillons d'essayer certains choses, d'en éviter certaines autres, et de faire attention à d'autres choses qui seront très bien dans certains contextes et épouvantables dans d'autres. Cela fonctionne très bien et nous avons reçus beaucoup de retours positifs quant à cette approche.

Nous avons eu également des retours de personnes qui étaient un peu désorientées. Elles avaient besoin de s'accrocher à quelque chose de... moins spécifique au contexte... avec quelques règles. Sur la base de ces retours, nous avons réfléchi et nous sommes revenus au modèle d'apprentissage Shu Ha Ri :

![Shu Ha Ri]({{ site.url }}assets/less/xshuhari.png)

Ce modèle montre les différentes étapes que traversent les apprenants lorsqu'ils apprennent de nouveaux concepts :

* Shu : suivre les règles pour apprendre les bases
* Ha : briser les règles et découvrir le contexte
* Ri : maîtriser et trouver son propre chemin


Nous avons alors réalisé que notre premier travail sur la mise à l'échelle ne fournissait rien au niveau shu, ce qui générait des difficultés et de la confusion pour les personnes qui démarraient à peine le développement agile dans de grands groupes produit. Cela devint encore plus évident lorsque d'autres approches à l'échelle, plus prédictives, commencèrent à fournir des conseils aux débutants. D'où...

## LeSS en tant que framework

LeSS est bien plus qu'un ensemble de principes et d'expériences. Il fournit aussi un framework avec des règles. Les [Règles LeSS (fr)](http://www.les-traducteurs-agiles.org/2016/12/29/less-les-regles-less.html) définissent ce qu'est (et n'est pas) LeSS et fournissent un framework concret pour mettre en oeuvre LeSS. Au sein du framework LeSS, les groupes produit peuvent mener des expériences et découvrir ce qui fonctionne le mieux pour eux à un certain moment.

Ceci est à la base du troisième livre sur LeSS, simplement nommé [Large-Scale Scrum](https://www.amazon.com/Large-Scale-Scrum-More-Craig-Larman/dp/0321985710). Dans ce livre, LeSS est défini avec :

* les Règles LeSS qui sous-tendent le framework LeSS (et le framework LeSS pour de plus grands groupes produit)
* les Guides de survie pour adopter LeSS
* les Expériences des deux premiers livres.


De cette manière, nous nous assurons que LeSS reste simple et respecte la nature fondamentale de Scrum. De plus, comme Scrum, LeSS fournit assez de pratiques concrètes pour démarrer et assez de flexibilité et de puissance pour passer à l'échelle.

---
Auteur : The LeSS Company B.V.  
Source : [Why LeSS - Large Scale Scrum (LeSS)](http://less.works/less/framework/why-less.html)  

---
Traducteur : [Fabrice Aimetti](http://www.fabrice-aimetti.fr/)  
Date de traduction : 29/12/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

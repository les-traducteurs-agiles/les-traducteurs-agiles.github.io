---
layout: post
title:  "Comment gérer les branches des cartographies des user stories"
date:   2017-08-15 00:00:01
published: true
tags:
- user story
---

## Question reçue récemment de Douglas Ferguson (mais qui m’est posée régulièrement)

Dans une cartographie de _user stories_, comment gérez-vous les processus multi-utilisateurs pouvant donner lieu à plusieurs branches ?  
Créez-vous différentes cartographies pour les différents utilisateurs et les différents flux ?

## Ma réponse :

C’est une question que l’on me pose souvent, et je fais de mon mieux pour éviter d’y répondre car je veux voir la conclusion à laquelle les gens vont arriver par eux-mêmes.

Pour moi, les seules règles valables concernant une cartographie sont :

1. Je suis en mesure de raconter une histoire - et je la raconte habituellement de gauche à droite
2. Je peux décomposer une histoire en alternatives ou en détails - et je le fais habituellement de haut en bas

Voila, c’est tout. Aucune autre règle. Et vous pouvez même violer ces règles si vous avez une bonne raison.

Si nous étions en train d’écrire un livre ici, les personnages auraient différentes options possibles, mais dans un livre déjà écrit, ils font une et une seule chose. Mais, si nous étions en train de raconter une histoire à propos d’un produit interactif, les gens pourraient utiliser le produit différemment à différents moments de la journée, ils pourraient faire les choses dans un ordre différent, et ils pourraient prendre une décision qui pourraient changer toutes les “étapes” qu’ils pourraient faire après cette décision. Ils ne se comportent pas comme les personnages d’un livre. Ça fait un peu foutoir. Et, parce que les personnes peuvent faire les choses de plein de manières différentes, la modélisation du processus devient difficile à accomplir. Donc je m’évite pas mal de peine en me remémorant la chose suivante :

> Une cartographie n’est pas un modèle précis du flux de travail d’un utilisateur. C’est un outil qui nous aide à travailler ensemble à raconter les histoires des utilisateurs

## Aplatissez le flux

Aussi lorsque quelqu’un me demande : “Dans ce processus, l’utilisateur fait les étapes A et B, mais à l’étape C, il prend une décision. Il pourrait prendre ensuite la branche vers les étapes D, E et F, ou bien il pourrait prendre l’autre branche et faire les étapes G, H, et I. Comment est-ce que je cartographie cela ?”

Dans un logigramme, cela pourrait ressembler à cela :

![logigramme]({{ site.url }}assets/jeff_patton/logigramme.jpg)

Je leur réponds que généralement je mets toutes les alternatives dans un flux de gauche à droite :  A, B, C, D, E, F, G, H, et puis I. Sur une cartographie, cela devrait ressembler à ceci :

![branches aplaties]({{ site.url }}assets/jeff_patton/branches-aplaties.jpg)

De manière générale, je mets les alternatives dans l’ordre dans lequel l’histoire a pu m’être raconté. J’utilise le récit de l’histoire pour ajouter les éléments de langage supplémentaire comme par exemple “ les utilisateurs pourraient prendre une décision lorsqu’ils arrivent à l’étape C et ils pourraient vouloir continuer en D, ou sauter ici en G ” . Dans une cartographie, je ne montre pas les branches comme je le ferais dans un logigramme. J’utilise la conversation pour communiquer les branches.

## Enroulez ensuite le tout

Voyant apparaître, de la manière dont je venais de la dessiner, cette très grande histoire, elle me paru tout d’un coup très longue. Je pouvais l’enrouler en 3 colonnes : le travail que je fais d’abord et qui conduit à prendre une décision, le travail que fais dans la première branche, et le travail que je ferais dans la seconde branche. Cette cartographie pourrait alors ressembler à ça :

![branches enroulées]({{ site.url }}assets/jeff_patton/branches-enroulees.jpg)

**Si vous transmettez une cartographie sans avoir une discussion** pour expliquer comment elle s’articule, cela ne marchera pas. Et c’est à ce moment que je me permets de vous rappeler que les _stories_ agiles tirent leur nom de l’action de raconter une histoire, et non de l’acte de documenter une histoire. Si vous ne pouvez discuter pour expliquer les choses, alors vous aurez besoin d’un diagramme de flux de travail, d’un logigramme, d’un cas d’utilisation, ou d’une modélisation quelconque pour pouvoir le faire.

**Si vous pensez que vous pourriez oublier des détails d’informations concernant les différentes branches**, alors c’est une bonne idée d’annoter les _stories_ ou de le faire à côté des _stories_. Écrivez juste ce qu’il faut pour vous aider à vous souvenir de la manière dont il faudra raconter l’histoire.

## Aplatissez le flux de plusieurs utilisateurs

En échangeant avec Doug, ce dernier m’évoqua ce qui suit :

>“ Imagines ce flux
>
> un marchand ajoute un nouveau produit à son catalogue — l’utilisateur parcoure le catalogue — l’utilisateur consulte les informations détaillées sur le produit — l’utilisateur passe commande — le service production reçoit la commande — le service livraison expédie le produit — l’utilisateur reçoit les informations de suivi de livraison
>
> Il s’agit donc d’un flux avec différents acteurs. Mes propres flux sont un peu plus complexes, spécifiques à mon cas d’utilisation et peuvent donner lieu à différentes branches, mais d’après ton FAQ il semble que je pourrais les aplatir sans trop de difficulté. ”

Eh oui, Doug, tu as tout compris. Et ainsi que tu peux le voir la carte ci-dessous a été dessinée selon ton récit.

>“ Cartographie du flux du processus produit avec différents types d’utilisateur ”

Si vous faites cela en prenant l’exemple donné précédemment, vous pourriez arriver à quelque chose qui pourrait ressembler à ceci :

![cartographie de l’ensemble du processus produit]({{ site.url }}assets/jeff_patton/carto-processus-produit.jpg)

Je n’ai pas écrit tous les détails sur les cartes, mais vous avez l’idée générale. C’est maintenant une cartographie qui en raconte beaucoup sur les _stories_ utilisateurs au sein de l’ensemble du processus produit.

## Ne cartographiez pas tout si vous n’avez pas à le faire

Je dois vous dire  que je ne construis pas toutes les cartographies de processus produits de cette manière sauf si je suis amené à reconstruire complètement un processus produit. Je travaille généralement avec des entreprises qui ont déjà un produit sur le marché, et qui aiment ajouter des nouvelles fonctionnalités ou de nouveaux éléments à leur produit. Quelques fois, elles font l’erreur d’imaginer qu’elles doivent cartographier l’ensemble de leur processus produit.

Ne faites pas cela. Cela prend beaucoup de temps. Et la seule raison pour le faire c’est d’aider les autres à comprendre votre processus produit s’ils ne le comprennent pas encore.

> “ À la place, cartographiez juste ce qui change. ”

Par exemple, si je veux ajouter la possibilité à un marchand d’ajouter un prix de vente spécial pour son produit, je cartographierais la partie de l’expérience du marchand où il met le produit en vente, et la partie de l’expérience du client où il voit le produit en vente.

Ce fragment de carte pourrait ressembler à ceci :

![Cartographier une possibilité]({{ site.url }}assets/jeff_patton/carto-une-possibilite.jpg)

## Faites ce qui a du sens pour vous

Je suspecte fortement que si je ne vous avais pas donné de conseil du tout, vous auriez trouver de votre côté. Donc si cela vous a permis de gagner un peu de temps, c’est cool.

Et mieux encore, si vous êtes arrivés à quelque chose de différent qui vous aide dans votre propre situation, alors je vous en prie de bien vouloir le partagez avec nous.

---  
Auteur : [Jeff Patton](http://jpattonassociates.com/about-jeff-patton/)  
Source : [How do I handle branches in Story Maps?](http://jpattonassociates.com/qa_branches_in_maps/)  
Date de parution originale : 13 Juillet 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 15/08/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

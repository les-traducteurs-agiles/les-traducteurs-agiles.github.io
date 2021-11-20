---
layout: post
title:  "Qui est le client ?"
date:   2021-04-12 00:01
published: true
tags:
- product owner
- client
---

C'est assez facile de balancer des termes comme « client » ou « utilisateur », mais qu'est-ce qu'ils signifient vraiment ? En réalité, il s'agit de concepts complexes, et notre but dans certaines _stories_ ne bénéficie pas toujours directement à l'utilisateur.

Les clients sont un sous-ensemble des parties prenantes ou de la communauté du projet, et à cet égard ils auront un impact sur le produit ou qui seront impactés par lui.

## Les types de clients

Je trouve très intéressant le modèle des différents types de clients proposé par Steve Blank et Bob Dorf dans leur ouvrage _The Startup Owner’s Manual_. (cf. [Réferences](#ref)) que l'on peut résumer ainsi :

**Les utilisateurs (finaux)**: Les personnes qui interagissent avec le logiciel.

**Les influenceurs** : Les personnes qui influencent l'acheteur. Ils sont souvent externes aux parties prenantes et certains d'entre eux peuvent être suffisamment influents pour être des lanceurs de tendances.

**Les recommandants** : Les personnes dont les opinions « font-ou-défont ».

**Les acheteurs économiques** : Ceux qui contrôlent ou qui approuvent un achat. Leur autorité leur est octroyée par le décideur ultime (s'il ne s'agit pas des mêmes personnes).

**Le décideur (ultime)** : Ceux qui ont l'autorité ultime pour acheter ou pas. Ils peuvent prendre le pas sur l'acheteur économique désigné.

\- et sans oublier -

**Les saboteurs** : Ceux qui peuvent faire dérailler le processus d'achat.

Dans ce modèle, une même personne peut avoir plusieurs rôles, c'est-à-dire être à la fois acheteur et utilisateur.

## En images

![Client = décideur ultime + acheteur économique + utilisateur, influencé par les influenceurs, recommandeurs, et les saboteurs.]({{ site.url }}assets/bill_wake/customer-fr.png)

## Client individuel - B2C

Dans le modèle B2C (« des entreprises aux particuliers »), ces différents rôles se confondent. Par exemple, je suis un musicien amateur et j'ai besoin d'une application musicale sur mon téléphone. Je suis à la fois l'utilisateur, l'acheteur économique et le décideur ultime. J'ai peut-être été influencé par des tests sur le produit, des retours d'expériences d'autres consommateurs, etc. Mon professeur de musique et mes amis musiciens sont des recommandants, et je ne m'attends pas à avoir dans mon entourage un saboteur.

## Client grande entreprise - B2B

Les choses sont différentes lors vous êtes en train de vendre à une grande entreprise. L'utilisateur, l'acheteur économique, et le décideur ultime sont généralement des personnes différentes. Plusieurs niveaux peuvent même exister pour chacun de ces rôles. Les utilisateurs peuvent avoir une certaine influence et peuvent ou pas avoir le rôle de recommandants.

Les influenceurs peuvent être des conférenciers, des rédacteurs de publications commerciales ou des revues en ligne, etc. Des tiers de confiance peuvent aussi être des recommandants comme par exemple le groupe Gartner.

Il peut y avoir également des saboteurs internes ou externes. Par exemple, une personne de l'équipe de recommandation qui préfère un autre produit. Ou peut-être que le groupe des Ops déteste l'application proposée … et étant donné qu'elle sera aux manettes du test de l'application, elle sera en position de force pour peser de tout son poids sur la balance.

Vous êtes maintenant en mesure de comprendre l'intérêt d'un tel modèle lorsque vous considérez les défis que les entreprises doivent relevés lorsqu'elles vendent à d'autres entreprises.

## Le client petite et moyenne entreprise - B2B

Une petite entreprise a un niveau de complexité intermédiaire. Le client est souvent propriétaire, et aussi décideur. Le plus souvent, le client est aussi utilisateur (du moins à un certain niveau d'encadrement ou de supervision) ; il peut y avoir ou pas d'autres utilisateurs.  

## Le problème de l'agence

À chaque fois que vous avez des types de clients différents se retrouvent impliqués dans l'achat du produit, et plus spécifiquement lorsque l'un d'entre eux utilise l'argent des autres, vous avez alors des _problèmes d'agences_ (cf. [Références](#ref)) : qui agit en tant qu'agent pour qui ?

Autrement dit, les gens sont davantage motivés par maximiser leur propre profit plutôt que disons l'entreprise pour laquelle il travaille. Est-ce quelqu'un a choisi ce produit par qu'il s'agit du meilleur choix, ou simplement parce que dépenser $5 Millions lui permet d'apparaître comme plus important ?

## Qui sont les bénéficiaires ?

Revenons aux _user stories_ dans ce contexte de B2B. L'utilisateur est rarement le bénéficiaire de la _story_. Une « Autre » règle d'or s'applique ici : celui qui a l'argent fait la loi.

Tout d'abord, les _stories_ sont choisies au bénéfice du sponsor qui paye pour leurs développements. Vous avez probablement remarqué que lorsque vous achetez en ligne à l'apparition du moment de - « Comment souhaitez-vous payer ? » l'option « Payer en centimes d'euro » n'apparaît jamais.

![Il faut atteindre d'abord les objectifs des sponsors, les objectifs clients et accessoirement les objectifs utilisateurs.]({{ site.url }}assets/bill_wake/donwhill-fr.png)

Après avoir pris en considération le point de vue du sponsor, le prochain niveau à prendre en compte est souvent celui de « pour stimuler les ventes » (c'est-à-dire que vous réalisez les fonctionnalités qui sembleront être davantage faites pour apparaître dans les études comparatives que pour les utilisateurs finaux), ou c'est « pour faire gagner de l'argent à l'entreprise qui achète ». Par exemple, il m'est arrivé d'entendre des dirigeants demander un logiciel pour surveiller leurs employés, mais je n'ai jamais entendu les employés le demander.

Cet article n'a pas pour objectif de dire qu'il n'existe pas de _stories_ dont l'utilisateur serait le bénéficiaire, il en existe beaucoup. Mais dans le cas plus spécifique du B2B, toutes les _stories_ ne le sont pas. Il est compréhensible que les entreprises aient besoin d'un modèle soutenable d'activité « ou sinon … ». Mais il y a, à mon avis, trop de _stories_ qui se font au détriment de quelqu'un ou du moins qui en laisse la possibilité.

Il n'y a pas que les _stories_ B2B qui ont ce problème ; beaucoup d'apps ont des coûts cachés que les utilisateurs rejetteraient s'ils en avaient connaissance. Une fois, j'ai eu une app de Sudoku qui a transformé mon téléphone en bouillotte (minage de bitcoins ?). Il existe de nombreux cas documentés de violations dissimulées ou involontaires de la vie privée des utilisateurs.

Je ne veux pas jeter le discrédit sur les _stories_  qui sont là pour offrir un bénéfice à l'utilisateur, ou pour leur permettre de faire ce qu'ils veulent faire dans leur contexte d'utilisation. Il s'agit simplement de reconnaitre que si la connaissance est synonyme de pouvoir alors il s'agit de connaissance embarquée.

## Conclusion

Il est facile d'utiliser les mots de « client » ou d' « utilisateur », mais dans les cas plus spécifiques de ventes en B2B, ces concepts s'avèrent plus complexes. Nous avons vu brièvement le modèle de Steve Blank et Bob Dorf avec plusieurs éléments spécifiques : utilisateur, acheteur économique, décideur ultime, recommandant, influenceur, et saboteur.

Les acheteurs et les utilisateurs ne sont pas généralement une seule et même personne, ce qui amène la question « à qui la _story_ bénéficie ? ». Ce n'est pas toujours l'utilisateur.

## <a id="ref"></a> Références

* [Agency Problem](https://www.investopedia.com/terms/a/agencyproblem.asp), Investopedia.

* [The Startup Owner’s Manual](https://www.amazon.com/exec/obidos/ASIN/B084RHMYZM/xp123com), Steve Blank et Bob Dorf.

---
Auteur : [Bill Wake](https://xp123.com/articles/about/)  
Source : [Who is the Customer?](https://xp123.com/articles/who-is-the-customer/)  
Date de parution originale : 3 Mars 2021  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 12/04/2021  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

---
layout: post
title:  "Un nouveau cadre de travail de développement logiciel : une équipe au complet"
date:   2017-08-27- 00:00:01
published: true
tags: 
- agile
- nouveau cadre de travail de développement logiciel
---

## Bon Voyage[^1]

Pour des raisons qui m’échappent encore, j’ai commencé une série d’articles décrivant ce que je ferais si je devais créer un [nouveau cadre de travail de développement logiciel](http://www.les-traducteurs-agiles.org/2017/07/26/nouveau-cadre-de-travail-idees.html). Je vous rassure tout de suite je ne vais pas faire cela, néanmoins je pense qu’écrire en partant de ce postulat va me donner l’opportunité de voir comment le temps a pu changer mon point de vue sur ce qui est important, sur ce qui est possible et sur ce qui est amusant.

Dans certains de ces articles, il se peut que je parte du manifeste agile. Dans d’autres comme celui-ci, j’essayerai au moins de faire le lien entre les idées et le manifeste. Pour moi, le manifeste continue à incarner largement ce que nous étions il y a 20 ans et ce que je continue à être aujourd’hui.

Le manifeste, ce sont des valeurs et des principes auxquels je souscris et qui, je pense, sont très importants. Toutefois, je crois que ce qui se produit dans le monde dépend de nos actes, pas seulement de nos convictions. Par conséquent, j’écrirai avant tout sur les pratiques … les choses que nous faisons concrètement.

L’exercice d’une pratique doit se faire de manière assidue. Autrement dit : vous n’êtes pas supposez la faire aveuglément. Vous êtes supposé la faire avec vos yeux et votre esprit ouvert, observant ce qu’il se passe quand vous le faites, quand vous ne le faites pas, et quand vous l’adaptez.

Nous pouvons considérer certaines de ces pratiques comme des points de départs, et nous escomptons qu’un jour vous pourrez aller au-delà de ces pratiques (mais sans toutefois vous en éloignez). D’autres peuvent être considérées comme des idéaux qui resteront à notre avis en dehors de votre portée, mais vous verrez que ça vaut le coup d’essayer de les faire. Dans tous les cas, j’essaierai de décrire comment j’envisage ces pratiques, ce qu’il y a avant elles, ce qu’il y a après.

Mais ce ne sont que des hypothèses de ma part. Aujourd’hui est un nouveau départ. Je suis sur le point de partir. Grimpez à bord et voyons ce qu’il va se passer.

## Pratiques

Lorsqu’il s’agit des pratiques, je commence généralement par XP. “XP c’est comme Scrum, sauf que ça marche.”[^2]. Toutefois, XP est très spécifique et a été créé il y a maintenant 20 ans, nous aurons donc besoin d’y jeter un œil. Aujourd’hui, je vais commencer avec mon diagramme XP “officiel” :

![Pratiques XP]({{ site.url }}assets/ron_jeffries/circles-fr.jpg)  

Dans le cadre de l’exploration de ce “nouveau cadre”, mon intention est d’examiner chacun des éléments d’origine d’XP et de les utiliser comme point de départ pour explorer ce sur quoi je crois aujourd’hui. Aujourd’hui, je vais écrire sur l’_équipe au complet_.


## L’équipe au complet

Au moment où j’écris, je pense que je vais conserver ce nom pour cette pratique.

L’idée que je présente ici inclue la notion Scrum d’“équipe pluri-disciplinaire”. L’idée de Scrum est que l’équipe de développement ait toutes les compétences nécessaires pour livrer l’incrément du produit. L’_équipe au complet_ englobe aussi la pratique XP connue sous le nom de “Client sur site” que l’on mentionne parfois, et qui correspond au “Product Owner” de Scrum.

Nous devons déconstruire un peu tout ça, parce qu’il y a beaucoup de choses à voir là-dedans.

### Équipe de développement pluri-disciplinaire

Nous avons à réaliser un [incrément](http://ronjeffries.com/categories/increment) toutes les semaines ou quelque chose comme ça. L’incrément doit être opérationnel, intégré, testé, et faire tout ce que le Client a sélectionné (voir planification) parmi toutes les choses à faire entre maintenant et les itérations à venir, celles ayant le plus de valeur. Si nous voulons faire cela de manière responsable, nous ne pouvons pas nous reposer un tantinet soit peu, si ce n’est pas du tout, sur des compétences clés en dehors de l’équipe. Le produit a besoin d’être testé : nous ne pouvons pas attendre le département de tests logiciels. Si le produit utilise une base de données, nous allons avoir besoin de l’administrer. Nous ne pouvons pas attendre le département de gestion des bases de données. Un manuel est-il nécessaire ? Nous ne pouvons pas attendre la visite mensuelle de la rédactrice technique.

Néanmoins, c’est quelque fois un peu idéaliste et déraisonnable. Comme a pu le suggérer mon cher collègue [Al Shalloway](https://twitter.com/AlShalloway), si il y a seulement dix métallurgistes présents dans l’entreprise, peut être sera t’il impossible de disposer d’un métallurgiste dans notre équipe. Eh oui, mais aussi peut être est-ce un indice qu’il ne devrait pas avoir plus de dix équipes ayant besoin d’aide de la part d’un métallurgiste. Et cela signifie aussi que l’équipe serait bien folle de prendre en charge une _story_ exigeant un métallurgiste si elle n’est pas mesure d’en obtenir un lorsque c’est nécessaire.

La pratique de l’_équipe au complet_ représente toutefois un idéal. Nous n’aurons pas toujours quelqu’un dans la pièce qui connaît tout ce que nous avons besoin de savoir. Notre boulot, en tant que membres de l’équipe ayant une attitude responsable, est de travailler constamment pour s’assurer que cela n’arrive que rarement.

### Client sur site / Product Owner

Dans XP, nous avons la notion de “client sur site”, qui idéalement devrait être le vrai client du produit. Dans Scrum, nous avons la notion de “Product Owner”, quelqu’un ayant la responsabilité métier pour maximiser la valeur de l’effort de l’équipe scrum. Certaines personnes font référence au _Product Owner_ comme étant “la seule personne à qui on peut tordre le cou” dans l’équipe. C’est dit d’une manière un peu plus rude que je ne l’aurais exprimé moi-même, mais l’idée est bien qu’une telle personne devrait être tenu pour responsable par le métier.

Kent Beck, le créateur d’eXtreme Programming, a dit un jour qu’il pensait que la séparation entre le client sur site et les développeurs[^3] était un problème majeur dans XP, mais qu’il ne voyait pas de solution de contournement.

Dans la plupart des entreprises aujourd’hui, les dirigeants[^4] veulent déléguer la responsabilité à un seul individu. Généralement, le concept d’une équipe pleinement en charge du projet, (et pouvant _rendre des comptes_ ce qui correspond à ce que les _dirigeants_ sous-entendent) est absent. L’idée ici derrière, est malheureusement, trop souvent de savoir qui blâmer et punir lorsque les choses tournent mal.

Néanmoins, quelques entreprises et expériences exceptionnelles sont à noter. Zappos aux États-Unis, Semco au Brésil, et d’autres encores, sont des organisations sans hiérarchie.  Les gens se réunissent, approfondissent les idées, obtiennent des budgets d’une façon ou d’une autre et s’auto-organisent pour faire le boulot. Le manifeste parle d’équipes auto-organisées, comme Scrum et XP. Je pense que notre intention, à nous auteurs du manifeste, est bien celle la, et qu’aucun d’entre nous ne sait jusqu’à quel point cela pourra aller.

Je me rappelle avoir assister à un Scrum Gathering [^5] à côté d’un responsable de chez Disney. Il m’a raconté qu’il n’avait pas voulu être le “_Product Owner_”. Il a voulu que l’_équipe_ s’approprie le produit. Il a voulu être le “_Product Champion_”, apportant à l’équipe son soutien, la guidant, la coachant, lui apportant ce dont elle avait besoin pour faire le produit. Un tel individu pourra sûrement être le “_Product Champion_” de plusieurs équipes. En tant que tel, il serait tenu pour responsable chez Disney d’objectifs stratégiques. Qui sait, du chiffre d’affaire, ou du nombre de sourire par unité de temps. Enfin quelque chose d’important chez Disney.

Et il pourrait ne pas tenir quiconque de ses équipes “responsable” si un quelconque échec se produisait. Peut-être le pire qu’il pourrait faire serait de venir les voir après plusieurs mois de travail et leurs dire :

> “Bon les gars, comme vous me l’avez dit, il semble malgré tout nos efforts, nous soyons tout simplement dans l’incapacité de réaliser un bon film sur des limaces sans cervelle mangeant des ordures. Je suis désolé, mais il va falloir chercher ailleurs pour trouver quelque chose à nous mettre sous la dent. Malgré ce changement de stratégie, il n’arrivera rien à aucun d’entre vous, et nous travaillerons sur une meilleure idée dès que possible. Merci à vous : nous en reparlons bientôt.”

### Tentative de conclusion

Vu sous cet angle, le point idéal[^6] à atteindre pour une _équipe au complet_ est sans aucun doute une équipe auto-organisée, comprenant à la fois les compétences techniques et les compétences métiers, pour produire le produit dont l’entreprise a besoin. Cette _équipe au complet_ aurait la responsabilité d’utiliser son budget judicieusement, y compris la responsabilité d’abandonner le produit et d’essayer quelque chose d’autre si c’est la bonne chose à faire.

Cela peut sembler assez irresponsable à la plupart d’entre nous qui ont travaillé dans de grandes entreprises. Cela peut sembler plutôt raisonnable à ceux d’entre nous qui ont construit quelque chose “dans notre garage” ou qui font partie d’une petite _startup_. Et à ceux d’entre nous qui sont partis d’une _startup_ à une société en capital-risque, ou qui a été rachetée par une grande entreprise, qui ont pu voir ce qui peut se mal se passer quand quelqu’un qui assume la _direction_ et qui commence à prendre des décisions comme si nous étions revenus aux jours où nous travaillions dans un garage. 

Mon point de vue maintenant est que l’_équipe au complet_ incarne l’ensemble du spectre des équipes auto-organisées, et que le point idéal serait une _équipe_ qui n’aurait ni actionnaire, ni patron, ni responsable. L’_équipe_ serait son propre chef et se gérerait elle-même. C’est sûrement un idéal et il n’est pas certain que nous y arriverons tous, ou même que nous le devrions.

[^1]: NdT - en français dans le texte 

[^2]: Je ne me rappelle pas qui de moi ou de Chet est à l’origine de cette citation. Disons que c’est la faute de Chet. Oui, c’est un peu sarcastique. Et disons aussi, que Jeff Sutherland lui-même dit que pour atteindre un haut niveau de productivité Scrum a besoin des pratiques XP. Donc dans un certain sens, c’est tout à fait exact.

[^3]: Le Client et le Développeur sont les deux rôles fondamentaux d’XP. D’autres rôles ont été identifiés par la suite, comme le Coach et le Traqueur. La traque est une activité nécessaire pour l’équipe et il serait bénéfique que l’équipe puisse avoir de l’aide de ce côté-là. Nous parlerons prochainement du Coach au cours de cette série d’articles, peut-être dans un article dédié aux rôles.

[^4]: Dirigeants, Responsables, actionnaires. Vous voyez sans doute de qui je veux parler. Une chose qui je l’espère sortira de cette série d’articles est que le concept d’Agile milite en faveur d’une manière d’envisager autrement le travail, la responsabilité, l’autorité, et d’autres choses du même acabit.

[^5]: NdT - Grand rassemblement annuel de la communauté Scrum

[^6]: NdT - Un point idéal est type de point à l’infini en mathématique et représente le point croisement de droites parallèles dans un plan hyperbolique à l’infini.


---
Auteur : [Ron Jeffries](http://ronjeffries.com/about.html)  
Source : [A New Software Development Framework: Whole Team](http://ronjeffries.com/articles/017-02ff/new-framework-1/)  
Date de parution originale : 26 Juin 2017  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 27/08/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}




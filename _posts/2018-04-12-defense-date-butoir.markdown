---
layout: post
title:  "En défense de la date butoir"
date: 2018-06-12 00:01
published: true
tags:
- dark scrum
- scrum
- incrément
---

<div align="right" style="float:right; margin:10px; padding-bottom:5px; font-style: italic; width:40%; text-align:left; border-style:outset" >Il y a toujours une date butoir</div>

Chaque produit ou chaque projet possède une date butoir, une date après laquelle si vous ne livrez pas la chose, vous êtes mort[^1] . Faisons-un peu de math ensemble.

Donc. Étant donné que nous avons une date butoir. Si le logiciel ne fonctionne pas pour cette date, nous sommes dans la merde. Quelqu’un sera déçu. Les conséquences pourraient être terribles, elles pourraient être pour ainsi dire anodine. Mais, nous aurons “échouer”. Cela serait très mauvais.

<div align="right" style="float:right; margin:10px; padding-bottom:5px; font-style: italic; width:40%; text-align:left; border-style:outset" >Nous devons avoir terminé le jour-dit.</div>

Par conséquent, le logiciel se doit de fonctionner ce jour-là. Intégré, testé, opérationnel, documenté, prêt à être mis aux mains des utilisateurs. Il doit fonctionner. Il doit être sans aucune anomalie - ou du moins sans aucune anomalie significative.

Nous pouvons prendre en compte chaque aspect de “fini”  indépendamment et séparément. Le logiciel doit-il être documenté ? Alors il devra être documenté pour le dernier jour. Doit-il être intégré (vous connaissez la réponse) ? Alors il devra être intégré pour le dernier jour. Et ainsi de suite.

Chaque aspect de fini, d’en-cours, de prêt - vraiment chaque aspect - doit être fini pour ce jour-là.

<div align="right" style="float:right; margin:10px; padding-bottom:5px; font-style: italic; width:40%; text-align:left; border-style:outset" >Et le jour d’avant ?</div>

Qu’en est-il du jour d’avant la date butoir ? Si le logiciel doit être intégré, testé, opérationnel, documenté et ainsi de suite pour demain, il serait mieux que tout ce qui doit être intégré, testé, opérationnel, documenté le soit le jour d’avant ? Franchement, à moins que vous ne travailliez toute la nuit, il serait préférable que tout soit terminé à 99,999%. Peut-être y’a t’il un point quelque part dans la documentation qui devrait plutôt être un point-virgule ou quelque chose d’autre, mais regardons les choses en face, s’il y a quelque chose d’incorrect la veille, il y a peu de chances que nous soyons en capacité de le trouver et de le corriger pour être prêt à la date butoir.

Donc si la date butoir est le jour 100, nous devrions être vraiment prêt le jour 99. Il n’y a pas grand chose que nous puissions faire entre le jour 99 et le jour 100, et s’il neige ou quelque chose d’autre de catastrophique se passe, nous ne pourrions même pas être en mesure de faire quoi que ce soit.

<div align="right" style="float:right; margin:10px; padding-bottom:5px; font-style: italic; width:40%; text-align:left; border-style:outset" >Il semble qu’il y a une espèce de schéma qui se dessine au fur et à mesure de cette réflexion.</div>

Vous voyez où cela nous mène. Nous ne pouvons pas faire grand chose entre le jour 98 et le jour 99, nous devrions donc être prêt pour le jour 98. Oh bien sûr, nous pourrions faire quelques petites modifications, ici et là, à la marge pendant ces deux jours, mais de manière réaliste, il n'y a pas grand chose que nous soyons en mesure de faire.

<div align="right" style="float:right; margin:10px; padding-bottom:5px; font-style: italic; width:40%; text-align:left; border-style:outset" >Est-ce que ce serait stupide de dire que nous devrions prêt à livrer dès le jour 1 ?</div>

Il est impossible que nous puissions livrer quoi que ce soit dès le jour 1, n’est-ce-pas ?

Eh bien, au jour 1 nous n’avons pas de code, par conséquent notre code est complètement testé et intégré. Nous pourrions très bien prendre un CD vierge et le donner à quelqu’un, et toute la documentation pour notre logiciel qui ne fait rien pourrait être contenue dans ce CD.

Donc à part peut être n’avoir aucun CD sous la main, nous sommes prêt à livrer en jour 1.

<div align="right" style="float:right; margin:10px; padding-bottom:5px; font-style: italic; width:40%; text-align:left; border-style:outset" >OK, c’est simplement un de vos tours de passe-passe mental de Jedi. Qu’en est-il pour le jour 2 ?</div>

Jusqu’à présent tout va plutôt bien ! Mais qu’en est-il du jour 2 ? Pouvons-nous être prêt à livrer quoi ce que ce soit en jour 2 ? Ne pouvons-nous pas écrire une petite fonctionnalité faisant partie de notre projet, la tester, l’intégrer, et la documenter ? Dans la négative, peut être qu’elle n’est pas assez petite. Autrement dit, quelques lignes de code, quelques lignes de tests, quelques lignes pour compiler, quelques lignes de documentation … et hop livrez-la !

<div align="right" style="float:right; margin:10px; padding-bottom:5px; font-style: italic; width:40%; text-align:left; border-style:outset" >Oh allez, c’est pas sérieux, nous pouvons pas faire tout ce qui est à faire en une seule journée !</div>

Il semble donc que le problème soit le jour 2. Nous étions bien lors du jour 1, avec rien d’implémenté et par conséquent complètement à jour au niveau des tests, de l’intégration, et de la documentation. Mais le jour 2 ? Il se peut que nous ne soyions pas tout à fait en mesure de coordonner pour décider quoi faire, pour le faire, pour le tester, pour le compiler, et pour le documenter en une seule journée.

<div align="right" style="float:right; margin:10px; padding-bottom:5px; font-style: italic; width:40%; text-align:left; border-style:outset" >Mais, et si nous pouvions le faire ?</div>

Réfléchissez, je crois qu’il est sans doute toujours possible de livrer un nouveau produit testé et intégré tous les jours, mais je vous concède volontiers que ce n’est pas facile et tout particulièrement en jour 2. Mais mettons de côté nos soucis concernant le jour 2 pour l’instant et réfléchissons à ce qui se passerait si nous pouvions faire ce qui suit tous les jours :

* Planifier une ou deux fonctionnalités minuscules;
* La concevoir ;
* La compiler ;
* La tester ;
* L'intégrer ;
* La documenter.

Si nous pouvions le faire - et peut être s’agit d’un gros si -  alors nous pourrions atteindre n’importe quelle date butoir avec notre produit prêt à partir en livraison. Et si nous pouvions travailler sur les choses importantes d’abord et moins importantes plus tard, nous pourrions atteindre la date butoir avec les meilleurs résultats avec le temps et le budget dont nous disposons.

<div align="right" style="float:right; margin:10px; padding-bottom:5px; font-style: italic; width:40%; text-align:left; border-style:outset" >Les meilleurs résultats possibles ? C’est pas mal du tout !</div>

Tout à fait ! Réfléchissez-y ! Si nous pouvions simplement livrer un système qui soit un tout petit peu mieux, et toujours opérationnel, chaque jour, nous pourrions atteindre la date butoir avec le meilleur résultat possible ! Vraiment !

<div align="right" style="float:right; margin:10px; padding-bottom:5px; font-style: italic; width:40%; text-align:left; border-style:outset" >Mais et si nous ne pouvons pas ?</div>

Ce plan très simple peut échouer d’une seule manière : si nous ne le faisons pas. Il y a seulement deux manières qui feraient que nous ne pourrions pas le faire. Nous pourrions ne pas essayer, ou nous ne pourrions pas être capable de le faire. Maintenant que nous voyons ce qu’est un plan intelligent, nous allons sûrement l’essayer. Donc qu’est-ce que pourrait nous empêcher de le faire ?

Eh bien, une myriade de chose pourrait nous empêcher d’offrir un système opérationnel testé en jour 2, ou à n’importe quel autre jour. Remarquez, toutefois, que si nous avons réussi par le passé à avoir un système opérationnel testé, il est impossible de ne pas en avoir un par la suite : si celui que nous essayons de construire demain ne fonctionne pas, nous avons toujours celui d’aujourd’hui. Il ne montrera pas beaucoup de progrès pour le jour d’aujourd’hui, mais nous l’aurons. Nous serons donc toujours capable de livrer la meilleure version possible.

<div align="right" style="float:right; margin:10px; padding-bottom:5px; font-style: italic; width:40%; text-align:left; border-style:outset" >Le plus dur est laissé au lecteur …</div>

Je ne vais pas essayer de lister et de corriger toutes les choses qui pourraient nous retenir de faire dans ce court article, mais parce que je l’ai vu faire de nombreuses fois, je suis assez certain que nous pouvons toujours avoir une version complètement testée, intégrée et documentée le plus tôt possible pour n’importe quel produit qui commence à partir de zéro. (Avec du vieux code cela peut être plus difficile, mais si vous pouvez le construire … vous êtes sur la voie !)

Peu importe, nous pouvons débattre de ceci ailleurs. Mon sujet est ici est un cas simple. Peut être que vous ne pouvez pas le faire en jour 2. Je pense que vous pouvez le faire au jour 5 ou au jour 10. Peut être qu’en de plus rares occasions, cela prendra jusqu’au jour 15 ou même 20.

<div align="right" style="float:right; margin:10px; padding-bottom:5px; font-style: italic; width:40%; text-align:left; border-style:outset" >”Faites-le simplement.” <br/> - comme le dirait une certain déesse grecque <br/> - ou peut être comme le dirait un petit gars en vert</div>

Mon sujet ici est … de le faire. Prêtez attention à rien d’autre dans les premières étapes de vos efforts qu’à réaliser une petite version complètement intégrée, testée, documentée. Plus elle est petite mieux c’est, parce que c’est plus facile quand c’est petit. Ne visez pas une version avec dix fonctionnalités. Faites une version avec une fonctionnalité. Puis faites-en une autre et une autre et une autre. Prêtez attention à ce qui est sur votre chemin et améliorez-le. Prêtez attention à ce dont le produit a besoin ensuite et concentrez-vous dessus. Continuez de la sorte jusqu’à la date butoir.

Pour moi, cette idée est l’essence du développement agile de logiciel. Oh oui bien sûr, je soutiens les valeurs de Cœur d’Agile : Collaborer, Livrer, Réfléchir, Améliorer[^2], ainsi que celles de _Modern Agile_ Rendre les gens étonnants, Livrer de la valeur de manière continue, Faire de la sécurité personnelle un pré-requis, Expérimenter et apprendre rapidement[^3]. Il s’agit d’idées géniales de la part de gens géniaux.

Moi, je ne suis pas quelqu’un de génial, je suis quelqu’un avec un cerveau très simple. Ces idées, parmi les meilleures que j’ai eu, sont essentielles pour réussir avec “Agile”, du moins à mon avis.

Toutefois, si vous ne montrez pas un vrai logiciel opérationnel tout le temps, vos échanges avec l’encadrement seront affaiblis, vos échanges avec vos utilisateurs seront affaiblis, vos retours d’informations venant du monde extérieur, de votre ordinateur, de votre code seront affaiblis … et vous ne pourrez pas prospérer.

For me, running tested software is central. All those other ideas support it, but the software’s what we’ve got to do. So find a way to do it and if you find yourself losing heart, ask me or my betters.

Pour moi, un logiciel testé opérationnel est central. Toutes les autres idées permettent de soutenir ça, mais c’est le logiciel que nous devons faire. Donc, trouvez une manière de le faire et si vous sentez que vous perdez foi, demandez à moi ou à ceux qui sont meilleurs que moi.

Bonne chance !

[^1]: Peut-être y-a-t-il des exceptions à cette règle. Ce n’est pas la voie sur laquelle parier. Arriver à un certain point, ils n’auront plus de budget ou de patience ou d’autre chose. De toute manière, peu importe sur ce que vous êtes en train de travailler actuellement, il y a de toute manière une date qui vous attirera des ennuis si vous ne livrez pas d’ici celle-ci.

[^2]: Le Cœur d’Agile d’Alistair Cockburn

[^3]: Modern Agile par Joshua Kerievsky et plein d’autres personnes


---
Auteurs : [Ron Jeffries](http://ronjeffries.com/about.html)  
Source : [Deadline Defense](https://ronjeffries.com/articles/018-01ff/deadline-defense/)  
Date de parution originale : 27 Février 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 12/06/2018  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

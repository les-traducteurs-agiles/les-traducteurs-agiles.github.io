---
layout: post
title:  "TEC et priorités - comment être plus rapide et davantage focalisé sur un sujet ?"
date:   2017-12-10- 00:00:01
published: true
tags: 
- kanban
---

La plupart des problèmes organisationnels que l’on retrouve habituellement peuvent trouver leur source dans la gestion des priorités et du TEC (travail en cours). Avoir une bonne gestion à tous les niveaux de l’organisation peut faire une énorme différence ! J’ai pas mal expérimenter à ce sujet et voici donc quelques principes généraux pratiques :

**TEC = Travail en cours = élément sur lequel nous avons commencé à travailler et qui n’est pas encore terminé**, élément qui prend une partie de notre bande passante, qui prend des ressources, etc … Même des choses bloquées ou en attente sont du TEC.

![Visualiser et limiter le TEC]({{ site.url }}assets/henrik_kniberg/Visualize-and-limit-WIP-fr.jpg)

* Le TEC est ce qu’il est, quel que soit les priorités (les priorités sont ce sur quoi nous devrions nous concentrer, le TEC est ce sur quoi nous travaillons vraiment. Certaines fois, ces différentes choses coïncident …) 
  
* C’est presque toujours une **bonne idée de visualiser le TEC**, que ce soit au niveau d’une équipe ou d’une entreprise ou à tout autre niveau. Il est difficile de discuter de TEC invisible, difficile de le challenger, et difficile de le limiter. Et par conséquent, **un TEC invisible a tendance à grossir et à nous ralentir**.
  
* **Rendez le TEC visible-dans-ta-face !** Idéalement sur le mur, étant donné que tout le monde pourra le voir (et ainsi en discuter) sans avoir à chercher et à ouvrir un document. Tout élément qui n’est pas sur le mur, tend à être ignoré ou oublié. Une visualisation analogique (pense-bête adhésif etc) donne de meilleurs résultats généralement, toutefois montrer une visualisation numérique sur un écran peut donner des résultats aussi.
  
* **Utilisez un “seuil de bruit” pour éviter le micromanagement.** Éviter d’encombrer la visualisation avec une centaine de petits éléments. Par exemple, le niveau de bruit pour une visualisation d’équipe pourrait être “si c’est moins de deux heures de boulot, faites-le, ne perdez pas de temps à le mettre sur un pense-bête”. Au niveau d’un département, le niveau de bruit pourrait être “les éléments qui impliquent plus d’une équipe pour plus d’une semaine”. Les éléments plus petits que ça sont autorisés à “passer sous le radar” (ce qui offre comme petit bonus supplémentaire d’inciter à diviser les choses à traiter en petits morceaux).
  
* S’il y a beaucoup de bruits, **agrégez et visualisez le bruit** (afin qu’il puisse être aussi discuté/challengé/limité). Par exemple “le nombre de tickets Jira actuellement ouvert” au lieu d’afficher chaque ticket individuellement.
  
* Le but est de visualiser tout le TEC significatif pesant sur l’équipe, le département ou le projet ou quoi que ce soit d’autre, et de le **faire de telle manière qu’il n’implique pas de devoir gérer une centaine de pense-bête sur le mur.**
  
* C’est presque toujours une bonne idée que de **définir des limites pour le TEC**. La limite du TEC est simplement “la quantité de choses que nous pouvons avoir en cours avant que nous ne commencions à sombrer dans le multitâche et dans la coordination au-delà de tout espoir”. Commencez par une limite assez haute et réduisez-la progressivement, c’est une excellente manière pour se débarrasser du superflu. C’est d’ailleurs l’un des principes clés en Kanban.
  
* **Le TEC actuel sera certaines fois plus haut que la limite du TEC**. C’est tout à fait normal. C’est un système d’alerte. Le TEC actuel est simplement notre réalité actuelle, alors que la limite du TEC est notre réalité souhaitée. Les visualiser tout les deux permet de rendre le problème explicite. Aussi longtemps que nous serons au-dessus de la limite, notre objectif principal sera de finir les choses (ou de les abandonner) et nous serons super-restrictif quant au sujet de commencer de nouvelles choses.

“[The Impact of Agile – Quantified](https://www.rallydev.com/sites/default/files/ImpactAgile_Quantified.pdf)” est une étude intéressante qui montre comment les limites du TEC peuvent grandement améliorer la qualité et la productivité.

**Les priorités sont quelque chose de différent.**

![Priorités en cascade]({{ site.url }}assets/henrik_kniberg/Cascading-priorities-fr.jpg)

* Les priorités sont les **principes généraux qui sont là pour nous aider à décider quel nouveau TEC est à traiter** (lorsque nos limites du TEC le permettent), et quelles choses sont à refuser ou à reporter. Sans priorités claires, nous risquons des prises d’initiatives incohérentes ou une sous-optimisation. 
  
* Les priorités nous aident aussi à **résoudre les conflits de ressources** au sein de notre TEC actuel (“Nous avons besoin de Joe pour ces deux tickets, sur lequel doit-il se concentrer d’abord ?” ou “Donnons un coup de main à l’équipe X d’abord, le travail demandé par l’équipe Y a un niveau de priorité plus bas”)
  
* **Le nombre d’éléments prioritaires devraient être limitées** aussi ! Quelque chose comme 1 à 3 items est généralement suffisant. Parce que si tout est important, rien n’est important ! Et si la liste est trop longue, personne ne la lit ou s’en souvient.
  
* Les priorités **peuvent être d’ordre général** (“nos priorités actuelles sont 1) rembourser la dette technique, et 2) améliorer l’expérience utilisateur du backoffice.”)
  
* **… ou spécifiques** (“nos priorités actuelles sont 1) Livrer la fonctionnalité X, et 2) Prototype la fonctionnalité Y, et 3) Installer le nouvel outil de _build_”)
  
* Les priorités **peuvent correspondre directement aux items du TEC** (“Ces 3 items du TEC sont top prioritaires”, ou “les items du TEC sur le tableau sont rangés de haut en bas par ordre de priorité”). Mais ils n’ont pas besoin d’être spécifiques.
  
* Un test de priorités utiles est :
  * 1) “Cette liste de priorité **nous aide à décider quoi faire aujourd’hui et quoi ne PAS faire aujourd’hui !**”
  * 2) “Cette liste de priorité est tellement concise et claire que **toutes les personnes impliquées la connaissent par cœur !**”. 
  * 3) “Nous avons tous **compris pourquoi ces priorités ont un sens** pour l’entreprise”.  
&nbsp;  
  
* **Les priorités ne sont pas exhaustives.** Nous pouvons avoir beaucoup de choses en cours qui ne sont pas liées directement à notre top 3 des priorités.
C’est tout à fait normal, mais :
  * **Le travail non-prioritaire ne devrait pas par défaut interférer avec le travail prioritaire.** Il y a bien sûr des exceptions (“le serveur vient juste de tomber, relançons-le MAINTENANT !”), utilisez donc le bon sens et parlez-en.  
&nbsp;  
  
* Principe général :
  * 1) Êtes-vous en mesure de contribuer à un item de priorité forte aujourd’hui (directement ou indirectement) ? Si oui, faites-le ! Vous n’êtes pas certain ? Posez la question !
  * 2) Si vous n’êtes pas en mesure de contribuer à un item de priorité forte, alors travaillez sur quelque chose de priorité moindre, mais ne le laissez pas perturber les personnes travaillant sur des éléments de priorité forte.
  * 3) Soyez explicite à propos de votre choix et pourquoi.  
&nbsp;  
  
* **Les priorités sont en cascade** (ou hiérarchique, si vous préférez, j’ai simplement essayé de trouver un mot ayant une moins mauvaise connotation).
  * Votre équipe a des priorités. Ainsi que votre département. Ainsi que votre entreprise. **Les priorités de niveau élevé priment sur les priorités de niveau moindre, et sont vitales pour la cohérence au niveau de l’entreprise.** Ce qui signifie :
    * 1) **Les priorités de plus faible niveau devraient, au mieux, être en cohérence avec les priorités de niveau élevé** (ex: “La priorité du département est Y, la priorité de l’équipe est Y”, ou “la priorité du département est Y, la priorité de l’équipe est X et elle contribue à Y”).
    * 2) **Les priorités de plus faible niveau devraient, à minima, ne pas interférer avec les priorités de niveau élevé** (ex : “la priorité du département est Y, ce qui implique la plupart des autres équipes, notre équipe n’est pas en mesure de contribuer vraiment, donc nous prioriserons à la place X, et nous ferons en sorte de ne pas prendre du temps aux personnes travaillant sur Y”).  
&nbsp;  
  
* **Evitez les priorités individuelles.** Cela tend à tuer le travail d’équipe. Il est mieux de privilégier le partage de priorités à un niveau un peu plus élevé, comme une équipe, un domaine d’activité ou un projet.
  
* Les priorités changent (bien sûr !)
  * Il est utile d’avoir des **réunions récurrentes de priorisations** pour réévaluer les priorités (lors de chaque sprint pour une équipe, toutes les 6 semaines pour un département, ou toute autre périodicité pertinente).
  * … mais les priorités peuvent aussi changer à n’importe quel moment !
  * **Les priorités de niveau plus élevé ne devraient pas changer souvent,** car elles ont tendance à avoir des effets de bord sur les priorités de moindre niveau et sur le TEC. Cela engendre de la confusion. La fréquence des réunions de priorisations devrait correspondre grosso modo à la fréquence à laquelle nous nous attendons que les priorités ont besoin de changer.  
&nbsp;  
  
* Les priorités à long terme et celles à court terme peuvent figurer sur la même liste !
  * Par exemple “nos priorités sont 1) le support client, 2) le projet X, 3) la dette technique”. Le projet X pourrait être à court terme puis pourrait être remplacé par le projet Y, alors que le support client pourrait rester au top niveau priorité pendant encore des années et des années !  
&nbsp;  
  
* **Lorsqu’une liste de priorité a plus d’un item, soyez clair sur ce qu’il signifie vraiment.**
  * Exemple : Si nos top priorités sont “projet A et projet B”, qu’est-ce que cela signifie ? Est-ce que A est plus important que B ? Ou sont-ils la même importance, mais plus important que les autres projets ? Devrions-nous essayer de travailler exclusivement sur A lorsque cela est possible, ou devrions-nous partager notre temps de manière équitable entre A et B ?
  * Aucune règle n’est nécessaire, seulement des principes généraux.
  
Utilisés de manière approprié, les priorités en cascade, la visualisation du TEC et les limites du TEC peuvent vraiment aider votre organisation à se focaliser et de manière très rapide !

---
Auteur : [Henrik Kniberg](https://www.crisp.se/konsulter/henrik-kniberg)  
Source : [WIP and Priorities – how to get fast and focused!](http://blog.crisp.se/2014/09/25/henrikkniberg/wip-and-priorities)  
Date de parution originale : 25 Septembre 2014  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 10/12/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}




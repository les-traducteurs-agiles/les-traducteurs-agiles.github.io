---
layout: post
title:  "Ne passez pas à l'échelle, réduisez l'échelle de votre produit !"
date:   2021-04-05 00:01
published: true
tags:
- à grande échelle
- scrum
---

> La contradiction inhérente à appliquer Scrum à l'échelle, et 5 stratégies pour l'éviter

À la fin de cet article (vous pouvez aussi [l'écouter en anglais](https://www.buzzsprout.com/466339/6049342) sur notre podcast), vous aurez découvert que :

* Il y une contradiction inhérente au principe d'appliquer Scrum à l'échelle de plusieurs équipes développant un même produit ;
* On peut échapper à cette contradiction en n'augmentant pas le nombre d'équipes, mais en réduisant la complexité du produit ;
* Réduire la complexité d'un produit est comparable à découper le travail à faire dans le Backlog de Produit. Au lieu d'un seul produit de grande taille, vous aurez plusieurs produits plus petits autour d'un objectif fédérateur ;
* Réduire la complexité d'un produit permet d'augmenter la capacité de chaque équipe à se concentrer sur la valeur et à devenir plus réactive vis-à-vis de ses parties prenantes. Au niveau de l'organisation, cela permet de réduire les risques et d'encourager une culture d'expérimentation et d'entreprenariat.

# Difficile d'appliquer Scrum à l'échelle

Appliquer Scrum à l'échelle, c'est vraiment difficile non ? Comment travailler à plusieurs équipes sur un même produit ? Combien de Product Owners devrions-nous avoir pour un produit de grande taille ? Comment différentes équipes peuvent-elles livrer un Incrément terminé à chaque Sprint ? Comment gérer le nombre croissant de dépendances entre les équipes ? Honnêtement, je pense que dans la plupart des cas, appliquer Scrum à l'échelle revient à résoudre le mauvais problème. Et je dis cela indépendamment du _framework_ que vous utilisez, Nexus, LeSS ou SAFe. Laissez-moi vous expliquer pourquoi.

![les _frameworks_ à l'échelle]({{ site.url }}assets/the_liberators/image2-fr.png)  

Légende : Les _frameworks_ à l'échelle ne sont pas une solution pour des produits complexes. Ils risquent d'ajouter seulement de la complexité. Illustration par [Thea Schukken](https://www.linkedin.com/in/theaschukken/)


Le cadre de travail Scrum existe essentiellement pour affiner des éléments de grande taille en éléments plus petits, des projets entiers en _Sprints_, et des fonctionnalités de grande taille en plus petits éléments du Backlog de Produit. Bien qu'il soit souvent difficile, ce processus de découpage de grandes choses en éléments plus petits est un excellent moyen de réduire les risques ; les petits éléments sont plus simples, plus faciles à contrôler, et génèrent moins de gaspillage quand ils ne fonctionnent pas (ce qui arrive souvent pour du travail complexe). Faire plus petit c'est aussi aller plus vite. Ce sentiment est très bien exprimé dans l'une de mes citations favorites : « Ce qu'un développeur peut faire en un jour, deux développeurs peuvent le faire en deux ». Cette volonté de simplicité est inscrite fortement au sein même de Scrum, comme [Gunther Verheyen](https://ullizee.medium.com) l'exprime en disant : « face à la complexité, la simplicité est notre chemin ». La solution la plus simple --- en termes de nombre de variables --- est plus efficace qu'une solution plus compliquée.

> « Le _framework_ Scrum existe essentiellement pour affiner de grands éléments en éléments plus petits, des projets entiers en _Sprints_, et de grandes fonctionnalités en petits éléments du Backlog de Produit. »

Et donc quel rapport cela a-t-il avec le passage à l'échelle des développements sur un produit ? Le passage à grande échelle ajoute intrinsèquement de la complexité, car elle introduit plus de variables. Il y a plus d'équipes, plus de personnes impliquées dans le développement, plus de dépendances techniques potentiellement, plus d'opportunités de dynamiques de groupes négatives, et plus de place pour de la politique. Je suis sûr que la plupart d'entre nous accepterons ceci également. Comment se fait-il que nous utilisions un cadre de travail qui encourage la simplicité d'une part, tout en augmentant la complexité en ajoutant plus d'équipes d'autre part ?

# L'hypothèse de l'effet miroir

Une raison à cela résiderait dans une complexité qui serait intrinsèque au produit. Dans ce cas, le produit est considéré si gros qu'il nécessite tout simplement plusieurs équipes sans aucune alternative possible. Mais cette logique est absurde. Si le produit est si gros et/ou si complexe, en quoi est-ce une bonne idée de refléter cette complexité du produit dans la complexité du groupe de personnes qui le développent ?

> « En quoi est-ce une bonne idée de refléter cette complexité du produit dans la complexité du groupe de personnes qui le développent ? »

Une explication à cela est l'inverse de la loi de Conway. Cette loi établit que « toute organisation qui conçoit un système produira une conception dont la structure est une copie de la structure de communication de l'organisation ». Bien que l'effet en soit inversé, les organisations semblent implicitement refléter la complexité du produit dans la complexité de l'organisation du développement. McCormack, Ruskan & Baldwin (2011) ont trouvé des preuves de cette « hypothèse de l'effet miroir » en étudiant plusieurs organisations, et en conclurent que « le produit développé par des organisations les équipes sont relativement autonomes est significativement plus modulaire que le produit d'organisations où elles le sont moins ». Cela signifie-t-il que les produits complexes nécessitent toujours des organisations de développement complexes ?

Quand il s'agit de passage à l'échelle, et des _frameworks_ associés tels que LeSS, SAFe et Nexus, il semble y avoir une hypothèse implicite que seul le nombre d'équipes est une variable, et non la complexité du produit lui-même. Derrière cette hypothèse se trouve une approche très différente du développement de produit.

# Ne passez pas à l'échelle, diminuez la complexité de votre produit

Au lieu d'augmenter le nombre d'équipes, que se passerait-il si nous appliquions une stratégie de découpage au produit lui-même pour réduire sa complexité ? Tout comme nous découpons des projets entiers en plus petits _Sprints_, et de grands éléments du Backlog de Produit en plus petits, nous pouvons découper de grands produits en plus petits produits. En faisant cela, nous réduisons leur complexité et les rendons plus simples, plus petits, et leurs risques plus contrôlables. Nous pouvons rendre les produits suffisamment petits pour qu'une poignée d'équipes Scrum, préférablement même une seule, puisse livrer un incrément utile et de valeur de ce produit à ses parties prenantes.

Cette approche peut paraître similaire aux « [feature teams](http://www.les-traducteurs-agiles.org/2017/01/06/less-equipes-feature.html) ». La différence est que les feature teams travaillent (généralement) sur des fonctionnalités de bout en bout d'un seul Backlog de Produit partagé. Quand vous réduisez l'échelle de votre produit en plus petits produits, vous obtenez effectivement des Backlogs de Produits séparés et des équipes Scrum indépendantes qui agissent réellement comme des équipes produits.

# Stratégies possibles de réduction d'échelle

Comment pouvez-vous découper un produit de grande taille en produits plus petits et plus simples ? Voici quelques stratégies avec lesquelles nous avons travaillé. Elles partagent deux caractéristiques. La première est qu'elles correspondent à des coupes verticales d'un produit plus grand ; chaque petit produit continue d'apporter de la valeur par lui-même à ses parties prenantes. La seconde est que les équipes Scrum deviennent ou restent capables de livrer un incrément utilisable du produit à leurs parties prenantes (principalement les utilisateurs et les clients) à chaque Sprint.

#### 1. Découpez votre produit suivant les groupes de parties prenantes qu'il sert

Une stratégie est de découper un grand produit en plus petits suivant les groupes de parties prenantes (principalement les utilisateurs et les clients) qu'il sert. Prenez par exemple des logiciels de comptabilité tels que QuickBooks, Exact, ou Xero. Une approche est de considérer la suite logicielle complète comme « le produit ». Développer ce produit peut facilement nécessiter des douzaines d'équipes Scrum. Une autre approche est de considérer différents groupes de parties prenantes ; entrepreneurs, PME, grands comptes, organisations gouvernementales et ONG. Dans ce cas, le produit devient « comptabilité pour les entrepreneurs », « comptabilité pour les ONG », et ainsi de suite. Ce découpage peut se poursuivre autant que nécessaire pour conserver une organisation de développement aussi simple que possible. Par exemple, « comptabilité pour les entrepreneurs aux Pays-Bas » (NDT : on note ici que l'auteur est néerlandais) ou « comptabilité pour les boutiques en ligne ». Le découpage le plus efficace est celui qui aboutit au plus petit nombre d'équipes Scrum qui peut livrer un produit cohérent pour un ensemble identifié de parties prenantes.

#### 2. Découpez votre produit suivant les fonctionnalités qu'il remplit

Une autre stratégie est de découper un produit de grande taille en produits plus petits suivant les besoins fonctionnels qu'il remplit. Un bon exemple de cela est Google, avec sa large gamme de produits adaptés à des besoins spécifiques ; Google Drive pour le stockage de fichiers, Google Slides pour les présentations, Google Docs pour les documents, et Google Photos pour les images. Chaque produit est de taille réduite, remplit un but spécifique, et est utilisé par des différents groupes de parties prenantes.

#### 3. Découpez votre produit par destruction créatrice

Au lieu de découper votre produit en produits plus petits, la complexité de votre produit peut aussi être réduite en supprimant ce qui n'a plus suffisamment de valeur ou d'utilité. Ce processus de destruction créatrice retire des fonctionnalités et du code qui nécessite d'être maintenu, hébergé, et géré par le support, et qui, par conséquent, ne sera plus susceptible de générer des bugs.

#### 4. Ne découpez pas votre produit par couches techniques

Une stratégie répandue est de découper les produits en suivant les couches applicatives. Donc une équipe est chargée de la base de données, une autre du code back-end, et une autre du front-end. C'est une mauvaise idée. Bien que cette stratégie produise des équipes hautement spécialisées, ce qui pourrait sembler être un avantage, aucune de ces équipes ne peut livrer un logiciel utilisable par elle-même. Si un groupe de parties prenantes demande une nouvelle fonctionnalité, il est probable que toutes ces équipes devront fournir du travail (modifications sur la base de données, le _back-end_ et le _front-end_) pour livrer cette fonctionnalité.

#### 5. Plusieurs produits peuvent sembler n'en faire qu'un

Ce serait une erreur de considérer que le découpage de votre produit en plusieurs plus petits signifie automatiquement que vous ne pouvez les présenter ensemble comme un plus grand produit. Google est un bon exemple de cela, avec son écosystème riche de produits fonctionnant ensemble. Une autre approche est la place de marché, où les clients peuvent ajouter ou supprimer des modules additionnels pour répondre à leurs besoins. Une autre approche encore est une stratégie d'association d'éléments graphiques, regroupant les interfaces dans un tableau de bord unifié.

# Gérer les parties communes

Quelle que soit la stratégie que vous utilisez pour découper verticalement votre produit en plus petits produits, ils auront beaucoup en commun. Il y aura probablement besoin de partager une charte graphique uniforme, ainsi qu'un modèle de sécurité partagé, une plateforme de stockage, un moteur de calcul de taxes, et des règles métier. Certaines de ces parties communes pourraient devenir des produits à part entière ; un moteur de calcul de taxes pour l'Allemagne, un autre pour les Etats-Unis. Pour d'autres parties communes dont on ne peut faire des produits autonomes à part entière, d'autres solutions pourront émerger. Par exemple, la charte graphique peut être fournie sous la forme d'un guide de styles partagé, un _framework_ de conception partagé (ex : Material Design ou Bootstrap), ou des thèmes partagés. Les solutions techniques réutilisables, comme un modèle de sécurité ou des règles métier, peuvent être partagées avec des packages et de modules de code (ex : NuGet, NPM).

Si l'on observe les avancées du développement logiciel de ces dernières années, il est évident que la technologie avance dans une direction qui rend la réduction d'échelle progressivement plus facile. Les produits monolithiques peuvent être découpés en microservices, des services indépendants, qui peuvent être maintenus et développés par des équipes Scrum autonomes. Les équipes de développement peuvent utiliser des stratégies comme le modèle du figuier étrangleur pour procéder à ce découpage progressivement. La conteneurisation de type Docker permet de déployer très simplement des services de façon indépendante, dans de petits conteneurs virtualisés que l'on peut facilement déplacer vers d'autres serveurs. Les patterns de conception et les concepts d'architecture tels que l'Event Sourcing et CQRS sont conçus spécifiquement pour permettre à ces services de communiquer de façon robuste. Donc, en termes de technologies et de _frameworks_, il existe beaucoup d'outils disponibles.

# Les avantages à réduire l'échelle de votre produit

* La majorité des dépendances des équipes Scrum vis-à-vis d'autres équipes disparaissent. A condition d'être suffisamment pluridisciplinaires, cela permet aux équipes Scrum de livrer un incrément terminé à chaque Sprint, de raccourcir la boucle de feedback, de réduire les risques, et de rendre l'équipe plus réactive aux attentes de ses parties prenantes.
* La gestion de produit est simplifiée car chaque petit produit a son propre Product Owner avec un mandat complet sur ce produit. Il n'est plus nécessaire de gérer les complexités de la gestion de produit à l'échelle de douzaines d'équipes. Ou pire, de créer des hiérarchies de propriété de produits, qui étouffent la réactivité et l'autonomie. Au lieu de cela, les Product Owners travaillent avec les parties prenantes de leur produit --- utilisateurs, clients, et autres équipes --- pour faire évoluer le produit afin qu'il corresponde à leurs attentes.
* Chaque produit peut avoir sa propre balance profit/pertes, ce qui permet de déterminer plus facilement quels produits apportent de la valeur et sont utiles, et lesquels sont candidats à la création destructrice. Des produits séparés peuvent être vendus si besoin. Cela encourage une approche entrepreneuriale.
* L'approche modulaire des produits à petite échelle permet de lancer plus facilement des expérimentations sur de nouveaux produits potentiels. Quand l'expérimentation échoue, le souffle de l'explosion est circonscrit uniquement à ce produit.
* Cette approche encourage l'antifragilité. Lorsqu'un produit de grande taille échoue[, les dégâts sont beaucoup plus significatifs que pour un petit produit. Quand les organisations disposent effectivement d'un essaim de « petits produits » autour d'un objectif commun, l'essaim évolue suivant que certains produits réussissent et d'autres non.

![les défis]({{ site.url }}assets/the_liberators/image1-fr.png)  

#### Réduire l'échelle de vos produits peut créer de l'antifragilité contre les facteurs de stress et les défis qui se présentent. Illustration par [Thea Schukken](https://www.linkedin.com/in/theaschukken/)

Évidemment, réduire l'échelle d'un produit n'est pas une baguette magique. Elle présente ses propres défis. Par exemple, à quoi ressemble le marketing de plusieurs petits produits au lieu d'un seul plus grand ? Comment coordonner les changements qui affectent plusieurs produits ? Comment garder le travail réalisé par les équipes Scrum intégré avec l'objectif plus large de l'organisation ? Comment arriver à gérer les parties communes entre produits et à réduire le travail en double ? Mais comparé aux défis de passer à l'échelle le développement d'un unique produit entre de nombreuses équipes, il me semble que surmonter les défis de la réduction d'échelle du produit a plus de chances d'aboutir à une plus grande attention portée à la valeur, la réactivité, une culture qui encourage l'expérimentation, et un sens général de l'entreprenariat dans les équipes.

> « Quand il s'agit de complexité, le défi n'est pas de 'penser grand', mais de 'penser petit' »

# Un changement de paradigme

Quand il s'agit de complexité, le défi n'est pas de « penser grand », mais de « penser petit ». C'est le changement de paradigme qui est au cœur du _framework_ Scrum. Mais dans le développement de produit, nous tombons souvent dans le piège de « penser grand » et appliquer Scrum à l'échelle en ajoutant plus d'équipes. Nous ajoutons de la complexité par inadvertance. Cela a tendance à ralentir le travail, à l'alourdir avec des dépendances, et à augmenter les risques. Dans cet article, je défends l'approche opposée.

Au lieu d'essayer de refléter la complexité de votre produit dans la complexité des équipes, pourquoi ne pas découper votre produit en produits plus petits et moins complexes ? Cette stratégie de réduire les risques en découpant de grands morceaux en plus petits devrait vous être profondément familière, puisque c'est une part inhérente du _framework_ Scrum. N'est-il pas intéressant que nous revenions si souvent à « penser grand » quand il s'agit de passer à l'échelle, quand peut-être nous serions avantagés en « pensant petit » ?

# Références

MacCormack, Alan; Rusnak, John; Baldwin, Carliss Y. (2011). « [Exploring the Duality between Product and Organizational Architectures: A Test of the Mirroring Hypothesis](https://dash.harvard.edu/bitstream/handle/1/34403525/maccormack%2Cbaldwin%2Crusnak_exploring-the-duality.pdf) ».
SSRN Working Paper Series.
[doi](https://fr.wikipedia.org/wiki/Digital_Object_Identifier):[[10.2139/ssrn.1104745](https://doi.org/10.2139%2Fssrn.1104745)

---
Auteur : [Christiaan Verwijs](https://chrisverwijs.medium.com/about)  
Source : [Don't Scale Up. Scale Your Product
Down!](https://medium.com/the-liberators/dont-scale-up-scale-your-product-down-c70f335ccf3a)  

---
Traducteurs : [Samuel Chapal](https://www.linkedin.com/in/samuel-chapal/?originalSubdomain=fr) (texte), [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/) (images)  
Relecture : [Patrick Roux](https://www.linkedin.com/in/patrick-roux/), [Samuel Chapal](https://www.linkedin.com/in/samuel-chapal/?originalSubdomain=fr), [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 05/04/2021    

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

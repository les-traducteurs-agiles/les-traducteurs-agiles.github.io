---
layout: post
title:  "20 Anti patterns de product owners pour Scrum"
date:   2015-09-05 15:10:55
published: true
tags:
- product owner
---

## Des mauvaises odeurs chez les product owners

Pendant toute ma vie professionnelle, les gens m'ont parlé pendant des heures de l'importance de bons patterns de conception. Je crois que nous avons tous acheté des livres sur les patterns de conceptions, les recettes de cuisines ou tout autre sorte d'ouvrages nous donnant les bonnes pratiques dans tel ou tel domaine. Je n'ai rien contre ça et comment le pourrais-je ? J'ai moi-même écrit un livre boîte-à-outils sur les rétrospectives agiles :). Tous ces ouvrages sont utiles et nécessaires mais pendant ma carrière j'ai compris qu'écrire sur les bonnes pratiques n'est pas suffisant. Nous devons écrire à propos de ce que nous ne devrions pas faire, les anti patterns, les mauvaises odeurs comme je les appelle.

Lors des prochaines semaines, je vais passer un peu de temps à écrire là-dessus. J'écrirai plusieurs articles sur les mauvaises odeurs dans les différents rôles de Scrum et sur les différentes erreurs que font habituellement les entreprises lorsqu'elles implémentent scrum. Je commencerai cette série sur les mauvaises odeurs des product owners. J'ai déjà écrit [ici](http://lmsgoncalves.com/2013/02/27/common-mistakes/) sur les problèmes arrivant d'ordinaire aux product owners dans les organisations, et aujourd'hui je vais ajouter de nouveaux problèmes à cette liste. Si vous êtes intéressés par les anti patterns, cliquez [là](http://lmsgoncalves.com/tag/anti-pattern/), vous y trouverez tous les articles de mon blog sur ce sujet.

### Pas de product owner unique pour une équipe

Je vois ce phénomène assez souvent dans les organisations qui ont implémenté SAFe (Scaling Agile Framework) par le passé, qui l'ont abandonné et sont revenus vers du Scrum simple. Dans le cadre SAFe, il y a deux rôles : le product manager et le product owner. Le product manager est celui qui pense davantage en terme stratégique, le product owner est celui qui est plus dans les activités quotidiennes.

Quand les entreprises reviennent vers Scrum, les deux rôles n'existent plus, seul existe le product owner mais les entreprises ne veulent licencier personne donc elles affectent deux product owners à l'équipe même si elles continuent d'agir comme précédemment : une personne est affectée à la stratégie et l'autre aux activités quotidiennes, je vois ceci comme un échec.

Je crois qu'il est extrêmement difficile de travailler dans ce scénario, vous devez avoir une seule personne pour l'ensemble du produit, comme l'un de mes amis a l'habitude de dire "un seul cou" [^1].

[^1]: En français, nous dirions une seule tête mais l'utilisation du cou fait aussi référence à l'expression "single wring able neck" à propos de la responsabilité du product owner dans la décision de la priorisation des éléments du product backlog et donc à la fin par rapport à la réalisation du bon produit attendu des utilisateurs et dans le cas contraire c'est le seul à qui le cou serait tordu - NdT

#### Solution :

Les entreprises doivent comprendre qu'il n'est pas possible d'avoir ce scénario et qu'elles doivent offrir un environnement dans lequel chaque équipe a un seul product owner.

### Interférence dans le travail quotidien

J'ai pu observer cela dans plusieurs organisations et principalement pour deux raisons. La première est que le product owner était par le passé le chef de projet type qui courait après les gens pour que le boulot soit fait. La deuxième cause repose sur le fait que le scrum master ne soit pas fort et que le product owner doit intervenir et faire une grande partie des activités du scrum master, qu'il finisse par prendre le rôle trop au sérieux pour finir par contrôler et interférer plutôt qu'aider.

Dans cette situation, il est normal de voir les product owners prendre un rôle assez actif au quotidien, manipulant le processus normal. Un autre problème que je vois assez souvent est que les product owners tracent ce que font les développeurs, j'ai vu plusieurs fois des product owners parler à des développeurs et leurs demandant ce qu'ils étaient en train de faire parce qu'aucune tâche n'était associée à leur nom. Maintenant imaginez ce que les développeurs ressentent lorsqu'ils subissent ce type de contrôle.

#### Solution :

Je crois que la solution dans ce cas est de trouver un scrum master fort et expérimenté. Un scrum master expérimenté comprend assez bien ces deux rôles (scrum master et product owner) et il peut tutorer le product owner pour permettre à l'équipe de prendre la responsabilité de ses propres tâches. L'un des rôles des scrum masters est de protéger l'équipe des intrusions, avoir un scrum master fort et expérimenté à l'intérieur de l'équipe permettra à celle-ci de rester isolée et protégée des interférences non souhaitées, et en même temps d'aider les product owners à adopter les bons comportements.  

### Des stories construites en couches produit

C'est un sujet épineux. Au cours des derniers mois, j'ai travaillé avec des équipes qui n'étaient pas en capacité de livrer aussi vite qu'elles l'auraient fait si elles avaient utilisé d'autres approches. Elles font une des erreurs habituelles, elles ont des user stories construites en couches produit. Ceci a comme conséquence que les user stories sont dépendantes les unes des autres retardant d'autant la mise à disposition d'un produit utilisable par un client.

#### Solution :

En général, une bonne user story devrait être écrite pour couvrir toutes les couches du produit. Cela devrait être la finalité d'une user story. La solution à ce problème est de tutorer l'équipe et le product owner sur ce sujet. J'arrive à bien à le faire comprendre lorsque j'explique aux développeurs que cela ne sert à rien si nous livrons 200 user story côté serveur si l'utilisateur ne peut pas les utiliser sans la partie cliente. Ci-dessous une image d'Ángel Medinilla montrant de manière flagrante comment les stories devraient être construites.

![couches-produit]({{ site.url }}assets/anti_patterns_product_owners/pic1.png)

### Aucune visibilité de l'avancement du product backlog

Généralement le scrum master réalise des burn down charts montrant comment se déroule le sprint. C'est une pratique assez répandu, ce qui est moins répandu est le burn up ou le burn down de livraison ou de produit. C'est un problème assez répandu dans beaucoup d'organisations dans lesquelles j'ai pu travailler. Ne pas avoir ce type d'informations rend la vie du product owner plus difficile parce qu'il est plus difficile de savoir si l'équipe est dans les clous ou pas.

Avec ce type d'informations disponible le product owner peut prendre de meilleures décisions sur le périmètre afin de livrer le produit dans les temps, et apporter la plus grande valeur possible au client.

#### Solution :

La solution ici est assez facile. Le product owner devrait construire un burn down/burn up de produit exactement comme le scrum master le fait, mais à la place d'être focalisé sur le sprint, le product owner devra se focaliser sur la livraison. Un exemple de ce que cela peut donner peut être observé ci-dessous.

![Burnup]({{ site.url }}assets/anti_patterns_product_owners/Burnup.png)

### Le backlog est rempli de tout un galimatias et non d'user stories en bonne et due forme.

Ce problème est de loin le plus répandu de ceux que j'ai pu observer ces dernières années. La plupart du temps, le product owner n'écrit pas les stories dans un format utilisable, il écrit juste quelques mots et c'est tout. Le problème avec cette approche repose sur le fait que personne en dehors du product owner ne pourra comprendre de quoi parle la user story. Pour être honnête, j'ai vu des exemples de stories dans lesquelles même le product owner ne savait plus ce qu'il voulait solutionner avec certaines des users stories qu'il avait écrite.

#### Solution :

La solution que je préconise dans le cas présent est celle présentée par Roman Pichler dans son article : "[10 astuces pour écrire de bonnes user stories](http://www.romanpichler.com/blog/10-tips-writing-good-user-stories/)".

### Le product owner est dans l'incapacité de faire quoi que ce soit et n'agit pas en tant que gardien du backlog.

J'ai vu cette situation dans certaines des entreprises pour lesquelles j'ai travaillé. Malheureusement, ces entreprises ne réalisent pas à quel point cela est dangereux. Dans ces entreprises, le product owner n'avait pas le pouvoir de décider quoi que ce soit et les responsables pouvaient changer le backlog autant qu'ils le voulaient.

Cette situation conduit les product owners à ne plus s'occuper du produit. Ils commencent à ne plus se soucier du ROI, et ils perdent complètement leur comportement d'entrepreneur.

Cela se produit généralement dans un environnement de management traditionnel, où les entreprises veulent contrôler l'ensemble des éléments du product backlog, ni ne laisser aucune liberté ni ne faire confiance au product owner.

#### Solution :

De part mon expérience, cette situation est assez difficile à résoudre, principalement parce que la plupart du temps le problème vient des responsables au-dessus du product owner.

Dans ce cas, le scrum master ou le coach agile ont un rôle fondamental à jouer. Il est responsable pour parler avec l'encadrement (ou avec quiconque ayant cette façon de se comporter.) et pour expliquer l'impact que peut avoir ce comportement sur l'entreprise et sur la qualité du produit.

J'ai été témoin de plusieurs situations dans lesquelles le coach agile était capable d'expliquer à la direction ce qui était en train de se passer et qui était capable d'aider l'encadrement à changer de comportement.

### Le product owner qui utilise des estimations pour fixer les dates butoirs des démos pour les clients

Ici nous avons un problème typique rencontré habituellement chez les personnes qui ne comprennent pas les bases du développement logiciel. Cela va au-delà du développement agile de logiciel. Les personnes qui font cela ne comprennent pas comment le développement logiciel fonctionne, et donc leurs estimations ne sont que des calculs approximatifs ; elles ne garantissent en rien que tout sera fait pour une certaine date.

#### Solution :

Un certain nombre de personnes viennent me voir en me disant que quelques fois nous ne choisissons pas les dates de livraisons et que nous avons des dates butoirs à respecter. Par conséquent, il n'y a aucune manière de faire autrement dans ce type de configuration, les clients veulent seulement avoir leur produit.

Pour ceux qui ne me connaissent pas, j'ai travaillé pendant des années pour une grande entreprise de téléphones portables, je comprends donc ce que veut dire des dates dictées par le marché. Chaque année, nous avions les ventes des fêtes de fin d'année pour lesquelles les téléphones devaient être sortis ; il n'y avait pas d'autre solution, donc comment pouvons-nous gérer cela ? La réponse est simple : suivez les principes de bases de l'agilité.

Le product owner doit informer le client qu'après chaque sprint l'équipe a quelque chose a montré (et avec cet argument, le product owner devrait avoir ses démos). Pendant la démo/revue de sprint, le client a l'opportunité de donner des retours d'informations sur ce qui a été livré, et le plus important, a l'opportunité de sélectionner les choses les plus importantes présentes dans le backlog, ce qui permettra à l'équipe de toujours livrer ce qui a le plus de valeur pour le client.

En même temps (et c'est l'une des pratiques les plus fréquemment omises), le product owner vérifie le statut global de la livraison en utilisant les burndowns de livraisons. Cette pratique permet au product owner de savoir exactement où l'équipe arrivera, et de commencer une discussion avec le client pour déterminer ce qui peut être abandonné dans le cas où l'équipe n'est pas capable de livrer dans les temps.

Si le client n'est pas ouvert à ces suggestions, l'entreprise devrait commencer à reconsidérer si le client est quelqu'un avec qui l'entreprise voudrait travailler dans le futur. Les problèmes qui surviendront lors de futurs échanges seront si complexes que cette relation n'apportera aucun avantage à aucune des deux parties.

### Le product owner est trop occupé pour l'équipe, il est en relation avec beaucoup trop d'équipes

Je vois ce problème trop souvent. Des product owners qui sont complètement surchargés par le travail sont des product owners débordés.

#### Solution :

Un product owner ne devrait pas travailler avec plus de deux équipes. Bien sûr, il s'agit d'une règle générale, il pourrait être possible d'en avoir plus, mais si il/elle en a plus, cela peut être difficile d'apporter un soutien plein et entier aux équipes.

### Le product owner est trop occupé pour l'équipe, il passe beaucoup de temps en réunion avec les clients

Ce cas est un peu différent du précédent, mais le résultat est le même (pour l'équipe). Dans les deux cas, l'équipe n'a pas l'assistance de son product owner, ce qui rend difficile la tâche de développer le bon logiciel.

#### Solution :

Le boulot du product owner n'est pas simple ; c'est un boulot énorme et complexe, quelques fois le produit est si complexe qu'une personne seule pourrait ne pas être capable de tout gérer.

J'ai vu certaines entreprises mettre des analystes métiers dans les équipes ; ces personnes prenaient la responsabilité de parler avec les clients pour déterminer les besoins du marché, laissant la responsabilité de l'aspect technique du produit au vrai product owner. J'ai vu cette technique dans plusieurs entreprises et en fait, cela fonctionnait plutôt bien.

### Le product owner proxy (ou de proximité)

Cette personne agit comme un substitut pour le vrai product owner. Cela peut aboutir à un retard dans la prise de décisions ou même des conflits. Roman Pichler, l'auteur de _Agile Product Management with Scrum_, donne l'exemple d'une entreprise où le PO était trop occupé pour remplir son rôle, l'entreprise fit appel par conséquent à un PO poxy. En conclusion, différents conflits se produisirent car le PO proxy n'avait pas été habilité à prendre des décisions et que toutes les décisions étaient supposées être faites par le PO officiel qui n'était jamais disponible.

#### Solution :

Chaque cas est différent, mais voici une solution qui pourrait s'appliquer de manière générale, je crois que nous pourrions essayer d'utiliser la même approche que dans le premier exemple : avoir un analyste métier dans l'équipe qui pourrait aider le product owner a avoir plus de temps pour aider l'équipe à livrer le bon produit.

### Le comité product owner

Cela arrive dans les entreprises qui créent un comité pour être responsable pour un produit. Lorsqu'il n'y a personne responsable pour le produit, cela peut conduire à un retard dans la prise de décisions. Souvent, la plupart des personnes impliquées veulent obtenir le consensus entre toutes les parties, et cela conduira à des réunions longues qui n'aboutiront à rien. C'est le cas typique de "trop de chefs dans la même cuisine". C'est un problème assez similaire à l'un des problèmes que j'ai évoqué précédemment.

#### Solution :

Chaque produit devrait avoir un seul product owner. De part mon expérience, si nous avons plusieurs personnes responsables pour un produit alors en fait nous n'en avons aucune. N'assignez jamais plus d'un product owner sur un produit. Si vous avez plusieurs produits qui sont liés les uns aux autres, vous pourriez avoir besoin d'un programme. Dans ce cas, vous devriez avoir un responsable de programme ou un product owner en chef comme certaines entreprises peuvent l'appeler, mais jamais avoir plus d'une personne responsable pour un produit.

### Le product owner sacrifie la qualité du produit afin de livrer le produit plus vite

J'ai vu cela arrivé assez souvent, tout spécialement quand le product owner est sous pression de l'extérieure. Les parties prenantes poussent les product owners à livrer le produit au plus vite, même si la qualité n'est pas au rendez-vous.

Bien sûr, cette approche sera préjudiciable à l'entreprise sur le long terme ; tout le monde sait qu'une qualité médiocre du logiciel créera des problèmes tôt ou tard et portera atteinte à la réputation du fournisseur.

#### Solution :

Ce problème est assez sérieux et, à mon avis, c'est quelque chose qui fait partie de la culture d'entreprise (de ne pas se soucier de la qualité). La méthode la plus utile que j'ai pu trouver pour réduire ce problème est la présence d'une définition du fini (DdF)[^2].

[^2]: Dod (Definition of Done) en VO - NdT

Une DdF est une simple liste de tâches définies par l'équipe qui représente toutes les activités qui doivent être faites avant que la story rentre en production. Pour en savoir plus à ce sujet, consultez ce [blog](http://lmsgoncalves.com/2014/10/05/15-ideas-definition-of-done-dod/).

Sans une DdF, c'est plus facile pour un product owner de pousser l'équipe dans ses retranchements ; si c'est liste est présente, il est possible pour les développeurs de montrer qu'une story n'est pas finie tant que toutes les tâches qui font partie de la DdF ne sont pas terminées. De part mon expérience, cela peut aider à réduire le problème.

### Confondre le rôle de product owner et celui de scrum master

J'ai vu cela arrivé plusieurs fois dans des entreprises où les scrum masters restaient inactifs pendant plusieurs semaines. Dans cette situation, les product owners n'ont plus l'aide dont ils ont besoin et ils commencent à s'occuper de toutes les activités internes de l'équipe. Arrivé à un certain point, le product owner ne sait plus quel est son propre rôle, et ce qu'est le rôle de scrum master. Cela provoque pas mal de confusion et, encore pire, des conflits et de la méfiance entre le product owner et le scrum master.

#### Solution :

La solution ici est assez simple, mais elle n'est pas du tout facile à implémenter. Dans ce cas, il est extrêmement important d'avoir un scrum master fort et expérimenté. Les grands scrum masters sont capable de faire leur travail les doigts dans le new, mais encore plus important, ils sont capables de tutorer les autres dans leurs propres travails. Les grands scrum masters sont aussi des grands coachs, par conséquent, avoir un scrum master fort et compétent dans cette situation est fondamental pour améliorer ces situations.

### Le product owner qui s'attend à un engagement accru parce "selon son expérience, cela ne devrait pas prendre aussi longtemps"

Il est assez habituel de voir ce type de comportement de la part de chefs de projet de la vieille école, pour lesquels les engagements étaient donnés sous la contrainte des chefs de projets ou bien des parties prenantes. Une autre hypothèse possible repose sur le fait que certains product owners sont d'anciens responsables techniques ou des architectes. Dans cette situation, l'équipe discute avec quelqu'un qui a de grandes compétences techniques et qui s'attend à ce que l'équipe résolve plus rapidement les problèmes.

#### Solution :

Dans ces deux situations, le boulot de scrum master est assez important ; il doit protéger l'équipe. Il doit expliquer au product owner que l'équipe a la responsabilité de ses estimations. Ses membres sont ceux qui décident de la quantité de travail nécessaire pour livrer et qu'il n'y a rien qu'il puisse faire. Le scrum master doit expliquer au product owner que les membres de l'équipe font de leur mieux et qu'il doit leurs faire confiance.

### Ils sont product owners parce qu'ils sont responsables/chefs de département

Dans certaines entreprises, le product owner a un semblant de pouvoir, et certaines personnes vont essayer d'obtenir cette position même s'ils n'ont aucun intérêt dans le produit lui-même. Ils utilisent cette position comme d'un tremplin pour accroître leur pouvoir politique. Comme vous pouvez l'imaginez, la plupart du temps le résultat obtenu manque de qualité ou est de piètre qualité, ce qui conduit à une frustration générale.

#### Solution :

Dans ce cas, je crois vraiment qu'il n'y a grand chose que je puisse suggérer ; la direction doit comprendre que le product owner est extrêmement important pour l'entreprise et que seules les personnes comprenant les clients et le marché peuvent faire un bon boulot. Assigner des personnes qui ne comprennent ni le marché ni les clients à ces postes est un aller-simple vers l'échec. Je peux simplement suggérer que la direction devrait assigner ce poste à des personnes selon leurs compétences et non sur la base d'intérêt politique.

### Le product owner qui pensent que ce n'est pas leur rôle de maintenir le backlog ou qui délèguent l'écriture des user stories à l'équipe et/ou au SM

(Heureusement) Je n'ai pas vu cela arrivé très souvent pendant ma carrière, mais cela peut arriver. Ce type de product owner pense que son boulot est seulement de jeter des idées dans le backlog et que quelqu'un d'autre devrait faire le travail fastidieux de transformer ces idées en stories. Ce type de product owner pense que son travail est trop important pour perdre du temps en tâches secondaires.

#### Solution :

Je crois que le scrum master et l'équipe elle-même ont un rôle important à jouer ici. Ensemble ils doivent expliquer au product owner que tout cela c'est son boulot. Ils doivent expliquer que sans un backlog bien maintenu, l'équipe ne peut pas faire son propre travail. Les stories devraient être discutées entre le product owner et l'équipe. Le product owner est en dernier ressort la personne responsable pour garder le product backlog en bonne et due forme.

Le scrum master et l'équipe doivent montrer au product owner qu'il est extrêmement difficile de faire quoi que ce soit si le product backlog n'est pas maintenu. Une bonne story doit être claire, écrite de façon optimale selon le format [INVEST](http://www.les-traducteurs-agiles.org/story/2015/02/23/investissez-dans-de-bonnes-stories-et-dans-des-taches-smart.html) (Indépendante, Négociable, (de) Valeur, Estimable, (Suffisamment) petite et Testable) avec les critères d'acceptances adéquates.

### Le product owner qui pense qu'un scrum master est seulement un chef de projet dont le rôle est de pester après les gens pour qu'ils fassent leurs boulots

Malheureusement, il y a encore beaucoup de gens qui ne comprennent rien au comportement humain. Il y a beaucoup de gens qui pensent encore que les punitions et la mise sous pression au travail est une bonne manière de motiver les gens. Beaucoup de ces product owners croient encore que les gens sont paresseux et qu'ils ont besoin de chefs de projets pour les garder disciplinés, et bien sûr (selon leur point de vue) le scrum master est tout à fait désigné pour ce boulot.

#### Solution :

La solution n'est pas du tout facile à mettre en place. Je crois vraiment que cela a plus a voir avec un état d'esprit qu'avec n'importe quel processus agile. Je suggérerais aussi de faire suivre une bonne formation agile à ce product owner pour être certain qu'il comprenne que ces rôles sont dans le développement agile de logiciels.

Pour compléter cela, je lui ferais suivre aussi une bonne formation sur les motivations intrinsèques pour lui permettre de comprendre ce qui motive réellement les personnes à faire du bon boulot. S'il ne souhaite pas suivre l'une de ces sessions de formations, alors lui donner à lire le livre _Drive_ de Daniel Pink.

### Le product owner qui refuse de choisir entre les cinq principaux éléments prioritaires

Je vois cela assez souvent ; le product owner désigne la plus importante story comme un Doit-avoir, puis apparaît une autre story qu'il indique comme étant plus importante, elle devient alors une Doit-doit-avoir, et ainsi de suite. Cela montre clairement que le product owner ne comprend pas réellement quelle doit être la chose (unique) la plus importante qui doit être réalisée pour le prochain sprint.

Cela devient vraiment dangereux lorsque des équipes travaillent sur plusieurs problématiques importantes. Il n'y a pas si longtemps, certaines de mes équipes travaillaient sur différents objectifs à accomplir en un seul sprint. Le résultat fût médiocre, elles n'étaient pas concentrées, et alors que tous le monde travaillait sur tout, les équipes échouaient systématiquement à atteindre ses objectifs.

#### Solution :

Ici, il est important que le product owner comprenne quelles sont les choses les plus importantes qui doivent être livrées aux clients. Les product owners doivent comprendre que l'équipe ne peut pas tout livrer en même temps, par conséquent ils doivent vraiment comprendre quelle est la priorité principale qui devrait être terminée pour le prochain sprint.

Lorsque nous avons appliqué cette règle dans quelques unes de mes équipes, elles se sont focalisées sur leur objectif de manière radicale et elles ont commencé à livrer davantage de stories par sprint. Mais plus important que ça, elles ont commencé à livrer des fonctionnalités complètement implémentées qui pourraient être livrées aux clients. Avant, les équipes livraient beaucoup de choses, mais aucune des fonctionnalités n'étaient prêtes, bloquant ainsi la livraison aux clients.

### Le product owner qui insiste pour architecturer la conception de la solution

J'ai mentionné précédemment que quelque fois le product owner est un ex-architecte ou un ex-responsable technique. Cela a pour conséquence qu'il est normal d'avoir ce type d'anti patterns. Le product owner veut être responsable de l'architecture du produit, rendant ainsi folle l'équipe.

#### Solution :

Le scrum master et l'équipe doivent expliquer au product owner que la conception de l'architecture n'est pas de sa responsabilité. J'ai toujours aimé donné l'explication suivante : le scrum master et l'équipe sont responsables du "comment" : comment le produit est réalisé. Le product owner est responsable du "quoi", ce qui veut dire que le product owner devrait être le seul qui dit qu'est-ce qui est supposé être réalisé.

### Le product owner qui ne se considère pas comme faisant partie de l'équipe

Je ne vois pas trop souvent cet anti pattern, mais plusieurs personnes me l'ont signalé, par conséquent je l'ajoute à ma liste. Comme le titre le suggère, le product owner ne se sent pas comme faisant partie de l'équipe. Il sent qu'il devrait être responsable pour livrer des stories et rien de plus. Comme vous pouvez l'imaginez, la coopération entre les membres de l'équipe et le product owner ne sera pas au beau fixe, et arrivé à un certain point la coopération deviendra extrêmement difficile.

#### Solution :

Le guide scrum indique :

"L'équipe scrum comprend un product owner, l'équipe de développement, et un scrum master."

Bien sûr, ce n'est pas parce que le guide scrum l'indique, qu'il est garantit que le product owner se considèrera comme faisant partie de l'équipe. Mais, je pense néanmoins que cela pourrait être un bon point de départ. Le scrum master ou l'équipe pourraient lui expliquer, que selon le manuel, le product owner fait officiellement partie de l'équipe. En plus de cet argument, l'équipe et le scrum master pourraient expliquer au product owner qu'ils ne sont pas capables de faire un super boulot à moins que le product owners ne se rapprochent plus d'eux. Et cela pourrait être un bon sujet pour une rétrospective.

J'espère que vous avez aimez cet article :) J'écrirai davantage sur ces sujets ces prochaines semaines :)

---
Auteur : [Luis Gonçalvès](http://lmsgoncalves.com/about/)  
Source : [20 Product Owners Anti Patterns in Scrum](http://lmsgoncalves.com/2014/09/29/product-owner-anti-patterns/)  
Date de parution originale : 29 Septembre 2014  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 05/09/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

---
layout: post
title:  "Scrum, le guide du maître"
date:   2014-07-03 21:26:55
tags:
- équipe
- scrum
---
## La traversée des plaines du développement logiciel

Dans cet article, je vais vous introduire à une notation symbolique et visuelle qui nous permettra d'évoquer plusieurs phénomènes relatifs à Scrum. La notation utilisée pour le développement logiciel sera basée sur la métaphore des jeux de rôles médiévale-fantastique. Cette métaphore existe dans ma tête depuis un certain temps et je l'utilise dans mon travail quotidien en tant que scrum master et je m'y réfère fréquemment à travers mon imagination. En écrivant à l'aide de cette métaphore certains aspects du développement agile de logiciels, je voulais tester jusqu'où conduirait-elle(et de manière surprenante, à mon avis, elle peut mener très loin). Aussi, j'ai entrepris de rédiger un article plutôt ludique, pour des personnes connaissant les deux sujets.

### Équipe = Groupe

Commençons avec l'équipe. Un groupe de braves aventuriers, traversant les vastes plaines du développement logiciel, bravant le danger les attendant à chaque tournant.

<div align="center">
  <img title="Le groupe" src="{{ site.url }}assets/gdm_scrum/party.png" />
</div>

Comme vous pouvez le constater, les membres de l'équipe ne sont pas identiques, car chacun à des compétences spécifiques. Imaginez respectivement l'expert en base de données, le testeur et le concepteur d'IHM en guerrier, magicien et voleur. Remarquez que bien qu'ils soient différents, ils ont tous la même importance... C'est une question d'une bonne conception de jeu. Si un prêtre ne peut rien faire d'autre que guérir (et donc il ne serait rien de plus qu'un rabais ambulant sur des potions de guérisons), tout le monde voudra jouer le magicien.

Mais, à propos de l'expérience ? Est-il évident qu'un développeur de base de données expérimenté puisse être plus important qu'un expert mobile débutant ? Eh bien, regardons cela de plus près. Vous le savez d'expérience sur D&D : dès que vous êtes le seul magicien ou voleur autour de la table, vous êtes important, peu importe que vous soyez niveau 3 ou 21. Si personne n'est capable de neutraliser la malédiction de la méchante sorcière, ou de crocheter la serrure de la porte de la prison, ils se reposent tous sur vous.

Si vous avez un groupe jouant ensemble depuis de nombreuses années et que votre guerrier a atteint le niveau 17, et que maintenant vous avez un nouvel ami qui veux jouer un guerrier également, que faites-vous ? Il fait un pitoyable d6 de dégâts alors que votre ancien guerrier fait 3d12 avec sa hache. Si l'équipe fait remarquer cela à la nouvelle recrue, elle perdra vite sa motivation et n'atteindra jamais l'expérience requise pour devenir valable. Une relation de type maître-padawan pourrait fonctionner, mais généralement cela ne fonctionne qu'un temps. Cela est plus particulièrement criant dans la vraie vie où la nouvelle personne vient de passer 5 ans d'études ou plus et que maintenant elle veut faire des choses ayant un véritable impact, et non plus être l'apprenti de quelqu'un à nouveau. À mon avis, la meilleure solution est le changement de classe. Votre vieux guerrier a une origine plutôt tribale (rappelez-vous la hache), alors que la nouvelle recrue peut être un noble chevalier sachant l'héraldique, l'histoire et sachant même lire. Que se passerait-il maintenant si vous enleviez la classe générique du guerrier du jeu, et introduisez barbares et chevaliers comme des spécialisations ? Cela fonctionne pareil pour l'équipe. Vous avez déjà un développeur de systèmes dorsaux (backend - NdT) extrêmement expérimenté mais vous en avez besoin d'un deuxième, alors arrive une nouvelle personne. A la place d'avoir un développeur de systèmes dorsaux (backend - NdT) junior pour un certain temps, choisissez un aspect (ou une bibliothèque, un sous-système ou n'importe quoi d'autre) et faites-le se spécialiser dessus. A la place d'avoir un développeur de systèmes dorsaux (backend - NdT) junior, vous avez maintenant un expert en journalisation dans l'équipe. Chouette. Et aussi longtemps que vous êtes le seul expert en journalisation ...

_Remarque : nous venons de discuter dans une certaine mesure de la spécialisation entre les membres de l'équipe et de comment cela devrait fonctionner. Je voudrai insister sur la conclusion une fois de plus : la spécialisation des compétences est souhaitable. La spécialisation des responsabilités ne l'est pas. La totalité de l'équipe prendra avantage d'avoir quelqu'un qui soit réellement un expert sur le système de journalisation, et qui pourra intervenir si tous les autres ne sont pas en mesure de répondre. Mais cela signifie tout de même que la recrue prendra toute tâche non relative à la journalisation si la tâche doit être faite immédiatement. Ce que nous ne pouvons pas accepter est l'attitude "Je ne suis pas en charge de la journalisation, laissons Thomas s'en occuper, je m'occupe uniquement de la base de données". Chaque membre de l'équipe prendra chaque tâche qui doit être faite, à moins que la tâche soit suffisamment difficile pour qu'il ne puisse pas la traiter. Et il est attendu de chaque membre de l'équipe d'acquérir certaines compétences basiques dans des domaines qui ne sont pas de son expertise, de cette manière, l'expert en journalisation pourra faire, disons, 90% des tâches sur les bases de données. Pour les 10% restant, il pourra appeler alors l'expert en base de données._

Revenons à notre métaphore médiévale-fantastique. Considérons un groupe typique comprenant un guerrier, un magicien et deux rôdeurs. Soudain, le magicien meurt. Comme vous le savez bien, le maître du jeu a raconté l'histoire d'un tragique accident sur le plan éternel de la peur mais nous savons tous que Thilo, qui joue le magicien, a une nouvelle petite amie et à mieux à faire maintenant que jouer à D&D avec ses copains. Dans le projet, cela signifie que notre concepteur d'IHM a quitté l'entreprise.

<div align="center">
  <img title="Une perte dans le groupe" src="{{ site.url }}assets/gdm_scrum/party_loss.png" />
</div>

Nous avons maintenant un groupe avec un guerrier, deux rôdeurs elfes mangeurs d'herbe et aucun magicien. Que pouvons-nous faire ? Si nous continuons comme cela, nous serons morts dès que nous ferons face au premier mort-vivant vulnérable uniquement à la magie. Alors nous rapportons un problème sur les tableaux scrum. Maintenant tout le monde est au courant de l'affaire mais cela n'aide pas vraiment. Nous pouvons escalader auprès de l'encadrement que nous avons un problème de ressources à cause du départ de Thilo. Il est probable que l'encadrement comprendra qu'il nous manque une ressource. En tant qu'excellents responsables, ils se réuniront, réfléchiront, feront de la politique, tireront quelques fils et trouveront finalement une autre ressource. Une bonne recrue, bien sûr, quelqu'un d'expérimenté, de bonne réputation et ayant d'excellentes compétences en tir à l'arc.

<div align="center">
  <img title="Le groupe avec des rôdeurs" src="{{ site.url }}assets/gdm_scrum/party_only_rangers.png" />
</div>

Que dalle ! Comment cela aurait-il pu être évité ? Dans un monde idéal, votre patron connaît D&D. Il pourrait dire la différence entre un combat à distance et un combat au corps à corps et connaîtrait les différences subtiles entre la magie cléricale et la magie des arcanes. En réalité, la dernière fois qu'il y a sans doute joué remonte au temps où l'Œil Noir (jeu de rôle très connu Outre-Rhin - NdT) appartenait encore à Schmidt Spiele (éditeur du jeu l'Œil Noir - NdT). Et, même s'il savait, il a probablement eu 2 candidatures suite à la parution de son annonce de recrutement externe et les deux candidats ne pourront commencer que dans six mois au mieux, donc il a dû promettre certaines faveurs à quelques amis pour faire venir la personne qu'il vous a fourni.

Maintenant c'est à vous de jouer, et cela veut dire que Legolas doit ramasser le bâton du magicien et devenir un apprenti magicien. Par "devenir" je ne veux pas dire temporairement jusqu'au retour de Thilo mais devenir un magicien pour de bon. Après avoir travaillé pendant des années pour devenir un tireur d'élite, ça craint, mais qui a dit que la vie était juste ? Et de nouveau : aussi longtemps que vous êtes le seul magicien ...

Encore qu'ici, il y a quelque chose qui s'est mal passé. À mon avis, il s'agit de l'usage du terme "ressource", alors vous vouliez vraiment dire en fait "il nous manque un Thilo". En désignant les personnes comme des "ressources", cela implique une force de travail générique, remplaçable, ce qui signifie avoir en tête une image très mesquine lorsqu'il s'agit de développement logiciel. En guise de solution, je propose de bannir le terme "ressource" lorsque l'on se réfère à des êtres humains, et de le remplacer par le terme "compétence". Vous pourriez vous demander pourquoi ne pas aller jusqu'au bout du raisonnement et désignez les humains par ce qu'ils sont, c'est à dire des humains. Mais en l'appliquant dans la situation précédente, vous iriez vous plaindre à votre patron en lui disant "il nous manque un humain depuis le départ de Thilo" et conséquemment, il pourrait vous amener une fillette de 13 ans le lendemain, qui est bien évidemment un merveilleux être humain. Mais en fin de compte, ce n'est pas ni la personnalité gagnante de Thilos ni ses blagues qui manquent au projet, mais le fait que personne ne sait comment s'occuper désormais cette satané base de données. Il s'agit donc de "compétence", et non d'"humain". Et dans l'exemple précédent, le patron aurait donc pu comprendre "il nous manque une compétence depuis le départ de Thilo" et il aurait donc pu répondre "quelle compétence ?". Peut-être, (mais seulement peut-être), l'ensemble de la situation pourrait avoir été mieux se goupiller.

### Product owner = Oracle aveugle

Comme évoqué précédemment, le groupe voyage à travers les vastes plaines du développement logiciel. Et ils le font pour une bonne raison, ils veulent atteindre le château mystique dans les nuages, dénommée la vision produit.

<div align="center">
  <img title="Le château dans les nuages" src="{{ site.url }}assets/gdm_scrum/cloud_castle.png" />
</div>

Parce que personne ne sait où exactement le château est situé, il leurs fût adjoint un vieil homme revêtu d'une cape marron, et d'un bandeau sur ses yeux aveugles. Le vieil homme est un sage mystique, un oracle, qui peut voir le château à l'horizon. Le vieil homme est acheminé à dos d'âne afin qu'il ne trébuche pas sur un caillou ou ne se perde et chaque soir, il indique au groupe la direction à suivre sur la carte. Examinons le tableau de plus près.

<div align="center">
  <img title="Sprint" src="{{ site.url }}assets/gdm_scrum/sprint_fr.png" />
</div>

À chaque sprint, le groupe se déplace, affrontant les dangers et les pièges au gré des aventures, se rapprochant toujours un peu plus du château. Nous traçons une flèche sur la carte pour marquer leur progression. Désormais, chacun a son rôle. Le groupe doit comprendre que l'oracle est le seul qui peut vraiment voir le château dans les nuages. Sans lui, ils ne l'atteindront jamais. L'oracle doit comprendre qu'à l'exception de sa compétence mystique, il n'est qu'un vieil homme aveugle voyageant avec une bande d'aventuriers vétérans. Ils savent comment traverser les rivières, affronter les trolls en chemin et éviter de se faire dépouiller par les hobgobelins. Vous l'aurez sûrement deviné maintenant que l'oracle est le product owner.

À la fin, le groupe (y compris le product owner) est jugé sur la progression réalisée en direction du château.

<div align="center">
  <img title="Vers le château" src="{{ site.url }}assets/gdm_scrum/sprint_direction_of_castle_fr.png" />
</div>

Toute progression dans une autre direction est perdue. Une progression dans une direction très différente (une déviation de plus de 90°par rapport au château) est même nuisible. Sur cette image, les responsabilités sont claires. La longueur de chaque flèche dont l'équipe est responsable, est appelée la vélocité de l'équipe. Le product owner est responsable pour donner la bonne direction dans laquelle ils doivent aller.

### Partie prenante = Panthéon

Alors quelle sorte d'étrange compétence mystique permet de voir un château dans les nuages ? Comment est-ce que l'oracle produit cette image ? Comment sait-il qu'il s'agit une compétence mystique, et qu'il n'est pas juste cinglé ? Comment l'équipe sait-elle ?

Restons dans notre décor de campagne médiévale-fantastique. L'oracle est une sorte de prêtre, en relation avec certaines divinités, appelées parties prenantes. Elles suivent leurs propres raisonnements et intérêts pour des raisons que nous autres mortels ne pouvons pas comprendre. Mais chacune d'entre elles a son propre château dans les nuages et chacune veut que les aventuriers l'atteignent. S'il provoque la colère des dieux, l'oracle est dans la panade. Pour commencer, l'oracle détermine ce que les dieux veulent et en fait une représentation mentale (étant aveugle c'est la seule carte à sa disposition, pauvre hère). Évidemment, il ne peut atteindre tous les châteaux en même temps. Donc, il classe les différentes divinités par ordre d'importance. Si vous provoquez la colère d'un dieu, il faut que vous soyez sûr qu'il s'agit bien d'un dieu mineur. Alors à quoi cela ressemble t'il sur une carte ?

<div align="center">
  <img title="Plusieurs châteaux" src="{{ site.url }}assets/gdm_scrum/several_castles_fr.png" />
</div>

Notre mystique décide de guider notre groupe vers l'endroit marqué en rouge, considérant qu'il s'agit de l'endroit le moins risqué.

Toutefois, les dieux n'ont pas le même degré d'importance. Chaque prêtre jure allégeance plus particulièrement à un seul dieu. Dans le monde réel, c'est celui avec le budget, et qui est appelé sponsor du projet. Atteindre ses objectifs est obligatoire. Dit autrement, tout le reste est optionnel. A tout entendre, c'est comme si l'oracle avait finalement très peu de liberté où placer le château sur la carte. En réalité cela dépend de la visibilité du château dans les nuages du sponsor du projet. Certains sponsors ont des idées claires, comme de l'eau de roche, sur où ils veulent que l'équipe soit avec des périmètres bien définis. Ils choisissent des product owners uniquement parce qu'eux-mêmes n'ont pas le temps de voyager avec l'équipe. Mais certains sponsors produisent des images très floues, et le château reste caché derrière les nuages.

<div align="center">
  <img title="Au loin" src="{{ site.url }}assets/gdm_scrum/broad_castles_fr.png" />
</div>

Dans le second cas, le product owner à un espace à l'intérieur duquel il voyage. Il peut y construire son propre château dans les nuages.

Maintenant considérons une situation plus complexe et discutons de ce qu'un oracle avisé ferait.

<div align="center">
  <img title="Beaucoup de châteaux" src="{{ site.url }}assets/gdm_scrum/many_castles_fr.png" />
</div>

Phil, le sponsor, a donné une vision au product owner sous la forme d'une subvention européenne, de quelques mots à la mode et de très vagues idées (a) à propos de "personnages virtuels détaillés". Tom, une partie prenante aurait préféré aller sur la réalisation de "mondes massifs", pour lesquels il a une idée très claire pour une application sympa (b), mais sa demande de subvention a été rejetée, et donc il n'est pas devenu sponsor. Swen a un projet sur la réalisation de personnages virtuels et plus particulièrement sur leurs expressions faciales (c). C'est dans le périmètre donné par la subvention européenne du sponsor et avec une date butoir proche. Jörg a également un projet sur les "personnages virtuels ", mais il est intéressé plus particulièrement sur un moteur physique crédible (d). Son idée pourrait être dans le périmètre donné par la subvention européenne, mais elle est assez différente de celle de Swen.

Alors qu'est-ce que devrait faire le product owner ?

a) Tout d'abord, quoi qu'il fasse, il devrait rester à l'intérieur de cet espace. Aussi longtemps qu'il aura Phil à ses côtés, il sera protégé en cas d'ennui, par une entité puissante.

b) La vision de Tom ne peut être suivie. Tom devrait en être informé, et cela diminuera peut-être sa colère. Pour en être certain, l'information de la situation devrait être remontée d'abord à Phil, afin qu'il puisse protéger plus tard le product owner de la colère éventuelle de Tom contre lui et de ses tentatives d'harcèlement. Mis à part ça, il a plusieurs possibilités.

<div align="center">
  <img title="Plan a" src="{{ site.url }}assets/gdm_scrum/many_castles_opt_a_fr.png" />
</div>

Une option est d'aller d'abord au château de Swen et d'être certain d'y arriver pour la date butoir. Après cela, il change d'objectif et va dans une direction proche du château de Jörgs. De cette façon, et Swen et Jörg seront content de lui. Toutefois, Phil le jugera selon la progression faite en direction de son château, et cette progression a été réduite par ce détour.

<div align="center">
  <img title="Plan b" src="{{ site.url }}assets/gdm_scrum/many_castles_opt_b_fr.png" />
</div>

Aussi une option différente pourrait être de construire un château quelque part entre l'idée de Swen et de Jörg et d'y aller en droite ligne. Swen et Jörg seront moins content, mais la progression en direction de Phil en sera meilleure.

Les deux plans sont valables et ces décisions doivent être prise par le product owner.

### Problèmes = Rencontres

Que serait l'aventure sans les rencontres ? L'oracle indique au groupe d'aller à l'est, de l'autre côté de la grande rivière. Le pont s'est effondré, la rivière est haute, le bac a été capturé par des pirates et un druide protège les arbres de la forêt qui pourraient être utilisés pour construire un radeau. Une journée ordinaire dans la vie d'un aventurier.

Le groupe discute maintenant sur ce qu'il faut faire : tuer les pirates, négocier avec le druide ou partir à la recherche d'un autre pont. Les personnes du groupe le font aussi pendant la réunion de planification de sprint et dans les réunions quotidiennes, c'est ce qu'ils ont l'habitude de faire, c'est ce à quoi ils excellent. Certaines fois, pendant qu'ils en discutent, l'oracle est présent, assis sur son âne. L'impliquer quelques fois peut être bonne idée. Peut-être a t-il une idée que tout le monde a raté (n'avions-nous pas signé un traité avec les pirates avec les pirates l'année dernière ?). Lorsque la solution implique diverger du chemin prévu, il devrait être consulté à chaque fois. Il peut contribuer en donnant des informations, par exemple : bien que nous devrions essayer de traverser la rivière, nous sommes un peu trop au nord, le mieux pour chercher un pont serait plus au sud.

Mais les problèmes peuvent arriver tout de même. Beaucoup d'oracles étaient des aventuriers tout à fait capables lorsqu'ils étaient jeunes et ils pourraient devenir assez retors. Par exemple, ils pourraient dirent "tuons juste les pirates". "Ce ne sont que des fillettes, ils s'enfuient toujours. À mon époque, nous avions l'habitude de massacrer les pirates par centaines.". Dans ce cas, l'oracle pourrait se voir gentiment rappeler d'aller s'asseoir sur son âne et de se taire car a) les pirates de son époque n'avaient pas d'arbalètes à tir rapide, b) ces pirates sont plusieurs douzaines et ils ont un troll des marais avec eux (qu'il ne peut pas voir parce qu'il est aveugle). Il pourrait ne pas faire dans le style "vous êtes tous des lâches", mais il pourrait dire : "Je pourrai tuer tous les pirates moi-même" Mais en fait, il ne pourrait pas. Tout le monde le sait, et l'oracle l'a prouvé lui-même en engageant les aventuriers. S'il pouvait voyager seul, il l'aurait fait depuis longtemps. À ce moment précis, le scrum master pourrait intervenir et rassurer l'oracle à qui probablement l'aventure ne manque qu'à lui-même.

C'est normalement le travail de l'équipe que de résoudre des problèmes. Quelques fois, la meilleure solution implique un petit détour. Dans ce cas, ils devraient consulter le product owner. Quelques fois, il pourrait arriver avec une solution comme celle-ci : si nous devons inclure de toute manière cette bibliothèque gestuelle, alors remontons les cinq stories suivantes concernant la gestuelle. Ainsi Jörg peut reporter la date butoir du logiciel pour son projet et nous marquons des points supplémentaires.  

<div align="center">
  <img title="Un nouveau plan" src="{{ site.url }}assets/gdm_scrum/many_castles_replan_fr.png" />
</div>

La carte ressemble maintenant à ceci. À l'origine, l'oracle voulait voyager directement vers le château. Mais avec la rivière bloquée, ils ont dû aller vers le sud pour trouver un autre pont. Puis l'oracle décida que de là où ils étaient maintenant, aller vers le château de Jörg serait des points facilement gagnés, donc ils prirent cette direction. Ce processus est appelé la replanification, et fait partie du cœur même de scrum. En fait, c'est cette particularité qui fait que les méthodes agiles sont différentes de la gestion classique de projets.

Gardons à l'esprit que l'oracle est aveugle, donc qu'il ne voit pas la rivière, ni les pirates, ni le druide. D'un autre côté, les aventuriers n'ont pas de contact avec le royaume des arcanes, ils connaissent les châteaux dans le ciel uniquement parce que l'oracle n'arrête pas de leur en parler. C'est une situation qui demande une confiance mutuelle. Énormément.

Alors comment les aventuriers peuvent-ils mal utiliser la confiance de l'oracle. S'ils s'approchent d'un village qu'ils connaissent, ils pourraient inventer ou exagérer quelque problème pour inciter le groupe à y aller afin de passer une nuit avec l'élu de leur cœur et ou prendre un verre à la taverne. Dans le monde réel, cela correspond à exagérer les problèmes avec certaines bibliothèques que les programmeurs n'apprécient pas, ou surestimer les problèmes qui pourraient être potentiellement résolus par certaines technologies qu'ils voudraient tester depuis longtemps pour des raisons personnelles. Et même plus, car cela implique passer un temps significatif à regarder YouTube pendant les heures de travail ou à se plaindre de problèmes, pendant qu'à vrai dire, les avancées sont petites parce qu'ils arrivent tard et qu'ils font de longues pause-déjeuner. L'oracle pourrait suspecter ce qui se passe mais il n'a pas vraiment moyen de savoir. Pour des situations comme celle-là, il y a un scrum master.

Et comment l'oracle peut-il mal utiliser la confiance des aventuriers ? Eh bien, il pourrait ne pas être un oracle mais seulement un vieux trouduc d'ivrogne juché sur une âne. Sa vision pourrait être obscure et confuse et il pourrait être lui-même incertain où le voyage devrait mener. Bien que cela soit involontaire ou malheureux, cela trahit réellement le groupe lorsqu'il maquille les raisons des intérêts supérieurs qui expliquent le pourquoi il change toujours d'avis. A nouveau, en aucune manière les aventuriers ne peuvent le dire et s'ils suspectent réellement leur oracle d'être un escroc, ils devraient aller voir le scrum master.

Une deuxième chose qui pourrait se produire est que l'oracle pourrait être un dieu du mal déguisé (une sorte de partie prenante camouflée). Dans le monde réel, c'est le cas du product owner qui a des intérêts propres dans le produit qui le détourne de la mission définie par le sponsor. Cette situation est à la fois dangereuse et difficile à identifier. L'équipe entière pourra avoir de sérieux ennuis après le projet lorsque surviendra la question "je vous ai envoyé sur une mission pour réaliser un éditeur 3D sur navigateur, alors pourquoi, bordel de merde, m'avez-vous livré un traitement de texte multi-plateforme ?". Une fois que la situation a été identifiée par le scrum master, il n'y a plus aucune raison d'échanger avec le product owner. S'il communique ouvertement et dès le début, qu'il agit également en tant que partie prenante, il pourrait exister une chance pour pouvoir gérer la situation. Mais une fois qu'il a menti - en gardant cette information pour lui - à propos de son double rôle, il doit être remplacé sans pitié.

### Résolution de problème = Souterrains

Jusqu'à présent, nous avons uniquement considéré les aventures en surface, où le groupe traverse la plaine, qui à part quelque rivière ou montagne au loin, sur laquelle ils sont libres d'aller à leur gré. Dans le monde réel, cela correspond à l'implémentation de fonctionnalité sur une plateforme opérationnelle. Nous allons par petites étapes d'une version opérationnelle du système à une autre, et la discussion tourne principalement autour de ce qui a du sens pour un utilisateur, moins sur comment y arriver. C'est l'idéal de scrum.

Quelques fois, nous le savons tous, le projet n'est pas du tout comme cela. Nous sommes piégés dans un labyrinthe de problèmes, nous avons cinq branches différentes mais aucune d'entre elles ne compile et nous ne savons toujours pas laquelle de cet ensemble de cinq librairies Bluetooth, pour lesquelles nous avons créées les branches, est la meilleure sur laquelle poursuivre.

Dans un monde médiévale-fantastique, cela correspond à de l'exploration souterraine. Sous terre, dans le noir, il n'y a ni cartes ni directions. Vous ne savez jamais à quelle distance de la sortie avant que nous n'arriviez dehors et vous ne savez jamais quels monstres vous attend au prochain tournant. Lorsqu'un groupe fait de l'exploration souterraine, cela a plusieurs conséquences. Tout d'abord, l'oracle n'est plus d'aucune aide, parce que savoir que le château est à l'est , ne vous dit pas si vous devez tourner à gauche ou tourner à droite dans le labyrinthe. Deuxièmement, le groupe ne sait jamais à quelle distance se trouve la sortie avant de l'atteindre réellement. Ces deux choses sont de bonnes raisons pour ne jamais pénétrer dans les souterrains.

<div align="center">
  <img title="Souterrains" src="{{ site.url }}assets/gdm_scrum/dungeons_fr.png" />
</div>

Alors qu'est qui nous y conduit d'abord ? Ordinairement, il y a trois raisons. En premier, l'aventure pourrait commencer dans un souterrain. Dans le monde réel, cela signifie que pour des raisons extérieures (le client a mis quelque contrainte ou la subvention européenne nous y oblige), nous devons utiliser une technologie qui ne nous est pas familière et que nous devons intégrer et maîtriser. Dans ce cas, l'exploration souterraine ne peut être éviter. Afin de réussir, nous devons gérer les problèmes qui sont inhérents. Et là, nous devrions faire attention à trois points.

En premier, nous devrions faire attention de ce que nous appelons la "user story zéro" à DFKI (Deutsche Forschungszentrum für Künstliche Intelligenz GmbH - Centre de recherches allemand sur l'intelligence articielle où travaille l'auteur - NdT). Lorsque nous commençons sous terre, nous implémentons toujours une première user story intégrant toutes les technologies utilisées dans le projet dans une application "hello world" ("bonjour au monde" - NdT), qui est construite automatiquement par une application de construction de système. Une fois seulement après que cette story zéro soit terminée, des stories apportant de la valeur métier sont faites, et sont comptées à partir de de la valeur un.

_Notez que dans un décor de campagne typiquement médiévale-fantastique, le groupe voyage en surface pour atteindre un souterrain, puis vont sous terre pour tuer quelques monstres. C'est le cas, parce que du point de vue du récit, vous voulez affrontez les plus gros risques à la fin de l'histoire. (Cela fait du plus de suspens - NdT). Dans le monde réel, vous mettez tous les risques que vous ne pouvez pas éviter au début du projet, donc arriver à ce point, notre sympathique analogie entre le développement agile de logiciel et les aventures médiévales-fantastiques tombe un peu à l'eau._

En second, nous devons être sûr que le product owner ne soit pas trop frustré. Comme évoqué précédemment, il est virtuellement inutile sous-terre et nous devons nous en occupé d'une manière ou d'une autre. La solution est facile à écrire : il doit uniquement s'asseoir sans bouger, se relaxer et attendre. Mais nous le savons tous, il est sous une énorme pression, et il deviendra inévitablement de plus en plus frustré lorsque la user story zéro échouera à assembler. Apportez-lui du café ou un alcool, emmenez-le au cinéma ou achetez-lui un chat, n'importe quoi qui puisse l'aider. Il doit juste tenir le coup. Le dernier point est que nous pourrions être dans une situation où la durée totale du projet n'est pas assez longue pour sortir du souterrain, soit nous pourrions sortir trop tard pour atteindre un état stable acceptable à la fin du projet. Donc gardez cela à l'esprit, le product owner et le scrum master doivent garder un œil là-dessus ensemble et estimer la date la plus tard possible à laquelle la user story zéro doit être réalisée afin que le projet n'échoue pas de manière horrible. Si cette date arrive avec des problèmes non résolus, en conséquence la situation doit être remontée à l'encadrement sans délai. Mais à part ceci, ni le scrum master ni le product owner ne devraient être impliqués, car après tous les aventuriers sont des experts dans la bonne vieille exploration souterraine.

Il y a deux raisons de plus d'aller en exploration souterraine. L'une d'elle est, que le product owner et l'équipe décide de le faire ensemble d'un commun accord. Pensez à la Moria. Caradhras s'avérait infranchissable, la route du sud faisait se rapprocher la communauté trop près d'Isengard, mais ils devaient passer les Montagnes Brumeuses. Et même si Gandalf connaissait les dangers des profondeurs et les redoutait à juste titre, ils décidèrent de tenter leurs chances dans les grandes ténèbres. Dans le monde réel, la situation correspond au changement de bibliothèque graphique en milieu de projet ou au commencement d'une grosse réingénierie qui ne peut pas être facilement subdivisée. Ce n'est pas quelque chose que vous voulez faire, mais quelques fois, les alternatives semblent pires. Si l'équipe prends cette voie, tous les membres de l'équipe devraient être impliqués dans la décision, ainsi que le product owner et le scrum master. Après tout, la situation est à peu de choses près identique à celle de la "user story zéro" excepté qu'il y a une option de plus disponible à tout moment, c'est-à-dire quitter les souterrains et continuer la longue route du sud, en affrontant Sarouman Dans le monde réel, cela signifierait gérer les manques de votre vieille bibliothèque graphique et implémenter les éléments graphiques manquants manuellement. Notez qu'afin de conserver cette possibilité ouverte, l'exploration souterraine devrait toujours se faire sur une branche séparée, ce qui est une bonne idée de toute manière. L'option sortons-de-cet-enfer-maintenant devrait être évoquée à chaque réunion de planification de sprint tant que le groupe est sous terre.

Il y a une troisième raison d'aller dans les souterrains. C'est la chose affreuse qui pourrait arriver maintenant ou plus tard, c'est ce que l'on appelle les quêtes secondaires, et qui peuvent arriver intentionnellement ou accidentellement. Comment cela arrive t'il ? L'équipe pourrait affronter ses problèmes quotidiens ordinaires, disons une bande de gobelins dans une hutte. Alors qu'ils explorent la hutte, ils trouvent une geôle. Espérant un butin facile, ils fouillent la geôle, qui s'avère étonnamment grande. Dans la quatrième pièce, ils trouvent un tunnel. Et on ne sait comment, ils ratent le moment où ils auraient dû réaliser que cette chose est un putain de vaste souterrain et que le nettoyer complètement ne sera pas la même chose que d'affronter les gobelins. Notez la différence subtile entre gérer une rencontre (résoudre des problèmes et prendre les décisions habituelles pour les résoudre) et aller dans un souterrain. La première devrait être faite par l'équipe et ils n'ont pas besoin de consulter le product owner pour cela. La différence entre nettoyer une geôle et explorer un souterrain n'est pas simplement qualitative, c'est une question de savoir jusqu'où il faut aller dans les profondeurs et pendant combien de temps. Une règle au doigt mouillé, toute chose qui peut être réglée en un seul sprint n'est pas un souterrain mais une rencontre. Si aller dans le tunnel veut dire une story à zéro point pendant un sprint entier ou plus, c'est un souterrain.

Dans le monde réel du développement logiciel, la quête secondaire arrive généralement soit lorsque le refactoring nous échappe (vous le savez bien : un changement en amenant un autre) ou lorsqu'un membre de l'équipe veut tester une technologie et s'y retrouve alors piégé. Quoiqu'il en soit, la situation arrive dans une variété de cas, dans lesquels les aventuriers ne remarquent pas vraiment le danger qui les guette, ou lorsqu'ils le sentent, attirés par la curiosité, l'appel de l'aventure ou l'espoir d'un butin, ils continuent tout de même, ignorant les plaintes de l'oracle. D'une manière ou d'une autre, la solution est simple. Ils doivent quitter le souterrain tout de suite, sans discussion et sans regrets. Le scrum master pourrait les aider dans cette décision et les y forcer si nécessaire.

### Technologie suspecte = Marais

En plus des rencontres et des souterrains, il y a un autre type d'obstacle qui existe et que j'appelle le marais. Dans un monde médiévale-fantastique, nous savons de manière presque certaine ce que sont les marais, c'est-à-dire une capacité de mouvement réduite et des tonnes de rencontres, avec une forte probabilité de combats et de maigres combats. Donc les aventuriers doivent, dès que possible, faire un grand détour pour contourner le marais.

Dans le monde réel du développement logiciel, les marais sont ce que j'appelle la technologie suspecte. Cela peut être un ensemble d'exigences non fonctionnelles (haut-débit plus mobile) ou technologiques (Bluetooth plus Windows) ou même une approche algorithmique (peut être des algorithmes génétiques) qui sent les emmerdes.

L'oracle a un mauvais pressentiment parce qu'il est déjà allé dans le marais par le passé et a eu des mauvaises expériences ou qu'il connaît quelqu'un qui y est allé ou qu'il a lu quelque chose à ce propos. Aussi voudrait-il faire contourner le marais aux aventuriers sans qu'ils s'en rendent compte. Est-ce que cela est une bonne idée ? Non. Pour les mêmes raisons que les aventuriers ne devraient pas prendre la décision d'aller dans le souterrain tout seuls, l'oracle ne devrait pas décider de contourner le marais. Inévitablement, l'oracle sera sur le chemin de l'équipe qui essaient d'affronter les rencontres. Pire, contourner le marais implique changer constamment de direction, ce qui rendra l'équipe confuse et mènera à une défiance mutuelle. Donc, à la place d'essayer de contourner subrepticement le marais, il devrait partager l'information avec l'équipe qu'il suspecte la présence d'un marais. La décision de traverser ou de contourner devrait être prise ensemble. Après tout, peut être qu'un membre de l'équipe est un expert de la technologie Bluetooth et est convaincu qu'il pourra y guider l'équipe sans embûches. Si la décision est prise de contourner, le groupe sait au moins pourquoi ils tournent en ronds.

Bien évidemment, la même approche devra être prise si quelqu'un d'autre que l'oracle sent le marais. Seuls les membres de l'équipe sont généralement conscients qu'ils doivent partager cette information, alors que la tentation de prendre l'autre route à-l'insu-de-son-plein-gré est plus grande pour le product owner.

### La fin = le banquet final de la livraison

Ayant réussi à faire leur chemin parsemé de multiples dangers et de rencontres, à traverser les rivières et éviter les marais et les souterrains, le groupe a finalement atteint le château mystique dans les nuages. Ils apprécient de boire un verre à la taverne et d'obtenir beaucoup de points d'expériences (montée de niveau !). Seulement, au matin, ils se font réveillés par un nouvel oracle qui leurs parle d'un autre château, encore plus haut dans les nuages et encore plus beau. Mais c'est une autre livraison et une autre histoire qui devra être racontée une autre fois.

J'espère que vous avez aimé lire cette petite analogie entre le jeu de rôle papier et scrum, une analogie qui nous a conduit bien loin de manière surprenante.

---
Auteur : [Tim Dahmen](https://www.blogger.com/profile/06849271494105946136)  
Source : [A Dungeon Master Guide to Scrum](http://dungeonmasterguidetoscrum.blogspot.de/)  
Date de parution originale : 19 Novembre 2013  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 03 Juillet 2014  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) œuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

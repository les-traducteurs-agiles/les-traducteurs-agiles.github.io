---
layout: post
title:  "Éviter l'itération zéro"
date:   2011-11-19 00:01
published: true
tags:
- itération
- sprint
---

Les équipes nouvellement agiles réalisent souvent qu'elles ont beaucoup à faire avant d'avoir leur nouveau processus de développement à pleine vitesse. Examinant cette colline énorme et inconnue en face d'eux, beaucoup d'équipes agiles choisissent de faire une itération zéro (ou un sprint zéro) pour se préparer avant de commencer à livrer régulièrement des incréments de fonctionnalités. Pendant cette période, ils essaient de mettre tous les éléments en ordre de marche :

* Une liste de fonctionnalité à développer
* Un planning de livraison ou un calendrier pour ces fonctionnalités
* La mise en place de l'infrastructure de développement tel qu'un gestionnaire de configuration ou des serveurs d'intégration continue
* L’étude ou la pratique des compétences dans les nouvelles technologies qu'ils s'attendent à utiliser


... et autres efforts d'encadrement, d'infrastructures ou techniques.

Ils essayent d'avoir tous les travaux préliminaires en dehors du chemin afin qu'ils puissent démarrer à pleine vitesse à l'itération une. De par mon expérience, ils ne sont pas encore prêts à aller à pleine vitesse. Les choses sont rarement aussi finalisées que prévues après une itération, et souvent ne sont pas en phase avec les réels besoins du projet. La liste des fonctionnalités ne sera probablement pas complète, mais la tentative d’exhaustivité aboutira à un tas d’idées peu réfléchies. Nous n’avons pas assez de données sur la vitesse à laquelle les choses vont avancer pour se projeter dans l’avenir. L'infrastructure sera peut-être ou peut-être pas la meilleure pour supporter le projet, mais il y a de grandes chances que le projet se conforme à l'infrastructure plus que le contraire. Le choix des technologies sera fait de manière spéculative plutôt qu'en fonction des besoins du projet. Même si nous pouvons le faire de manière correcte, nous aurons pris beaucoup de décisions basées sur moins d'informations que nous en aurons durant le cycle de vie du projet.

Et nous aurons brûlé une itération sans produire aucun logiciel fonctionnel pour tester nos décisions.

Mon conseil est d'emprunter une idée du Lean et de regarder la situation d'un point de vue extérieur. Demandez-vous, "qu'est-ce-que cela changerait de commencer à livrer ?"

Le backlog initial a seulement besoin d'avoir un élément pour commencer à livrer. Si vous avez beaucoup trop d'inconnues, alors commencez juste avec un élément. Réunissez les parties prenantes du métier, les développeurs, les testeurs et toute personne ayant besoin d'être à la réunion (Utilisateurs expérimentés ? Exploitation/Support ?) pour en parler. (Je nomme cette réunion les [Trois Amigos](http://blog.gdinwiddie.com/2010/02/25/a-lingua-franca-between-the-three-or-more-amigos/)). Quelle est la chose évidente ayant besoin d'être faite ? (_Astuce : ce n'est pas "l'authentification". Commencez par l'objectif principal du système._) Je ne peux imaginer une situation où un projet soit commencé sans aucune idée.

Prenez cette seule chose et [coupez-la en fines tranches](http://blog.gdinwiddie.com/2011/05/01/splitting-user-stories/). Décidez des exemples représentant l'acceptation de ces tranches. Quelques tranches auront des questions auxquelles on ne pourra pas répondre. Mettez-les de côté pour le moment. Choisissez la tranche la plus centrale traversant de part en part, ou aussi près que possible du concept entier. Estimez-la pour une itération de l’équipe. (Les estimations n'ont pas à être "exactes". Ce sont juste des estimations.) Commencez à la construire.

Formez-vous à la technologie pendant que vous accomplissez le véritable travail. Apprenez les parties aidant à construire le système, plutôt que développer le système selon un quelconque framework. Quand vous ne savez pas comment accomplir quelque chose, ou que vous pensez à plusieurs approches qui pourraient fonctionner, faites des spikes minimalistes pour obtenir l'information nécessaire pour prendre une décision.

Au fur et à mesure, commencez lentement à construire votre infrastructure de développement. Mettez en place un dépôt local de code. Vous pourrez toujours migrer le code vers un dépôt "officiel d'entreprise" plus tard. Pour l'instant, il n'y a pas suffisamment de code. Faites un simple script de build-et-test, afin que chacun livre de la même manière. Vous pourrez toujours ajouter d'autres cibles de livraison plus tard. Si vous avez du temps, vous pouvez mettre en place un serveur d'Intégration Continue. Sinon, faites-le juste manuellement. Récupérez le code et livrez dans un espace de travail propre. Faites ce qui est nécessaire pour faire fonctionner le code afin que vous puissiez démontrer l’application.

Si vous ne pouvez réaliser cette tranche en une itération, c'est qu'elle n’est probablement pas assez fine. Ou, peut-être vous n'avez pas encore résolu un problème technique essentiel. Ou que l'objectif n'est pas encore assez clair. Déterminez quel obstacle entrave le plus votre chemin, résolvez-le et essayez encore.

Plus probablement, vous aurez fait cette tranche en moins d'une itération. Si vous avez fait cette tranche avant la fin de l'itération, alors tirez une autre tranche. Estimez-la pour "le reste de l'itération". Répétez autant que nécessaire. Dès que vous aurez réalisé une tranche, vous aurez un incrément du produit potentiellement livrable.

Oui, il y a encore de l'infrastructure de développement à développer. Inutile de se précipiter pour le faire. Continuez juste à l'améliorer, afin qu'elle vous aide à en réaliser plus. Oui, il y a encore des compétences techniques à développer. Cela devrait être toujours le cas. Continuez juste à expérimenter et repoussez vos limites.

Oui, il y aura des fonctionnalités à ajouter au backlog, à affiner, à ordonner, à découper en stories et ordonner à nouveau. Cela devrait continuer tout au long du projet. Cela fait partie du processus d' "avancement". Oui, il reste la nécessité de [projections](http://blog.gdinwiddie.com/2010/04/22/projecting-into-the-future/) afin d’estimer à quelle date la fonctionnalité sera disponible, ou combien de fonctionnalités peuvent être livrées pour une certaine date. Quand vous pensez que vous avez assez d'informations sur ce qui doit être fait, alors considérez le planning de livraison initial. Vous aurez aussi accumulé un peu d'information à propos de la vitesse à laquelle les choses sont faites.

Il y aura encore beaucoup de lacunes dans votre connaissance de ce qui est doit être fait et à quelle vitesse sont faites les choses. Ne croyez pas que votre planning de livraison soit "exact". Il s'agit juste d'une canne d’aveugle pour vous aider à juger comment vont les choses. Continuez à planifier, à sonder avec la canne autant que nécessaire. Et le temps passant, votre indication sur la vitesse à laquelle se développe le système s'améliorera. Même quand vous pensez que le planning de livraison est achevé, il a besoin d'être continuellement revu et ajusté. Étant donné qu'il n'est jamais fini avant la livraison, il n'y a pas d'urgence pour le définir à un niveau de finition élevé.

Ce type de démarrage est vraiment comme le “départ de la baie d'Hudson” que Johanna Rothman décrit dans son livre, [Manage It (pp. 52-53)](http://www.amazon.com/gp/product/0978739248/ref=as_li_ss_tl?ie=UTF8&tag=alberg30-20&linkCode=as2&camp=217145&creative=399349&creativeASIN=0978739248).

_L'approche “départ de la baie d'Hudson” provient de la Hudson Bay Company dans les années 1600-1700 dans le Nord-Est du Canada. La Hudson Bay Company équipait les négociants en fourrure. Pour être certain que les négociants n'oublient rien de ce dont ils avaient besoin, ils quittaient la baie d'Hudson et campaient quelques kilomètres plus loin. En campant quelques kilomètres plus loin, les négociants s'assuraient de n'oublier aucuns outils ou fournitures, avant d'abandonner la civilisation. Avec un bref démarrage dans leur voyage, ils avaient une meilleure idée de leur capacité à endurer l'hiver._

Il n'y a vraiment aucune raison (autre que "ce n'est pas la manière dont nous faisons les choses ici") que cela ne fonctionne pas au démarrage pour n'importe quelle équipe ou projet. C’est un bon moyen d’apprendre la manière de faire la plus adaptée à la situation courante tout en faisant un peu de progrès. J'utilise cette technique dans mon plan de transition [Agile en six mois](http://blog.gdinwiddie.com/2011/03/14/agile-in-6-months/).


---
Auteur : [George Dinwiddie](http://blog.gdinwiddie.com/about/)  
Source : [Avoid Iteration Zero](http://blog.gdinwiddie.com/2011/05/25/avoiding-iteration-zero/)  
Date de parution originale : 25 Mai 2011  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Relecteur : [Sylvain Fraïssé](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 19/11/2011  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

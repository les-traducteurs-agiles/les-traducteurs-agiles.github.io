---
layout: post
title:  "Comment cartographier les user stories de la mauvaise manière"
date:   2015-10-13 21:00:55
published: true
categories: 
- user-stories
- pratique
---

**Summary**:

When Lisa Crispin’s team got an opportunity to put the story mapping ideas she picked up from Jeff Patton into practice, they excitedly rushed into it and missed a few steps. Find out what happened, what didn't happen, and what they learned from it all.

Lorsque l'équipe de Lisa Crispin a eu l'opportunité de mettre en pratique l'idée de cartographie des user stories qu'elle avait emprunté de Jeff Patton, l'équipe s'est ruée dessus avec empressement et elle a raté quelques étapes. Vous allez découvrir ce qui s'est passé, ce qui ne s'est pas passé, et ce qu'elle en a appris.

During the past few years, I’ve participated in a couple of workshops and talks by Jeff Patton where I learned about [story mapping](http://www.agileproductdesign.com/blog/the new backlog.html). This is a hands-on way to model a theme or project and slice it into user stories. Jeff first wrote about it in a January 2005 Better Software article, “[How You Slice It.](http://www.stickyminds.com/articles/magfeature/its-all-how-you-slice-it)”

Lors de ces dernières années, j'ai participé à quelques ateliers et conférences de Jeff Patton où j'ai pu découvrir la [cartographie des user stories](http://www.agileproductdesign.com/blog/the new backlog.html). Il s'agit d'un outil prêt-à-l'emploi pour modéliser un thème ou un projet et le découper en user stories. La première fois où Jeff a écrit à ce sujet fut dans un article de _Better Software_ intitulé ["Tout est dans la manière dont vous le découpez"](https://dl.dropboxusercontent.com/u/50968566/Cartographie_user_stories/Tout_est_dans_la_mani%C3%A8re_dont_vous_d%C3%A9coupez.pdf).

What I learned from Jeff is to start by gathering your development team and business stakeholders. Create personas to represent your various types and roles of users, then think about how each persona would use your system or feature. What would they do first? What would they do next? Make a timeline of user activities using index cards on a wall, a table, or a floor. Then, go back and look at each user activity in detail and create user tasks and details about those tasks, which will eventually become user stories. Write those on cards, too, and stack them vertically under the corresponding user activity.

De ce que j'ai appris de Jeff, il faut commencer par rassembler votre équipe de développement et vos parties prenantes. Créer ensuite des personas pour représenter vos différents types et rôles des utilisateurs, puis penser à comment chaque persona devrait utiliser votre système ou votre fonctionnalité. Qu'est-ce qu'ils feraient d'abord ? Qu'est-ce qu'ils feraient ensuite ? Faire une frise temporelle des activités utilisateurs sur un mur, une table ou sur le sol. Puis, prendre du recul et examiner chaque tâche utilisateur en détail et créer les tâches utilisateur et les détails concernant ces tâches, qui deviendront éventuellement des user stories. Ecrire celles-ci sur des cartes aussi, et les empiler verticalement en-dessous l'activité utilisateur correspondante.

Once the story map is in place, you can slice them into user stories and plan which ones go into each iteration and release. You should walk the story map with stakeholders and see if you can think of any other details or issues. The story map helps you think about the value the system delivers.

Une fois que la cartographie des user stories est en place, vous pouvez la découper en user stories et planifier lesquelles iront dans chaque itération et version. Vous devriez parcourir la cartographie des user stories avec les parties prenantes et voir si vous pouvez pensez à d'autres détails ou à d'autres problèmes. La cartographie de story vous aide à réfléchir sur la valeur que le système délivre.

**Eager to Try It**
Like most teams I know, our team struggles with getting the right level of detail on requirements for each user story before we start testing and coding. We don’t want big design up front, but we don’t want to waste a bunch of time going back and forth to the product owner and other business experts to nail down specifications during development. Brainstorming techniques such as mind mapping have helped us, but we still feel we lose too much time with requirements churn.

**Excités d'essayer**
Comme la plupart des équipes que je connais, notre équipe se débat pour obtenir le bon niveau de détails sur les exigences de chaque user story avant que de commencer à tester et à coder. Nous ne voulons pas faire de conception préalable, mais nous ne voulons pas perdre du temps à faire du va-et-vient avec le _product owner_ et les autres experts métiers pour fixer `nail down`les spécifications pendant le développement. Des techniques de remues-méninges telles que les cartes heuristiques nous y ont aidé, mais nous avons  toujours le sentiment que nous perdons trop de temps avec la génération `churn`des exigences.

I’ve been agitating for some time to try story mapping and see if it might help us flesh out details about a theme and its user stories in advance of coding. I was pleased one recent afternoon when our ScrumMaster told me, “We want to story map the ‘We Help You Choose’ theme tomorrow.”

J'avais envie depuis quelques temps d'essayer la cartographie des user stories et voir si elle pouvait nous aider à matérialiser les détails d'un thème et ses user stories en avance par rapport au développement. J'étais donc contente lorsqu'un après-midi notre _ScrumMaster_ vint me dire : "Nous voulons essayer la cartographie de user stories pour le thème de demain 'Nous vous aidons à choisir'."

I was thrilled to finally get my wish, but I was also swamped. I was leaving for Agile Testing Days in Potsdam in a couple days, and we were in the middle of a difficult and busy sprint. I didn’t have time to go back and study up on exactly how to do story mapping. I thought I could wing it. (Cue shark attack music.)

J'étais ravi que finalement mon voeu soit exaucé, mais j'étais aussi embêtée. Je devais partir pour les Agile Testing Days [^1] à Postdam dans quelques jours, et nous étions en plein milieu d'un sprint difficile et bien rempli. Je n'avais pas le temps pour revenir et étudier attentivement comment faire précisément une cartographie de stories. Je pensais que je pourrais survoler. (on entend alors une musique d'attaque de requins bien connue).

[^1]: conférénce dédiée aux tests logiciels en approche agile

One thing I understood about story mapping is that all stakeholders need to participate. We’re often missing important stakeholders in our brainstorming and estimating meetings, so I insisted that all stakeholders for this theme must be present for our story mapping session. In this case, that was only one person, but many themes we do involve multiple stakeholders.

La chose que j'avais compris à propos de la cartographie des user stories était que toutes les parties prenantes doivent participer. Souvent, il nous manquait des parties prenantes essentielles dans nos réunions d'estimations et de remues-méninges, aussi ai-je insisté pour que toutes les parties prenantes de ce thème soient présentes pour notre session de cartographie des user stories. Dans ce cas, il s'agissait d'une seule personne, mais beaucoup des thèmes que nous nous occupons impliquent de plusieurs parties prenantes.

**Doing It Wrong**
We gathered in our conference room with index-card-sized sticky notes, Sharpies, and a rolling whiteboard. Here’s a little context about our domain: Our application automates all aspects of selling, creating, and managing 401(k) retirement plans. The “We Help You Choose” theme that we were planning revolves around a third-party vendor that helps 401(k) participants decide how to invest their retirement funds. If an employer providing a 401(k) plan to its employees wants to offer this service, the employer has to pay extra.

**Mal le faire**
Nous nous sommes rassemblés dans notre salle de conférence avec des grandes notes adhésives, des `sharpies`, et un tableau blanc. Voici quelques informations pour comprendre le contexte de notre domaine : notre application automatise tous les aspects de la vente, de la création et de la gestion de plans de retraites `401(k)`. Le thème "Nous vous aidons à choisir" que nous devions planifier reposait sur un vendeur tiers aidant les participants `401(k)` à décider comment investir les fonds de pensions. Si un employeur procurant un plan `401(k)` à ses employés voulait offrir ce service, cet employeur devait payer un extra.

We had ten people in the room. The first thing I forgot is that you should divide into small groups of three to five people and have each group map the theme. Uh oh.

Nous étions dix personnes dans la pièce. La première chose que j'ai oublié a été que j'aurais dû les répartir en petits groupes de trois à cinq personnes et que chaque groupe cartographie le thème. Oh oh.

I started by asking our business experts about the personas for the theme. Who would be using it? The answer was the sales representative. Unfortunately, our stakeholders knew almost nothing about these sales reps, so we couldn’t really flesh out the personalities of this persona. This was not a good start! All we could do was call him “Sammy Sales Rep” and say he was interested only in making the sale.

J'ai commencé par poser des questions à nos experts métiers au sujet des personas pour le thème. Qui devrait l'utiliser ? La réponse fût les commerciaux. Malheureusement, nos parties prenantes ne connaissaient quasiment rien au sujet des commerciaux, donc nous ne pourrions pas vraiment incarnés les personnalités dans ce persona. Ce n'était pas un bon début ! Tous ce que nous pourrions faire serait de l'appeler "Sammy le commercial" et dire qu'il était intéressé seulement par réaliser une vente.

Next, I asked everyone to get up and grab a permanent marker and some sticky notes and start timelining the user tasks for this theme. What would Sammy Sales Rep do first? What would he do next? We knew the theme revolved around establishing a new 401(k) plan, so we would organize the user tasks around that.

Ensuite, j'ai demandé à chacun de se lever, de prendre un marqueur et quelques notes adhésives et de commencer à mettre des tâches utilisateurs sur une frise temporelle pour ce thème. Qu'est-ce que Sammy le commercial ferait d'abord ? Qu'est-ce qu'il ferait ensuite ? Nous savions que le thème tournait autour de la mise en place d'un nouveau plan `401(k)`, et donc que nous devrions organiser les tâches utilisateurs autour de cela.

Nobody got out of their chair. If only I had remembered about dividing into smaller groups! I repeated my request more assertively. The ScrumMaster got up and came to join me. Nobody else moved. In hindsight, I should have switched from doing the story map on the rolling whiteboard to doing it on the conference table, but I didn’t think of that.

Personne ne s'est levé de sa chaise. Si seulement j'avais pu me rappeler de la répartition en petits groupes ! J'ai répété ma requête de manière plus assertive. Le _ScrumMaster_ s'est levé et est venu se joindre à moi. Personne d'autre ne s'est levé. Après coup, je pense que j'aurais dû faire la cartographie des stories sur la table de conférence à la place de la faire sur le tableau, mais sur le moment je n'y ai pas pensé. 

Giving up on getting people to physically move, I asked, “What’s the first thing Sammy Sales Rep would do?” He’s going to create a 401(k) plan for an employer. This is a multi-step wizard, so the timeline seemed fairly obvious. I wrote “Step 1” on a sticky note and put it on the rolling whiteboard. The sales rep would enter company information, then select contribution options for the plan, then select mutual funds or the “Help Me Choose” options, and so on.

Ayant abandonné le fait que les personnes se déplacent physiquement, j'ai posé la question, "Quelle est la première chose que Sammy le commercial ferait ?". Il va créer un plan `401(k)` pour un employeur. C'était un appât à tiroir, afin que la frise temporelle paraisse assez évidente. J'ai écris "Étape 1" sur une note adhésive et je l'ai mise sur le tableau blanc. Le commercial saisirait les informations concernant l'entreprise, puis sélectionnerait les options de contributions pour le plan, puis sélectionnerait les fonds mutualisés ou les options "Aidez-moi à choisir", et ainsi de suite.

Once we had this timeline of tasks, we went back and drilled into the details. What would change with each step compared with what sales reps do currently when they create a 401(k) plan? We noted the details needed for each UI page and some technical implementation requirements.

Une fois que nous avons eu la frise temporelle pour ces tâches, nous avons pris du recul et nous sommes entrés dans les détails. Qu'est-ce qui changerait à chaque étape par rapport à ce que font aujourd'hui les commerciaux lorsqu'ils créent un plan `401(k)`. Nous avons noté alors les détails nécessaires pour chaque page d'IHM ainsi que quelques exigences pour l'implémentation.

Unfortunately, we had started off at too detailed a level. We first should have identified “user activities”—the high-level things users do to achieve a particular goal. Establishing a 401(k) plan is an activity of the sales rep user. Managing the fund lineups is a user activity. We started with “user tasks”—specific steps within a user activity. “Select a fund lineup” is a user task within the activity of establishing a 401(k) plan.

Malheureusement, nous avions commencé à un niveau trop détaillé. D'abord, nous aurions dû identifier les "activités utilisateurs" - les éléments haut niveau que font les utilisateurs pour accomplir un objectif donné. Établir un plan `401(k)` est une activité de l'utilisateur Commercial. Gérer le regroupement des fonds est une activité utilisateur. Nous avons commencé avec les étapes spécifiques des "tâches utilisateurs" existantes au sein d'une activité utilisateur. "Sélectionner un regroupement de fonds" est une tâche utilisateur au sein de l'activité d'établir un plan `401(k)`.

Nevertheless, we got through a timeline of what Sammy Sales Rep would do. We also thought of the need for a user interface to manage the “We Help You Choose” program as well as a report. We also wrote stickies for a system to manage the “mutual fund lineups” that would be offered and for some reports to track which 401(k) plans have chosen a “fund lineup.” We included many details about each step of the timeline, both from a user perspective and a technical-implementation perspective.

Malgré tout, nous avons parcouru la frise temporelle de ce que Sammy le commercial ferait. Nous avons aussi pensé au besoin pour l'interface utilisateur de pouvoir gérer le programme "Nous vous aidons à choisir" ainsi qu'à un rapport de synthèse. Nous avons aussi écrit des notes adhésives pour le système de gestion du "regroupement des fonds mutualisés" qui serait offert et pour les quelques rapports permettant le suivi des plans `401(k)` ayant choisis un "regroupement des fonds". Nous avons incorporé beaucoup d'éléments détaillés sur chaque étape de la frise temporelle, à la fois d'une perspective utilisateur et d'une perspective d'implémentation technique.  

I also forgot that we should have walked through the story map with the stakeholders. This serves as a way of testing the map and finding additional details. Of course, now that we had the map, we could do that later.

J'ai aussi oublié que nous aurions dû parcourir la cartographie des stories avec les parties prenantes. C'est une manière de tester la carte et de trouver des détails supplémentaires. Bien sûr, maintenant que nous avions la cartographie, nous pourrions le faire plus tard.

**What Did We Get out of It?**
By the end of the meeting, I knew I had made several mistakes around the story mapping. I apologized to the team, threw my hands up in a “failure bow,” and said, “How fascinating!” I asked them to applaud my failure. I hoped we would still learn something.

**Qu'est-ce que nous avons fait pour nous sortir de là ?**
Vers la fin de la réunion, j'ai su que j'avais fait plusieurs erreurs sur la cartographies des user stories. J'ai présenté mes excuses à l'équipe, j'ai levé mes mains en faisant la forme d'un arc cassé `"failure bow"`, et j'ai dit : "Comme c'est fascinant !". Je leur ai demandé d'applaudir à mon échec. J'ai espéré que aurions encore quelque chose à apprendre.

When the meeting concluded, I looked back at my notes on story mapping and found what I’d missed. I went back to the rolling whiteboard and added sticky notes for the missing “user activities” row. (We had implied user activities, but we hadn’t specified them on the whiteboard.) I color-coded some of the details under each user task to reflect which were technical implementations, which were outstanding questions, and which were known tasks. Now, it looked more like a story map (see figure 1).

Lorsque la réunion a pris fin, je suis revenu sur mes notes à propos de la cartographie des user stories et j'ai trouvé ce que j'avais raté. Je suis revenu vers le tableau blanc et j'ai ajouté les notes adhésives pour la ligne "activité utilisateur" manquante. (Nous avions des activités utilisateur implicites, mais nous ne les avions pas spécifié sur le tableau blanc). J'ai colorié certains détails selon un code couleur en dessous de chaque tâche utilisateur pour indiquer lesquelles étaient des implémentations techniques, lesquelles étaient des questions importantes, et lesquelles étaient des tâches connues. Et maintenant, cela ressemblait plus à une cartographie de stories (voir figure 1).

![story mapping](http://www.stickyminds.com/sites/default/files/article/2012/Crispin Lisa Story Mapping 01.jpg)

I talked with my teammates to get their feedback on our somewhat misguided “stry mapping” attempt. Since they didn’t know how story mapping was supposed to work either, they were OK with it. They felt that we had flushed out some details about stories in the theme that otherwise may not have come out until we started coding.

J'ai demandé à mes co-équipiers leur feedback sur notre tentative de "cartographie des user stories" quelque peu raté. Étant donné que nous ne savions pas comment la cartographie des user stories était censé fonctionner, ils étaient OK avec ça. Ils avaient ressenti que nous avions mis en lumière certains détails sur les stories de ce thème que nous n'aurions pas pu voir autrement qu'au moment de coder.

One programmer observed that he thought the story mapping was valuable because the stakeholder (I’ll call him “Z”) was at the meeting. Often, we only have the product owner to represent the stakeholders. Z turned out to be more receptive to simpler solutions than our product owner, and since he was the actual stakeholder, he got to make decisions. We got more information just from having Z participate in the meeting.

Un programmeur a fait remarquer qu'il pensait que la cartographie des stories avait de la valeur car la partie prenante (je l'appellerai "Z") était présente à la réunion. Le plus souvent, nous avions seulement le product owner pour représenter les parties prenantes.  Z s'avéra plus réceptif à des solutions plus simples que notre product owner, et étant donné qu'elle était la véritable partie prenante, elle se devait de prendre les décisions. Nous avons donc eu plus d'informations par la seule présence de Z à la réunion.

**Next Time**
We started working on the user stories for this theme in the very next sprint. We felt we were starting with a better shared understanding than we sometimes do for a new theme. We had sliced the theme into appropriately-sized user stories and understood the dependencies between them. However, confusion about part of the model for the underlying relationships cropped up that caused hours of wasted time and discussion. This is just what we were trying to avoid with story mapping, but it still occurred. That was frustrating.

**La prochaine fois**
Nous avons commencé à travailler sur les user stories de ce thème le sprint d'après. Nous avons ressenti que nous commencions avec une meilleure compréhension commune que nous le faisons certaines fois pour un nouveau thème. Nous avons découpé le thème en user stories de taille appropriée et nous avons compris leurs dépendances. Toutefois, une certaine confusion sur une partie du modèle concernant des relations implicites est survenu qui a provoqué plusieurs heures en perte en temps et en discussion.  C'est justement ce que nous avions tenter d'éviter avec la cartographie des stories, et cela arrivait encore. C'était très frustrant.

In spite of still having some “requirements churn,” my teammates feel that story mapping is worth trying again. They think it has potential as a brainstorming technique. Next time, we’ll divide into two smaller groups, each will produce a map, and then we’ll consolidate. We’ll know to start with user activities and then drill down into user tasks and details. We’ll try mapping on the conference table, so I’m not the only one writing down the user activities, tasks, and details.

En dépit d'avoir encore quelques `churn` "petits bouts d'exigences", mes co-équipiers sentent que la cartographie des stories vaut le coup de l'essayer. Ils pensent qu'elle a autant de potentiel qu'une technique de _brainstorming_. La prochaine fois, nous nous répartirons en deux petits groupes, chacun produisant une carte, que nous consoliderons ensuite. Nous saurons commencer par les activités utilisateurs et ensuite les approfondir en tâches utilisateurs et en détails. Nous essayerons la cartographie sur la table de conférence, afin que je ne sois pas la seule personne à écrire les activités, tâches et détails utilisateurs.

Even failures help us learn. I’m glad that I saw my mistakes and acknowledged them instead of getting discouraged. We improve by trying experiments, and the team is willing to continue this one. I’ll keep you posted!

Même les échecs nous permettent d'apprendre, je suis heureuse d'avoir vu mes erreurs et de les avoir reconnues plutôt que de m'être découragée. Nous nous améliorons en essayant des expériences, et l'équipe est d'accord pour continuer dessus. Je vous tiendrai au courant !

About the author
Lisa Crispin's picture
Lisa Crispin

À propos de l'auteur
![Photo de Lisa Crispin]()
Lisa Crispin

Lisa Crispin is co-author of Agile Testing: A Practical Guide for Testers and Agile Teams and Extreme Testing and a contributor to Beautiful Testing. Lisa has worked as a tester on agile teams for the past ten years and enjoys sharing her experiences via writing, presenting, teaching, and participating in agile testing communities around the world. Visit www.lisacrispin.com.

Lisa Crispin est la co-auteure d'_Agile Testing: A Practical Guide for Testers and Agile Teams and Extreme Testing_ et une contributrice à _Beautiful Testing_. Ces dix dernières années, Lisa a travaillé en tant que testeur dans des équipes agiles et est heureuse de partager ses expériences à travers l'écriture, la présentation, l'enseignement, et la participation à des communautés agiles autour du globe.
Consultez www.lisacrispin.com  

---  
Auteur : [Lisa Crispin](http://lisacrispin.com/about/)  
Source : [Story Mapping The Wrong Way](http://www.stickyminds.com/article/story-mapping-wrong-way?page=0%2C2)  
Date de parution originale : 12 Décembre 2011  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 13/10/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share buttons.html %}



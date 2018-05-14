---
layout: post
title:  "Indicateurs Scrum"
date:   2017-10-24 00:01
published: true
tags: 
- scrum
- scrum master
- indicateurs
---

Il y a des tas d'indicateurs qui pourraient être collectés pour évaluer les compétences, le succès, l'ingéniosité, la qualité et la quantité de travail d'une équipe de développement logiciel. Si vous souhaitez vous faire une idée des indicateurs à collecter, jetez un coup d'oeil aux 185 pratiques du [CMMI pour le Développement](https://www.sei.cmu.edu/cmmi/index.cfm). L'Agilité, au contraire de CMMI, n'a pas besoin de "preuve" sur le fait que les pratiques d'ingénierie sont appliquées et ne dispose, par conséquent, que de peu d'indicateurs qu'une Equipe de Développement pourrait collecter pour mesurer le succès de chaque sprint. Ci-dessous, on a 9 indicateurs qu'une Equipe Scrum pourrait envisager d'utiliser :

1. Stories finies vs Stories engagées
2. Gestion de la Dette Technique
3. Vélocité de l'Equipe
4. Qualité Livrée au Client
5. Enthousiasme de l'Equipe
6. Amélioration du Processus de Rétrospective
7. Communication dans l'Equipe Scrum
8. Adhésion de l'Equipe Scrum aux Règles Scrum et aux Pratiques d'Ingénierie
9. Compréhension par l'Equipe Scrum du Périmètre et de l'Objectif du Sprint.

Pour répondre à la question de savoir qui devrait collecter ces indicateurs et mesurer le succès de l'Equipe Scrum, envisageons qui dans Scrum est responsable du succès de l'équipe. Lors de la description du rôle du ScrumMaster, le Guide Scrum énonce que : "Le ScrumMaster forme l'Equipe Scrum en la coachant et en la guidant pour être plus productive et pour produire des produits de plus grande qualité." C'est clairement la responsabilité du ScrumMaster de mesurer le succès de l'équipe, ne serait-ce que pour augmenter la productivité de l'équipe et la qualité du produit. Le ScrumMaster peut utiliser un radar, comme illustré ci-dessous, pour suivre l'Equipe Scrum.

![Indicateurs du Sprint de l’Équipe Scrum]({{ site.url }}assets/fabrice_aimetti/Scrum-Team-Metrics_fr.png)

Utiliser un radar est un moyen facile pour le ScrumMaster de suivre et comparer les résultats de sprint en sprint.

Vous trouverez ci-dessous la description courte de chaque indicateur, la façon dont il peut être mesuré, et quelques problèmes qui pourraient générer un faible score. Tout indicateur supplémentaire ou commentaires sur ces 9 indicateurs sont les bienvenus.

## 1. Stories finies vs Stories engagées

Cet indicateur est utilisé pour mesurer la capacité de l'équipe de développement à connaître et comprendre ses compétences. La mesure est faite en comparant le nombre de stories engagées lors de la planification du sprint au nombre de stories identifiées comme terminées lors de la revue de sprint. Un score faible peut découler de l'un des points suivants qui méritent toute votre attention :

* L'Equipe n'a pas de story de référence pour faire ses estimations relatives (voir Vélocité de l'équipe),
* Les membres de l'Equipe ne comprennent pas tous la story de référence (voir Vélocité de l'Equipe),
* Le Product Owner ne fournit pas assez d'informations à l'équipe de développement (voir Communication de l'Equipe, Compréhension par l'Equipe Scrum du Périmètre et de l'Objectif du Sprint),
* Le périmètre des exigences a dérivé (voir Compréhension par l'Equipe Scrum du Périmètre et de l'Objectif du Sprint),
* L'Equipe a été perturbée (voir Adhésion de de l'Equipe Scrum aux Règles Scrum & aux Pratiques d'Ingénierie, Enthousiasme de l'Equipe).


Même si l'Equipe termine les stories sur lesquelles elle s'est engagée, il y a certaines choses que le ScrumMaster pourrait regarder :

* L'Equipe a baissé son niveau d'engagement et a travaillé à un rythme plus faible que le rythme normal (voir Vélocité de l'Equipe),
* L'Equipe a un ou plusieurs "héros" (voir Enthousiasme de l'Equipe),
* L'engagement sur les stories a été respecté mais le produit est "buggé" (voir Gestion de la Dette Technique, Qualité Livrée au Client).


## 2. Gestion de la Dette Technique

Cet indicateur mesure l'endettement technique global de l'équipe ; les problèmes connus à la fin du sprint. On compte généralement les bugs mais aussi les livrables tels que le matériel de formation, la documentation utilisateur, le support de livraison, etc. Un score faible peut découler de l'un des points suivants qui méritent toute votre attention :

* Le Client n'est pas pris en compte pendant le sprint (voir Qualité Livrée au Client).
* Faible voire aucune "Définition du Fini" incluant l'introduction de zéro bug (voir l'Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie).
* Le Management perturbe l'Equipe en la forçant à livrer avant que l'Equipe soit prête (voir l'Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie).
* L'Equipe travaille sur de multiples stories, ce qui compromet la qualité et le fait de finir les stories au fur et à mesure que la fin du sprint approche (voir l'Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie).
* L'Equipe crée des bugs qui reflètent ses avis sur la façon dont les choses devraient fonctionner plutôt que d'écouter le Client (voir Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie, Qualité Livrée au Client).


Même si la dette technique n'augmente pas, il y a certaines choses que le ScrumMaster pourrait regarder :

* L'Equipe ne documente pas les problèmes trouvés ou corrigés (voir Communication dans l'Equipe, l'Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie).
* L'Equipe n'implique pas le Client/Product Owner pendant les tests d'acceptation (voir Communication dans l'Equipe, l'Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie).


## 3. Vélocité de l'Equipe

L'indicateur de vélocité mesure la cohérence des estimations de l'équipe de sprint en sprint. L'estimation des stories est menée de façon relative avec les autres stories, en utilisant généralement les points de story. La mesure est faite en comparant les points de story finis dans le sprint avec les points finis dans le sprint précédent à +/- 10% (le [Test Nokia](http://ayeba.wikispaces.com/Nokia%20Test) utilise +/- 10%). Un score faible peut découler de l'un des points suivants qui méritent toute votre attention :

* Le Product Owner ne fournit pas assez d'informations à l'équipe de développement (voir Communication dans l'Equipe, Compréhension par l'Equipe Scrum du Périmètre et de l'Objectif du Sprint).
* La taille de l'Equipe change entre les sprints (généralement, le noyau de l'équipe reste cohérent ; des exceptions peuvent être faites pour les absences, comme les vacances et la maladie).
* L'Equipe ne comprend pas le périmètre du travail au démarrage du sprint (voir Compréhension par l'Equipe Scrum du Périmètre et de l'Objectif du Sprint, Communication dans l'Equipe, Stories finies vs Stories engagées).
* L'Equipe est perturbée (voir l'Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie).
* Les stories de référence de l'Equipe ne sont pas applicables à la version courante (voir Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie).
* L'Equipe réalise des versions courtes (< 3 sprints) ou un travail de maintenance (l'Equipe pourrait regarder du côté de Kanban ou de XP au lieu de Scrum dans ces circonstances).


Même si l'Equipe semble avoir une vélocité cohérente, il y a certaines choses que le ScrumMaster pourrait regarder :

* Un niveau d'engagement bas de l'Equipe et un travail à un rythme plus lent que le rythme "normal" (voir Stories finies vs Stories engagées).
* L'Equipe a un ou plusieurs "héros" (voir Enthousiasme de l'Equipe).
* La vélocité est cohérente mais le produit est "buggé" (voir Gestion de la Dette Technique, Qualité Livrée au Client).


## 4. Qualité Livrée au Client

Dans la plupart des entreprises, votre seule raison d'être est de livrer un produit de qualité au client et de maintenir le client heureux. Scrum essaye que le résultat de chaque sprint apporte de la avleur au client, c'est-à-dire un "incrément de produit potentiellement déployable". Ce n'est pas nécessairement un produit livré mais un produit qui peut être montré aux clients en tant que version de travail, pour solliciter les commentaires, avis et suggestions des clients, autrement dit, sommes-nous en train de construire un produit dont le client a besoin. Ceci peut être encore mieux mesuré en interrogeant les clients et les parties prenantes. Ci-dessous un radar concernant l'enquête de satisfaction menée à l'issue de la Revue de Sprint :

![Enquête de Satisfaction du Client suite à la Revue de Sprint]({{ site.url }}assets/fabrice_aimetti/Customer-Satisfaction-Survey-Sprint-Review_fr.png)

Le ScrumMaster peut documenter tous les avis des clients et parties prenantes en utilisant un radar facile à lire.

Un faible score peut découler de l'un des points suivants qui méritent toute votre attention :

* Le Product Owner ne comprend pas réellement ce que le client veut ou ce dont le client a besoin (voir Communication dans l'Equipe).
* Le Product owner ne communique pas adéquatement les besoins du client à l'équipe de développement (voir Communication dans l'Equipe, Compréhension par l'Equipe Scrum du Périmètre et de l'Objectif du Sprint).
* Les clients ne sont pas impliqués dans le développement des stories (voir Communication dans l'Equipe).
* Le Client n'est pas impliqué dans la définition des critères d'acceptation des stories (voir Communication dans l'Equipe).
* Des bugs sont livrés avec le produit (voir Gestion de la Dette Technique).


Même si le client est satisfait avec le produit du sprint, il reste certaines choses que le ScrumMaster peut regarder :

* Le produit est "buggé" (voir Gestion de la Dette Technique).
* Les clients et parties prenantes ne sont pas tous invités, représentés, ou ne participent pas à la revue de sprint (voir Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie, Communication dans l'Equipe).


## 5. Enthousiasme de l'Equipe

L'enthousiasme est une composante majeure d'une Equipe Scrum qui réussit. Si elle en manque, aucun processus ou méthodologie n'apportera d'aide. Il existe de nombreux signaux avant-coureurs qui, non interprétés, peuvent conduire à une perte d'enthousiasme. C'est au ScrumMaster de reconnaître ces symptômes et de prendre des actions appropriées pour chaque circonstance particulière, puisque le ScrumMaster a pour objectif de maintenir l'Equipe productive et heureuse. Mesurer l'enthousiasme de l'équipe peut être très subjectif et il est préférable de l'observer lors des différentes réunions du sprint : planification, revue et mêlée. Pourtant, l'approche la plus simple est de poser directement la question à l'Equipe Scrum : "Etes-vous heureux ?" et "Quelle est votre niveau de motivation ?". Un faible score peut découler de l'un des points suivants qui méritent toute votre attention :

* Le ScrumMaster prend trop de temps pour supprimer les obstacles.
* Le nombre d'obstacles pendant le sprint est trop élevé.
* L'équipe est perturbée par les managers ou le Product owner (voir Stories finies vs Stories engagées).
* Certains membres de l'équipe ne peuvent pas contribuer à certaines parties du produit, autrement dit, c'est un manque de formation à la pluridisciplinarité.
* Les membres de l'équipe travaillent trop longtemps, donc ne travaillent pas selon un rythme soutenable (voir Stories finies vs Stories engagées).
* Des conflits internes émergent entre le Product Owner et l'Equipe.
* Des conflits internes émergent entre les membres de l'Equipe.
* L'Equipe répète les mêmes erreurs (voir Amélioration du Processus de la Rétrospective).
* L'Equipe grogne, se plaint ou se chamaille continuellement.
* Les membres de l'Equipe ne se passionnent pas pour leur travail
* L'Equipe ne fait preuve ni de créativité ni d'innovation.


## 6. Amélioration du Processus de Rétrospective

L'indicateur d'Amélioration du Processus de la Rétrospective mesure la capacité de l'Equipe Scrum à réviser, au sein des pratiques et du framework Scrum, son processus de développement pour le rendre plus efficace et agréable dans le prochain sprint. Le Guide Scrum mentionne que "Le but de la Rétrospective [du Sprint] est d'examiner le déroulement du dernier Sprint d'un point de vue individus, relations, processus et outils. Cet examen doit identifier et prioriser les éléments majeurs qui fonctionnent correctement et les éléments qui, réalisés différemment, pourraient améliorer les choses. Cela inclut la composition de l'Equipe Scrum, l'organisation des réunions, les outils, la définition du "fini", les méthodes de communication et les processus de transformation des éléments du Backlog Produit en quelque chose de fini". Ceci peut être mesuré en utilisant le nombre d'éléments identifiés lors de la rétrospective, le nombre d'éléments de la rétrospective sur lesquelles l'Equipes s'est engagé dans le sprint, et le nombre d'éléments gérés/résolus à la fin du sprint. Un faible score peut découler de l'un des points suivants :

* L'Equipe n'identifie pas d'éléments d'amélioration car elle a l'impression qu'elle ne peut rien faire ou que c'est hors de son contrôle, autrement dit l'Equipe ne s'auto-organise et ne s'auto-gère pas.
* Pendant le sprint, le Product Owner, le ScrumMaster ou le Management découragent tout travail d'amélioration au dépend des stories.
* Pendant le sprint, l'Equipe décourage tout travail d'amélioration au dépend des stories.
* L'Equipe ne fait pas la démarche interne de regarder sa propre performance et son propre environnement pendant la rétrospective.
* L'Equipe ne reconnaît pas ou ne traite pas les erreurs récurrentes (voir Enthousiasme de l'Equipe).


## 7. Communication dans l'Equipe Scrum

L'indicateur de Communication est une mesure subjective de la façon dont l'Equipe, le Product Owner, le ScrumMaster, les Clients et les Parties prenantes ont des communications ouvertes et honnêtes. Le ScrumMaster, lorsqu'il observe et écoute l'Equipe, le Product Owner, les Clients et les autres Parties Prenantes pendant le sprint, aura des indications et des indices sur la façon dont chacun communique. Un faible score peut découler de l'un des points suivants :

* Le Client n'est pas activement impliqué dans le développement des stories (voir Qualité Livrée au Client).
* Le Client ne fournit pas de critères d'acceptation pour les stories (voir Qualité Livrée au Client, Gestion de la Dette Technique).
* L'Equipe ne fournit pas de tests d'acceptation au Client pour la revue et les commentaires (voir Qualité Livrée au Client, Gestion de la Dette Technique).
* L'Equipe et le Client n'exécutent pas les tests d'acceptation ensemble (voir Qualité Livrée au Client, Gestion de la Dette Technique).
* Le(s) Client(s) et les autres Parties Prenantes ne sont pas invités/présents à la Revue de Sprint (voir Qualité Livrée au Client).
* Le ScrumMaster ne garantit pas que les Clients soient interrogés après chaque Revue de Sprint (voir Qualité Livrée au Client).
* Le Product Owner n'est pas disponible en cours de journée pour collaborer avec l'Equipe Scrum (voir Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie).
* Les stories du Product Owner ne concernent pas des fonctionnalités d'un point de vue Client (voir Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie, Qualité Livrée au Client).
* Le Product Owner ne fournit pas d'information sur les "douleurs" ou les "besoins" du Client à l'Equipe (voir Stories finies vs Stories engagées).
* L'Equipe ne documente pas les problèmes trouvés ou corrigés (voir Gestion de la Dette Technique).
* Le Product Owner ne comprend pas réellement ce que le client veut ou dont il a besoin (voir Qualité Livrée au Client).
* Le Product Owner ne communique pas de façon adéquate les besoins du client à l'équipe de développement (voir Qualité Livrée au Client, Stories finies vs Stories engagées).
* L'Equipe ne mène pas les mêlées quotidiennes (voir l'Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie).
* L'Equipe Scrum ne mène pas de planification de la version (voir l'Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie).
* L'Equipe Scrum ne mène pas de planification du sprint (voir Adhésion de l'Equipe Scrum aux Règles Scrum et Pratiques d'Ingénierie),
* L'Equipe Scrum ne mène pas de Revue de Sprint (voir l'Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie),
* L'Equipe Scrum ne mène pas de Rétrospective (voir l'Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie).
* L'Equipe Scrum n'affiche pas de façon visible le burndown de la version (voir l'Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie).
* L'Equipe Scrum n'affiche pas de façon visible le burndown du sprint (voir l'Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie).
* L'Equipe Scrum n'affiche pas de façon visible les stories et les critères d'acceptation (voir l'Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiqes d'Ingénierie).
* L'Equipe Scrum n'affiche pas de façon visible les exigences non fonctionnelles qui s'appliquent au sprint entier ou à la version entière (voir l'Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie).


## 8. Adhésion de l'Equipe Scrum aux Règles Scrum & Pratiques d'Ingénierie

Les règles de Scrum sont définis dans le [Guide Scrum](http://www.les-traducteurs-agiles.org/2017/11/12/guide-scrum-novembre-2017.html) par Ken Scwaber et Jeff Sutherland. Bien que Scrum ne prescrivent pas de pratiques d'ingénierie, comme le fait XP, la plupart des entreprises définiront plusieurs pratiques dans le cadre des projets d'ingénierie logiciel. Le ScrumMaster est responsable sur le fait de responsabiliser l'Equipe Scrum sur ces règles et sur les pratiques d'ingénierie définies. Cet indicateur peut être mesuré en comptant les infractions qui apparaissent à chaque sprint. Un faible score peut découler de l'un des points suivants qui méritent toute votre attention :

* Le Management ou le Product Owner perturbent l'Equipe en la forçant à livrer avant que l'Equipe soit prête (voir Gestion de la Dette Technique).
* Faible voire aucune "Définition du Fini" incluant l'introduction de zéro bug (voir Gestion de la Dette Technique).
* Le Client n'est pas pris en compte pendant le sprint (voir Gestion de la Dette Technique).
* L'Equipe crée des bugs qui reflètent ses avis sur la façon dont les choses devraient fonctionner plutôt que d'écouter le Client (voir Gestion de la Dette Technique).
* L'Equipe ne documente pas les problèmes trouvés ou corrigés (voir Gestion de la Dette Technique).
* L'Equipe n'implique pas le Client/Product Owner pendant les tests d'acceptation utilisateur (voir Gestion de la Dette Technique).
* L'Equipe est perturbée (voir Stories finies vs Stories engagées, Vélocité de l'Equipe).
* Le ScrumMaster ne protège pas l'Equipe des perturbations.
* Les stories de référence de l'Equipe ne sont pas applicables à la version courante (voir Vélocité de l'Equipe).
* Les clients et les parties prenantes ne sont pas tous invités, tous visibles, ou ne participent pas tous à la revue de sprint (voir Qualité Livrée au Client).
* Le ScrumMaster ne garantit pas que l'Equipe Scrum adhère aux valeurs, pratiques et règles de Scrum.
* Le ScrumMaster ne garantit pas que l'Equipe Scrum adhère aux pratiques et règles d'ingénierie de l'entreprise, du département et de l'Equipe Scrum.
* Le ScrumMaster ne forme pas l'Equipe Scrum en la coachant et en la guidant pour être plus productive et produire davantage de produits de qualité.
* Le ScrumMaster n'aide pas l'Equipe Scrum à comprendre et mettre en oeuvre l'auto-organisation et la multi-disciplinarité.
* Le ScrumMaster ne garantit pas que l'Equipe Scrum dispose d'une "Définition du Fini" opérationnelle pour les stories.
* Le ScrumMaster ne garantit pas que l'Equipe ait une mêlée quotidienne.
* Le ScrumMaster ne garantit pas que l'Equipe affiche en bonne place le burndown de la version.
* Le ScrumMaster ne garantit pas que l'Equipe affiche en bonne place le burndown du sprint.
* Le ScrumMaster ne garantit pas que l'Equipe affiche en bonne place les stories du sprint et les critères d'acceptation.
* Le ScrumMaster ne garantit pas que la réunion de planification du sprint soit menée.
* Le ScrumMaster ne garantit pas que la réunion de revue du sprint soit menée.
* Le ScrumMaster ne garantit pas que la réunion de rétrospective du sprint soit menée.


## 9. Compréhension par l'Equipe de Développement du Périmètre et de l'Objectif du Sprint

La Compréhension par l'Equipe de Développement du Périmètre et de l'Objectif du Sprint est une mesure subjective sur la façon dont le Client, le Product Owner et l'Equipe interagissent, comprennent et se focalisent sur les stories et l'objectif du sprint. L'objectif du sprint est large et énonce l'intention générale du sprint. L'objectif est généralement abstrait et n'est pas testable en tant que tel, mais il est aligné avec la valeur qu'il est prévu de livrer au Client à la fin du sprint. Le périmètre ou l'objectif du sprint sont définis dans les critères d'acceptation des stories. Les stories et les critères d'acceptation sont des "espaces réservées aux conversations" et ne sont pas excessivement détaillés. Le Product Owner et le Client définissent les critères d'acceptation mais le Product Owner seul définit l'objectif du sprint. Le ScrumMaster peut toujours utiliser le score "Stories finies vs Stories engagées" et "Vélocité de l'Equipe" comme des indications qu'il y a un problème de compréhension des stories et de l'objectif, mais il vaut mieux le détecter à travers les contacts quotidiens en interagissant avec l'Equipe Scrum. Un faible score peut découler de l'un des points suivants qui méritent toute votre attention :

* Le Product Owner ne fournit pas assez d'informations à l'équipe de développement, autrement dit les besoins du Client (voir Stories finies vs Stories engagées, Vélocité de l'Equipe, Communication dans l'Equipe).
* Le Product Owner ne donne pas d'objectif au sprint.
* Le Product Owner ne comprend pas en quoi consiste une approche de développement incrémental.
* Le périmètre des exigences dérive ; le Product Owner ajoute des choses dans le périmètre des stories, ou ajoute des critères d'acceptation non vus lors de la planification du sprint (voir Stories finies vs Stories engagées, Vélocité de l'Equipe, Communication dans l'Equipe).
* L'Equipe ne comprend pas le périmètre du travail à réaliser au début du sprint (voir Vélocité de l'Equipe, Communication dans l'Equipe).


---
Auteur : [Bob Boyd](https://plus.google.com/103254508605258884244)  
Source : [Scrum Metrics](http://implementingagile.blogspot.fr/2011/06/scrum-metrics.html)  
Date de parution originale : 26 Juin 2011  

---
Traducteur : [Fabrice Aimetti](http://www.fabrice-aimetti.fr/)  
Date de traduction : 24/10/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



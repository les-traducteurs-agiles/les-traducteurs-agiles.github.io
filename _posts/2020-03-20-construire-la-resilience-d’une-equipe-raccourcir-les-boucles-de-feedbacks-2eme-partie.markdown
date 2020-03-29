---
layout: post
title:  "Construire la résilience d’une équipe : Raccourcir les boucles de feedbacks (2ème partie)"
date:   2020-03-20 21:38
published: false
tags:
- agile
- équipe
---

This series is about helping a team create a less brittle environment—more resilience. [Part 1](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-work-together-part-1/) was about individual work. This part is about shortening feedback loops.

Cette série aborde le sujet d'aider une équipe a créer une environnement mois fragile - plus résilient. La [1ère partie](http://www.les-traducteurs-agiles.org/2020/03/18/construire-la-resilience-d-une-equipe-travailler-ensemble-1ere-partie.html) évoquait le travail individuel. Cette partie traite du raccourcissement des boucles de retours d'informations (_feedback_)

Brief description of the problem at a recent client: Person A checked in code that broke an “unrelated” part of the system. I'll call this checking in code in Email that broke Search. (Yes, I changed the names of the functionality because the names don't matter.)

Voici la brève description d'un problème évoqué récemment par un client : Une Personne A avait inséré du code qui avait cassé une autre partie du système sans aucun rapport avec ce dernier. Je vas intitulé cela « Plantage du moteur de recherche après insertion de code dans la partie courriel » (Oui, j'ai changé les noms de la fonctionnalité par les noms n'ont que peu d'importance dans le fond.)

The managers didn't understand. Neither did the team. However, they now had a production support problem that they needed to fix.

Les managers ne comprenaient pas. Ni l'équipe. Toutefois, ils avaient mainteant un problème de production à régler.

They had one piece of feedback: the checkin broke “unrelated” code. It was time to see their feedback loops.

Un seul retour d'informations était à leur disposition : le code inséré avait cassé une autre code « sans rapport » avec celui-ci. Il était temps de jeter un coup d'œil à leur boucle de feedback.

## See Your Feedback Loops

## Visualisez vos boucles de feedback

Every project (or effort) has at least one feedback loop. That's when you release to customers.

Chaque projet (ou chaque effort) que vous faites possède au moins une boucle de feedback. C'est celle que vous avez lorsque vous livrez quelque chose aux clients.

[![](https://www.jrothman.com/wp-content/uploads/2020/02/Lifecycle.serial.reality-300x208.png)](https://www.jrothman.com/wp-content/uploads/2020/02/Lifecycle.serial.reality.png)If you use a waterfall approach, you more likely have the undesired feedback loops, as in the image, “Several Possible Realities of a Serial Lifecycle.”

Si vous utilisez une approche en cascade, vous avez probablement des boucles de feedbacks non désirées, comme dans cette image, « Plusieurs réalités possibles d'un cycle de vie en série ».

The more often you release internally, the more often you can get early feedback.

Plus vous livrez souvent en interne, plus vous aurez des feedbacks

The more often you release to customers, the more _validated_ feedback you can get. Production support issues are validated feedback. You might not like that feedback, but that's customer feedback.

Plus vous livrez souvent aux clients, plus vous obtenez des retours d'informations validés. Les problèmes de productions sont des retours d'informations validés.  Vous pourriez ne pas aimer ce retour d'informations, mais il s'agit de retours d'informations clients.

In this case, the project team had no automated tests. The team called the product people “product owners.” (They weren't, but that's a different problem.) These product people executed manual tests. Worse, they only tested the happy paths.

Dans ce cas, l'équipe projet n'avait pas de tests automatisés. L'équipe appelait les personnes du métier « product owners ». (Elles ne l'étaient pas, mais c'est là un problème différent). Ces personnes du métier exécutaient des tests manuels. Pire encore, ils ne testaient que les cas nominaux.

The product people didn't know how to test the possible error paths. They didn't know enough about the insides of the product to look for unwanted interactions.

Les personnes du métier ne savaient pas comment tester les cas non nominaux susceptibles de donner des erreurs. Ils ne connaissaient pas assez les entrailles du produit pour chercher les interactions indésirables.

Neither did the developers. These developers had no built-in feedback mechanisms.

Et c'était pareil pour les développeurs. Les développeurs n'avaient pas de mécanismes de retours d'informations inclus dans leur code.

## Automated Tests Are About Feedback

## Les tests automatisés c'est du feedback

A gajillion years ago, when I wrote code for a living, I wrote my tests after I wrote the code. I admit it.

Il y a un quadrillion d'années, lorsque je codais pour gagner ma vie, j'écrivais mes tests après avoir codé. Je dois l'admettre.

I was extremely good at writing tests that ignored my errors. Yes, I would test everything except the places I had made mistakes. I became extremely good at reading octal or hex dumps (depending on the machine and language). (There was a time when I could read the Fortran stack trace and know exactly where I had screwed up. Oh, the bad old days.)

J'étais même très bonne pour écrire des tests qui pouvaient ignorer mes erreurs. Oui, je testais tout à l'exception des endroits où j'avais fait des erreurs. Je devins très bonne à lire les _dumps_[^1] en hexadécimal ou en octal (selon le type de machine et le langage utilisé). (Il fût un temps où je pouvais lire les traces d'appels de la pile d'exécution en Fortran et de savoir exactement où je m'étais planté. Oh, ces bons vieux mauvais jours).

We have other tools now. We can use TDD, BDD, ATDD and get feedback _before_ we write code. See these definitions:

De nos jours, nous savons d'autres outils. Nous pouvons utiliser TDD, BDD, ATDD et obtenir des retours d'informations _avant_ d'écrire du code. Vous pouvez consultez les définitions à partir des liens ci-dessous :

* [Test-Driven Development](https://www.agilealliance.org/glossary/tdd/)
* [Behavior Driven Development](https://www.agilealliance.org/glossary/bdd)
* [Acceptance-Test Driven Development](https://www.agilealliance.org/glossary/atdd/)

I happen to like David Bernstein's book, [Beyond Legacy Code (Amazon)](https://amzn.to/32URR5S) and on the [Prags](https://pragprog.com/book/dblegacy/beyond-legacy-code), as a way to integrate reasonable technical practices into your work now. (You might read the updated _Pragmatic Programmer_ or any of the other test-driven books available. Heck, read them all to learn and practice.)

Il se que David Bernstein a écrit un livre que j'apprécie beaucoup, Beyond Legacy Code (disponible sur [Amazon](https://amzn.to/32URR5S) et [PragProg](https://pragprog.com/book/dblegacy/beyond-legacy-code)) qui décrit un ensemble de pratiques techniques facilement intégrables à votre processus de travail. (Vous pourriez également la version mise à jour de _Pragmatic Programmer_ ou tout autre livre sur le développement piloté par les tests disponible. Oh et puis flûte, lisez-les tous, apprenez et mettez en pratique.)

I learned about test-driven development in all its various forms after I stopped writing code professionally.  However, I use the ideas of specification by example when I write, even though I write in a natural language (English).

J'ai appris le développement piloté par les tests dans toutes ces formes après que j'ai arrêté d'écrire du code dans le cadre de ma vie professionnel. Toutefois, j'utilise les idées des spécifications par l'exemple lorsque j'écris, même si j'écris en langage naturel (en Anglais).

You've noticed I often tell stories in my posts and books. Those are examples. I use them to help you realize the context and when that context does and does not apply to you. Just as important, the example grounds my writing and offers me feedback as I write.

Vous avez sans doute remarqué que je raconte souvent des histoires dans mes articles et dans mes livres. Il s'agit d'exemples. Je les utilise dans l'objectif de vous aider à prendre en compte le contexte et quand ce contexte s'applique ou ne s'applique pas à votre cas. De manière toute aussi importante, l'exemple permet d'ancrer dans le réel mes écrits et m'offre du feedback lorsque j'écris.

I'm not perfect. I'm sure I go off on tangents in blog posts that leave you saying, “Huh?” Even so, the examples help give me feedback as I write. With any luck, I bring you along with me, even if I head off on a tangent.

Je ne suis pas parfaite. Je suis certaine que quelques fois je prends des tangentes dans certains articles de blogs qui vous laisse avec un certain "hein ?". Même ainsi, les exemples m'aident à donner du feedback lorsque j'écris. Avec un peu de chance, cela vous permet de rester avec moi, même si j'avais pu prendre une tangente.

This team decided to visualize their feedback loops.

Cette équipe a décidé de visualiser ces boucles de feedback.

## How Long Are Your Feedback Loops?

## Quelle est la durée de vos boucles de feedback ?

You might think your feedback loops are pretty short. They might be. Have you measured your value stream to actually see your cycle time? See a “blank” value stream map in [Measure Cycle Time, Not Velocity](https://www.jrothman.com/mpd/project-management/2019/09/measure-cycle-time-not-velocity/).

Vous pourriez pensez que vos boucles de feedback sont plutôt courtes. Cela pourrait être le cas. Avez vous mesurez votre chaîne de valeur pour voir vraiment quel est votre temps de cycle ? Vous pouvez en savoir plus sur la cartographie de la chaîne de valeur dans mon article [Measure Cycle Time, Not Velocity (VO)](https://www.jrothman.com/mpd/project-management/2019/09/measure-cycle-time-not-velocity/).

[![](https://www.jrothman.com/wp-content/uploads/2020/03/NonResilientTeamBeforeProblem-300x168.png)](https://www.jrothman.com/wp-content/uploads/2020/03/NonResilientTeamBeforeProblem.png)Here's what this team's value stream map looked like for just one feature. They hadn't discovered the problem in this value stream.

Voici à quoi pouvait ressembler la carte de la chaîne de valeur de cette équipe pour une seule fonctionnalité. Elle n'avait pas encore découvert le problème dans cette chaîne de valeur.

Note that their work time is 1/4th the time they spent waiting.

Vous pouvez remarquer que le temps de réalisation de la fonctionnalité représente 1/4 du temps total où l'équipe a passé du temps à attendre.

But,  three days after they checked in this “done” work, they discovered this problem where the Email checkin affected the Search.

Mais, trois jours après qu'elle ait inséré son code en « production », elle a découvert le problème « Plantage du moteur de recherche après insertion de code dans la partie courriel ».

[![](https://www.jrothman.com/wp-content/uploads/2020/03/NonResilientTeamAfterProblem-300x171.png)](https://www.jrothman.com/wp-content/uploads/2020/03/NonResilientTeamAfterProblem.png)When they realized they had a problem with this checkin, they started to write tests and do a code review.

Lorsqu'elle a réalisé le problème avec cette insertion de code, elle a commencé à écrire des tests et faire des revues de code.

The team took another 3.5 days—on top of the previous 4+ days—to complete this work.

L'équipe pris 3,5 jours supplémentaires - en plus des 4+ jours précédents - pour terminer son travail.

And, all their other work was delayed by these 3.5 days.

Et tous le reste du travail à faire a été retardé par ces 3,5 jours.

They were way behind now. All because they didn't have enough short feedback loops.

Elle était bien en retard désormais. Tout ça, parce qu'elle n'avait pas des boucles de feedbacks suffisamment courtes.

## More Frequent Feedback Helps Build Resilience

## Des retours d'informations plus fréquents aident à construire la résilience

The more frequent your feedback, the more resilient your actions can be. This team wrote tests when they were under pressure, with a production support problem. They didn't do a code review until they were stuck.

Plus vous obtenez des feedbacks fréquemment, plus vos actions deviennent résilientes. L'équipe a écrit les tests lorsqu'elle était sous pression, avec un problème de production à régler. Elle n'avait pas fait de revue de code avant de l'avoir sur les bras.

Tests—especially pervasive, small tests—can create resilience in a team. Even if you don't [work as a team (Part 1)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-work-together-part-1/), tests can help you build resilience.

Les tests - et tout spécialement des petits tests systématiques - peuvent créer de la résilience dans une équipe. Même si vous ne travaillez pas [ensemble en tant qu'équipe (cf. 1ère partie)](http://www.les-traducteurs-agiles.org/2020/03/18/construire-la-resilience-d-une-equipe-travailler-ensemble-1ere-partie.html), les tests peuvent vous aider à construire la résilience.

Tests provide support for change.

Les tests offrent un support pour ce changement.

Here's how I think about this:

Voici comment j'en conçois le déroulement :

* Create small chunks of work.
* Create pervasive automated tests so you know how to change the code when you need to. (Yes, there is a need for manual tests, and those often take much more time to run. I'm talking about automated tests here.)
* Measure how many feedback loops you have and their duration. (Consider measuring your cycle time.)

* Faire une petite quantité de travail
* Faire systématiquement des tests automatisés afin que vous sachiez comment vous pourrez modifier le code lorsque vous en aurez besoin. (Oui, il y a besoin de tests manuels, ces derniers prennent généralement bien plus de temps à être exécuter. Je parle ici de tests automatisés.)
* Mesurer le nombre de boucles de feedbacks que vous avez et leurs durées (prenez bien en considération le fait de mesure votre temps de cycle)

How did this team work themselves out of their hole(s)?

Comment cette équipe s'en est-elle sortie ?

1.  First, they used user stories to define the work.
2.  They defined acceptance criteria for ATDD.
3.  They used (with some reluctance) a combination of TDD and BDD. They didn't all agree on what to do. However, they started to write tests first. That helped them with the design, not the code.
4.  They measured their cycle time. After some practice, they managed to get their cycle time down to under a day.

1. Tout d'abord, elle a utilisé des _user stories_ pour définir son travail
2. Elle a défini des critères d'acceptances pour faire de l'ATDD
3. Elle a utilisé (avec quelques réticences) une combinaison de TDD et de BDD. Tous les membres de l'équipe n'étaient pas d'accord sur qu'est-ce qu'il fallait faire. Toutefois, ils ont commencé à écrire des tests d'abord. Cela les a aidé avec la conception, pas avec le code.
4. Elle a mesuré son temps de cycle. Après un peu pratique, elle a géré son temps de cycle pour le faire passer en-dessous d'une journée.

The more you can do to shorten your feedback loops, the more resilience your team has.

Plus vous en faites en sorte de réduire vos boucles de feedback, plus vous renforcer la résilience de votre équipe.

The series:

* [Build Team Resilience: Work Together (Part 1)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-work-together-part-1/)
* [Build Team Resilience: Shorten Feedback Loops (Part 2)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-shorten-feedback-loops-part-2/)
* [Build Team Resilience: Work “Anywhere” and “Anytime” (Part 3)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-work-anywhere-and-anytime-part-3/)
* [Build Team Resilience Summary (Part 4)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-summary-part-4/)

La série :

* [Construire la résilience d'une équipe : travailler ensemble (1ère partie)](http://www.les-traducteurs-agiles.org/2020/03/19/construire-la-resilience-d-une-equipe-travailler-ensemble-1ere-partie.html)
* * [Construire la résilience d'une équipe : Raccourcir les boucles de feedbacks (2ème partie - traduction à venir)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-shorten-feedback-loops-part-2/)
* [Construire la résilience d'une équipe : Travailler « n'importe où » et « n'importe quand » (3ème partie - traduction à venir)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-work-anywhere-and-anytime-part-3/)
* [Construire la résilience d'une équipe en résumé (4ème partie - traduction à venir)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-summary-part-4/)

[^1]: NdT : Copie du contenu de tout ou partie d'une base de données ou de la mémoire d'une machine sous la forme d'un fichier à des fins d'analyse.  

---
Auteur : [Prénom_Nom](url_bio)  nbsp
Source : [Titre_article_en_vo](url_article_en_vo)  nbsp
Date de parution originale : jj_MMMM_yyyy  nbsp

---
Traducteur : [Prénom_Nom](url_bio)  nbsp
Date de traduction : jj/mm/yyyy  nbsp

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

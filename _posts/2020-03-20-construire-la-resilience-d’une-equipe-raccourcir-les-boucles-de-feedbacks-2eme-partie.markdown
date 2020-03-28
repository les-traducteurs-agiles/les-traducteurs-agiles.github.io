---
layout: post
title:  "Construire la résilience d’une équipe : Raccourcir les boucles de feedbacks (2ème partie)"
date:   2020-03-20 21:38
published: true
tags:
- agile
- équipe
---

This series is about helping a team create a less brittle environment—more resilience. [Part 1](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-work-together-part-1/) was about individual work. This part is about shortening feedback loops.

Cette série aborde le sujet d'aider une équipe a créer une environnement mois fragile - plus résilient. La [1ère partie](http://www.les-traducteurs-agiles.org/2020/03/18/construire-la-resilience-d-une-equipe-travailler-ensemble-1ere-partie.html) évoquait le travail individuel. Cette partie traite du raccourcissement des boucles de retours d'informations (_feedback_)

Brief description of the problem at a recent client: Person A checked in code that broke an “unrelated” part of the system. I'll call this checking in code in Email that broke Search. (Yes, I changed the names of the functionality because the names don't matter.)

Voici la brève description d'un problème évoqué récemment par un client : Une Personne A avait inséré du code qui avait cassé une autre partie du système sans aucun rapport avec ce dernier. Je vas intitulé cela « Insérer du code dans la partie courriel ayant cassé le moteur de recherche » (Oui, j'ai changé les noms de la fonctionnalité par les noms n'ont que peu d'importance dans le fond.)

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



A gajillion years ago, when I wrote code for a living, I wrote my tests after I wrote the code. I admit it.



I was extremely good at writing tests that ignored my errors. Yes, I would test everything except the places I had made mistakes. I became extremely good at reading octal or hex dumps (depending on the machine and language). (There was a time when I could read the Fortran stack trace and know exactly where I had screwed up. Oh, the bad old days.)



We have other tools now. We can use TDD, BDD, ATDD and get feedback _before_ we write code. See these definitions:



* [Test-Driven Development](https://www.agilealliance.org/glossary/tdd/)
* [Behavior Driven Development](https://www.agilealliance.org/glossary/bdd)
* [Acceptance-Test Driven Development](https://www.agilealliance.org/glossary/atdd/)



I happen to like David Bernstein's book, [Beyond Legacy Code (Amazon)](https://amzn.to/32URR5S) and on the [Prags](https://pragprog.com/book/dblegacy/beyond-legacy-code), as a way to integrate reasonable technical practices into your work now. (You might read the updated _Pragmatic Programmer_ or any of the other test-driven books available. Heck, read them all to learn and practice.)



I learned about test-driven development in all its various forms after I stopped writing code professionally.  However, I use the ideas of specification by example when I write, even though I write in a natural language (English).



You've noticed I often tell stories in my posts and books. Those are examples. I use them to help you realize the context and when that context does and does not apply to you. Just as important, the example grounds my writing and offers me feedback as I write.



I'm not perfect. I'm sure I go off on tangents in blog posts that leave you saying, “Huh?” Even so, the examples help give me feedback as I write. With any luck, I bring you along with me, even if I head off on a tangent.



This team decided to visualize their feedback loops.



## How Long Are Your Feedback Loops?



You might think your feedback loops are pretty short. They might be. Have you measured your value stream to actually see your cycle time? See a “blank” value stream map in [Measure Cycle Time, Not Velocity](https://www.jrothman.com/mpd/project-management/2019/09/measure-cycle-time-not-velocity/).



[![](https://www.jrothman.com/wp-content/uploads/2020/03/NonResilientTeamBeforeProblem-300x168.png)](https://www.jrothman.com/wp-content/uploads/2020/03/NonResilientTeamBeforeProblem.png)Here's what this team's value stream map looked like for just one feature. They hadn't discovered the problem in this value stream.



Note that their work time is 1/4th the time they spent waiting.



But,  three days after they checked in this “done” work, they discovered this problem where the Email checkin affected the Search.



[![](https://www.jrothman.com/wp-content/uploads/2020/03/NonResilientTeamAfterProblem-300x171.png)](https://www.jrothman.com/wp-content/uploads/2020/03/NonResilientTeamAfterProblem.png)When they realized they had a problem with this checkin, they started to write tests and do a code review.



The team took another 3.5 days—on top of the previous 4+ days—to complete this work.



And, all their other work was delayed by these 3.5 days.



They were way behind now. All because they didn't have enough short feedback loops.



## More Frequent Feedback Helps Build Resilience



The more frequent your feedback, the more resilient your actions can be. This team wrote tests when they were under pressure, with a production support problem. They didn't do a code review until they were stuck.



Tests—especially pervasive, small tests—can create resilience in a team. Even if you don't [work as a team (Part 1)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-work-together-part-1/), tests can help you build resilience.



Tests provide support for change.



Here's how I think about this:



* Create small chunks of work.
* Create pervasive automated tests so you know how to change the code when you need to. (Yes, there is a need for manual tests, and those often take much more time to run. I'm talking about automated tests here.)
* Measure how many feedback loops you have and their duration. (Consider measuring your cycle time.)



How did this team work themselves out of their hole(s)?



1.  First, they used user stories to define the work.
2.  They defined acceptance criteria for ATDD.
3.  They used (with some reluctance) a combination of TDD and BDD. They didn't all agree on what to do. However, they started to write tests first. That helped them with the design, not the code.
4.  They measured their cycle time. After some practice, they managed to get their cycle time down to under a day.



The more you can do to shorten your feedback loops, the more resilience your team has.



The series:

* [Build Team Resilience: Work Together (Part 1)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-work-together-part-1/)
* [Build Team Resilience: Shorten Feedback Loops (Part 2)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-shorten-feedback-loops-part-2/)
* [Build Team Resilience: Work “Anywhere” and “Anytime” (Part 3)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-work-anywhere-and-anytime-part-3/)
* [Build Team Resilience Summary (Part 4)](https://www.jrothman.com/mpd/management/2020/03/build-team-resilience-summary-part-4/)


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

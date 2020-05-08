---
layout: post
title:  "Questions/Réponses à propos de la vélocité - 8ème partie"
date:   2020-05-06 00:00
published: false
tags:
- vélocité
---

In our [previous post](http://agileotter.blogspot.com/2018/11/q-and-on-velocity-part-vii.html), we discussed doing smaller units of work, and doing no more of them than we need to fulfill an end-user's needs. This way, we get many things done, we deliver more quickly, and we develop less unneeded code (provided we get frequent feedback from users).  

Dans notre [précédent article](http://www.les-traducteurs-agiles.org/2020/04/15/questions-reponses-a-propos-de-la-velocite-7eme-partie.html), nous avons discuté à propos de faire de plus petites unités de travail et de ne pas en faire plus qu'il n'est nécessaire pour répondre au besoin de notre utilisateur final. De cette manière, nous terminons davantage de choses, nous les livrons plus rapidement, et nous développons moins de code inutile (étant donné que nous avons des retours d'informations réguliers de la part des utilisateurs).

Fans of agile software development will recognize this as one of the axiomatic concepts behind agile, derivative of much earlier work on [incremental and iterative development](https://en.wikipedia.org/wiki/Iterative_and_incremental_development).  Without incremental, iterative development and feedback, a process can hardly be said to be agile in any way whatsoever.  

Les fans du développement agile de logiciels reconnaîtront là l'un des concepts axiomatiques derrière agile, basé sur des travaux beaucoup plus anciens comme le [développement itératif et incrémental](https://en.wikipedia.org/wiki/Iterative_and_incremental_development). Sans développement incrémental, itératif et sans retours d'informations, un processus quel qu'il soit aura du mal à se dire agile d'une quelconque manière.

So we pick up the conversation today at that point:  

Donc, reprenons la conversation à partir de ce point aujourd'hui.

> A: ...But I we get 23 points now, and they're as big as the 1/19th sized ones.  
> B: That has two possible explanations.  
> A: What is the first explanation  
> B: That they're assigning more points to same-sized work: _inflation_.  
> A: Why would they do that?

> A : ... Mais, j'ai … nous avons obtenu 23 points aujourd'hui et ils ont la même taille que ceux qui correspondaient à 1/19ème de sprint.  
> B : Il y a deux explications possibles.  
> A : Quelle est la première explication ?  
> B : C'est qu'ils affectent davantage de point à un travail de taille équivalente : _inflation_.  
> A : Pourquoi feraient-ils cela ?

People in an organization are constantly trying to satisfy their bosses. When organizations put pressure on developers to produce more points, developers start to find ways to score more points. There are some hilarious examples in [Joshua Kerievsky's article](https://www.industriallogic.com/blog/stop-using-story-points/) on story points at the Industrial Logic [blog](http://blog.industriallogic.com/). Sometimes it is intentional but not always.  

Les salariés dans une entreprise essayent de satisfaire constamment leurs patrons. Lorsque les entreprises mettent la pression sur les développeurs pour produire davantage de points, les développeurs commencent à trouver des biais pour faire monter le score du nombre de points. Il y a quelques exemples hilarants dans un [article de Joshua Kerievsky](https://www.industriallogic.com/blog/stop-using-story-points/) sur les _story points_ publié sur le [blog](http://blog.industriallogic.com/) d'Industrial Logic. Certaines fois, c'est fait intentionnellement, mais pas toujours.

When a team turns in an 8-point sprint/iteration/whatever, and are disappointed, they often look back over the week and realize that they _under-estimated_ some of the stories which were harder than they looked, and that is the reason it was only 8 points. It should have been 15. In reaction, they give higher point-count estimates the next time.  This kind of inflation isn't to deceive, but to better reflect reality and truth. But now the team turns in a more satisfying 15 point sprint, and exactly the same amount of work is being done.  

Lorsqu'une équipe a fait 8 points sur un sprint, une itération ou autre chose d'équivalent, et qu'elle est déçue, elle regarde souvent en arrière sur la semaine écoulée et elle réalise qu'elle a _sous-estimée_ certaines _stories_ qui étaient plus difficiles qu'elles ne paraissaient. Et c'est la raison pour laquelle le sprint a fait seulement 8 points alors qu'il aurait dû faire 15 points. En réaction, elle fera des surestimations la prochaine fois. Ce genre d'inflation n'est pas fait dans une intention de duper, mais pour mieux refléter la réalité et la vérité. Mais maintenant l'équipe est davantage satisfaite de faire un sprint à 15 points avec la même quantité de travail accomplit.

That people misinterpret this as acceleration is not the team's intention. They merely are taking credit for the amount of work they actually did.  

L'interprétation qui en est faite par certaines personnes comme étant une forme d'accélération n'est pas dans l'intention de l'équipe. Elle s'octroie simplement un crédit plus amplement mérité pour ce travail qu'elle ne l'avait fait auparavant.

"Scoring points" and "having higher scores" classicly illustrates [Goodhart's law](https://en.wikipedia.org/wiki/Goodhart%27s_law). A measure (of completion rate) which is a reasonable measure, once chosen as a goal, ceases to be a valid measure.  

« Marquer des points » et « avoir des hauts scores » illustrent de manière très classique la [loi de Goodhart](https://fr.wikipedia.org/wiki/Loi_de_Goodhart). Un indicateur (d'un taux de réalisation) qui est un indicateur raisonnable, une fois choisit comme objectif, cesse d'être un indicateur valide.

You will hear development teams in scrum-like processes talking about work "blowing up."  That means "like a balloon" not "like dynamite."  There was some story that seemed like a 2-pointer, but turned out to take most of the sprint because there was more risk and uncertainty that anyone realized.  

Vous entendrez certaines équipes de développement engagées dans des processus _à là_ scrum parlant de travail "qui explose". C'est-à-dire « comme un ballon » et non « comme de la dynamite ». Comme par exemple pour une _story_ à qui l'on donne un petit 2, mais qui s'avère prendre la quasi totalité du sprint parce qu'elle comporte tout un tas de risques et d'incertitudes que personne n'a vu.

A story may have seemed simple: "add a discount code field." The product owner/manager/boss may have said: "that should only be a two-point story."  

Une _story_ peut avoir semblé simple : « ajouter un champ pour un code de réduction». Le _product owner/manager_ ou le patron ont peut être dit : « cela ne devrait être qu'une _story_ a deux points ».

It seems easy. It should be easy to operate. What could be simpler? It's one field on a form, and you subtract some value from the total.  

Cela semble facile. Cela devrait être facile à réaliser ? Qu'est-ce qui pourrait être plus simple que ça ? Il s'agit d'un champ dans un formulaire et vous soustrayez une valeur d'un total.

But these things are seldom simple. Marketing and accounting want tracking, and expiry for discounts, and demographic limits on the usage. Discounts need to appear on the customer's receipt as an indicator that they got a good deal from the company (marketing!). Discounts need to be represented in billing reports.  

Mais ce genre de choses sont rarement aussi simple. Le marketing et la comptabilité veulent un traçage des remises, des dates expirations des réductions, des données à caractère démographiques liées à l'utilisation des réductions. Les réductions doivent apparaître sur la facture du client pour montrer qu'il a fait une bonne affaire (marketing !). Les remises doivent figurées sur les rapports de vente.

There may be special discounting reports used to measure the success of promotions. There may be anti-fraud ramifications.  

Il peut y avoir des rapports dédiés aux remises pour mesurer le succès des promotions. Il peut y avoir des ramifications anti-fraudes.

Then someone decides that there should be many discount codes, and they should combine in some ways but not others. Now UX has to redesign the data entry screen, and there are complicated rules. Maybe those need a new microservice?  

Puis tout d'un coup quelqu'un décide qu'il devrait y avoir plusieurs codes de réductions et qu'ils devraient se combiner d'une certaine façon et pas d'une autre. Désormais l'expérience utilisateur doit redessiner le nouveau formulaire, et il y a des règles compliquées. Peut être a t'on besoin d'un nouveau microservice ?

But it was a three-point story, right? This raises questions:  

Mais c'était une _story_ a 3 points, n'est-ce pas ? Cela amène les questions suivantes :

* Why did the team only turn in 5 points this sprint?
* What's WRONG with them?
* Why are they slowing down?
* What can we do to motivate them to go faster?
* Team X turned in 50 points compared to this team's 5, why are they 10x better?
* Does this team need a PIP?

* Pourquoi l'équipe a fait seulement 5 points à ce sprint ?
* Qu'est-ce qui se passe MAL chez elle ?
* Pourquoi ralentit-elle ?
* Qu'est-ce qui peut la motiver à aller plus vite ?
* L'équipe X a fait 50 points par rapport à cette équipe qui en a fait 5, pourquoi l'équipe X fait-elle 10 fois mieux ?
* Est-ce que cette équipe a besoin d'un plan d'amélioration des performances ?


These are **the wrong questions.**  They are based on a faulty assumption, and acting on them will only make things worse. We discussed [curiosity spaces](https://agileotter.blogspot.com/2016/08/the-curiosity-space.html) related to velocity in [Part VI,](https://www.industriallogic.com/blog/stop-using-story-points/) which you may want to revisit at this time.  

Il s'agit là de **mauvaises questions**. Elles sont basées sur de mauvaises hypothèses et agir dans leurs sens ne fera qu'empirer les choses. Nous avons discuté précédemment de l'[espace de curiosité](http://www.les-traducteurs-agiles.org/2016/10/16/espace-de-curiosite.html) en relation avec la vélocité évoquée en [partie 6](http://www.les-traducteurs-agiles.org/2020/03/26/questions-reponses-a-propos-de-la-velocite-6eme-partie.html) que vous pourriez vouloir rejeter un coup d'œil peut être maintenant.

Ultimately, the thing to understand about teams using time boxes is that about the same amount of work is being done every week (barring absences and meetings and events on company time). [Velocity is mostly illusion](https://agileotter.blogspot.com/2012/09/14-weird-observations-about-agile-team.html).  

Enfin, la chose à cmprendre à propos des équipes utilisant des temps impartis est relatif à une même quantité de travail faite chaque semaine (exception faite des absences, des réunions et des évènements pris sur le temps de l'entreprise). [La vélocité est la plupart du temps une illusion](https://agileotter.blogspot.com/2012/09/14-weird-observations-about-agile-team.html).

Consider Goodhart's law, curiosity, exploding stories, and inflation.  

Considérer la loi de Goodhart, la curiosité, les _stories_ qui explosent et l'inflation.

Then come back to join us for [part IX](http://agileotter.blogspot.com/2019/08/q-and-on-velocity-part-ix.html).

Puis revenez vous joindre à nous pour la [9ème partie](http://agileotter.blogspot.com/2019/08/q-and-on-velocity-part-ix.html).

---
Auteur : Tim Ottinger  
Source : [Q and A on velocity, Part VIII ](http://agileotter.blogspot.com/2018/12/q-and-on-velocity-part-viii.html)  
Date de parution originale : 19 Décembre 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 06/05/2020  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

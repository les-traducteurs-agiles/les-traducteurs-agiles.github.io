---
layout: "post"
title: "Questions/Réponses à propos de la vélocité - 9ème partie"
date: "2020-11-16 09:58"
published: false
tags:
- vélocité
---

In the [last installment](http://agileotter.blogspot.com/2018/12/q-and-on-velocity-part-viii.html), we talked about reasons that velocity goes up without any more accomplishment by the team. This is a disturbing occurrence to many managers who want to use velocity as a measure of productivity, and their insistence on treating low velocity as a productivity measure.  

Lors de notre [dernière discussion](http://www.les-traducteurs-agiles.org/2020/05/08/questions-reponses-a-propos-de-la-velocite-8eme-partie.html), nous avons évoqué les raisons pouvant expliquer une augmentation de la vélocité sans que l'équipe ait accompli quoi que ce soit de plus. C'est quelque chose de plutôt assez troublant pour des managers souhaitant utiliser la vélocité comme mesure de productivité, et qui veulent utiliser de manière insistante une vélocité disons faible comme telle.

We'll pick up the conversation from there.  

Nous allons reprendre la conversation à partir de là :

> A: I don't _like_ the "estimating in larger numbers" explanation. What is an alternative explanation?  
> B: Perhaps they've developed skills, knowledge, and/or techniques that make it easier to get more work done.

> A : Je _n'aime pas trop_ l'explication des « estimations très élevées ». Quelle est l'explication alternative ?
> B : Eh bien, peut-être l'équipe a-t-elle développé des compétences, des connaissances et/ou des techniques qui rendent les choses plus faciles à faire.

There are a few ways of measuring efficiency. One of the least useful is output over time. If one team of people produce more in a week than another, isn't the one more efficient? It's not possible to say.  

Il existe diverses façons de mesurer l'efficacité. L'une des moins utiles est de mesurer la production dans le temps. Lorsqu'une équipe produit davantage qu'une autre lors d'une même semaine, n'est-elle pas plus efficace ? C'est impossible à dire.

They may put out a disproportionate amount of effort in order to get a higher yield. That could be arguably more _productive_ but it is not more _efficient_. If it's harder to get more work done, then you have a kind of productivity that won't scale and won't sustain.  

Celle-ci a peut-être fait un effort considérable et disproportionné afin de pouvoir produire davantage. C'est sans aucun doute être plus _productif_ mais ce n'est pas être plus _efficace. S'il est plus difficile de finir davantage de tâches, alors vous vous retrouvez dans une situation telle que il est impossible, à votre modèle de productivité, de passer à plus grande échelle et soutenable dans le temps.

People eventually get tired of working harder. They eventually come to resent longer hours. When the work doesn't get easier and there is always more of it, the team will lack [profluence](http://anarchycreek.com/2010/04/06/coaching-profluence-for-motivation/) and will become demoralized.  

Les gens vont finir à la longue se fatiguer à force de travailler de plus en plus dur. Ils vont finir par en avoir marre de faire des heures à rallonge. Lorsque le travail ne devient pas plus facile et qu'il y en a toujours de plus en plus, l'équipe va manquer de [profluence](http://anarchycreek.com/2010/04/06/coaching-profluence-for-motivation/) et qu'elle va se démoraliser.

Another way of seeing efficiency is energy used over output produced. There are some very easy ways to produce a lot of output. Almost all of these are horrible ideas. A copy-paste artist on the team can produce hundreds or thousands more lines of code than an experienced programmer who understands the system. It seems like "more output" but it's mostly waste -- a copy-paste artist will use 1000 lines of code where an expert needs maybe three. The copy-paste artist will create rampant duplication in the codebase which makes the code harder to maintain, slower to compile, and larger in-memory footprint. That's before we talk about the quality and safety of their approaches.  

Une autre manière d'envisager l'efficacité est de mesurer l'énergie utilisée par rapport à la production effectuée. Il y a des manières très faciles de produire de grandes quantités de choses. La plupart d'entre elles sont horribles. Un virtuose du copier-coller peut produire des centaines ou des milliers de lignes de code de plus qu'un développeur qui a une bonne compréhension du système. Cela semble être « plus productif » mais c'est plutôt du gâchis -- un virtuose du copier-coller va faire 1 000 lignes de codes là où un expert en fera peut être trois. Le virtuose du copier-coller va étouffer la base de code à cause de cette duplication rampante qu'il aura engendré - ce qui va rendre le code de plus en plus dur à maintenir, de plus en plus lent à compiler, et une empreinte mémoire de plus en plus grande. Et tout ça avant que nous ne commencions à parler de qualité et de sécurité de leur approche.

My favorite is effort over outcome. If I can get just as good a _result_ with 15 minutes today or by putting in four days of hard work then it's more efficient to do it in 15 minutes. This is a flexible idea, because one can define the result they wish to see. There is always quality to consider in choosing an outcome. If my 15 minutes is a dirty hack that degrades the design of the code so people cannot make changes without causing defects, then it's probably an outcome we can't afford.  

Ma favorite est l'effort fourni par rapport au résultat produit. Si je peux juste obtenir un bon _résultat_ en 15 minutes aujourd'hui ou au bout de quatre jours de dur labeur alors il est plus efficace de le faire en 15 minutes. C'est une idée flexible, parce que l'on peut définir le résultat comme étant quelque chose que l'on souhaite voir. La qualité est toujours quelque chose à prendre en considération lorsque que l'on choisit un certain résultat. Si ce que je fais en 15 minutes est un bidouillage merdique qui dégrade la conception du code de telle manière que personne ne pourra effectuer de changements ultérieurs sans provoquer des bogues, alors il s'agit d'un résultat que nous ne pouvons nous permettre.  

Luckily, there are techniques and skills involved here. If we do a good job of [code craft](https://www.amazon.com/Beyond-Legacy-Code-Practices-Software/dp/1680500791), we can make a system easy to change safely. These are skills that Josh Kerievsky has called "[tech safety](https://www.industriallogic.com/blog/techsafety/)." I like the term. To move safely and efficiently sounds like programming nirvana.  

Fort heureusement, il y a des techniques et des compétences à l'œuvre ici. Si nous faisons du bon boulot d'[artisanat logiciel](https://www.amazon.fr/Beyond-Legacy-Code-Practices-Software/dp/1680500791), nous pouvons créer un système qui est facile à changer en toute sécurité. Il s'agit de compétences que Josh Kerievsky appelle la « [sécurité technique](https://www.industriallogic.com/blog/techsafety/) ». J'aime bien ce terme. Marier sécurité et efficacité est le nirvana du développement.

> A: How do I know if that's the case?  
> B: Have you spoken with them?  
> A: I've told them how important it is that they go faster. What else do you want me to tell them?  
> B: Have you _asked_ them, and _listened_?  
> A: If it is important, shouldn't they just tell me?

> A : Comment puis-je savoir si c'est le cas ?  
> B : En avez-vous parlé avec eux ?  
> A : Je leur ai dis à quel point il était important qu'ils aillent plus vite. Qu'est-ce que vous voulez d'autre que je leur dise ?  
> B : Est-ce que vous leur avez _demandé_ et _écouté_ ?  
> A : Si c'est si important, n'auraient-ils pas dû juste m'en parler ?  

One of the more frustrating problems of being a boss is that people are afraid to tell you things and they're afraid to ask you things. It's quite annoying. Concerns of [role success](http://agileotter.blogspot.com/2015/10/principles-for-large-organizations.html) tend to taint everyday events. Even though it should be part of the job to keep one's managers informed, more employees tend to keep the managers away instead.  

L'un des problèmes les plus frustrants lorsque l'on est un responsable, c'est que les gens ont peur de vous dire les choses et de vous demander des choses. C'est assez ennuyant.  Les préoccupations liés au [succès du rôle](http://agileotter.blogspot.com/2015/10/principles-for-large-organizations.html) tendent à ternir les évènements quotidiens. Même si cela devrait faire partie du boulot de tenir informé son responsable, de plus en plus d'employés tendent plutôt à tenir éloignés leur responsable.

Especially if the managers are scary; if they make demands, if they insist on results the team doesn't know how to provide. If they cancel vacations or demand long hours, then they'll likely be seen as tyrants; this shuts down communication.  

Et c'est le cas si les managers sont effrayants ; s'ils font des demandes, ou s'ils insistent pour obtenir des résultats que l'équipe ne sait pas comment les lui fournir. S'ils annulent les congés ou demandent à l'équipe de travailler plus longtemps, alors ils seront probablement perçus comme des tyrans ; cela coupe la communication.

People will tend to avoid having unpleasant and unsupportive interactions. As a result they won't come to managers to ask for support and they won't bring bad news to the manager. They will hide. They will go dark.  

Les gens auront tendance à éviter des interactions désagréables ou malsaines. En conséquence, ils ne viendront pas voir les managers pour leur demande un soutien quelconque et ils ne lui apporteront aucune mauvaises nouvelles non plus. Ils se cacheront. Ils vont se dissimuler.

Avoid this problem.  

Évitez ce problème.

There are few things more powerful and rich in learning than to get involved with a team that is doing the work. You can learn how much of a struggle the daily tasks are, or how dull. You can see how much the team is impeded by interruption, risk, and uncertainty.  

Il existe peu de choses plus puissantes et plus riches en terme d'apprentissage que de s'impliquer activement au sein de l'équipe qui fait le boulot. Vous pouvez apprendre à quel point les tâches quotidiennes peuvent être difficiles ou ennuyeuses. Vous pouvez voir à quel point l'équipe peut être gênée par les interruptions, les risques et l'incertitude.

One can establish a relationship of honest feedback with others regardless of position in a hierarchy. It has to do with respect and straightforward communication, but also with support and relationship.  

Il est possible d'établir une relation honnête avec les autres sans tenir compte de la position hiérarchique. Il est question ici de respect et de communication directe mais aussi de soutien et de qualité de la relation.

>   
> B: Notice that they've gone from 19 to 23 points & you don't know how they did it.  
> A: I assumed that they went from 19 to 23 because they're working harder.  
> B: Yes, you did.

>   
> B : Vous avez remarqué que l'équipe est passée de 19 à 23 points et que vous ne savez pas comment elle a fait.  
> A : Je suppose qu'elle est passée de 19 à 23 parce qu'elle a travaillé plus dur.  
> B : Oui, vous avez raison.

We can often assume that "working harder" is the answer. There is a disconcerting belief that workers are withholding their effort and only a stern word or motivational speech from their manager will get them to actually make an effort. This is a wrong and dangerous idea. [Even when it seems true it is the wrong dangerous idea](https://agileotter.blogspot.com/2015/09/confirmation-bias-and-twelve-day.html) to have.  

Nous supposons souvent que « travailler plus dur » est la réponse. C'est une croyance déconcertante que les collaborateurs retiennent leur efforts et que seul un avertissement sévère ou un discours motivant de leur manager va leur faire faire cet effort. C'est une idée fausse et dangereuse. [Même si elle semble vrai, il s'agit d'une idée dangereuse](https://agileotter.blogspot.com/2015/09/confirmation-bias-and-twelve-day.html).

[Peter Scholtes](https://en.wikipedia.org/wiki/Peter_Scholtes) said this:  

[Peter Scholtes](https://en.wikipedia.org/wiki/Peter_Scholtes) a dit ceci :  


> **The greatest managerial cynicism** is that workers are withholding a certain amount of effort that must be bribed from them by means of various incentives, rewards, contests, or merit pay programs. Most managers are not conscious of such a pessimistic belief, but many of their "motivational programs" are conducted as though this cynical premise were true.

> **Le plus grand cynisme managériale** c'est lorsque les collaborateurs retiennent leur effort, de les leur soutirer de différentes manières : récompenses, compétitins, ou programme de prime au mérite. La plupart des managers ne sont pas conscient de cette croyance pessimiste, mais une grande partie de leur « programme de motivation » est faite comme si cette prémisse était vraie.  

We don't want our people to be _working harder_. We want them to be _more accomplished_. If we conflate the goals then we are in the kinds of problems we discussed in [Part V](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-v.html) when we said "take away their tools." Making their lives hard does nothing useful for the bottom line.  

Nous ne voulons pas que nos collaborateurs _travaillent plus dur_. Nous voulons qu'ils soient _plus accomplis_. Si nous confondons les objectifs alors nous nous retrouvons dans les types de problèmes dont nous avons discuté dans la [partie V](http://www.les-traducteurs-agiles.org/2019/07/15/questions-reponses-a-propos-de-la-velocite-5eme-partie.html) lorsque nous avons parlé de « leur prendre leurs outils ». Leurs rendre la vie plus difficile ne donne rien de bon au niveau du résultat.

Join us for [Part X](https://agileotter.blogspot.com/2019/09/q-and-on-velocity-part-x.html) when we talk about learning, experimenting, and accelerating processes.

Joignez-vous à nous pour la [partie X](https://agileotter.blogspot.com/2019/09/q-and-on-velocity-part-x.html) où nous parlerons expérimentation et accélération des processus.

---
Auteur : Tim Ottinger  
Source : [Q and A on velocity, Part IX ](http://agileotter.blogspot.com/2019/08/q-and-on-velocity-part-ix.html)  
Date de parution originale : 22 Août 2019  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : --/11/2020  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

---
layout: post
title:  "Questions/Réponses à propos de la vélocité 5ème partie"
date:   2019-07-14 00:00
published: true
tags:
- vélocité
---

In [Part IV](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-iv.html), we talked about the thorny clashes between the reality of promises, and the reality of development. This installment picks up on some truths about working harder and going faster.  

Lors de la [4ème partie](http://www.les-traducteurs-agiles.org/2019/05/26/questions-reponses-a-propos-de-la-velocite-4eme-partie.html), nous avons abordé les confrontations plutôt épineuses qu'il peut y avoir entre la réalité des promesses, et la réalité du développement. Cet épisode revient sur certaines vérités au sujet de travailler plus dur et d'aller plus vite.

> A: Wait a second... You never actually said we can't go faster. You only said that trying harder and adding people weren't the way.  
>
> B: That is true.  
>
> A: So we _could_ possibly go faster?  
>
> B: Certainly.  

> A: Attendez une seconde ... Vous n'avez jamais parlé en fait que nous ne pouvons pas aller plus vite. Vous avez seulement dit qu'essayer de manière plus poussée ou d'ajouter davantage de personne n'était pas la voie à suivre.  
>
> B: C'est vrai.  
>
> A: Donc nous _pourrions_ aller plus vite ?  
>
> B: Tout à fait.  

Frankly, we don't know how fast developers might be able to go. I've had friends call and tell me about taking on work that was estimated and doing it in a morning when the code was well-factored, readable, and well-tested. My friend said that "all the functions I needed were already written and easy to find."  

Pour parler franchement, nous n'avons aucune idée de la vitesse à laquelle des développeurs seraient capable d'atteindre. Un ami m'a appelé et m'a raconté avoir pris en charge un travail qui avait été estimé et de l'avoir réalisé en une matinée car le code était bien structuré, lisible et bien testé. Mon ami m'a dit "toutes les fonctions dont j'avais besoin avaient déjà été écrites et faciles à trouver"

Robert Martin always said that the speed of today's development work mainly depends on the quality of the code you will be working on. Low-quality code? Low speed. High-quality code? High speed.  

Robert Martin dit toujours que la vitesse des travaux de développement d'aujourd'hui dépend principalement de la qualité du code sur lequel vous allez travailler. Du code de mauvaise qualité ? Petite vitesse. Du code de très bonne qualité. Grande vitesse.

In addition, we've asked around and found that developers spend about 25% of their time in meetings (the more senior spend more time). That's 25% right off the top.  

En plus, nous avons fouiné un peu partout et avons constaté que les développeurs passent environ 25% de leur temps en réunion (les plus séniors passant plus de temps). C'est 25% tout de suite.

Of the time remaining, most developers are spending 60%-80% of their time fixing defects. That's a heck of a lot of time. If they could go two times slower, but produce no bugs, they would be at least 10% faster.  

La plupart des développeurs passent en partie le reste de leurs temps, environ 60 à 80% à corriger des anomalies. C'est un sacré bout de temps; S'ils pouvaient aller deux fois moins vite, mais en ne produisant aucune anomalie, ils iraient au moins 10% plus vite.

Of the time that's left, silos and approval processes and other interruptions force developers to spend a bit of their time waiting for other people. Work sits in queues.  

Par rapport au temps qu'il reste, le travail en silos, les mécanismes d'approbation dans le processus de travail et autres interruptions obligent les développeurs à passer une partie de leurs temps à attendre d'autres personnes. Le travail fait la queue dans une file d'attente.

And of course, when a programmer's work has to wait in a queue, the conscientious programmer keeps busy by pulling an extra task off the queue.  

Et bien sur, lorsque le travail d'un développeur attend dans une queue, le programmeur consciencieux reste occupé en prenant du boulot supplémentaire supplémentaire de ce qu'il y a dans sa propre liste de choses à faire.

Now when work is returned from testing, or from an approver, or from some kind of review, it has to sit in a queue waiting for the developer to be available again. The average corporate programmer we asked has about 5 concurrent tasks (or branches) open. It can be as high as 15.  

Toutefois lorsque les travaux reviennent des tests, ou de la validation, ou d'une autre forme de revue, ces travaux doivent rejoignent la file d'attente pour que le développeur soit à nouveau disponible pour les prendre en charge. Le développeur moyen type en entreprise que nous avons pu interroger a envirn 5 tâches concurrentes (ou branches) ouvertes. Cela peut monter jusqu'à 15.

You can see the time is whittled away to near-nothingness. It's no surprise that a piece of work takes forever to develop, even though the developer is busy and has a lot of tasks in progress at any given time.  

Vous pouvez voir le temps se réduire à peau de chagrin. Cela n'est en aucun cas surprenant qu'un bout de travail puisse prend un temps infini à être développé, même si le développeur est occupé et a beaucoup de tâches en cours à n'importe quel moment.

Developers say "I'm not blocked, I have plenty of other tasks to work on," and it's true. But _**the work itself**_ is blocked. The work is not going to production soon enough _because_ the developers are busy doing something else. This is why Lean advocates say "watch the baton, not the runner."  Flow efficiency is about the throughput of a system, not about the busyness of the workers.  

Les développeurs disent "Je ne suis pas bloqué, j'ai plein d'autres choses sur lesquelles travailler" et c'est vrai. Mais _**le travail lui en tant que tel**_ est bien bloqué. Le travail ne va pas aller suffisamment tôt en production _parce que_ les développeurs sont occupés à faire quelque chose d'autre. C'est pourquoi les pratiquants Lean disent "regarder le bâton, pas le coureur." L'efficacité du flux est lié au débit d'un système, non sur la charge des employés.

It's a messy system, made messier by processes that include a lot of silos, individual effort, quick plate-emptying, approval cycles, branches, and what-not.  

C'est un système bordélique, rendu encore plus bordélique par des processus incluant de nombreux silos, d'efforts individuels, un vidage rapide d'assiette, cycles d'approbations, de branches et je ne sais quoi encore.

**Most of our systems seem to do more software   
prevention than software development.**  

**La plupart de nos systèmes semblent faire plus de la prévention   
logiciel plus que du développement logiciel**
{: style="text-align: center;"}

But still, the quality of the code is the big determinant. If the code is well-organized, and good tooling is used, and the developer is familiar with the system, and the change doesn't introduce any major architectural rearrangements, ... well, how amazingly fast might it be?  

Mais toutefois, la qualité du code est le grand déterminant. Si le code est bien organisé, et qu'un bon outillage est utilisé, et que le développeur est familier avec le système, et le changement n'introduit pas de réarrangements architecturaux majeurs; … eh bien, quelle vitesse surprenante pourrait-il bien atteindre

Faster should be easily possible, but getting there may be hard human work, and not just for developers.  

Il serait facile d'aller plus file, mais arriver là peut s'avérer être un travail acharné du point de vue humain et pas uniquement pour les développeurs.

On the topic of hard human work:  

À ce sujet :

> A: So how can we get the developers to work harder?  
>
> B: Take away their tools. Add more bureaucracy. Use slow computers and dead programming languages.  
>
> A: And that will bring up the velocity?  
>
> B: No. You asked how to make their work harder.
 This highlights a problem in the approach to getting more done.  In [Part II](https://agileotter.blogspot.com/2018/07/q-on-velocity-part-ii.html), we hinted at this. [In 2009's Platitudes of Doom](http://agileotter.blogspot.com/2009/08/platitudes-of-doom.html) article, we went on about this at length. There is this assumption that the reason work is slow is that people aren't working hard enough.  

> A: Donc, comment pouvons-nous amené les développeurs à redoubler d'effort ?  
>
> B: Enlevez-leurs leur outils. Ajoutez plus de bureaucracie. Faites-leur utiliser des ordinateurs plus lents et d'anciens langages de programmaiton.  
>
> A: Et cela va ramener de la vélocité ?  
>
> B: Non. Vous avez demandé à comment les faire redoubler d'efforts.
 Ceci met en lumière un problème dans l'approche d'en faire plus. Dans la [deuxième partie](http://www.les-traducteurs-agiles.org/2019/01/29/questions-reponses-a-propos-de-la-velocite-2eme-partie.html), nous avons fait allusion à cela. Dans mon article de 2009 intitulé [Platitudes of Doom](http://agileotter.blogspot.com/2009/08/platitudes-of-doom.html)[^1] article,nous avons traité de cela en profondeur. Il y a ce postulat qui est que la raison pour laquelle le travail avance lentement c'est parce que les personnes ne travaillent pas avec assez d'acharnement.  

The focus on business and effort is not helpful.  

Être focalisé sur la charge et les efforts n'est d'aucune aide.

The above conversation is a bit tongue-in-cheek but illustrates the point that the problem isn't in busyness and effort expended, but in results being attained.   Most programmers are working far harder than they should have to and creating far less value in doing so.  

La conversation précédente est un peu ironique mais illustre le point que le problème n'est pas dans la charge et dans les efforts accrus, mais dans les résultats obtenus. La plupart des programmeurs travaillent bien plus dur qu'ils ne le devraient et créent de cette manière bien moins de valeur.

If we insist on putting more effort into the work, we end up getting more brute-force, and not the best results we hope for. This will be discussed more whenever I get into writing up **The Journey**.  

Si nous insistons à mettre plus d'effort dans le travail, nous finissons par obtenir par quelque chose qui ressemble à plus de la force brute, et non avec de meilleurs résultats comme nous pouvons espérer. Cela sera abordé de manière plus approfondie lorsque je me mettrai à l'écriture de **The Journey**.

> A: We want them to work harder so that we get more done.  
>
> B: If you want to accomplish more, shouldn't you make the work _less hard_?  
>
> A: We just want it done.  
>
> B: Of course, and so do they.
Here is the interesting magic. If we want people to get more done, we are more likely to succeed in removing the waste and uncertainty and risk from the process, rather than by putting greater effort and strain into it.  

> A: Nous voulons qu'ils travaillent plus dur afin que nous puissions faire plus de choses.  
>
> B: Mais si vous voulez accomplir davantage, ne devriez-vous pas rendre le travail _moins dur_ ?  
>
> A: Nous voulons juste que le boulot soit fait.  
>
> B: Bien sûr, et eux aussi..
Voici ce quelque chose de magique et d'intéressant. Si nous voulons que les gens puissent en faire plus, nous aurons probablement plus de chances de réussir en enlevant tout le superflu, l'incertitude, et le risque du processus, plutôt que d'y mettre de plus grand efforts et d'y mettre plus de pression.  

Again, [in part II](https://agileotter.blogspot.com/2018/07/q-on-velocity-part-ii.html) we talked about the formula of effort provided to do a task over effort required. Scroll down to the graphic that illustrates this point and the text that surrounds it.  

De nouveau, dans la [3ème partie](http://www.les-traducteurs-agiles.org/2019/04/08/questions-reponses-a-propos-de-la-velocite-3eme-partie.html), nous avons évoqué la formule de l'effort fourni pour faire une tâche par rapport à l'effort demandé. Allez juqu'au diagramme illustrant ce oint et le texte associé.

 This snippet of the discussion is really just restating the points that you've already seen.  But there is some chance that you are not a long-time reader of this humble blog, out in the wastelands of blogger's dark corner, so maybe it will help to give you some more reading on the topic. To wit:  

Cet extrait de la discussion a pour de but de simplement redire les points que vous avez déjà vu. Mais il y a une certaine probabilité que vous n'êtes pas un lecteur de longue date de ce modeste blog, perdu dans un coin sombres dans les vastes terres des bloggueurs, donc cela vous aidera peut être d'avoir davantage de chsoes à lire sur ce sujet. À savoir :

* [Part III ](https://agileotter.blogspot.com/2018/07/q-and-on-velocity-part-iii.html)talks about uncertainty, risk, and effort. This is a helpful context.

* LA [3ème partie](http://www.les-traducteurs-agiles.org/2019/04/08/questions-reponses-a-propos-de-la-velocite-3eme-partie.html) aborde les sujets de l'incertitude, du risque et de l'effort. Cela peut s'avérer utile.

* It can be [unsafe to increase effort](https://agileotter.blogspot.com/2013/05/increasing-effort-is-unsafe-in-too-many.html).

* Il peut être [dangereux d'accroître les efforts](https://agileotter.blogspot.com/2013/05/increasing-effort-is-unsafe-in-too-many.html)[^1].

* The presence of [uncertainty, risk, and effort](https://agileotter.blogspot.com/2018/03/predictability-as-maturity-or-system.html) confound predictability and must be considered.

* La présence d'[incertitude, de risque et d'efforts](https://agileotter.blogspot.com/2018/03/predictability-as-maturity-or-system.html)[^1] viennent contrecarrer la prévisibilité et doivent être pris en considération.

* However, these issues are inextricable parts of programming, which is [mostly thinking](https://agileotter.blogspot.com/2014/09/programming-is-mostly-thinking.html).

Toutefois, ces éléments font partie de manière inextricable de la programmation, qui consiste [majoritairement à réfléchir](https://agileotter.blogspot.com/2014/09/programming-is-mostly-thinking.html)[^1].

* As such, we don't know that the work we're given[ is even possible ](https://agileotter.blogspot.com/2014/10/preplanning-poker-is-this-story-even.html)sometimes.

* En tant que tel, nous ne savons pas si le boulot qu'on nous donne [est même possible](https://agileotter.blogspot.com/2014/10/preplanning-poker-is-this-story-even.html)[^1] certaines fois.

Maybe the programming isn't slow, considering the condition of the code base and the presence of risk and uncertainty in the requirements, the difficulty of predicting intellectual effort, etc.

Peut être que la programmantion n'est pas lente, si l'on considère l'état de la base du code et la présence du risque et de l'incertitude dans les exigences, la difficulté de prévoir l'effort intellectuel, etc.


**Maybe the estimates are low, rather than the work being slow?**

**Peut-être que les estimations sont basses au lieu de dire que le travail est lent**

**We don't really know.**

**Nous ne savons pas vraiment.**

We only know that there exists a difference between what we expect (and want) and what we are really achieving. We can look at that as a betrayal, or we can look at it as[ a curiosity space](https://agileotter.blogspot.com/2016/08/the-curiosity-space.html).  

Nous savons seulement qu'il existe une différence entre ce que nous nous attendons (et voulons) et ce que nous réalisons vraiment. Nous pouvons considérer cela comme d'une trahison, ou nous si nous pouvons la considérer comme d'un [espace de curiosité](http://www.les-traducteurs-agiles.org/2016/10/16/espace-de-curiosite.html)

I know which of those choices leads to blame and frustration, and which leads to alignment and improvement.

je sais quels sont les choix qui mènent au blame et à la frustration, et lesquels mène à l'alignement et à l'amélioration.

But I'll let you ponder that until [Part VI](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-vi.html).

Mais je vais vous laisser méditer là-dessus jusqu'à la [6ème partie](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-vi.html)

[^1]: en vo

---
Auteur : Tim Ottinger  
Source : [Q and A on Velocity, part V](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-v.html)  
Date de parution originale : 23 Octobre 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 14/07/2019  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

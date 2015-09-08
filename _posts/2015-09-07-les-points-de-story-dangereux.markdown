---
layout: post
title:  "Les story points considérés comme dangereux - ou pourquoi le futur de l'estimation se situe vraiment dans notre passé"
date:   2015-09-07 21:00:55
published: false
categories: 
- estimation
---

Wednesday, January 25, 2012
# Story Points Considered Harmful - Or why the future of estimation is really in our past...

# Les story points considérés comme dangereux - ou pourquoi le futur de l'estimation se situe vraiment dans notre passé.

This article is the companion to a [talk](http://www.sigs-datacom.de/oop2012/oop2012-eng/conference/sessiondetails.html?tx_mwconferences_pi1[showUid]=818&tx_mwconferences_pi1[anchor]=%23Ndo3&tx_mwconferences_pi1[s]=0) that myself and [@josephpelrine](https://twitter.com/josephpelrine) gave at OOP 2012.

Cet article est le pendant de la [conférence](http://www.sigs-datacom.de/oop2012/oop2012-eng/conference/sessiondetails.html?tx_mwconferences_pi1[showUid]=818&tx_mwconferences_pi1[anchor]=%23Ndo3&tx_mwconferences_pi1[s]=0) que [@josephpelrine](https://twitter.com/josephpelrine) et moi-même avons donné à l'OOP 2012.

http://1.bp.blogspot.com/-EUBtGnhNy1Y/TyCFzQjVwLI/AAAAAAAAAQA/HfV1jBwZwzM/s1600/Stars%2Bbanner.jpg

We have a lot to learn from our ancestors. One that I want to focus on for this post is [Galileo](https://fr.wikipedia.org/wiki/Galil%C3%A9e_%28savant%29).
Galileo was what we would call today a techie. He loved all things tech and was presented an interesting technology that he could not put down. Through that work he developed optic technology to build first a telescope and later a microscope.
Through the use of the telescope and other approaches he came to realize and defend the [Heliocentric](http://en.wikipedia.org/wiki/Heliocentrism) view of the universe: the Earth was not the center of the Universe, but rather moved around the Sun.
This discovery caused no controversy until Galileo wrote it down and apparently discredited the view held by the Church at that time. The Church believed and defended that the Universe was neatly organized around the Earth and everything moved around our lanet.
We now know that Galileo was right and that the Church was - as it often tends to be with uncritical beliefs - wrong. We now say obviously the Earth is round and moves around the Sun. Or do we...

Nous avons beaucoup à apprendre de nos ancêtres. Celui que je veux mettre en avant plus particulièrement pour cet article est [Galilée](https://fr.wikipedia.org/wiki/Galil%C3%A9e_%28savant%29).
Galilée a été ce que nous appellerions aujourd'hui un technophile. Il aimait tout ce qui était techno et un jour, il lui fut présenté une technologie intéressante qu'il ne pouvait pas ignorer. Grâce à elle, il développa la technologie optique pour construire d'abord le téléscope et plus tard le microscope. Grâce à l'utilisation du télescope et d'autres approches, il arriva à la constatation et à la défense d'une conception [héliocentrique](https://) de l'univers : la Terre n'était pas le centre de l'univers, mais plutôt tournait autour du soleil.
Cette découverte ne provoqua pas de controverse jusqu'à ce que Galilée l'écrivit et discrédita à priori la conception défendu par l'Église à cette époque. L'Église croyait et défendait la conception que l'univers était organisé de manière ordonné autour de la terre et que toute chose tournait autour de notre planète.
Nous savons maintenant que Galilée avait raison et que l'Église avait - comme souvent cela tends à être le cas avec les croyances - tort. De nos jours, nous disons de manière évidente que la terre est ronde et tourne autour du soleil. Ou est-ce que nous ...

## The Flat Earth Society

## La société de la terre plate

Actually, there are still many people around (curious word, isn't it?) the planet that do not even believe that the Earth is round! Don't believe me? Then check [The Flat Earth Society](http://en.wikipedia.org/wiki/Flat_Earth_Society).

Pour de vrai, il y a encore des gens autour (bizarre comme mot, hein ?) du globe qui ne croient même pas que la terre est ronde !  Vous ne me croyez pas ? Alors regardez par vous même la [société de la terre plate](https://).

The fact that is that even today many people hold uncritical beliefs about how our world really works. Or our projects in the case of this post...

Le fait est que même aujourd'hui, il y a beaucoup de gens qui ont des croyances sur comment notre monde tourne vraiment. Ou nos projets dans le cas de cet article ...

## Estimation soup

## La soupe de l'estimation

We've all been exposed to various estimation techniques, in an Agile or traditional project. Here are some that quickly come to mind: Expert Estimation, Consensus Estimation, Function Point Analysis, etc. Then we have cost (as opposed to only time) estimation techniques: COCOMO, SDM, etc. And of course, **the topic of this post: Story Point Estimation. What do all of these techniques have in common? They all look towards the future!**
Why is this characteristic important?

Nous avons tous vu différentes techniques d'estimation que ce soit dans un projet agile ou traditionnel. En voici quelques uns qui viennent tout de suite à l'esprit : estimation par un expert, estimation par consensus, analyse par point de fonction, etc ... Puis nous avons les techniques d'estimation du coût (par opposition à celui portant uniquement sur le temps) : COCOMO, SDM, etc ... Et bien sûr, **le sujet de cet article : l'estimation en point de story. Qu'est que toutes ces techniques ont en commun ? Elles regardent toutes vers le futur !**
Pourquoi est ce que cette caractéristique est-elle importante ?

## The Human condition

## La condition humaine

This characteristic is nt because looking at the future is always difficult! We humans are very good at anticipating immediate events in the physical world, but in the software world what we estimate is neither immediate, nor does it follow any physical laws that we intuitively understand!
Take the example of a goal-keeper in a football (aka soccer) match. She can easily predict how a simple kick will propel the ball towards the goal, and she can do that with quite a high accuracy (as proven by the typically low scores in today's football games). But even in soccer, if you face a player like [Maradona](http://en.wikipedia.org/wiki/Diego_Maradona), or [Beckham](http://en.wikipedia.org/wiki/David_Beckham), or [Crisitiano Ronaldo](http://en.wikipedia.org/wiki/Cristiano_Ronaldo) it is very difficult to predict the trajectory of the ball. Some physicists have spent considerable amount of time analyzing the trajectory of Beckham's amazing free kicks to try to understand how the ball moves and why. Obviously a goal-keeper does not have the computers or the time to analyze the trajectory of Beckham's free kicks therefore Beckham ends up scoring quite a few goals that way. **Even in football, where well-known physics laws always apply it is some times hard to predict the immediate future!**
The undisputed fact is that we, humans are very bad at predicting the future.
But that is not all!

Ce n'est pas parce que regarder vers le futur est toujours difficile ! Nous, humains excellons à anticiper les évènements immédiats dans le monde physique, mais dans le monde du logiciel ce que nous estimons n'est ni immédiat, ni ne suit aucune des lois physiques que nous comprenons intuitivement !
Prenez l'exemple du gardien de but dans un match de football. Il peut facilement prédire comment une simple frappe propulsera le ballon vers les buts, et il pourra faire cela avec une assez bonne précision (comme le prouve les scores habituellement faibles dans les matchs de football d'aujourd'hui). Mais même dans le football, lorsque vous êtes face à un joueur comme [Maradona](http://fr.wikipedia.org/wiki/Diego_Maradona), or [Beckham](http://fr.wikipedia.org/wiki/David_Beckham), or [Crisitiano Ronaldo](http://fr.wikipedia.org/wiki/Cristiano_Ronaldo) cela devient très difficile de prévoir la trajectoire de la balle. Certains physiciens ont passé un temps considérable  à analyser la trajectoire des coups francs de Beckham pour essayer de comprendre comment la balle se déplaçait et pourquoi. De manière évidente, un gardien de but n'a pas les ordinateurs ou le temps d'analyser la trajectoire des coups francs de Beckham, par conséquent cela a permis à Beckham de marquer un certain nombre de buts de cette manière. **Même dans le football, où des lois bien connues de la physique s'appliquent, il y a des fois où cela devient difficile de prédire le futur immédiat !**
C'est un fait indiscutable que nous, humains, sommes très mauvais à prédire le futur.
Mais ce n'est pas tout !

## This is when things get Complex

## C'est maintenant que les choses deviennent complexes

Lately, and especially in the agile field we have been finding a new field of study: Complexity Sciences.
A field of study that tries to identify rules that help us navigate a world where even causality (cause and effect) are challenged.
An example may be what you may have heard of, the Butterfly effect: "where a small change at one place in a nonlinear system can result in large differences to a later state".
Complexity Sciences are helping us develop our own understanding of software development based on the theories developed in the last few years.
Scrum being a perfect example of a method that has used Complexity to inspire and justify its approach to many of the common problems we face in Software development.
Scrum has used "self-organization", and "emergence" as concepts in explaining why the Scrum approach works. Here's the problem: there's a catch.

Dernièrement, et tout spécialement dans le domaine agile, nous avons trouvé un nouveau domaine d'étude : les sciences de la complexité.
Il s'agit d'un domaine d'étude qui essaye d'identifier les règles qui nous permettent de nous déplacer dans un monde où la causalité même (cause et effet) est remise en question.
Un exemple dont vous avez peut être entendu parler est l'effet papillon : "où un petit changement quelque part dans un système non linéaire peut avoir comme résultat des différences importances à un état ultérieur". Les sciences de la complexité nous permettent d'accroître notre compréhension du développement logiciel sur la base des théories développées ces dernières années.
Scrum est le parfait exemple d'une méthode qui a utilisé la complexité pour s'inspirer et justifier son approche sur beaucoup des problèmes habituels auxquels nous sommes confrontés dans le développement logiciel.
Scrum a utilisé "l'auto-organisation", et "l'émergence" comme concepts pour expliquer pourquoi l'approche Scrum fonctionne. Voici le problème : il y a un piège.

## Why did this just happen?

## Pourquoi est-ce que cela est arrivé ?

In a complex environment we don’t have discernible causality!
Sometimes this is due to delayed effects from our actions, most often it is so that we attribute causality to events in the past when in fact no cause-effect relationship exists (Retrospective Coherence). But, in the field of estimation this manifests itself in a different way.
In order for us to be able to estimate we need to assume that causality exists (if I ask Tom for the code review, then Helen will be happy with my pro-activeness and give me a bonus. Or will she?) The fact is: in a Complex environment, this basic assumption of the existence of discernible Causality is not valid! **Without causality, the very basic assumption that justifies estimation falls flat!**

Dans un environnement complexe, nous n'avons pas de causalité discernable !
Quelque fois cela est dû aux conséquences retardées de nos actions, d'ailleurs c'est tellement le cas, le plus souvent que nous attribuons la causalité des évènements dans le passé alors qu'en fait il n'y a aucune relation de cause à effets (cohérence rétrospective). Mais dans le domaine de l'estimation, cela se manifeste d'une autre manière.
Afin que nous puissions estimer nous devons présumer que la causalité existe (si je demande à Tom de faire une revue de code, alors Helen sera contente que je sois pro-actif et me donnera un bonus. N'est-ce pas ?) Le fait est : que dans un environnement complexe, la présomption de base est que l'existence d'une causalité discernable n'est pas valide ! **Sans causalité, la présomption même de base qui justifie l'estimation tombe à plat !**

## Solving the the lack of internal coherence in Scrum

## Résoudre le manque de cohérence interne de Scrum

So, which is it? Do we have a complex environment in software development or not? If we do then we cannot - at the same time - argue for estimation (and build a whole religion on it)! In contrast, if we are not in a complex environment we cannot then claim that Scrum - with it’s focus on solving a problem in the complex domain - can work!
**So then, the question for us is: Can this Story Point based estimation be so important to the point of being promoted and publicized in all Scrum literature?**
Luckily we have a simple alternative that allows for the existence of a complex environment and solves the same problems that Story Points were designed (but failed to) solve.

Alors, quel est-il ? Avons-nous un environnement complexe dans le domaine du développement logiciel ou pas ? Si nous en avons un alors nous ne pouvons pas - en même temps - argumenter en faveur de l'estimation (et bâtir toute une religion dessus) ! À contrario, si nous ne sommes pas dans un environnement complexe nous ne pouvons pas alors proclamer que Scrum - avec son accent mis sur la résolution de problème dans un domaine complexe - puisse fonctionner !

## The alternative prediction device

## L'outil de prédiction alternatif

The alternative to Story Point estimation is simple: just count the number of Stories you have completed (as in "Done") in the previous iterations. They are the best indicator of future performance! Then use that information to project future progress. Basically, the best predictor of the future is your past performance!
Can it really be that simple? To test this approach I looked at data from different projects and tried to answer a few simple questions

L'alternative à l'estimation en story points est simple : compter seulement le nombre de stories que vous avez terminées (comme étant "finies") dans les itérations précédentes. Elles sont le meilleur indicateur d'une futur performance ! Utilisez alors cette information pour projeter les futurs avancées. De manière très basique, le meilleur indicateur du futur est votre performance passée !
Est-ce vraiment aussi simple ? Pour tester cette approche j'ai examiné les données de différents projets et j'ai essayé de répondre à quelques questions simples. 
 
## The Experiment

## L'expérience

* Q1: Is there sufficient difference between what Story Points and ’number of items’ measure to say that they don’t measure the same thing?
* Q2: Which one of the two metrics is more stable? And what does that mean?
* Q3: Are both metrics close enough so that measuring one (number of items) is equivalent to measuring the other (Story Points)?

* Q1 : Existe-t-il une différence suffisante entre ce que les story points et la mesure du "nombre d'éléments" pour dire qu'ils ne mesurent pas la même chose ?
* Q2 : Laquelle de ces deux métriques est-elle la plus stable ? Et qu'est-ce que cela signifie ?
* Q3 : Est-ce que ces métriques sont-elles assez proches afin que la mesure de l'un (le nombre d'élément) soit équivalente à la mesure de l'autre (story points) ? 

I took data from 10 different teams in 10 different projects. I was not involved in any of the projects (I collected data from the teams directly or through requests for data in Agile-related mailing lists). Another point to highlight is that this data came from different size companies as well as different size teams and projects.
And here's what I found:

J'ai examiné les données de 10 équipes différentes de 10 projets différents. Je ne faisais pas partie d'aucun de ces projets (j'ai récupéré ces données des équipes directement ou par le biais de demandes d'informations dans les listes de diffusion dédié à l'agilité). Un autre point à souligner est que ces données viennent d'entreprises de tailles différentes aussi bien que tailles d'équipes et de projets différentes.
Et voici ce que j'ai trouvé :

* Regarding Question 1: I noticed that there was a stable medium-to-high correlation between the Story Point estimation and the simple count of Stories completed (0,755; 0,83; 0,92; 0,51(!); 0,88; 0,86; 0,70; 0,75; 0,88). With such a high correlation it is likely that both metrics represent a signal of the same underlying information.
* Regarding Question 2: The normalized data (normalized for Sprint/Iteration length) has similar value of Standard Deviation(equally stable). Leading me to conclude that there is no significant difference in stability of either of the metrics. Although in absolute terms the Story Point estimations vary much more between iterations than the number of completed/Done Stories
* Regarding Question 3: Both metrics (Story Points completed vs Number of Stories completed) seem to measure the same thing. So...

* Sur la question 1 : j'ai remarqué qu'il y avait une corrélation moyenne à élevée stable entre l'estimation en story points et le comptage simple des stories terminées (0,755; 0,83; 0,92; 0,51(!); 0,88; 0,86; 0,70; 0,75; 0,88). Avec une corrélation si élevée, il est probable que les deux métriques représentent le signal d'une même information sous-jacente.
* Sur la question 2 : Les données normalisées (normalisées pour la durée d'un sprint ou d'une itération) ont la même valeur d'écart-type (tout aussi stable). Cela m'amène à conclure qu'il n'y a pas de différence significative de stabilité de l'une ou l'autre de ces métriques. Même si en valeurs absolues les estimations en story points varient plus entre deux itérations que le nombre de stories terminées/finies.
* Sur la question 3 : Les deux métriques (les points de stories terminées par rapport au nombre de stories terminées) semblent mesurer la même chose. Donc ...

At this point I was interested in analyzing the claims that justify the use of Story Points, as the data above does not seem to suggest any significant advantage of using Story Points as a metric. So I searched for the published justification for the use of Story Points and found a set of claims in Mike Cohn's book "User Stories Applied" (page 87, first edition):

À partir de là, je me suis intéresser à l'analyse des arguments justifiant l'utilisation des story points, comme les données précédentes ne semble pas donner un avantage significatif pour l'utilisation des story points comme métrique. J'ai donc cherché une publication justifiant l'utilisation des story points et j'ai trouvé un ensemble d'arguments dans le livre "User Stories Applied" (page 87, 1ère édition) de Mike Cohn.

* Claim 1: The use of Story points allows us to change our mind whenever we have new information about a story
* Claim 2: The use of Story points works for both epics and smaller stories
* Claim 3: The use of Story points doesn’t take a lot of time
* Claim 4: The use of Story points provides useful information about our progress and the work remaining
* Claim 5: The use of Story points is tolerant of imprecision in the estimates
* Claim 6: The use of Story points can be used to plan releases

* Argument 1 :  L'utilisation des story points nous permet de changer d'avis lorsque nous avons une nouvelle information sur une story
* Argument 2 : L'utilisation des story points fonctionne à la fois pour les _epics_ et les stories plus petites
* Argument 3 : L'utilisation des story points ne prend pas beaucoup de temps
* Argument 4 : L'utilisation des story points donne des informations utiles sur notre avancée et le travail restant à faire
* Argument 5 : L'utilisation des story points tolère une certain imprécision dans les estimations
* Argument 6 : L'utilisation des story points peut être utilisée pour planifier les livraisons

This these claims hold?

Est-ce que ces arguments tiennent ?

## Claim 1: The use of Story points allows us to change our mind whenever we have new information about a story

## Argument 1 : L'utilisation des story points nous permet de changer d'avis lorsque nous avons une nouvelle information sur une story

Although there's no explanation about what "change our mind" means in the book, one can infer that the goal is not to have to spend too much time trying to be right. The reason for this is, of course, that if a story changes the size slightly there's no impact on the Story Point estimate, but what if the story changes size drastically?
Well, at this time you would probably have another estimation session, or you would break down that story into some smaller granularity stories to have a better picture of it's actual size and impact on the project.
On the other hand, if we were to use a simple metric like the number of stories completed we would be able to immediately assess the impact of the new items in the progress for the project.

Même s'il n'y a pas d'explications sur ce que "changer d'avis" veut dire dans le livre, nous pouvons en déduire que l'objectif n'est pas de passer trop de temps à essayer d'être exact; La raison pour ceci est, bien sûr, que si la story change de taille légèrement, il n'y a aucun impact sur l'estimation en story points, mais et si la story change de taille drastiquement ?
Eh bien, à ce moment-là vous voudriez probablement avoir une nouvelle session d'estimations, ou vous voudriez scinder cette story en stories plus petites pour avoir une meilleure image de sa taille et de son impact réel sur le projet.
D'un autre côté, si nous devions utiliser une métrique simple comme le nombre de stories terminées, nous serions capable d'évaluer immédiatement l'impact de nouveaux éléments dans l'avancée du projet.

http://91.68.209.12/bmi/3.bp.blogspot.com/-Cj3pwyqlG2g/Tx_i9xuGIDI/AAAAAAAAAPc/I5bSB8gG0s8/s320/claim%2B1%2Bgraph.jpg

As illustrated in the graph, if we have a certain number of stories to complete (80 in our example) and suddenly some 40 are added to our backlog (breaking down an Epic for example) we can easily see the impact of that in our project progress.
In this case, as we can see from the graph, the impact of a story changing it's meaning or a large story being broken down into smaller stories has an impact on the project and we can see that immediate impact directly in the progress graph.
This leads me to conclude that **regarding Claim 1, Story Points offer no advantage over just simply counting the number of items left to be Done**.

Comme illustré dans le graphique, si nous avons un certain nombre de stories à terminer (80 dans notre exemple) et que brusquement 40 sont ajoutés dans notre backlog (à partir de la scission d'un _epic_ par exemple) nous pouvons voir facilement l'impact que cela peut avoir sur l'avancée de notre projet.
Dans ce cas, comme nous pouvons le voir à partir du graphique, l'impact de la modification d'une story ou la division d'une grosse story en plus petites stories ont un impact sur le projet et nous pouvons voir l'impact immédiat directement sur le graphique.
Cela m'amène à conclure que **sur l'argument 1, les story points n'offrent aucun avantage sur le comptage simple du nombre d'éléments restant à finir**.

## Claim 2: The use of Story points works for both epics and smaller stories

Allowing for large estimates for items in the backlog (say a 100SP Epic) does help to account in some way for the uncertainty that large pieces of work represent.
However, the same uncertainty exists in any way we may use to measure progress. The fact is that we don’t really know if an Epic (say 100 SPs) is really equivalent to a similar size aggregate of User Stories (say 100 times 1 SP story). **Conclusion: there is no significant added information by classifying a story in a 100 SP category** which in turn means that calling something an "Epic" is about the same information as classifying it as a 100 Story Points Epic.

## Claim 3: The use of Story points doesn’t take a lot of time

Having worked with Story Points for several years this is not my experience. Although some progress has been done by people like Ken Power (at Cisco) with the [Silent Grouping technique](http://slidesha.re/AgileKonstanz_silentgrouping), the fact that we need such technique should dispute any idea that estimating in SP’s "doesn’t take a lot of time". In fact, as anybody that has tried a non-trivial project knows it can take days of work to estimate the initial backlog for a reasonable size project.


## Claim 5: The use of Story points is tolerant of imprecision in the estimates

Although you can argue that this claim holds - even if the book does not explain how - there's no data to justify the belief that Story Points do this better than merely counting the number of Stories Done. In fact, we can argue that counting the number of stories is even more tolerant of imprecisions (see below for more details on this)

## Claim 6: Story points can be used to plan releases

Fair enough. On the other hand we can use any estimation technique to do this, so how would Story Points be better in this particular claim than any other estimation technique? Also, as we will see when analysis Claim 4, counting the number of Stories Done (and left to be Done) is a very effective way to plan a release (be patient, the example is coming up).

## Claim 4: The use of Story points provides useful information about our progress and the work remaining

This claim holds true **if, and only if** you have estimated all of your stories in the Backlog and go through the same process for each new story added to the Backlog. Even the stories that will only be developed a few months or even a year later (for long projects) must be estimated! This approach is not very efficient (which in fact contradicts Claim 3).
Basing your progress assessment on the Number of Items completed in each Sprint is faster to calculate (number of items in the PBL / velocity in number of items Done per Sprint = number of Sprints left) and can be used to provide critical information about project progress. Here's a real-life example:

## The real-life use of a simpler metric for project progress measurement

In a company I used to work at we had a new product coming to market. It was not a "first-mover" which meant that the barrier to entry was quite high (at least that was the belief from Product Management and Sales).
This meant that significant effort was made to come up with a coherent Product Backlog. The Backlog was reviewed by Sales and Pre-Sales (technical sales) people. All agreed, we really needed to deliver around 140 Stories (not points, Stories) to be able to compete.
As we were not the first in the market we had a tight market window. Failing to meet that window would invalidate the need to enter that market at all.
So, we started the project and in the first Sprint we complete 1 single Story (maybe it was a big story -- truth is I don't remember). Worst, in the same period another 20 stories were added to the Product Backlog. As expected, the Product Management and Sales discovered a few more stories that were really a "must" and could not be left out of the product.
The team was gaining speed and in the second Sprint they got 8 stories to "Done". They were happy. At the same time the Product Manager and the Sales agreed to a cut-down version of the Product Backlog and removed some 20 stories from the Backlog.
After the third sprint the team had achieved velocities of 1 (first Sprint), 8 (second) and 8 (third). The fourth sprint was about to start and the pressure was high on the team and on the Product Manager. During the Sprint planning meeting the team committed to 15 new stories. This was a good number, as a velocity of 15 would make the stakeholders believe that the project could actually deliver the needed product. They would need to keep a velocity of 15 stories per sprint for 11 months. Could they make it?

## The climax

As the fourth sprint started I made a bet with the Product Manager. I asked him how many items he believed that the team could complete and he said 15 (just as the team had committed to). I disagreed and said 10. How many items would you have said the team could complete?
I ask this question from the audience every time I tell this story. I get many different answers. Every audience comes up with 42 as a possible answer (to be expected given the crowds I talk to), but most say 8, 10, some may say 15 (very few), some say 2 (very few). The consensus seems to be around 8-10.
At this point I ask the audience why they would say 8-10 instead of 15 as the Product Manager for that team said. Obviously the Product Manager knew the team and the context better, right?
At the end of the fourth sprint the team completed 10 items, which even if it was 20% more than what they had done in previous sprints was still very far from the velocity they needed to make the project a success. The management reflected on the situation and clearly decided that the best decision for the company was to cancel that product.

## Story Points Myth: Busted!

That company did that extremely hard decision based on data, not speculation from Project Managers, not based on some bogus estimation using whatever technique. Real data. They looked at the data available to them and decided to cancel the project 10 months before its originally planned release. This project had a team of about 20 people. Canceling the project saved the company 200 man-month of investment in a product they had no hope of getting out of the door!
We avoided a death-march project and were able to focus on other more important products for the company's future. Products that now bring in significant amount of money!

## OK, I get your point, but how does that technique work?

Most people will be skeptical at this point (if you've read this far you probably are too). So let me explain how this works out.
Don't estimate the size of a story further than this: when doing Backlog Grooming or Sprint Planning just ask: can this Story be completed in a Sprint by one person? If not, break the story down!
For large projects use a further level of abstraction: Stories fit into Sprints, therefore Epics fit into meta-Sprints (for example: meta-Sprint = 4 Sprints). Ask the same question of Epics that you do of Sprints (can one team implement this Epic in half a meta-Sprint, i.e. 2 Sprints?) and break them down if needed.

http://4.bp.blogspot.com/-d44ZmBaikOg/TyB0VGZRkFI/AAAAAAAAAPo/g1xho13s3rU/s1600/median%2Bstory%2Bsize%2Bgraph.jpg

By continuously harmonizing the size of the Stories/Epics you are creating a distribution of the sizes around the median:


Assuming a normal distribution of the size of the stories means that you can assume that **for the purposes of looking at the long term** (remember: this only applies on the long term, i.e. more than 3 sprints into the future) estimation/progress of the project, **you can assume that all stories are the same size**, and can **therefore measure progress by measuring the number of items completed per Sprint**.

## Final words

As with all techniques this one comes with a disclaimer: you may not see the same effects that I report in this post. That's fine. If that is the case please share the data you have with me and I'm happy to look at it.
My aim with this post is to demystify the estimation in Agile projects. The fact is: the data we have available (see above) does not allow us to accept any of the claims by Mike Cohn regarding the use of Story Points as a valid/useful estimation technique, therefore you are better off using a much simpler technique! Let me know if you find an even simpler one!

Oh, and by the way: stop wasting time trying to estimate a never ending Backlog. There's no evidence that that will help you predict the future any better than just counting the number of stories "Done"!

## How do I apply #NoEstimates to improve estimation? Here's how...

---
Auteur : [Vasco Duarte](https://plus.google.com/114992270681478709673)  
Source : [Story Points Considered Harmful - Or why the future of estimation is really in our past...](http://softwaredevelopmenttoday.blogspot.com.au/2012/01/story-points-considered-harmful-or-why.html)  
Date de parution originale : 25 Janvier 2012  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 29/08/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}


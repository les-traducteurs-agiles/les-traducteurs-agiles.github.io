---
layout: post
title:  "Tester et coder, et non coder « puis » tester "
date:   2022-03-06 20:09
published: true
tags:
- tag1
- tag2
---

> People always say "code and then test." I prefer "test and then code"
> — Janet Gregory

> Les gens disent toujours « coder et puis tester ». Je préfère « tester et puis coder ».
> — Janet Gregory

This quote was recently published with the question “Hmm😶 What’s your take on this?” You can read some of the comments [here](https://www.linkedin.com/feed/update/urn:li:activity:6737409868044607488/?commentUrn=urn%3Ali%3Acomment%3A(activity%3A6737409868044607488%2C6741737353498505217)&replyUrn=urn%3Ali%3Acomment%3A(activity%3A6737409868044607488%2C6741812479837515776)).

Cette citation a été récemment publiée avec la question suivante « Hmm 😶 Qu'en pensez-vous ? ». Vous pouvez lire les commentaires et les réponses à cette question [ici](https://www.linkedin.com/feed/update/urn:li:activity:6737409868044607488/?commentUrn=urn%3Ali%3Acomment%3A(activity%3A6737409868044607488%2C6741737353498505217)&replyUrn=urn%3Ali%3Acomment%3A(activity%3A6737409868044607488%2C6741812479837515776)).

It made me realize that I should probably write a blog post so that people don’t take out of context what I mean. The quote is “almost” correct, but not quite. One word makes all the difference in the world sometimes.

À la suite de cela, j'ai réalisé que je devrais probablement écrire un article de blog afin que les gens aient tous les éléments de contexte sur ce que je veux dire.

The quote people most likely hear me say is:

La citation que la plupart des gens risquent d'entendre est :

> “Throw away the ‘_then’_ in ‘code _then_ test’ – replace it with ‘**_and’_**. And maybe, also reverse the order to say, ‘**test  AND code’**. Put the test first.”

> « Jetez le « _puis_ » dans l'expression « coder _puis_ tester » — et remplacez le par « **_et_** ». Et peut être aussi inverser l'ordre de la phrase : « **tester ET coder** » en mettant le mot tester en premier. »

This came about because teams don’t think about the term ‘code then test’ as a problem. But every time someone says that phrase, it reinforces that testing comes after coding.

Cela vient du fait que les équipes ne pensent pas que le expression « coder puis tester » soit un problème. Mais à chaque fois que quelqu'un dit la phrase, cela ne fait que renforcer que le test vient après le codage.

Testing and coding shouldn’t be separated as stand-alone activities. They are part of the same development process. Code is not complete without testing – at least some kind of testing, although some testing activities can be completed without writing any code. An example of this might be when we do an experiment or a simulation to test an idea and the team decides not to follow-up.

Le test et le codage ne devraient pas être vues comme des activités séparées. Ils font partie d'un seul et même processus de développement. Le code est incomplet sans le test — du moins sans une certaine forme de test, même si certaines activités de test peuvent être considérées comme complètes sans écrire une seule ligne de code. Un exemple de cela pourrait être lorsque nous faisons une expérience ou une simulation pour tester une idée et que l'équipe décide de ne pas donner suite.

I was chatting with [Paul Seaman](https://twitter.com/beaglesays) about the Linked-In conversation because I saw his name in one of the comments. He was surprised with some of the comments from folks. He asked, “Why do people think BDD and TDD are about testing? Both could be activities which help and influence testing choices but are not testing.”

Je discutais avec Paul Seaman](https://twitter.com/beaglesays) à propos de cette conversation sur Linked-In car j'avais vu son nom sur l'un des commentaires. Il était surpris par certains des commentaires. Il a demandé « Pourquoi les gens pensent-ils que le BDD et le TDD font partie du domaine du test ? Ces deux activités pourraient aider au sujet des tests mais il ne s'agit pas de tests en tant que tel  ».

TDD – it is about design and building testability into the code. BDD (behavior-driven development) and ATDD (acceptance test-driven development) are about getting shared understanding about what we are going to build. That said, I look at as these practices as testing activities since we are testing ideas and assumptions. It is a testing activity that the whole team can participate in to help make sure we understand the feature or story.

Le TDD (le développement piloté par les tests) traite de la testabilité de la conception et de la réalisation au sein du code. Le BDD (le développement piloté par le comportement) et l'ATDD (le développement piloté par les tests d'acceptation) traite de la manière d'avoir une compréhension commune sur ce que nous allons réaliser. Ceci étant dit, je considère ces pratiques comme étant des activités de test étant donné que nous testons des idées et des postulats. Il s'agit d'une activité de test à laquelle l'ensemble de l'équipe peut participer afin d'aider à être certain que nous comprenons la fonctionnalité ou la _story_.

This leads into the next point that Paul was concerned about. Sweeping statements such as “the best and most efficient way to avoid bugs in code is to test the requirements” may put emphasis on the wrong thing. For example, the assumption that “better requirements (whatever better might mean) automatically reduces coded bugs” doesn’t hold for him. I like his thought that “Better quality software requires a holistic goodness in systems of development not a singular focus.”

Ceci nous mène au point de préoccupation suivant de Paul. Échanger les affirmations telles que «  la meilleure manière et la plus efficace pour éviter les anomalies dans le code est de tester les exigences » peut mettre trop d'emphase sur la mauvaise chose. Par exemple, le postulat que « de meilleures exigences (quelque soit la signification de meilleures) réduisent automatiquement le nombre d'anomalies dans le code » ne lui convient pas. J'apprécie sa réflexion sur « une meilleure qualité logicielle exige une forme de bienveillance holistique dans les systèmes en développement et non une simple focalisation ».

Paul and I have shared many conversations over the past year, and we’ve discussed many of these themes. We both agree the Linked-In thread could have been a great discussion about collaborating through the lifecycle of development – how we influence, assist, and try to make sure the product that build, ships successfully.

Nous avons partagé, Paul et moi, de nombreuses discussions tout au long de l'année dernière, et nous avons discuté de nombreux thèmes différents. Nous sommes tous les deux d'accord que la discussion présente sur Linked-In aurait pu être une grande discussion sur la collaboration tout au long du cycle de vie de développement — comment nous influençons, aidons et essayons d'être sûr que le produit soit réalisé et livré avec succès.

It’s not about testing specific aspects like requirement, or code. It’s about how can we give fast feedback. It is one of the reasons, I created this diagram trying to show continuous testing.

Il ne s'agit pas de tester des aspects spécifiques comme les exigences ou le code. Il s'agit de la mnaière dont nous obtenons un retour d'informations rapide. C'est l'une des raisons pour lesquelles j'ai créé ce diagramme qui essaye de montrer le test en continu.


![shift left shift right diagram](https://janetgregory.ca/wp-content/uploads/sites/16/2021/01/shift-diagram.jpg)

![illustration déplacer à gauche - déplacer à droite]({{ site.url }}assets/janet_gregory/shift-diagram-fr.png)

I was influenced by Dan Ashby’s [continuous testing](https://danashby.co.uk/2016/10/19/continuous-testing-in-devops/) model, and I am not completely happy with it yet, but it’s a start. For example, it’s not obvious to everyone what testing activities are happening in the formulate and build section. We need to have fast feedback and practices like ‘show me’ to have the programmer show what he/she coded so bugs can be found quickly and fixed immediately.

J'ai été influencépar le modèle du [test en continu](http://www.les-traducteurs-agiles.org/2018/07/08/les-tests-continus-dans-devops.html) de Dan Ashby ; toutefois je n'en suis pas complètement satisfaites, mais c'est un début. Par exemple, il n'est pas évident pour tout le monde que les activités de test se déroulent dans les sections formuler et réaliser. Nous devons avoir des retours d'informations et des pratiques rapides comme « montrez-moi » pour que le développeur montrer ce qu'il ou elle a codé afin que les anomalies puissent être trouvés rapidement et corrigés immédiatement.

In summary, testing is an integral part of the whole development and cannot be separated from the coding aspect of building a product. I think one of my new quotes will be:

En résumé, le test fait partie intégrante de l'ensemble du développement et ne peut être séparé de l'aspect code de la construction d'un proudit. Je pense que l'une de mes prochaines citations sera :

> Le codage est vraiment une petite partie de l'ensemble du cycle de livraison alors que le test y est présent tout du long.
> — Janet Gregory

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

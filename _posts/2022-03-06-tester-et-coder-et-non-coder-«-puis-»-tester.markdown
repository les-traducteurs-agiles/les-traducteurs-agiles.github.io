---
layout: post
title:  "Tester et coder, et non coder « puis » tester "
date:   2022-03-07 00:01
published: true
tags:
- test
---

> Les gens disent toujours « coder et puis tester ». Je préfère « tester et puis coder ».  
> — Janet Gregory

Cette citation a été récemment publiée avec la question suivante « Hmm 😶 Qu'en pensez-vous ? ». Vous pouvez lire les commentaires et les réponses à cette question [sur ce fil de discussion](https://www.linkedin.com/feed/update/urn:li:activity:6737409868044607488/?commentUrn=urn%3Ali%3Acomment%3A(activity%3A6737409868044607488%2C6741737353498505217)&replyUrn=urn%3Ali%3Acomment%3A(activity%3A6737409868044607488%2C6741812479837515776)).

À la suite de cela, j'ai réalisé que je devrais probablement écrire un article de blog afin que les gens aient tous les éléments de contexte sur ce que je veux dire. La citation est « presque correcte » mais pas tout à fait. Quelques fois, un seul mot peut faire toute la différence.

La citation que la plupart des gens vont entendre est :

> « Jetez donc le « _puis_ » dans la phrase « coder _puis_ tester » — et remplacez le par « **_et_** ».  
> Et peut être aussi inverser l'ordre de la phrase : « **tester ET coder** » en mettant le mot tester en premier. »

Cela vient du fait que les équipes ne pensent pas que l'expression « coder puis tester » puisse être un problème. Mais à chaque fois que quelqu'un dit cette phrase, cela ne vient que renforcer que le fait que le test vient après le codage.

Le test et le codage ne devraient pas être vues comme des activités séparées. Ils font partie d'un seul et même processus de développement. Le code est incomplet sans le test — du moins sans une certaine forme de test, même si certaines activités de test peuvent être considérées comme complètes sans écrire une seule ligne de code. Par exemple, lorsque nous faisons une expérience ou une simulation pour tester une idée et que l'équipe décide de ne pas donner suite.

J'ai discuté avec [Paul Seaman](https://twitter.com/beaglesays) à propos de ce fil de discussion sur Linked-In car j'avais vu son nom sur l'un des commentaires. Il était surpris par certains de ces commentaires. Il a demandé « Pourquoi les gens pensent-ils que le BDD et le TDD font partie du domaine du test ? Ces deux activités peuvent aider pour les tests mais il ne s'agit pas de tests en tant que tels  ».

Le TDD (le développement piloté par les tests) traite de la testabilité de la conception et de la réalisation au sein du code. Le BDD (le développement piloté par le comportement) et l'ATDD (le développement piloté par les tests d'acceptation) traite de la manière d'avoir une compréhension commune sur ce que nous allons réaliser. Ceci étant dit, je considère ces pratiques comme étant des activités de test étant donné que nous testons des idées et des postulats. Il s'agit d'une activité de test à laquelle l'ensemble de l'équipe peut participer en vue d'aider à être certain que nous comprenons la fonctionnalité ou la _story_.

Ceci nous mène au point de préoccupation suivant de Paul. Échanger les affirmations telles que «  la meilleure manière et la plus efficace pour éviter les anomalies dans le code est de tester les exigences » peut avoir comme effet de mettre trop d'emphase sur la mauvaise chose.  
Par exemple, le postulat que « de meilleures exigences (quelque soit la signification de meilleures) réduisent automatiquement le nombre d'anomalies dans le code » ne lui convient pas. J'apprécie sa réflexion qu' « une meilleure qualité logicielle exige une forme de bienveillance holistique dans les systèmes en développement et pas uniquement une attention particulière ».

Nous avons eu, Paul et moi, de nombreuses discussions tout au long de l'année dernière, et nous avons discuté de nombreux thèmes. Nous sommes tous les deux d'accord que le fil de discussion présent sur Linked-In aurait pu aboutir à une grande discussion sur la collaboration tout au long du cycle de vie de développement — comment nous influençons, aidons et essayons de faire en sorte que le produit soit réalisé et livré avec succès.

Il ne s'agit pas de tester des aspects spécifiques comme les exigences ou le code. Il s'agit de la mnaière dont nous obtenons un retour d'informations rapide. C'est l'une des raisons pour lesquelles j'ai créé ce diagramme qui essaye de montrer le test en continu.

![illustration déplacer à gauche - déplacer à droite]({{ site.url }}assets/janet_gregory/shift-diagram-fr.png)

J'ai été influencé par le modèle du [test en continu (VF)](http://www.les-traducteurs-agiles.org/2018/07/08/les-tests-continus-dans-devops.html) de Dan Ashby ; toutefois je n'en suis pas complètement satisfaite, mais c'est un début. Par exemple, il n'est pas évident pour tout le monde que les activités de test se déroulent dans les sections formuler et réaliser. Nous devons avoir des retours d'informations et des pratiques rapides comme « montrez-moi » pour que le développeur puisse montrer ce qu'il ou elle a codé afin que les anomalies puissent être trouvées rapidement et corrigées immédiatement.

En résumé, le test fait partie intégrante de l'ensemble du développement et ne peut être séparé de l'aspect code de la construction d'un proudit. Je pense que l'une de mes prochaines citations sera :

> Le codage est vraiment une petite partie de l'ensemble du cycle de livraison alors que le test y est présent tout du long.  
> — Janet Gregory

---
Auteur : [Janet Gregory](https://janetgregory.ca/about/)  
Source : [Testing And Coding, Not Coding “Then” Testing](https://janetgregory.ca/testing-and-coding-not-coding-then-testing/)  
Date de parution originale : 3 Janvier 2021  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 07/03/2021  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

---
layout: post
title:  "Leçons apprises en développement logiciel"
date:   2015-10-23 21:00:55
published: true
categories: 
- developpement
- pratique
---

Here is my list of heuristics and rules of thumb for software development that I have found useful over the years:

![Programming bookshelf]()

Voici ma liste d'heuristiques et de règles empiriques que j'ai pu trouver utiles tout au long de ces années dans le domaine du développement logiciel  :
 
## Development

## Développement

**1. Start small, then extend.** Whether creating a new system, or adding a feature to an existing system, I always start by making a very simple version with almost none of the required functionality. Then I extend the solution step by step, until it does what it is supposed to. I have never been able to plan everything out in detail from the beginning. Instead, I learn as I go along, and this newly discovered information gets used in the solution.

**1. Commencez petit, puis élargissez.** Que ce soit pour la création d'un nouveau système, ou pour l'ajout d'une fonctionnalité à un système existant, je commence toujours par une version très simple avec pour ainsi dire aucune des fonctionnalités exigées. Puis j'élargis la solution petit à petit, jusqu'à ce qu'elle fasse ce qu'elle est supposée faire. Je n'ai jamais été capable de tout planifier tout en détails dès le début. À la place, j'ai appris au fur et à mesure que j'avance, et la découverte de ces nouvelles informations est utilisée dans la solution.

I like this quote from John Gall:  “A complex system that works is invariably found to have evolved from a simple system that worked.”

J'apprécie tout particulièrement cette citation de John Gall : "Un système opérationnel complexe est invariablement le fruit de l'évolution d'un système opérationnel simple".

**2. Change one thing at a time.** When you develop, and some tests fail, or a feature stops working, it’s much easier to find the problem if you only changed one thing. In other words, use short iterations. Do one thing, make sure it works, repeat. This applies down to the level of commits. If you have to refactor the code before you add a new feature, commit the refactoring first, then (in a new commit) add the new feature.

**2. Modifiez une seule chose à la fois.** Lorsque vous développez, et que certains tests échouent, ou qu'une fonctionnalité cesse de marcher, il est plus facile de trouver le problème si vous avez modifiez une seule chose. Autrement dit, faites des itérations courtes. Faites une seule chose, soyez certain qu'elle fonctionne, répétez. Cela s'applique jusqu'au niveau des _commits_[^1]. Si vous devez refactorez[^2] le code avant de l'ajouter à une nouvelle fonctionnalité, commitez le refactoring d'abord, puis (dans un nouveau commit) ajoutez la nouvelle fonctionnalité.

[^1]: mécanisme d'enregistrements de fichiers utilisé dans des logiciels de gestion de configuration permettant de gérer l'historique du contenu des fichiers qui y sont enregistrés - NdT

[^2]: action par laquelle, tout ou partie du code d'une application est retravaillé en profondeur tout en conservant le service rendu à l'utilisateur

**3. Add logging and error handling early.** When developing a new system, one of the first things I do is adding logging and error handling, because both are useful from the very beginning. For all systems that are bigger than a handful of lines of code, you need some way of knowing what happens in the program. Perhaps not when it is working as expected, but as soon as it doesn’t, you must be able to see what’s happening. The same goes for error handling – errors and exceptions happen in the beginning too, so the sooner you handle them in a systematic way, the better.

**3. Ajoutez la gestion des journaux et des erreurs le plus tôt possible.** Lorsque vous développez un nouveau système, l'une des premières choses que je fais est d'ajouter la gestion des journaux et des erreurs, parce que les deux sont utiles dès le début. Pour tous les systèmes dont la taille est supérieure à quelques lignes de code, vous avez besoin d'une manière ou d'une autre de savoir ce qu'il se passe dans le programme. Peut être pas lorsqu'il fonctionne comme prévu, mais dès que le contraire se produit, vous devez être capable de voir ce qu'il se passe. Il en va de même pour la gestion des erreurs -  des erreurs et des exceptions se produisent dès le commencement, le plus tôt vous les gérez de manière systématique, le mieux c'est.

**4. All new lines must be executed at least once.** Before you are done with a feature, you have to test it. Otherwise, how do you know that it does what it is supposed to do? Often, the best way is by automatic tests, but not always. But no matter what, every new line of code has to be executed at least once.

**4. Toute nouvelle ligne de code doit être exécutée au moins une fois.** Avant que vous ayez fini avec une fonctionnalité, vous devez la tester. Sinon, comment savez-vous ce qu'elle est supposée faire ? Souvent, la meilleure manière de le savoir est par l'exécution de tests automatisés, mais pas toujours. Mais quoi qu'il en soit, chaque nouvelle ligne de code doit être exécutée au moins une fois.

Sometimes it can be hard to trigger the right conditions. Fortunately, it’s easy to cheat a bit. For example, the error handling on a database call can be checked by temporarily misspelling a column name. Or, an if-statement can be temporarily inverted (“if error” becomes “if not error”) in order to trigger something that rarely happens, just to make sure that code is run and does what it should.

Quelques fois, il peut être difficile de déclencher les bonnes conditions. Heureusement, il est facile de tricher un peu. Par exemple, la gestion des erreurs sur une base de données peut facilement être vérifiée en saisissant incorrectement et temporairement un nom de colonne. Ou bien, une condition `si` peut être temporairement inversée ("`si erreur`" devient "`si pas erreur`") afin de déclencher quelque chose qui arrive rarement, uniquement pour être certain que le code fonctionne et qu'il fait ce qu'il devrait faire.

Sometimes I see bugs that show that a certain line of code can never have been run by the developer. It can look fine when reviewed, but still not work. You avoid embarrassment if your policy is to always execute every new line you write.

Quelques fois je vois des bogues montrant qu'une ligne de code donnée n'a jamais été exécutée par le développeur. Elle peut sembler bonne lorsqu'elle est relue, mais ne pas fonctionner. Vous vous évitez des ennuis si vous décidez de toujours exécutez chaque nouvelle ligne que vous écrivez.

5. Test the parts before the whole. Well-tested parts save time. Often there are problems with integrating different parts, for example from mismatched or misunderstood interfaces between modules. If you can trust that the parts work as expected, it becomes much easier to track down the integration problems.

**5. Testez les parties avant l'ensemble**. Bien tester les parties permet de gagner du temps. Souvent il y a des problèmes avec l'intégration des différentes parties, par exemple avec des interfaces incomprises ou incompatibles entre les modules. Si vous pouvez avoir confiance dans le fonctionnement des --  que chaque partie fonctionne comme prévu, il devient beaucoup plus facile de pister les problèmes d'intégration. 

**6. Everything takes longer than you think.** Especially in programming. It is hard to estimate how much time a feature will take even if everything goes smoothly. But when developing software, it is quite common to run in to unexpected problems: a simple merge turns out to cause a subtle bug, an upgrade of a framework means some functions must be changed or an API call doesn’t work as promised.

**6. Tout prend plus de temps que vous ne le pensez.** Et tout spécialement en programmation. Il est difficile d'estimer combien de temps le développement d'une fonctionnalité prendra si tout se passe bien. Mais lors du développement d'un logiciel, il est assez habituel de rencontrer des problèmes imprévus : un simple `merge`[^3] aboutit à la survenance d'un bogue subtile à analyser, la montée de version d'un _framework_ peut signifier que quelques fonctionnalités doivent être modifiées ou que l'appel d'une API ne fonctionnent pas comme promis.  

[^3]: fusion du contenu d'un même fichier modifié au fil du temps par un ou plusieurs développement

I think there is a lot of truth in Hofstadter Law:  It always takes longer than you expect, even when you take into account Hofstadter’s Law.

Je pense qu'il y a beaucoup de vrai dans la loi de Hofstadter :  Cela prends toujours plus de temps que vous ne le pensez, même si vous prenez en compte la loi de Hofstadter.

**7. First understand the existing code.** Most coding requires changing existing code in some way. Even if it is a new feature, it needs to fit into the existing program. And before you can fit the new stuff in, you need to understand the current solution. Otherwise you may accidentally break some of the existing functionality. This is means that reading code is a skill that is as necessary as writing code. It is also part of the reason why seemingly small changes can still take a long time – you must understand the context in which you make the change.

**7. Comprenez d'abord le code existant.** La plupart du développement demande à changer le code existant d'une manière ou d'une autre. Même s'il s'agit d'une nouvelle fonctionnalité, elle doit s'insérer dans un programme existant. Et avant que vous ne puissiez y insérer la nouvelle fonctionnalité, vous devez comprendre la solution existante. Sinon vous pourriez cassez quelque chose accidentellement dans une fonctionnalité existante. Cela signifie que lire du code est une compétence aussi nécessaire qu'écrire du code. C'est aussi en partie l'une des raisons expliquant pourquoi ce qui pourrait sembler être des modifications mineures peut toujours prendre beaucoup de temps - vous devez comprendre le contexte dans lequel vous faites le changement.

**8. Read and run.** Fortunately, there are two complementary methods for understanding code. You can read the code, and you can run the code. Running the code can be a great help when figuring out what it does. Be sure to make use of both methods.

**8. Lisez et exécutez.** Heureusement, il y a deux méthodes complémentaires pour comprendre du code. Vous pouvez lire le code, et vous pouvez exécuter le code. L'exécution du code peut vous être d'une grande aide lorsque vous essayez de comprendre ce qu'il fait. Soyez certain de bien utiliser les deux méthodes.

## Troubleshooting

## Gestion des problèmes

**9. There will always be bugs.** I don’t like approaches to software development that claim to “get it right the first time”. No matter how much effort you put in, there will always be bugs (the definition of a bug pretty much is: “we didn’t think of that”). A much better approach is to have a system in place that lets you quickly troubleshoot problems, fix the bugs and deploy the fixes.

**9. Il y aura toujours des anomalies.** Je n'apprécie guère les approches en développement logiciel proclamant "pouvoir faire bien du premier coup". Quelque soit les efforts que vous déployez, il y aura toujours des anomalie (la définition d'une anomalie ressemble à peu près à ceci : "nous ne pensions pas à cela"). Une meilleure approche est d'avoir un système en place qui vous permet de gérer rapidement les problèmes, de corriger les bogues et de déployer les correctifs.

**10. Solve trouble reports.** Every developer should spend a portion of their time handling trouble reports from customers and fixing bugs. It gives you a much better understanding of what the customers are trying to do, how the system is used, how easy or hard it is to troubleshoot and how well the system is designed. It’s also a great way of taking responsibility for what you develop. Don’t miss out on all these benefits.

**10. Réglez les rapports d'anomalies.** Chaque développeur devrait passer une partie de son temps à gérer les rapports d'anomalies émis par les clients et à corriger les bogues. Cela vous donne une bien meilleure compréhension de ce que les clients essayent de faire, de comment le système est utilisé, de comment il est facile ou difficile de gérer les anomalies et de comment le système est conçu. C'est aussi une excellent manière de prendre la responsabilité de ce que vous développez. Ne ratez aucun de ces bénéfices.

**11. Reproduce the problem.** The first step when fixing a bug is to reproduce the problem. Then you make sure that when the fix is added, the problem is gone. This simple rule makes sure you are not assuming something is a problem when it isn’t, and makes sure the solution actually does what you think it does.

**11. Reproduisez le problème.** La première étape lors de la correction d'un bogue est de reproduire le problème. Puis assurez-vous que lorsque le correctif est mis en place, que le problème ait bien disparu. Cette règle simple vous permet d'être sûr que vous ne faites pas une supposition sur ce qu'est le problème alors qu'il n'en est rien, d'être certain que la solution fait réellement ce que vous pensez qu'elle fait.

**12. Fix the known errors, then see what’s left.** Sometimes there are several problems present that you know about. The different bugs can interact with each other and cause strange things to happen. Instead of trying to work out what happens in those cases, fix all the know problems and then see what symptoms remain.

**12. Corrigez les problèmes connus, puis regardez ce qu'il reste.** Souvent, il y a plusieurs problèmes dont vous avez connaissance. Les différents bogues peuvent interagir les uns avec les autres et provoquer la survenance d'étranges choses. À la place d'essayer de forcer ce qui arrive certains cas, corriger tous les problèmes connus et regardez si les symptômes persistent. 

**13. Assume no coincidences.** When testing and troubleshooting, never believe in coincidences. You changed a timer value, and now the system restarts more often. Not a coincidence. A new feature was added, and an unrelated feature becomes slower? Not a coincidence. Instead, investigate.

**13. Partez du principe qu'il n'existe pas de coïncidences.** Lors de la gestion des tests et des anomalies, ne croyez jamais aux coïncidences. Vous avez changé la valeur d'un compte à rebours, et maintenant le système redémarre plus souvent. Ce n'est pas une coïncidence. Une nouvelle fonctionnalité a été ajoutée, et une autre fonctionnalité n'ayant aucun rapport avec elle devient plus lente ? Ce n'est pas une coïncidence. À la place, enquêtez.

**14. Correlate with timestamps.** When troubleshooting, use the timestamp of events as a help. Look for even increments. For example, if the system restarted, and a request was sent out around 3000 milliseconds before, maybe a timer triggered the action that lead to the restart.

**14. Corrélez avec des timestamps[^4].** Lors de la gestion des anomalies, utilisez l'horodatage des évènements pour vous aider. Regardez pour des incréments identiques. Par exemple, si le système a redémarré, et qu'une requête a été envoyée environ 3 000 millisecondes avant, peut être que le compte à rebours a déclenché l'action ayant conduit au redémarrage.

[4]: terme informatique correspondant littéralement à des horodateurs - NdT

## Cooperation

## Coopération

**15. Face to face has the highest bandwidth.** When discussing how to solve a problem, being face to face beats video, call, chat and email. I am often amazed at how much better the solutions are after discussing them in person with colleagues.

**15. Le face à face possède la meilleure bande passante.** Lorsque vous discutez pour savoir comment résoudre un problème, le face à face est meilleur que la vidéo, la conversation téléphonique, le chat et le mél.  Je suis souvent stupéfait de la qualité des solutions après en avoir discuté en personne avec des collègues.

**16. Rubber ducking.** Whenever you are stuck, go to a colleague and explain the problem to them. Many times, as you talk, you realize what the problem is, even if your colleague doesn’t say a word. Sounds like magic, but works surprisingly often.

**16. `Rubber ducking`.** À chaque fois que vous êtes bloqué, allez voir un collègue et expliquez lui le problème, vous réaliserez alors ce qu'est le problème, même si votre collègue ne dit pas un mot. Ça à l'air magique, mais de manière surprenante, cela fonctionne souvent.

**17. Ask.** Reading and running the code is often great for figuring out what it does and how it works. But if you have the possibility to ask someone knowledgeable (perhaps the original author), use that option too. Being able to ask specific questions, and follow-up questions to those, can give you information in minutes that would otherwise take days to get.

**27. Demandez.** Lire et exécuter du code est souvent une bonne manière pour comprendre ce qu'il fait et comment il fonctionne. Mais si vous la possibilité de demander à quelqu'un ayant la connaissance (peut être l'auteur originel), utilisez aussi cette option. Pouvoir poser des questions spécifiques, et des questions subséquentes, peut vous donner des informations dans la minute qui vous prendrait autrement des jours à obtenir.

**18. Share credit.** Make sure to give credit where credit is due. Say: “Marcus came up with the idea to try…” (if he did), instead of “we tried …”. Go out of your way to mention who else helped or contributed.

**18. Partagez le crédit.** Soyez certain de donner le crédit lorsque celui-ci est dû. Dites : "Marcus est venu avec cette idée à essayer ..." (s'il l'a fait), à la place de "nous avons essayé ...". Changez vos habitudes et mentionner qui d'autre à contribuer ou à aider.

## Miscellaneous

## Divers

**19. Try it.** If you are unsure of how a certain language feature works, it is easy to write a little program that shows how it works. The same applies when testing the system you are developing. What happens if I set this parameter to -1? What happens if this service is down when I reboot the system? Explore how it works – fiddling around often reveals bugs, and at the same time it deepens your understanding of how the system works.

**19. Essayez-le.** Si vous n'êtes pas certain comment la fonctionnalité d'un certain langage fonctionne, il est facile d'écrire un petit programme montrant comment cela fonctionne. La même chose s'applique lors du test du système que vous êtes en train de développer. Que se passe t'il si je mets le paramètre à -1 ? Que se passe t'il si ce service est arrêté lorsque je redémarre le système ? Explorer comment ça marche - furetez autour révèlera souvent des anomalies, et en même temps cela approfondira votre compréhension du fonctionnement du système.

**20. Sleep on it.** If you are working on a difficult problem, try to get in a night’s sleep before you decide. Then your subconscious mind works on the problem even when you aren’t actively thinking about it. As a result, the solution can seem obvious the next day.

**20. Dormez dessus.** Si vous êtes en train de travailler sur un problème difficile, essayez de laisser passer une bonne nuit de sommeil avant de vous décider. Ensuite votre subconscient travaillera sur le problème même si vous n'y pensez pas activement. La solution pourra sembler évidente le lendemain.

**21. Change.** Don’t be afraid to change roles or jobs every once in a while. It is stimulating to work with different people, on a different product or in a different company. In my view, too many people just passively stay at the same job year after year, only changing if they are forced to.

**21. Changez.** Ne soyez pas effrayez de changer de rôles et de métiers de temps en temps. C'est stimulant de travailler avec des personnes différentes, sur un produit différent ou dans une entreprise différente. De mon point de vue, trop de personens reste passivement au même poste année après après, changeant uniquement lorsqu'elles sont forcées de le faire.

**22. Keep learning.** One of the great things with software development is that there is always room to learn and know more. Try out different programming languages and tools, read books on software development, take MOOC courses. Small improvements soon add up to make a real difference in your knowledge and abilities.

**22. Continuez à apprendre.** L'une des plus grandes choses dans le développement logiciel est qu'il y a toujours l'opportunité pour apprendre et savoir davantage. Essayez différents langages de programmations et différents outils, lisez des livres sur le développement logiciel, suivez des cours en ligne. De petits pas s'ajouteront bientôt pour faire une vraie différence dans vos connaissances et compétences.

---  
Auteur : [Henrik Warne]()  
Source : [Lessons Learned In Software Developement](http://henrikwarne.com/2015/04/16/lessons-learned-in-software-development/)  
Date de parution originale : 16 Avril 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 23/10/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share buttons.html %}



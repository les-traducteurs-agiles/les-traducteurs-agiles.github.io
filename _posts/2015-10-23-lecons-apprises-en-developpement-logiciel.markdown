---
layout: post
title:  "Leçons apprises en développement logiciel"
date:   2015-10-28 21:00:55
published: true
tags:
- pratique
- développement
---

Voici ma liste de trouvailles heuristiques et de règles empiriques que j'ai pu trouver utiles pour le développement logiciel tout au long de ces années  :

![Livres de programmation]({{ site.url }}assets/lecons_apprises/dsc_0566.jpg)

## Développement

**1. Commencez petit, puis élargissez.** Que ce soit pour la création d'un nouveau système, ou pour l'ajout d'une fonctionnalité à un système existant, je commence toujours par une version très simple avec, pour ainsi dire, aucune des fonctionnalités exigées. Puis j'élargis la solution petit à petit, jusqu'à ce qu'elle fasse ce qu'elle est supposée faire. Je n'ai jamais pu dès le départ tout planifier en détails . À la place, j'apprends au fur et à mesure que j'avance, et ces nouvelles informations, qui ont été découvertes, sont utilisées dans la solution.

J'apprécie tout particulièrement cette citation de John Gall : _"Un système opérationnel complexe est invariablement le fruit de l'évolution d'un système opérationnel simple."_

**2. Modifiez une seule chose à la fois.** Lorsque vous développez, et que certains tests échouent, ou qu'une fonctionnalité cesse de fonctionner, il est plus facile de trouver le problème si vous avez modifié une seule chose. Autrement dit, faites des itérations courtes. Faites une seule chose, soyez certain qu'elle fonctionne, répétez. Cela s'applique jusqu'au niveau des _commits_[^1]. Si vous devez refactorer[^2] le code avant de l'ajouter à une nouvelle fonctionnalité, faites le _commit_ du _refactoring_ d'abord, puis (dans un nouveau _commit_) ajoutez la nouvelle fonctionnalité.

[^1]: mécanisme d'enregistrements utilisé dans des logiciels de gestion de version permettant de gérer l'historique du contenu des fichiers qui y sont enregistrés - NdT

[^2]: action par laquelle, tout ou partie du code d'une application est retravaillé en profondeur tout en conservant le service rendu - NdT

**3. Ajoutez la gestion des journaux et des erreurs le plus tôt possible.** Lorsque vous développez un nouveau système, l'une des premières choses que je fais est d'ajouter la gestion des journaux et des erreurs, parce que les deux sont utiles dès le début. Pour tous les systèmes dont la taille est supérieure à quelques lignes de code, vous avez besoin d'une manière ou d'une autre de savoir ce qu'il se passe dans le programme. Peut être pas lorsqu'il fonctionne comme prévu, mais dès que le contraire se produit, vous devez être capable de voir ce qu'il se passe. Il en va de même pour la gestion des erreurs -  des erreurs et des exceptions se produisent dès le début, le plus tôt vous les gérez de manière systématique, le mieux c'est.

**4. Toute nouvelle ligne de code doit être exécutée au moins une fois.** Avant que vous ayez fini avec une fonctionnalité, vous devez la tester. Sinon, comment savez-vous ce qu'elle est supposée faire ? Souvent, la meilleure manière de le savoir est par l'exécution de tests automatisés, mais pas toujours. Mais quoi qu'il en soit, chaque nouvelle ligne de code doit être exécutée au moins une fois.

Quelques fois, il peut être difficile de déclencher les bonnes conditions. Heureusement, il est facile de tricher un peu. Par exemple, la gestion des erreurs sur une base de données peut facilement être vérifiée en saisissant de manière incorrecte et temporaire un nom de colonne. Ou bien, une condition "si" peut être temporairement inversée ("si erreur" devient "si pas erreur") afin de déclencher quelque chose qui arrive rarement, uniquement pour être certain que le code fonctionne et qu'il fait ce qu'il devrait faire.

Quelques fois je vois des anomalies qui montrent qu'une ligne de code donnée n'a jamais été exécutée par le développeur. Elle peut sembler bonne à la relecture, mais ne pas fonctionner. Vous vous éviterez des ennuis si vous décidez de toujours exécuter chaque nouvelle ligne que vous écrivez.

**5. Testez les parties avant l'ensemble.** Bien tester les parties permet de gagner du temps. Souvent il y a des problèmes avec l'intégration des différentes parties, par exemple avec des interfaces incomprises ou incompatibles entre les modules. Si vous pouvez avoir confiance dans le fonctionnement comme prévu de chaque partie, il devient beaucoup plus facile de pister les problèmes d'intégration.

**6. Chaque chose prend plus de temps que vous ne le pensez.** Et tout spécialement en programmation. Il est difficile d'estimer combien de temps le développement d'une fonctionnalité prendra si tout se passe bien. Mais lors du développement d'un logiciel, il est assez habituel de rencontrer des problèmes imprévus : un simple _merge_[^3] aboutit à la survenance d'une anomalie subtile à analyser, la montée de version d'un _framework_[^4] peut signifier que quelques fonctionnalités doivent être modifiées ou que l'appel d'une _API_[^5] ne fonctionne pas comme promis.  

[^3]: fusion du contenu d'un même fichier modifié au fil du temps par un ou plusieurs développement - NdT

[^4]: littéralement cadre de travail - il s'agit d'un ensemble cohérent de fonctionnalités ou de services permettant de faciliter le développement des applications

[^5]: littéralement interface de programmation - à travers cette interface un langage ou un logiciel expose les fonctions ou les services qu'il propose

Je pense qu'il y a beaucoup de vrai dans la loi de Hofstadter :  _Cela prends toujours plus de temps que vous ne le pensez, même si vous prenez en compte la loi de Hofstadter._

**7. Comprenez d'abord le code existant.** La plus grande partie de l'activité de développement exige le changement du code existant d'une manière ou d'une autre. Même s'il s'agit d'une nouvelle fonctionnalité, elle doit s'insérer dans un programme existant. Et avant que vous ne puissiez y insérer la nouvelle fonctionnalité, vous devez comprendre la solution existante. Sinon vous pourriez cassez quelque chose accidentellement au sein d'une fonctionnalité existante. Cela signifie que lire du code est une compétence aussi essentielle qu'écrire du code. C'est aussi en partie l'une des raisons expliquant pourquoi ce qui pourrait sembler être des modifications mineures peut toujours prendre beaucoup de temps - vous devez comprendre le contexte dans lequel vous faites le changement.

**8. Lisez et exécutez.** Heureusement, il y a deux méthodes complémentaires pour comprendre du code. Vous pouvez lire le code, et vous pouvez exécuter le code. L'exécution du code peut vous être d'une grande aide lorsque vous essayez de comprendre ce qu'il fait. Soyez sûr de bien utiliser les deux méthodes.

## Résolution des problèmes

**9. Il y aura toujours des anomalies.** Je n'apprécie guère les approches en développement logiciel proclamant "pouvoir faire bien du premier coup". Quelque soit les efforts que vous déployez, il y aura toujours des anomalie (la définition d'une anomalie ressemble à peu près à ceci : "nous n'avions pas pensé à cela"). Une bien meilleure approche est d'avoir un système en place qui vous permet de gérer rapidement les problèmes, de corriger les anomalies et de déployer les correctifs.

**10. Réglez les rapports d'anomalies.** Chaque développeur devrait passer une partie de son temps à gérer les rapports d'anomalies émis par les clients et à corriger les anomalies. Cela vous donne une bien meilleure compréhension de ce que les clients essayent de faire, de comment le système est utilisé, de comment il est facile ou difficile de gérer les anomalies et de comment le système est conçu. C'est aussi une excellent manière de prendre la responsabilité de ce que vous développez. Ne passez pas à côté de tous ces éléments bénéfiques.

**11. Reproduisez le problème.** La première étape lors de la correction d'une anomalie est de reproduire le problème. Ensuite assurez-vous une fois le correctif est mis en place, que le problème ait bien disparu. Cette règle simple vous permet d'être sûr que vous ne faites pas une supposition sur ce qu'est le problème alors qu'il n'en est rien, d'être certain que la solution fait réellement ce que vous pensez qu'elle fait.

**12. Corrigez les problèmes connus, puis regardez ce qu'il reste.** Souvent, il y a plusieurs problèmes dont vous avez déjà connaissance. Les différentes anomalies peuvent interagir les unes avec les autres et provoquer la survenance de choses étranges. À la place d'essayer de résoudre ce qui arrive dans ces cas-là, corriger déjà tous les problèmes connus et regardez si les symptômes persistent.

**13. Partez du principe qu'il n'existe pas de coïncidences.** Lors de la gestion des tests et des anomalies, ne croyez jamais aux coïncidences. Vous avez changé la valeur d'un compte à rebours, et maintenant le système redémarre plus souvent. Ce n'est pas une coïncidence. Une nouvelle fonctionnalité a été ajoutée, et une autre fonctionnalité n'ayant aucun rapport avec elle devient plus lente ? Ce n'est pas une coïncidence. Au lieu de ça, enquêtez.

**14. Corrélez avec la chronologie des évènements.** Lors de la gestion des anomalies, utilisez la chronologie des évènements pour vous aider. Regardez pour des incréments identiques. Par exemple, si le système a redémarré, et qu'une requête a été envoyée environ 3 000 millisecondes avant, peut être que le compte à rebours a déclenché l'action ayant conduit au redémarrage.

## Coopération

**15. Le face à face possède la meilleure bande passante.** Lorsque vous discutez pour savoir comment résoudre un problème, le face à face est meilleur que la vidéo, la conversation téléphonique, le chat et le mél.  Je suis souvent stupéfait de la qualité des solutions après en avoir discuté en personne avec des collègues.

**16. Pratiquez la méthode du canard en plastique[^6].** À chaque fois que vous êtes bloqué, allez voir un collègue et expliquez lui le problème, vous comprendrez alors quel est le problème, même si votre collègue ne dit pas un mot. Ça à l'air magique, mais de manière surprenante, cela fonctionne souvent.

[^6]: pour plus d'informations, le lecteur avisé pourra se reporter à cet [article](https://fr.wikipedia.org/wiki/M%C3%A9thode_du_canard_en_plastique) sur Wikipedia - NdT

**17. Demandez.** Lire et exécuter du code sont souvent de bonnes manières pour comprendre ce que le code fait et comment il fonctionne. Mais si vous la possibilité de demander à quelqu'un ayant la connaissance (peut être l'auteur originel), utilisez aussi cette option. Pouvoir poser des questions spécifiques, et des questions subséquentes, peut vous donner l'information dans la minute qui autrement vous prendrait des jours à obtenir.

**18. Partagez le mérite.** Soyez certain de donner le mérite à qui de droit. Dites : "Marcus a eu l'idée d'essayer ..." (s'il l'a fait), à la place de "nous avons essayé ...". Changez vos habitudes et mentionner qui d'autre à contribuer et à aider.

## Divers

**19. Essayez.** Si vous n'êtes pas certain comment la fonctionnalité d'un certain langage fonctionne, il est aisé d'écrire un petit programme montrant comment cela fonctionne. La même chose s'applique lors du test du système que vous êtes en train de développer. Que se passe t'il si je mets le paramètre à -1 ? Que se passe t'il si ce service est arrêté lorsque je redémarre le système ? Explorez comment ça marche - furetez à gauche et à droite révèlera souvent des anomalies, et en même temps cela approfondira votre compréhension du fonctionnement du système.

**20. Dormez dessus.** Si vous êtes en train de travailler sur un problème difficile, essayez de laisser passer une bonne nuit de sommeil avant de prendre votre décision. Votre subconscient va alors travailler sur le problème même si vous n'y pensez pas activement. La solution pourra vous sembler évidente le lendemain.

**21. Changez.** Ne soyez pas effrayé de changer de rôles et de métiers de temps en temps. C'est stimulant de travailler avec des personnes différentes, sur un produit différent ou dans une entreprise différente. De mon point de vue, trop de personnes restent passivement au même poste année après année, et changent uniquement lorsqu'elles sont forcées de le faire.

**22. Continuez à apprendre.** L'une des plus belles choses dans le développement logiciel est qu'il y a toujours l'opportunité d'apprendre et d'en savoir davantage. Essayez différents langages de programmations et différents outils, lisez des livres sur le développement logiciel, suivez des cours en ligne.
Et l'accumulation des petites avancées fera bientôt une vraie différence dans vos connaissances et dans vos compétences.

---  
Auteur : [Henrik Warne](http://henrikwarne.com/about/)  
Source : [Lessons Learned In Software Developement](http://henrikwarne.com/2015/04/16/lessons-learned-in-software-development/)  
Date de parution originale : 16 Avril 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 28/10/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

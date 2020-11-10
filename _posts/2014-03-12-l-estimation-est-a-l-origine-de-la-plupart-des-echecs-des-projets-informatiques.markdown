---
layout: post
title:  "L'estimation est à l'origine de la plupart des échecs des projets informatiques"
date:   2014-03-12 00:01
published: true
tags:
- estimation
---

## Synopsis

Je crois que l'estimation, et la manière dont elle est mal utilisée, est à l'origine de la majorité des échecs des projets informatiques. Dans cet article, j'essaierai d'expliquer pourquoi nous sommes si mauvais dans ce domaine et aussi pourquoi, une fois que nous sommes tombés dans le piège d'essayer de faire quelque chose s'approchant d'une estimation future, aucune méthode qu'elle soit TDD (Développement piloté par les tests), livraison continue ou * insérer ici votre pratique favorite ici*, ne sera d'aucune aide. La simple vérité est que nous ne serons jamais très bon en estimation, principalement pour des raisons en dehors de notre contrôle. Néanmoins, beaucoup de personnalités connues dans la communauté agile continuent de parler de l'estimation comme si c'était un problème qui pouvait être résolu et même si certains d'entre nous ont la chance de travailler dans des organisations qui apprécient la nature incertaine du développement logiciel, la plupart ne le sont pas.

## Plantons le décor
J'ai récemment tweeté quelque chose qui a eu de l'écho chez beaucoup de personnes :

![Tweet]({{ site.url }}assets/misc/tweet_rob_bowley.jpg)
"En estimation (lors d'un développement d'un logiciel NdT), vous n'avez en réalité seulement le choix qu'entre 5 minutes, 1 heure, 1-2 jours, environ 1 semaine, ensuite tous les paris sont ouverts."
"En estimation (lors d'un développement d'un logiciel NdT), vous n'avez en réalité seulement le choix qu'entre 5 minutes, 1 heure, 1-2 jours, environ 1 semaine, ensuite tous les paris sont ouverts."

C'était en réponse à [cet article](http://www.mountaingoatsoftware.com/blog/estimating-a-full-backlog-based-on-a-sample-of-it) de Mike Cohn proposant une technique pour l'estimation d'un backlog complet de 300(!) stories sans que vous ayez encore de données historiques sur la performance passée de l'équipe. Les avertissements présents dans l'article préviennent que ce n'est pas l'idéal, mais je pense qu'il est extrêmement dangereux de même suggérer qu'il s'agit de quelque chose que vous pourriez faire.
J'ai été longtemps fasciné par l'estimation et plus particulièrement pourquoi nous sommes si mauvais sur ce sujet. Cela débuta quand je fus impliqué dans un projet informatique pour lequel, même s'il fût par plusieurs aspects un succès, fût aussi un échec misérable résultant en une chasse aux sorcières nauséabonde et l'opprobre portée sur ceux qui avaient fait les estimations.
J'ai déjà écrit sur [le leurre de l'estimation](http://blog.robbowley.net/2008/06/06/estimation/), cette [expérience formatrice](http://blog.robbowley.net/2010/12/30/a-formative-experience/), puis animé ma session " Gérer le leurre de l'estimation" à 2/3 conférences dont [SPA 2009](http://www.spaconference.org/spa2009/sessions/session191.html). D'autres articles sur l'estimation sont accessibles dans les [archives](http://blog.robbowley.net/tag/estimation/).

## Pourquoi nous nous planterons toujours pour estimer

> “Cela prends toujours plus longtemps que ce que vous vous attendez, même si vous prenez en compte la loi de Hofstadter."Â
- Douglas Hofstadter, Godel, Escher, Bach: An Eternal Golden Braid

Depuis mes expériences tumultueuses avec l'estimation et mes recherches subséquentes dans ce domaine j'ai été très loin pour essayer d'améliorer la manière de faire des estimations. Dans mon organisation actuelle, nous récoltons depuis plus deux ans, des données de toutes nos équipes sur la durée de traitement d'un item (temps de cycle). C'est une véritable montagne de données à partir de laquelle nous sommes capables d'établir la moyenne et l'écart-type des temps de cycle.

 Taille (estimée) de la fonctionnalité | Nbre d'items achevés | Dévpt standard | Dévpt moyen standard | Moyen | Dévpt moyen + standard
--|---|---|---|---|--
 Small | 296 | 5,11 | -0,95 | 4,17 | 9,28
 Medium | 27 | 8,94 | 6,36 | 15,30 | 24,24
 Large | 5 | 28,75 | 22,85 | 51,60 | 80,35


Nous pouvons alors prendre une liste de demandes de fonctionnalités, en faire quelques estimations à grosses mailles en taille de t-shirt et être capable de donner facilement une plage de dates dans laquelle l'équipe est capable d'atteindre des jalons spécifiques (la plage représente l'incertitude - basse, moyenne, et haute basée sur la moyenne +/- l'écart-type, malin hein ?).

Correcte ?

Non.

Nous avons découvert qu'à moins de parler de choses arrivants dans les toutes prochaines semaines - période à laquelle où nous faisions généralement une analyse plus détaillés - nous étions soit à l'extrême fin de la plage d'estimation ou soit nous avions raté complètement les dates de jalon prévues. Cela prenait presque toujours plus temps que nous l'avions prévu. Vous pourriez argumenter d'une faible productivité de la part des développeurs, mais les projections étaient basées sur leurs précédentes performances donc c'est un argument peu recevable, et surtout lorsque nos données suggéraient aussi la diminution du temps de cycle pour les items traités.
Il y a deux grandes raisons pour lesquelles les choses ont pris plus longtemps que prévu :

### 1. Le biais cognitif

Extrait de [Wikipedia](http://en.wikipedia.org/wiki/Cognitive_bias) : _"Le biais cognitif est le terme général utilisé pour décrire des effets d'observation dans le cerveau humain, certains pouvant conduire à des distorsions de perception, des jugements incorrectes ou des interprétations illogiques"_.
En terme d'estimation, le biais cognitif se manifeste sous la forme du [biais optimiste](http://en.wikipedia.org/wiki/Optimism_bias) : _"tendance systématique démontrée de personnes d'être trop optimiste à propos de l'issue d'actions planifiées"_.
Il existe aussi le [leurre du planning](http://en.wikipedia.org/wiki/Planning_fallacy) : _"une tendance pour les personnes et les organisations de sous-estimer le temps nécessaire pour compléter une tâche, même lorsqu'ils ont eu une expérience précédente de tâches similaires dépassées"_.
C'est un énorme problème, spécialement quand vous essayez de faire une estimation à grosse maille à long terme. Nos cerveaux sont pré-cablés, non seulement pour être optimistes sur nos estimations, mais aussi pour tendre à penser seulement aux scénarios les plus favorables. Il y a peu de choses que nous puissions faire à part être conscient de ce qu'il se passe.
C'est seulement quand vous essayez de faire l'analyse correcte du projet que vous commencez à voir les autres choses que vous devez faire. Je me rappelle Dan North qui a dit une fois lors d'une présentation que l'estimation est comme "mesurer la côte de la Grande-Bretagne", plus vous vous rapprochez plus vous voyez de relief, d'anfractuosités, et plus longue elle est.

### 2. "Les inconnus connus et les inconnus inconnus

![Donald Rumsfeld]({{ site.url }}assets/misc/external image 061108donald_rumsfeld2.jpg)

Donald Rumsfeld fût moqué pour sa célèbre phrase "inconnus connus", mais il avait raison. Avec le développement logiciel, comme pour n'importe quel [système adaptatif complexe](http://en.wikipedia.org/wiki/Complex_adaptive_system), il y a beaucoup de choses que vous ne pouvez simplement pas prévoir. Nous pouvons, au mieux être conscient qu'il y a des éléments que nous ne pouvons pas prendre en compte dans nos estimations (inconnus connus), mais nous n'avons aucune manière de savoir combien de travail ils représentent. Le mieux que nous puissions faire est de savoir qu'ils sont là. Les inconnus inconnus ? Eh bien, ils sont [plus difficiles à prévoir](http://en.wikipedia.org/wiki/Black_swan_theory) :)


## Pourquoi l'estimation peut être si dangereuse

### Les estimations sont rarement juste des estimations.

Il y a toujours une énorme pression pour savoir quand les choses seront faites et pour de bonnes raisons. Les gens veulent être capable de faire leur travail et c'est difficile si elles ne peuvent pas prévoir quand les choses desquelles elles dépendent seront prêtes. C'est pourquoi une estimation est rarement "juste" une estimation. Les gens utilisent cette information, autrement ils ne seraient pas si acharnés à savoir au premier chef. Vous pouvez leur dire tout ce que vous voudrez, qu'ils ne peuvent pas se reposer dessus, mais ils le feront quand même. Comme Dan North le [tweetait](http://twitter.com/#%21/tastapod/status/116271851767992320) récemment, "les gens demandant du contrôle ou de la visibilité veulent une certitude. Qui n'existe pas".
Certains d'entre nous connaissent la fortune de respirer l'air raréfié des organisations éclairées où la nature imprévisible du développement logiciel est généralement accepté, mais soyons réaliste, la plupart ne le sont pas.

### Recadrer la définition du succès (ou _souligner l'échec de l'estimation_)

L'impact le plus significatif de donner des estimations est dès qu'elles sont dans le domaine public, elles ont tendance à modifier le centre de gravité / la perception du projet, spécialement quand les dates commencent à glisser. Invariablement, un projet de n'importe quelle durée raisonnable, qui aura débuté avec l'objectif honorable de résoudre un problème métier, changera rapidement de focale dès que l'estimation sera achevée.
En fait, il y a déjà ici en réalité un problème bien plus important. Pour la plupart des organisations, la définition du succès demeure "dans les délais et le budget", ce ne sont pas les rentrées financières générées par le projet ou l'amélioration de la productivité, ou de l'apport de nouveaux clients. Il est souvent dit que la vaste majorité des projets informatiques sont considérés comme des échecs et le [Standish Chaos Report](http://www1.standishgroup.com/newsroom/chaos_2009.php) est généralement cité ici. Le problème est qu'_ils_ définissent le succès comme le respect du coût et du délai. La totalité du rapport souligne l'[échec](http://martinfowler.com/bliki/WhatIsFailure.html) [continu](http://theagileexecutive.com/2010/01/11/standish-group-chaos-reports-revisited/) de l'estimation.
Au mieux, donner des estimations à long terme respecte juste la mentalité "dans les délais, dans le budget". Au pire, cela fait démarrer les projets avec de meilleures intentions, puis les entraîne au fond de ce gouffre de l'échec quasi-inévitable et vous - en tant qu'apporteur des estimations - avec.

### Les conséquences...

Toutes les erreurs typiques suivent de près le développement logiciel, et montrent le bout de leurs nez quand l'estimation nous laisse tomber. C'est la première cause des [marches forcées](http://en.wikipedia.org/wiki/Death_march_%28project_management%29). Le périmètre est restreint, la qualité est compromise (au bénéfice supposé du délai), les personnes commencent à se focaliser plus sur comment l'équipe travaille, la pression pour "travailler plus vite" monte, le moral baisse et ainsi de suite - tout cela finalement au détriment de l'objectif principal (à moins que cela soit fait bien sûr pour être dans les délais et le budget, mais comme nous le savons même cela ...).
C'est un cercle vicieux répété dans les organisations dans le monde entier, encore et encore. Je crois fermement que la raison principale de sa répétition est parce que nous ne pouvons échapper à notre obsession avec l'estimation.

## "Mais nous sommes simplement _incapables_ de donner des estimations"

C'est la réponse type lorsque je dis que nous devrions commencer à être brave et à dire simplement non aux demandes de donner des estimations sur n'importe quoi prenant plus de 1 ou 2 mois (au maximum) de travail. Ma réponse à cela est que s'il y a autant de chances que vous arriviez à quelque chose de significatif en jetant des dés ou en caressant la [toison (d'or NdT) de l'estimation](http://estimategoat.com/) alors quel objectif allez-vous satisfaire en faisant cela ?
Quelle est la moins pire situation ? Avoir une situation inconfortable avec votre patron maintenant ou lorsque - basé sur vos estimations - le projet aura dépassé d'un demi-million le budget avec six mois de retard ?

## Conclusion

Certaines personnes semblent encore vouloir s'attacher à l'idée que l'estimation est une activité valable et plus particulièrement que nous sommes capables de donner des estimations à long terme significatives, mais comme je l'ai expliqué ici, c'est un miroir aux alouettes. Mon conseil à quiconque dans cette situation de donner des estimations à long terme est d'être brave et de simplement que ce n'est pas quelque chose que nous pouvons faire, et de faire de son mieux pour expliquer pourquoi. C'est contre l'esprit du développement agile de logiciels, mais ce n'est même pas le sujet, c'est plutôt que c'est dans l'intérêt de personne - sauf, si vous êtes un prestataire logiciel qui se repose sur des frais sur changements de demandes pour continuer à avoir la bourse plein, mais ceci est une autre histoire.

## Epilogue - que faisons-nous à la place ?

C'est évident qu'il n'est pas bon de dire simplement "non", et de partir, et je ne suis certainement pas en train de défendre cela, mais c'est aussi un élément de cet article d'essayer et d'expliquer quelles sont les alternatives. Il y a pléthore de possibilités à partir d'ici, notamment dans les ouvrages dédiés à l'agilité et au lean et de partisans célèbres de l'agilité et du lean, mais mince alors, s'il y a une chose sur laquelle chacune de nos communautés passionnées peut se mettre d'accord est que les meilleurs logiciels viennent du développement itératif piloté par les retours , quelque chose qui est complètement à contrario avec la façon dont l'estimation est actuellement utilisée dans la plupart des organisations.


---
Auteur : [Rob BOWLEY](http://www.les-traducteurs-agiles.org/traducteurs/)  
Source : [Estimation is at the root of most software project failures](http://blog.robbowley.net/2011/09/21/estimation-is-at-the-root-of-most-software-project-failures/)  
Date de parution originale : 21 Septembre 2011  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 12/03/2014  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

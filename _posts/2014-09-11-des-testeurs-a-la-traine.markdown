---
layout: post
title:  "Des testeurs à la traîne"
date:   2014-09-11 22:48:55
tags: test
---
Des complaintes de ce genre, comme par exemple [celle-ci vue sur le yahoogroup Scrumdevelopment](http://groups.yahoo.com/group/scrumdevelopment/message/45191), sont entendues très couramment.

> Généralement dans les différentes phases (d'un projet - NdT), la charge de travail est différente pour un développeur et un testeur. Par exemple, lorsqu'un projet arrive près de la fin, la plupart des tâches restantes seront du test.  

Plusieurs signaux d'alarmes se déclenchent en moi à la lecture de ces deux phrases. Le premier signal d'alarme retentit sur "_différentes phases_". Pourquoi un projet de développement logiciel, et plus spécialement un ayant une durée de quelques semaines ou de quelques mois, a-t-il des phases ? L'autre signal d'alarme retentit sur "_à la fin, la plupart des tâches seront du test._" Décaler le test à la phase finale n'a jamais très bien fonctionné. Cela a _toujours_ résulté en fin de compte pour les testeurs en bout de chaîne d'être à la traîne.  

Est-ce que cette situation ne vous paraît-elle pas familière ? Si oui, que pouvons-nous y faire ?

La plupart des équipes essaient de vivre avec. J'ai vu des équipes institutionnaliser le "bout de chaîne" en implémentant pendant une itération puis en testant dans la suivante. Lorsqu'elles font cela, elles constatent généralement que les anomalies sont trouvées pendant les tests, ce qui a comme conséquence que l'implémentation s'étend ensuite sur deux itérations. Le travail remis à l'ouvrage dans la deuxième itération déborde sur le nouveau travail planifié pour cette itération, et par conséquent les choses continuent de glisser. Et comme il est difficile de dire lorsqu'un élément de travail est _vraiment_ terminé, il est difficile de savoir la quantité de travail tenant dans une itération et à quel moment la livraison sera prête. Souvent, les choses semblent être les mêmes qu'avant la mise en place d'un développement itérative en un temps imparti (NdT - timebox). Cela n'est pas une surprise, parce qu'il n'y a pas vraiment de développement itératif en un temps imparti. Il s'agit de phases de la méthode en cascade déguisées en habits d'agile.

Ne le faites tout simplement pas. Faites les choses complètement et complètement testées avant d'aller plus loin.

**Mais comment ? Ne devez-vous pas attendre que le code soit écrit avant de le tester ?**

Non, vous ne devez pas. Commencez à tester dès que le product owner décrit ce qui doit être fait. Distillez ce qu'il décrit jusqu'à l'essence même de la user story. Soyez certain que le product owner valide que cette distillation _potentiellement automatisable_ corresponde bien ce qu'il désire.

Ensuite, lorsque les développeurs seront en plein travail d'implémentation de la fonctionnalité, les testeurs devraient être en train d'automatiser le test qui la vérifie. Soyez certain, que c'est souvent quelque chose que les testeurs, et l'organisation pour laquelle ils travaillent, ne sont pas accoutumés. Au début, pendant que vous apprendrez, ce sera un peu lent et hésitant. Il est tout à fait compréhensible que les testeurs auront besoin d'un peu d'assistance de la part des développeurs lorsqu'ils automatiseront les tests - après tout, l'automatisation des tests est une forme de programmation.

Le résultat sera que la story ne sera pas prête pour l'acceptance jusqu'à ce que l'implémentation et le test soient faits, et que le test passe. C'est le minimum attendu, mais regardons aussi un peu plus loin.

Avec le temps, cela deviendra plus facile. Les testeurs apprendront à faire plus de tests d'automatisation en ayant besoin de moins d'aide. Le jeu de tests de régression résultant grossira, donnant un retour rapide d'informations que la fonctionnalité qui fonctionnait avant, fonctionne toujours. À la place d'avoir les testeurs de plus en plus à la traîne continuant de vérifier la même fonctionnalité itération après itération, ils seront de plus en plus en amont car le temps de passage des tests sera toujours à peu près le même. Ils auront _plus_ de temps pour faire des tests exploratoires, et cette charge d'exploration sera moindre sur les fonctionnalités élémentaires.  

Il est difficile de faire des tests d'acceptance automatiques un succès. Pourtant en fin de compte, c'est la seule chose qui peut faire du test un succès dans le développement itératif en un temps imparti. Si vous n'arrivez pas à le faire fonctionner, je peux vous garantir que les testeurs seront de plus en plus à la traîne.


---
Auteur : [George Dinwiddie](http://blog.gdinwiddie.com/about/)  
Source : [The testers get behind at the end](http://blog.gdinwiddie.com/2010/02/16/the-testers-get-behind-at-the-end/)  
Date de parution originale : 16 Février 2010  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 11/09/2014  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

---
layout: post
title:  "Le modèle INVEST - T comme stories Testables"
date:   2017-12-17 00:00:01
published: true
tags: 
- user stories
---

Dans le modèle INVEST, le T signifie Testable.

Une _story_ _testable_ est une _story_ pour laquelle, quelque soit les données en entrée, nous pouvons être d’accord sur le comportement du système ou des données attendues.

La testabilité n’exige pas que tous les tests soient définis complètement avant  l’écriture de la toute première ligne de code. Nous devons simplement être confiant - avec discernement -  que nous sommes à même de pouvoir les définir et de pouvoir nous mettre d’accord au sujet des tests.

La testabilité n’exige pas que les tests soient automatisés. Il y a des avantages à l’automatisation, mais les tests peuvent s’avérer utiles même sans.

La testabilité n’exige pas que nous traitions les tests comme des spécifications à part entière, dans lesquelles toute chose  qui s’avérerait manquante pourrait faire s’écrouler l’édifice tout entier. À la place, nous nous focalisons sur les tests intéressants qui permettent de clarifier certaines décisions pouvant prêter à confusion ou à controverse.

Tester, même en considérant les tests comme un outil collaboratif, n’est pas chose nouvelle. Il y a des outils pour aider à spécifier les tests - xUnit, Cucumber, fit, ou simplement le langage naturel. Mais l’usage des outils est insuffisant ; vous pouvez commettre encore beaucoup d’erreurs.

Nous allons regarder ensemble les défis auxquels vous pouvez faire face quel que soit l’outil ou la technique :

* La magie
* Le flou intentionnel
* L’infaisabilité technique
* Le non-déterminisme
* La subjectivité
* Les projets de recherche

## La magie

![Le bâton magique]({{ site.url }}assets/bill_wake/Magic_wand.png)

Certains tests reposent sur une part de magie ou d’intuition. Malheureusement, (quoi que nous puissions penser des humains) les ordinateurs ne possèdent ni l’un ni l’autre.

Un test se passe dans un certain contexte, avec des données en entrées et/ou des étapes, puis produit des résultats en sortie et/ou des effets de bord.

Ce n’est pas parce que nous écrivons des données en entrée et que nous obtenons des résultats que cela veut dire que nous avons un bon test. Les résultats doivent aussi être en fonction des éléments en entrée ; ils ne peuvent dépendre d’éléments en entrée non spécifiées. 

> Par exemple, nous aimerions avoir un programme permettant de prédire le cours de la bourse du lendemain en fonction de ceux des jours précédents.
>
> Nous avons beaucoup de cas de tests - près d’un siècle d’exemples concernant plusieurs centaines de titres en bourse. 
>
> Mais, au fond, ce que l’on veut c’est de la magie, à moins de croire en quelque chose de très improbable : que le cours de bourse du jour soit uniquement déterminé par l’historique des cours précédents. Supposons que 50% des raffineries de pétrole vont s’arrêter pour les 6 prochains mois. Croyez-vous vraiment que cette nouvelle n’affectera pas les cours des compagnies du pétrole, aériennes et automobiles ?

## Le flou intentionnel

Dans certains cas, des algorithmes existent mais des choix doivent être faits. Un certain flou peut s’avérer accidentel mais dans certains cas intentionnel : le service commercial veut rouge, et le marketing veut vert. Plutôt que de faire un choix qui pourrait vexer l’un ou l’autre, le test se cachera derrière un certain flou artistique en indiquant “la couleur appropriée”. 

## L’infaisabilité technique

Certaines choses sont faisables techniquement, voire même trop faciles à spécifier, mais qui sont infaisables au-delà d’un certain seuil. Par exemple, trouver le chemin exact le plus court possible sur une très grande carte est très coûteux.

Vous pouvez laisser tomber vos critères et vous contentez d’une approximation. Si nous reprenons l’exemple de la carte, avoir une précision approximative d’un facteur 2 s’avèrera substantiellement moins cher.

## Le non-déterminisme

Une partie du non-déterminisme est due à des facteurs aléatoires ou pseudo-aléatoires.

Une autre partie du non déterminisme se produit lorsqu’il existe une variété ou un ensemble de réponses acceptables.

![Boggle]({{ site.url }}assets/bill_wake/Boggle.png)

> Par exemple, je souhaite un programme de génération de puzzles qui, à partir d’une liste de mots, créant et affichant un plateau à la _Boggle_ c.à.d sous la forme  d’une grille de lettres à partir de laquelle vous pouvez former des mots, en allant d’une lettre à une autre adjacente dans n’importe quel ordre.
>
> Si cela peut être fait dans l’absolu, cela peut être fait sûrement de plusieurs manières, étant donné qu’à partir d’une solution vous pouvez en générer d’autres par réplication ou par rotation. (Vous pourriez avoir encore plusieurs autres solutions différentes.) 
>
> Je me fiche de savoir quelle solution est choisie ; n’importe solution valide me convient.

Au final, le résultat d’une opération arithmétique à virgule flottante n’est qu’une approximation d’une opération sur un nombre réel. En raison des variations possibles dans le calcul, vous pourriez obtenir des réponses qui varient d’un pouième.

Le premier défi avec le non-détermine est de reconnaître quand ce dernier se produit. Lorsque cela arrive, vous pourriez avoir à spécifier lorsque deux réponses sont équivalentes ou également acceptables 

## Subjectivité

Certains tests peuvent être définis correctement mais faire l’objet de standards subjectifs.

> Par exemple, “7 personnes sur 10 sont d’accord sur le fait que c’est amusant”. Vous pouvez préciser ce que vous voulez dire par personnes - mais “amusant” reste une notion subjective.

L’utilisabilité et d’autres éléments “non fonctionnelles” rencontrent le même genre de difficulté : “9 utilisateurs [pertinents] sur 10 peuvent accomplir une tâche standard en moins de 5 minutes après 30 minutes d’entraînement.”

Il n’y a aucune garantie en terme de faisabilité pour des tests subjectifs. De plus, ils peuvent être extrêmement coûteux à faire. Cependant, il n’est pas anormal d’en avoir, mais vous devez prendre conscience qu’il n’y a aucune garantie sur la facilité avec laquelle des standards subjectifs pourront être atteints.

## Le projet de recherche

Il est possible de spécifier ou de définir un test qui est valide, mais que vous ne savez pas vraiment résoudre. (Testable ? Oui ! Risqué ? Très !)

C’est-à-dire : vous pouvez écrire des tests pour quelque chose que vous ne savez comment implémenter, et toute estimation que vous ferez s’avèrera suspecte parce ce que vous estimez est un projet de recherche. 

> Par exemple, considérons le défi d’identifier des piétons dans la rue. À partir d’une image, nous pourrions demander à 1 000 personnes d’identifier les piétons avec un indice de confiance plutôt élevé. Mains nous ne sommes pas certain de comment les gens ont fait - nous pensons que cela peut être fait de manière algorithmique, mais le prouver peut représenter un projet de recherche de plusieurs années. (Toutefois, les progrès dans les véhicules autonomes montre que cela est possible).

Il n’y a rien de mal à avoir un projet de recherche si c’est ce dont vous avez besoin et que vous en acceptez le risque. Ne vous leurrez pas en pensant qu’il s’agit d’une simple affaire de programmation alors que ce n’est pas le cas.

## Mots-clés testables

Étant donné tous les défis relatifs aux tests que nous avons mentionnés ci-dessus, comment pouvons-nous être sûr que nous écrivons les bons tests ?

J’ai découvert qu’il y a des mots-clés qui peuvent vous alerter de problèmes potentiels présents dans les tests ou dans des discussions tournant autour des tests : 

* “**Juste**” – c’est un si petit mot, mais il est souvent utilisé comme un élément déstabilisant, pour minimiser l’importance de certaines difficultés sans les résoudre. (“Vérifie juste chacun de ces éléments par rapport aux autres.”)

* “**Approprié**,” “**correct**,” “**convenable**” – bien sûr vous souhaitez que la chose appropriée soit faite - mais cela ne définit pas pour autant ce qu’“approprié” signifie.

* “**Meilleur**,” “**pire**” – dire “meilleur” ne permet pas de définir qu’est ce qu’on entend par meilleur.

* “**le plus**,” “**le moins**,” “**le plus court**,” “**le plus long**” – si vous êtes clair sur ce que vous voulez le plus ou le moins, ça aide, mais ces mots peuvent cacher aussi des choix de qui peuvent s’avérer très couteux techniquement.

* “**Toutes les combinaisons**,” “**Toutes les permutations**” – ces expressions peuvent indiquer des choses qui sont bien définis mais qui peuvent s’avérer techniquement infaisable.

* “**N’importe lequel des**,” “**peu importe**” – ces expressions s’accompagnent souvent d’exemples non-déterministes. Elles sont légitimes, mais il peut s’avérer difficile de spécifier des cas tests avec de tels exemples. (Pourriez-vous lister toutes les solutions possibles ?)

* “**Amusant**,” “**facile à utiliser**,” “**personnes**,” “**aimer**“, … – on retrouve généralement ces mots dans des attributs non-fonctionnels, ou ils peuvent dissimuler un projet de recherches.

* “**Je saurai quand je le verrais**” – il n’y a aucune chance que vous y arriviez en une fois. 

## En résumé

Des _stories_ testables permettent aux équipes de se mettre d’accord sur ce qui est souhaité. Les tests favorisent la collaboration : elles permettent de clarifier ce qui serait confus, et de partager une compréhension commune entre les personnes.

Nous avons regardé certains des défis qui se posent aux tests :

* _Difficiles à corriger_: magie, flou intentionnel
* _Des défis dont il faut avoir conscience_: infaisaibilité technique, non-déterminisme
* _Des risques qu’il ne faut pas accepter accidentellement_: subjectivité, projets de recherche

Nous avons conclu avec quelques mots clés qui peuvent indiquer lorsque vous êtes face à des défis relatifs aux tests.

Cet article clôt la série d’articles dédiée au modèle INVEST. Vous trouverez ci-dessous les liens vers les articles précédents.

## Resources

* [INVESTissez dans de bonnes stories et dans des tâches SMART](http://www.les-traducteurs-agiles.org/story/2015/02/23/investissez-dans-de-bonnes-stories-et-dans-des-taches-smart.html)
  * [Le modèle INVEST - I comme stories Indépendantes](http://www.les-traducteurs-agiles.org/2017/02/21/le-modele-invest-les-stories-independantes.html)
  * [Le modèle INVEST - N comme stories Négociables](http://www.les-traducteurs-agiles.org/2017/03/12/le-modele-invest-les-stories-negociables.html)
  * [Le modèle INVEST - V comme stories ayant de la Valeur](http://www.les-traducteurs-agiles.org/2017/04/25/le-modele-invest-pour-des-stories-de-valeur.html)
  * [Le modèle INVEST - E comme stories Estimables](http://www.les-traducteurs-agiles.org/2017/08/08/le-modele-invest-pour-des-stories-estimables.html)
  * [Le modèle INVEST - S comme stories Suffisamment petites, extenSibles](http://www.les-traducteurs-agiles.org/2017/10/16/le-modele-invest-pour-des-stories-suffisamment-petites-extensibles.html)
  * [Le modèle INVEST - T comme stories Testables](http://www.les-traducteurs-agiles.org/2017/12/17/le-modele-invest-pour-des-stories-testables.html)


---
Auteur : [Bill Wake](http://xp123.com/about/)  
Source : [Testable Stories in the INVEST Model](https://xp123.com/articles/testable-stories-in-the-invest-model/)  
Date de parution originale : 09 Février 2017  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 17/12/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



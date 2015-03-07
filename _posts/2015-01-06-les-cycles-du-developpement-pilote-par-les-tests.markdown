---
layout: post
title:  "Les cycles du développement piloté par les tests (TDD)"
date:   2015-01-06 22:55:55
categories: TDD
---
Lorsque vous commencez à apprendre le développement piloté par les tests, cela semble simple et facile. Si comme moi vous l'avez appris en 1999, la règle était simplement d'écrire vos tests unitaires d'abord. En effet, à l'époque, nous appelions cela la conception préalable par les tests.  

En 1999, je me suis assis à côté de Kent Beck et me suis mis à travailler en binôme avec lui pour apprendre. Ce qu'il m'enseigna fût certainement de faire d'abord les tests ; mais cela impliquait un processus plus fin que ce que j'avais pu voir jusqu'à présent. Il écrivait _une ligne_ d'un test qui échouait, puis il écrivait la _ligne_ de code de production correspondante pour faire passer le test. Quelques fois, c'était un peu plus qu'une ligne ; mais l'échelle de grandeur qu'il utilisait était très proche du ligne à ligne.  

## **Seconde par seconde :** _le nano cycle_ : les trois lois du TDD

Quelques années plus tard, cette granularité fine fut codifiée en 3 règles : les fameuses [trois lois du TDD](http://programmer.97things.oreilly.com/wiki/index.php/The_Three_Laws_of_Test-Driven_Development).  

1. Vous devez écrire un test qui échoue avant d'écrire tout code de production
2. Vous ne devez pas écrire plus d'un test suffisant pour échouer, ou qui échouera à la compilation
3. Vous ne devez pas écrire plus de code que nécessaire pour faire passer le test en cours

Au fur et à mesure des années, moi, [et beaucoup d'autres](http://bit.ly/1AEPxKX), avons écrit sur ces trois lois. Elles existent maintenant sous différents styles, formats et injonctions. Mais le but a toujours été de promouvoir la granularité _ligne à ligne_ que j'avais expérimenté à l'époque avec Kent.  

Ces _trois lois_ sont le _nano-cycle_ du TDD. Vous les suivez presque seconde par seconde. Vous allez itérer dessus une douzaine de fois ou presque avant de finir un seul test unitaire.  

## **Minute par minute :** _le micro cycle_ : Rouge-Vert-Refactorer

Si nous revenons à une échelle de grandeur minute par minute, nous voyons le _micro cycle_ que suivent les pratiquants du TDD. Le _cycle_ [Rouge-Vert-Refactorer](http://www.jamesshore.com/Blog/Red-Green-Refactor.html).  

<div align="center">
    <img src="{{ site.url }}assets/cycles_tdd/06_rouge_vert_refactor.png" />
</div>

Ce cycle est exécuté généralement une fois par test terminé, ou une fois toutes les douzaines de cycles des trois lois. Les règles de ce cycle sont simples.
1. Créer un test unitaire qui échoue
2. Écrire le code de production qui fera passer ce test
3. Nettoyer le bordel que vous avez mis

Cette philosophie est basée sur l'idée que nos intellects limités ne sont pas capables de poursuivre deux objectifs simultanément de tout système informatique : 1. Corriger le comportement, 2. Corriger la structure. Le cycle RVR nous indique que le premier objectif est de faire un logiciel qui fonctionnement correctement ; et ensuite, _et seulement à ce moment-là_ , de se concentrer de donner à ce logiciel opérationnel une structure qui tienne à long terme. 

Là aussi, [beaucoup](http://bit.ly/1AESA5D) de personnes ont écrit sur ce cycle. En effet, l'idée dérive de l'[injonction originelle de Kent Beck](http://c2.com/cgi/wiki?MakeItWorkMakeItRightMakeItFast) :

> Faites-le fonctionner, faites-le bien, faites-le vite  

Une autre manière de considérer cette idée, c'est :  

> Faire fonctionner un logiciel, c'est seulement la moitié du boulot

[Deux choses](http://seasidetesting.com/2013/03/12/testing-and-the-two-values-of-software/) sont importantes aux yeux des clients à propos d'un logiciel. La manière dont il fait se comporter une machine ; et la facilité avec laquelle il peut être modifié. Un compromis sur l'une ou l'autre de ces deux valeurs et le logiciel aura moins de valeur pour les clients.  

Exécuter le cycle rouge/vert/refactorer prend environ une minute. C'est la granularité du refactoring. Le refactoring  n'est pas quelque chose que vous faites à la fin du projet : c'est quelque chose que vous faites _minute par minute_. Il n'existe aucune tâche sur le plan projet qui indique : refactoring. Il n'y a pas de temps réservé à la fin du projet, ou de l'itération, ou de la journée pour le refactoring. Le refactoring est un activité continue , pas quelque chose qui est effectuée tardivement (et donc optionnellement).  

## **Déca-minute par déca-minute :** _le milli cycle_ : spécifique/générique

En remontant au niveau des 10 minutes, nous voyons le milli cycle en action. [Le cycle spécifique/générique](http://thecleancoder.blogspot.com/2010/11/craftsman-63-specifics-and-generics.html).  

> Au fur et à mesure que les tests deviennent plus spécifiques, le code devient plus générique.  

Au fur et à mesure qu'une suite de tests grossie, elle devient plus spécifique, c'est à dire qu'elle devient une _spécification_ du comportement encore plus détaillée. Les bons développeurs d'applications font face à cet accroissement de spécifications par un accroissement de la _généricité_ de leur code. Pour le dire autrement : _les développeurs font fonctionner des cas spécifiques en écrivant du code qui fait fonctionner le cas général_.  

En règle générale, le code de production devient de plus en plus générique si vous pouvez penser aux tests que vous n'avez pas écrit ; mais que le code de production pourra faire passer tout de même. Si le changement que vous faites dans le code suite à un test, fais passer ce test, mais qu'il ne pourrait pas faire passer d'autres tests non écrits, alors vous êtes sûrement en train de faire un code de production trop spécifique.  

Il est souvent dit que la structure fine des trois lois et du cycle rouge/vert/refactorer conduisent à des  [optimisations locales](http://c2.com/cgi/wiki?RefactoringEqualsReparametrization). Sans un " schéma général ", le développeur ne peut donner au logiciel une structure correcte pour répondre au problème global, et peut conduire à la place à la mise en place d'une structure correcte pour le cas spécifique, mais incorrecte pour le cas général.  

Le symptôme de l'optimisation locale est " [d'être bloqué](http://thecleancoder.blogspot.com/2010/10/craftsman-62-dark-path.html) ". Afin de faire passer le prochain test, vous devez écrire une grosse quantité de code _en dehors_ du nano cycle des trois lois, et même en dehors du micro cycle du RVR. Autrement dit, vous avez pris un chemin qui vous force à sortir du processus du TDD.  

Une fois que vous êtes bloqué, la seule solution est de faire marche arrière sur les tests précédents, de les supprimer, jusqu'à que vous trouviez un test à partir duquel vous pourrez prendre un chemin différent.  

Pourquoi avez-vous été bloqué ? Parce que vous n'avez pas inclus assez de généricité au code de production. Vous avez rendu les tests trop spécifiques trop rapidement. La solution est de faire marche arrière et d'ajouter des spécificités aux tests plus lentement, tout en ajoutant de la généricité au code de production plus rapidement. Cela vous force  plus fréquemment à choisir un jeu de tests différent à suivre.  

Pour éviter d'être bloqué, nous évaluons notre position toutes les quelques minutes ; en recherchant les spécificités dans le code de production. Avons-nous pris des raccourcis pour rendre le code de production plus semblable aux tests d'une quelconque manière ? Est-ce que les modifications récentes au code de production ne permettent plus de faire passer plus de tests que nous n'en avions écrits ?  

C'est ce cycle que nous appliquons dans la [prémisse prioritaire de la transformation](http://en.wikipedia.org/wiki/Transformation_Priority_Premise). Nous recherchons les symptômes de la sur-spécification en vérifiant les types de code de production que nous avons écris.

## **Heure par heure** : _Le cycle primaire heure par heure_ : les limites 

Le dernier cycle du TDD est le cycle primaire qui permet aux autres cycles de nous conduire vers une [architecture propre](http://blog.8thlight.com/uncle-bob/2012/08/13/the-clean-architecture.html). Toutes les heures ou presque, nous nous arrêtons et vérifions si nous avons franchis, ou atteint, une limite architecturale significative. Souvent ces limites sont difficiles à voir en plein nano ou micro cycle. Vous pouvez commencer à les percevoir au niveau déca-minute,  même si notre attention est encore trop étroitement focalisée. 

Ainsi chaque heure ou presque, nous nous arrêtons et regardons le système dans sa globalité. Nous recherchons les limites que nous voulons contrôler. Nous prenons les décisions où tracer ces limites, et de quel côté de ces limites, nos activités actuelles devraient être contraintes. Ensuite, nous utilisons nos décisions pour reprendre de manière avisée les nano cycles, les micro cycles, et les milli cycles pour l'heure suivante  - le cycle _primaire_ - du développement piloté par les tests.  


---
Auteur : [Uncle Bob](http://www.8thlight.com/team/uncle-bob)  
Source : [The Cycles of TDD
](http://blog.cleancoder.com/uncle-bob/2014/12/17/TheCyclesOfTDD.html)  
Date de parution originale : 17 Décembre 2014  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 06/01/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

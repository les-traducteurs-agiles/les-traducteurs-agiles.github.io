---
layout: "post"
title: "Le développement à double voie n'est pas un duel de voies"
date: "2018-03-18 00:01"
tags: 
- agile
---

tl;pl

Si vous n'avez jamais entendu parler du terme "développement à double voie", cet article explique d'où vient ce terme et ce qu'il signifie. Voici quelques points de repères.

* Le travail de développement se focalise sur la prédictabilité et la qualité
* Le travail de découverte se focalise sur un apprentissage  et une validation à partir de ce que nous avons appris rapide
* La découverte et le développement peuvent être vus sous la forme d'une double voie parce qu'il s'agit de deux différents types de travail et de deux différentes manières d'appréhender les choses.
* La découverte est une partie essentielle du développement produit. Appliquez-la avec les mêmes principes agiles et lean à l'esprit.
* Si nous faisons le travail de découverte correctement, nous modifions substantiellement et pouvons éliminer pas mal d'idées.
* Tandis qu'un responsable produit, un concepteur ou ingénieur peuvent tout à fait  être capable de conduire et d'orchestrer le travail de découverte, ils doivent impliquer l'ensemble de l'équipe dans ce travail dès que cela est possible. Il est nécessaire que le travail de découverte et son avancée reste visible de l'ensemble de l'équipe.
* Après la livraison, continuez de mesurer et d'apprendre   

Maintenant, si quelqu'un vous demande le sujet de cet article, vous pouvez répondre sans avoir à lire les 1 500 mots qui vont suivre.

---

## Personne ne l'appelle vraiment à double voie

Il y a quelques années, je faisais une formation avec mon ami [Marty Cagan](http://svpg.com/). C'était juste le contenu de ma formation et de la sienne réunis ensemble pour une formation 3 jours. Mais lors de mon intervention, j'ai affiché un modèle que je montre habituellement lorsque j'aborde le sujet de comment la pensée Agile et la pensée produit fonctionnent ensemble dans le même processus. Ce modèle ressemble à peu près à cela :

![Modèle à double voie de Sy]({{ site.url }}assets/jeff_patton/sy-dual-track-model-fr.jpg)

J'avais dessiné ma propre version de ce modèle, donc il ne ressemble pas tout à fait à ça. Mais, Marty m'a demandé d'où venait ce modèle. J'ai ouvert le document original de Desiree Sy (prononcé Si) dénommé [Adapting Usability Investigations for Agile User-centered Design](https://uxpa.org/sites/default/files/agile-ucd_0.pdf)

<div align="left" style="float:left; padding-right:30px" >
  <img title="Desiree Sy" src="{{ site.url }}assets/jeff_patton/desiree-sy-200x200.jpg" />
</div>

Voici Desiree. Vous allez l'aimer. C'est quelqu'un de vraiment très intelligent.

Son article de 2007 décrit un schéma réccurent auquel un certain nombre de personnes qui font des travaux de conception et de validation de manière très rigoureuse en développement agile sont arrivés à la même conclusion. Parce qu'il s'agit de la seule manière qui peut vraiment fonctionner. À l'époque, Desiree travaillait chez Alias désormais filiale d'Autodesk ; elle et ses collègues travaillaient de manière assez fluide. Ensemble, ils faisaient ce que la plupart des personnes de l'époque considéraient comme quelque chose situé entre super-difficile et impossible. Mais, pour eux, cela semblait naturel. Pas forcément facile, mais ça marchait.

Marty m'a demandé "Comment s'appelle ce modèle ?"

"Il n'a pas vraiment de nom" ai-je dit. "C'est simplement la manière dont ça marche"

"Comment l'appelle t'elle ?" demanda Marty.

Nous avons parcouru le document et avons trouvé ce paragraphe.

![Citation de Desiree Sy]({{ site.url }}assets/jeff_patton/sy-dual-track-quote-fr.jpg)

Si je ne garde que la partie importante, voici ce que dit le texte

> "… nous travaillons étroitement avec les développeurs tout au long de la conception et du développement. Bien que les deux voies semblent séparées, en réalité, les concepteurs doivent communiquer tous les jours avec les développeurs."

Et c'est tout. Marty a commencé à utiliser ce terme dans ses formations à destination des responsables produit. Et étant donné que je fais des formations souvent aux mêmes personnes j'ai commencé à utiliser ce terme. Puis petit à petit d'autres ont commencé à utiliser ce terme.

Maintenant je dois vous dire que je déteste ce terme, et je vais vous dire pourquoi.

## C'est double voie et non un duel de voies

La plupart des gens ne lisent pas. C'est d'ailleurs un miracle que vous ayez lu jusque-là. Félicitations.

Mais les gens regardent les images. Et l'image d'une double voie semblent suggérer différents types de travaux faits par différentes personnes - comme les responsables produits et les concepteurs d'un côté essayant de deviner ce qu'il y a à mettre en place, et les développeurs essayant de deviner ce qu'il y a à construire. Et dans le pire des cas, vous pourriez l'interprêter en vous disant que les développeurs doivent attendre pendant plusieurs semaines que les responsables produit et les designeurs aient fini leur m\***. Ce n'est pas censé fonctionner comme cela. Si toute l'équipe doit être responsable du succès du produit, pas simplement de le construire, alors toute l'équipe doit comprendre et contribuer aux deux différents types de travaux.

J'aimerais un terme différent et une image différente. Mais, je n'ai pas de meilleur terme ou de meilleure image pour l'instant. Toutefois, je vais essayer de dessiner quelques illustrations afin de compléter celle-là.

## Il y a bien deux types de travaux et il n'y aucun moyen de faire autrement

### Travaux de développement

Si vous avez déjà travailler en mode agile avant, vous savez que les équipes parlent beaucoup de vélocité. Mais la vélocité dont elles parlent est la vélocité de développement. Les équipes tergiversent toujours dès qu'il s'agit de leur capacité de prévision. Au démarrage du sprint, elles estimeront leur vélocité, et à la fin, elles le mesureront. Idéalement, leurs prévisions seront exactes.

![Cycle de développement]({{ site.url }}assets/jeff_patton/development-cycle-768x296-fr.jpg)

Quand vous livrez quelque chose qui doit aller en production, la qualité est très importante. Si vous mettez du logiciel en production, la qualité, la scalabilité, la performance, la traduction, et plein d'autres sujets sont importants. Donc, le fruit des travaux de développement devrait être compilé, testé, puis revu par autrui pour vérifier tous ces éléments. Les équipes agiles parlent énormément de "logiciel potentiellement livrable" ce qui signifie en réalité qu'elles n'ont peut être pas suffisamment travaillé pour livrer, mais une fois qu'elles ont fini, la qualité est d'un niveau suffisant pour qu'elles puissent livrer en toute confiance.

> Les travaux de développement se concentrent sur la capacité de prévision et la qualité

### Les travaux de découverte

L'une des tragédies dans le développement logiciel, et pour ce que cela vaut dans toutes les activités de développement produit, est que la plupart de ce que nous faisons ne rencontrent pas le succès escompté. Nous n'obtenons pas le bénéfice attendu. C'est donc un problème. Mais, même avant ça, cela prend du temps pour en savoir suffisamment sur les problèmes que nous essayons de résoudre afin de prendre les bonnes décisions sur ce que nous devrions construire. Nous utilisons les travaux sur la découverte pour faire tout ça. Pour répondre aux questions, tester des idées, et éviter - autant que possible -  perdre du temps en surinvestissant sur des travaux de très bonne qualité que nous ne devrions pas faire tout simplement.

Nous voulons apprendre aussi rapidement, aussi peu cher, et aussi sans encombres que possible. La vélocité est donc importante aussi lors de la découverte - mais il s'agit d'une vélocité d'apprentissage.

> Les travaux sur la découverte se concentrent sur un apprentissage rapide et une validation de nos hypothèses rapide.

Parce que l'objectif est d'apprendre, et non d'avoir un logiciel opérationnel, la boucle d'apprentissage de la découverte ressemble à peu près à cela.

![Cycle de découverte]({{ site.url }}assets/jeff_patton/discovery-cycle-768x257-fr.jpg)

Cela commence par décrire :

* La compréhension que nous avons du problème que nous résolvons et pour qui
* La solution que nous devrions construire pour le résoudre
* Comment nous allons mesurer le succès

C'est notre pari, notre intuition, notre croyance, notre hypothèse. Tous ces mots inconfortables que les gens qui pensent construire ce qui est correct. Mais, à vrai dire, nous faisons toujours le pari que nous allons gagner. Dans ce pari, il y a beaucoup de suppositions, de risques, et peut-être même de questions. Pour concentrer notre apprentissage, nous allons choisir la supposition, le risque, ou la question qui nous effraye le plus et allons identifier une expérience ou une méthode pour apprendre. Puis l'appliquer. Puis utiliser ce que nous avons appris pour changer toutes ces croyances à propos des problèmes et des solutions.

Malheureusement, une des manières les plus coûteuses en temps et en argent pour apprendre est de créer un logiciel potentiellement livrable. Donc nous ne le faisons pas - à moins que nous n'ayons pas vraiment le choix de faire autrement pour apprendre, ou que nous ayons une confiance aveugle sur la réussite de notre pari. Rappelez-vous, nous ne parions pas sur le fait que nous allons finir dans les temps. Nous parions sur le fait que les personnes, ayant le problème que nous sommes en train de résoudre, essayerons, utiliserons et adopteront notre solution en toute bonne foi.

> La manière la plus coûteuse de tester notre idée est de réaliser un logiciel ayant un niveau de qualité suffisant pour aller en production.

C'est de cette manière que fonctionne la boucle d'apprentissage. Et voici un certain nombre de choses que vous devriez savoir à ce sujet.

**Nous faisons tout cela aussi vite que nous le pouvons.** En quelques heures lorsque c'est possible. Quelques fois cela peut prendre quelques jours. Mais, nous espérons que cela ne prendra pas quelques semaines. Par conséquent, nous devrions avoir plusieurs boucles d'apprentissages par la découverte dans un sprint-type de 2 semaines.  

**Les résultats des travaux de découverte ont comme conséquence d'éliminer les idées.** À la fin de chaque test, vous avez une décision à prendre : construire, éliminer ou continuer à apprendre. Oui, tout à fait, ce que je suis en train de dire ici est que les travaux de découverte peuvent et devraient avoir comme résultat d'éliminer des idées. Tout ne doit pas continuer. Certaines personnes peuvent se sentir mal à l'aise avec ça.

**Nous donnons une durée fixe aux cycles de découverte.** Pour éviter que les coûts liés aux travaux de découverte ne nous échappent, nous allons donner une durée fixe à un test ou à une expérience allant de quelques heures à quelques jours.

**Nous ne pouvons pas prévoir ce que nous allons apprendre demain** - du moins pas aisément. Lorsque nous apprenons quelque chose de vraiment valable, cela à tendance à changer en profondeur nos croyances du moment, et cela change vraiment ce que sera notre prochaine grosse supposition ou notre prochaine grosse question. Ça peut vraiment mettre le bordel.

L'enchaînement des boucles de découverte ressemblent à peu près à cela :

![Itérations de découverte]({{ site.url }}assets/jeff_patton/discovery-iterations-768x311-fr.jpg)

Désormais, il devrait être clair qu'à la fois les travaux de développement et les travaux de découverte sont essentiels. Mais l'état d'esprit avec lequel vous abordez ces travaux, et le processus pour les faire, sont très différents.

### OK, c'est en fait 3 types de travail différents …

Pour commencer à réaliser un logiciel, vous aurez besoin de prendre beaucoup de décisions tactiques au niveau de la conception. Ces décisions ne sont peut être pas des décisions à risque pour lesquelles il est nécessaire d'avoir une validation, mais elles doivent être prises tout de même. C'est souvent les concepteurs qui doivent prendre du temps en amont du développement pour affiner et achever les travaux de conception avant toute écriture de code.

> Si vous validez qu'un produit vaut le coup d'être réalisé, vous aurez probablement besoin de faire des travaux de conception détaillée avant de commencer à écrire du code

## Tout se passe en même temps

Ce serait super si nous pouvions tous nous concentrer sur les travaux de découverte, tout terminer, puis porter notre attention sur la conception tactique et le développement. Et cela pourrait marcher si tous les membres de l'équipe avaient les mêmes compétences. Mais étant donné que certains sont bons à écrire du code, d'autres bons sur la conception de l'expérience utilisateur, et d'autres bons à toute une variété d'autres choses, nous avons l'opportunité de faire plusieurs types de choses en même temps. Donc nous le faisons.

> Les travaux de découverte se déroulent de manière concurrente et continue aux travaux de développement.

J'ai dessiné dernièrement ce modèle unifié de la manière suivante :

![Diagramme double voie]({{ site.url }}assets/jeff_patton/dual-track-diagram-1024x577-fr.jpg)

Les travaux de découverte ont des cycles de longueurs irrégulières. C'est "Lean" dans le sens où nous essayons d'avoir un cycle de découverte aussi court que possible. Les idées dans ces moments-là changent et sont très souvent abandonnées. La meilleure manière d'avancer est de passer délibéremment en cycle de développement. Je ne suis pas certain de savoir comment montrer tout cela en un seul dessin. Mais, c'est que ce j'essaie de faire dans l'illustration ci-dessus.

> La découverte et le développement sont montrés sur deux voies distinctes parce qu'il s'agit de deux différents types de travaux, et de deux différents manières d'appréhender les choses.

## Deux voies, pas deux équipes

Mais, vous ne devriez pas y penser comme deux processus séparés - il s'agit simplement des deux parties d'un même processus. Et, je pense que vous faites aux développeurs et aux autres personnes de l'équipe un mauvais service que de ne pas les impliquer dans les travaux de découverte.

Il y a généralement assez de travaux de découverte à faire et plusieurs manières de s'impliquer pour que toute l'équipe ait quelque chose à faire. Si vous sentez une pression pour raccourcir les travaux de découverte pour "nourrir la bête", cela signifie généralement que vous prenez des décisions sur la réalisation du logiciel avant que vous en ayez appris assez pour être en confiance pour prendre des décisions. Dans le meilleur des cas, les effets sont incertains et de manière plus générale, les effets sont plutôt mauvais.

> Toute l'équipe est responsable quant aux effets du produits, et non simplement de la livraison dans les temps.

## Démystifier les mythes relatifs à la double voie

Laissez-moi disperser à nouveau les plus gros malentendus que les gens ont sur ce modèle.

Mythe :  La découverte est un processus précédant le développement agile. Cela ne devrait pas être le cas.

> La découverte est un partie essentielle du développement produit. Appliquez-la avec les mêmes principes agiles et lean à l'esprit.

Mythe : Tous les travaux passent de la découverte au développement. Non, ce n'est pas vrai.

> Si nous faisons correctement la découverte, nous modifions substantiellement et éliminons pas mal d'idées.

Mythe : L'équipe de découverte est différente de celle de développement. Cela ne devrait pas être le cas.

> Tandis qu'un responsable produit, un concepteur ou ingénieur peuvent tout à fait  être capable de conduire et d'orchestrer le travail de découverte, ils doivent impliquer l'ensemble de l'équipe dans ce travail dès que cela est possible. Il est nécessaire que le travail de découverte et son avancée reste visible de l'ensemble de l'équipe.

Mythe : Une fois que vous êtes passé de la découverte au développement, les travaux de découverte sont terminés. Ce n'est pas le cas.

Ce dernier malentendu emmerde vraiment mon ami Jeff Gothelf. Pour lui, le logiciel de qualité-production que nous venons de réaliser et qui a atteint un niveau de qualité de production, est considéré comme étant simplement notre dernière meilleure expérience.

> Continuez à mesurer et à apprendre même après que vous ayez livré.

Du point de vue de Jeff Gothelf, tout est découverte and nous apprenons à partir de tout ce que nous faisons ; que ce soit un prototype papier, ou la prochaine fonctionnalité dans votre logiciel en production. Je suis d'accord avec lui.

## Il y a bien davantage avec cette histoire

J'ai parlé conceptuellement sur ce que sont les travaux de découverte et de développement, et pourquoi vous devez les combiner en un seul processus. Mais, j'en ai dit très peu dit sur comment vous le faites en pratique. Vous devez vous sentir légèrement frustré. Désolé pour ça.

Mais il s'agit du tout premier article d'une série que je suis en train d'écrire. Les prochains articles aborderont :

* Comment maintenir la découverte visible dans un processus agile-type tel que Scrum
* Comment adapter une planification, un standup, ou des revues agiles-types afin qu'elles abordent à la fois la découverte et le développement
* Comment envisager votre prochaine super expérience et étaler l'investissement de la découverte tout au long du projet en toute confiance

Quelles sont les questions pouvant restant en suspens de votre côté ? Quel est votre plus grand défi lorsque vous faites ça ? Dites-moi quels sont les sujets que je devrais aborder et que je n'ai pas mentioné ci-dessus.

---  
Auteur : [Jeff Patton](http://jpattonassociates.com/about-jeff-patton/)  
Source : [Dual Track Development is not Duel Track](https://jpattonassociates.com/dual-track-development/)  
Date de parution originale : 10 Juillet 2017  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 18/03/2018  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}


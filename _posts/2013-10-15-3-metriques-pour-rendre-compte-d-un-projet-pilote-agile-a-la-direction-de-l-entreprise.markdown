---
layout: post
title:  "3 Métriques pour rendre compte d'un projet pilote agile à la direction de l'entreprise"
date:   2013-10-15 00:01
published: true
tags:
- indicateur
---

Lors de l'introduction de Scrum en entreprise, par le biais d'un projet pilote agile par exemple, se pose la question de savoir **comment rendre compte à la direction de l'entreprise**. Je suggèrerais d'utiliser les trois métriques suivantes comme point de départ :

1. **retour client**
2. **burnup de livraison**
3. **indice de bonheur**


Voici les détails et les raisons de mon choix :

## 1. Retour client
Vous pourriez avoir la plus grande vélocité et produire une grande quantité de logiciels, vous ne seriez quand même pas heureux si vous ne pouvez pas les vendre. Pour les vendre, vous avez besoin de clients qui veulent acheter votre logiciel. Ils voudront acheter votre logiciel, si vous leur offrez ce dont ils ont besoin. Alors ils seront satisfaits et vous féliciteront pour cela, directement (enquêtes, commentaires, etc.) ou indirectement (achat, nombre de clics, etc.). Et par conséquent **vous pourrez enregistrer des retours client**.

Les retours clients dépendent du type de produit que vous élaborez. Quelques exemples :

* métriques de conversion (comme par exemple [les métriques AARR du mouvement Lean Startup](http://500hats.typepad.com/500blogs/2007/09/startup-metrics.html)) (NdT : voir [Exemple d'indicateurs de conversion](http://ayeba.wikispaces.com/Exemple%20d%27indicateurs%20de%20conversion))
* nombre de clients qui achètent le produit
* nombre de clients qui recommandent le produit
* nombre d'anomalies
* niveau de satisfaction client (par exemple à travers une enquête après chaque revue de sprint).

## 2. Burnup de livraison (Release Burnup)

Avant d'utiliser un burnup, **regardons d'abord un burndown**. Le burndown de livraison vous permet de rendre visible la quantité de travail non fait. Cette ligne de burndown est tracée sur un diagramme avec le nombre de points de story ou d'épics sur l'axe des y et le numéro du sprint sur l'axe des x. Lorsque la ligne atteindra l'axe des x, cela correspondra au sprint pour lequel vous aurez épuisé les stories. Si vous souhaitez que la ligne croise l'axe des x à une certaine date, assurez-vous de modifier le contenu de votre product backlog en conséquence. Cela signifie, que vous devrez vous débarrasser des stories superflues ou des stories de faible valeur. Vous pourriez vouloir scinder les stories pour le faire (en ne gardant que la partie la plus valorisante d'une grosse story – NdT).

**Se débarrasser du travail (superflu) mène à la simplicité :**

> Simplicité – l'art de maximiser la quantité de travail non fait – est essentielle. — [principe du manifeste agile](http://agilemanifesto.org/iso/fr/principles.html).

![Burnup]({{ site.url }}assets/misc/burnup.png)
Exemple de burnup de livraison


Un product owner doit travailler dur pour rendre son produit simple. Cela mérite d'être rapporté auprès de la direction. Par conséquent, **une meilleure alternative au burndown de livraison pourrait être un burnup de livraison**.

Un burnup de livraison montre deux lignes sur les mêmes axes comme le diagramme de burndown. Une ligne trace la somme totale en story point du product backlog, l'autre ligne montre la somme de travail accompli en points de story (alias la vélocité). **Le point de rencontre de ces deux lignes sera le moment où vous n'aurez plus de travail à réaliser**. Si cette date ne vous convient pas, vous pouvez accroître la vélocité (qui augmentera la pente de la courbe du travail fait), ou vous pouvez élaguer votre product backlog (qui diminuera la pente de la courbe du product backlog).

## 3. Indice de bonheur

**Rendez visible l'humeur de l'équipe en traçant un indice de bonheur**. Pour cela, encouragez votre équipe à noter leur humeur sur un [calendrier niko-niko](http://agiletrail.com/2011/09/12/how-to-track-the-teams-mood-with-a-niko-niko-calendar). Puis pour chaque semaine, calculez la moyenne de l'humeur de l'équipe. Ensuite tracez cette moyenne sur un diagramme, l'axe des y sera l'échelle de l'indice de bonheur et l'axe des x, le temps en semaine. Avec le temps, vous aurez un historique plutôt fiable de l'humeur de l'équipe.

![Niko-niko]({{ site.url }}assets/misc/indice de bonheur.png)
Exemple d'indice de satisfaction

Une solution similaire peut s'appliquer quelque soit l'échelle : vous pouvez enregistrer l'humeur des services si vous calculez la moyenne des humeurs des équipes. De la même manière, **vous pouvez enregistrer la moyenne de l'humeur de toute une entreprise** si vous calculez la moyenne des humeurs des services. C'est l'indice de bonheur de l'entreprise, comprenez-vous ?

**Vous pouvez interpréter la courbe de l'indice de bonheur comme l'indice du cours de bourse**, où les cours seront ceux de votre travail en tant que coach agile ou manager. Si le cours monte, cela signifie que votre travail en tant que coach ou manager est bon et que vos derniers changements ont amélioré l'environnement de travail pour vos équipes. Si le cours baisse, votre travail en tant que coach ou manager devra s'améliorer et vos derniers changements n'ont pas eu l'effet escompté aux yeux de vos équipes.

## Pourquoi ces 3 métriques ?

Chacun de **ces métriques met l'accent sur un aspect bien particulier** lorsque vous commencez un projet pilote agile.

  | VUE DE L'INTÉRIEUR  | VUE DE L'EXTÉRIEUR
--|---|--
 ÉCONOMIQUE | 2. BURNUP DE LIVRAISON | 1. RETOUR CLIENT
 ÉMOTIONNEL | 3. INDICE DE BONHEUR | 1. RETOUR CLIENT

Modèle de métriques pour rapport à la direction d'un projet pilote agile.

* Le **retour client** reflète l'aspect économique et émotionnel vu de l'extérieur du produit que votre projet pilote agile réalise.
* Le **burnup de livraison** reflète l'aspect économique vu de l'intérieur du produit que votre projet pilote réalise.
* L'**indice de bonheur** reflète l'aspect émotionnel vu de l'intérieur de l'équipe qui travaille sur votre projet pilote agile.


Avec ces trois métriques, vous couvrez **les aspects les plus importants d'un projet pilote agile** du point de vue d'un responsable. Encore mieux, ces métriques s'expliquent plutôt rapidement, ce qui signifie qu'ils sont compatibles avec des cadres dirigeants.


---
Auteur : Bernd Schiffer  
Source : [3 Metrics for Reporting an Agile Pilot to Top Management](http://agiletrail.com/2011/09/19/3-metrics-for-reporting-an-agile-pilot-to-top-management/)  
Date de parution originale : 19 Septembre 2011  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 15/10/2013  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

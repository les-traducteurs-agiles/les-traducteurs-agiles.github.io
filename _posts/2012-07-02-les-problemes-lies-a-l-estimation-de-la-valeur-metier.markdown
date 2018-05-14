---
layout: post
title:  "Les problèmes liés à l'estimation de la valeur métier"
date:   2012-07-02 00:01
published: true
tags: 
- estimation
- product owner
---

De temps en temps, je vois des équipes qui souhaitent définir une "valeur métier" sur chacune des user stories. Ils le font pour une, voire deux raisons :

1. être capable de mesurer la quantité de "valeur métier" livrée à l'organisation, en le visualisant sur un graphe sprint après sprint
2. être capable de prioriser les user stories en comparant la valeur métier de chacune des stories par rapport à son coût.


Malheureusement, il y a quelques problèmes avec ce type de pratiques.

Premièrement, la valeur de petits bouts de fonctionnalités s'entremêle. Lorsque nous avons des fonctionnalités qui sont trop petites (comme doivent l'être des user stories), il est très difficile de définir une valeur précise sur chacune. Les économistes appellent cela le prix hédonique. L'exemple classique est de définir des valeurs sur les composants individuels d'une maison : taille, lieu, vue, ... Comment allez-vous valoriser chacune de ces caractéristiques de la maison ? Vous pouvez en savoir plus sur le prix hédonique sur [Investopedia](http://www.investopedia.com/terms/h/hedonicpricing.asp#axzz1zUnPt2fL) et cet exemple de [prix des séchoirs à vêtements](http://www.bls.gov/cpi/cpidryer.htm) montre combien le concept de prix hédonique peut être complexe.

Deuxièmement, la valeur d'un petit bout de fonctionnalité peut souvent représenter la valeur totale du produit. Par exemple, quelle est la valeur de la roue avant-gauche d'une voiture ? Bien, étant donné que je ne souhaite pas avoir de voiture sans cette roue, la valeur de cette roue représente la valeur totale de la voiture.

Maintenant que nous avons identifié deux problèmes avec l'estimation de la "valeur métier" d'une user story, parlons du problème à déterminer le coût d'une story.

## Le problème du coût réparti

Finalement, lorsque nous essayons de définir une valeur métier en points sur de petites fonctionnalités (comme les user stories), il y a le problème supplémentaire de déterminer le coût de la fonctionnalité. Il y a souvent le désir de calculer une sorte de retour sur investissement (ROI) des fonctionnalités, en comparant la valeur métier en points au coût de la story en points. Pourtant, avec de petites fonctionnalités, il apparaît souvent que le coût réel de l'implémentation d'une fonctionnalité est égal à la somme des coûts liés à l'implémentation de plusieurs petites parties du système, certaines d'entre elles (par exemple des travaux d'architecture) ne peuvent être estimées séparément.

Par exemple, le coût lié au remboursement d'un achat par carte de crédit devrait inclure certains travaux d'infrastructure d'abord liés à l'acceptation de la carte de crédit. Cependant, ce coût a probablement été estimé comme une partie de la story "acheter les articles qui composent mon panier". Le fait de ne pas réussir à répartir le coût de cette infrastructure de traitement de la carte de crédit entre les stories d'achat et de remboursement, peut mener à des décisions incorrectes en termes de ROI.

Comme pour le prix hédonique, cela fait des années que les économistes se battent avec ce sujet. Un exemple simple est l'élevage d'une vache et la vente de la viande bovine et du cuir. Comment devrait-on répartir le coût pour élever la vache entre les user stories "viande bovine" et "cuir" ? Nous pourrions dire que le coût concerne exclusivement la viande bovine et que le cuir est gratuit, mais ce serait incorrect, le contraire aussi d'ailleurs. Les bénéfices (viande bovine et cuir) doivent être considérés ensemble en les comparant au coût pour élever la vache.

## Que doit-on faire alors ?

Cela veut-il dire que nous ne pouvons jamais affecter une valeur métier aux fonctionnalités et que nous devons renoncer à l'analyse du ROI des user stories ? Pas nécessairement. Mais ce type d'analyse s'applique beaucoup mieux au niveau des epics (grosses user stories) et des thèmes (groupe de stories), car la valeur et le coût peuvent être correctement envisagés à ces niveaux.


---
Auteur : [Mike Cohn](https://www.mountaingoatsoftware.com/company/about-mike-cohn)  
Source : [The Problems with Estimating Business Value](http://www.mountaingoatsoftware.com/blog/the-problems-with-estimating-business-value)  
Date de parution originale : 19 Septembre 2010  

---
Traducteur : [Fabrice Aimetti](http://www.fabrice-aimetti.fr/)  
Date de traduction : 02/07/2012  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



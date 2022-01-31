---
layout: post
title:  "LeSS - Schéma d'adoption des équipes feature"
date:   2017-01-25 00:01
published: true
tags:
- less
- adoption
- conduite du changement
---

[<< Portail LeSS < Portail Adoption](http://www.les-traducteurs-agiles.org/2016/12/26/less-portail-adoption.html)

Un schéma d’adoption de l’équipe feature se révèlera être un outil utile lors de votre adoption du modèle des équipes features

## Schéma de périmètre et de spécialisation

Qu’est-ce qu’un composant ? Qu’est-ce qu’une feature ? Qu’est-ce qu’une spécialisation fonctionnelle ? Nous les avons considérés jusqu’à présent sous l’angle dichotomique mais la réponse à ces questions se vérifie dans un certain continuum. Un groupe a la responsabilité d’une classe alors qu’un autre groupe a la responsabilité de l’ensemble d’un sous-système. Chacune de ces équipes sont des équipes composant. Une échelle tout aussi similaire existe dans le domaine de la spécialisation fonctionnelle, certains des groupes gèrent jusqu’a cinq niveaux de tests, ce qui donne “l’intégration des tests dans l’équipe” une appellation quelque peu ambigüe ! Dessiner ces différents niveaux sur un schéma nous donne quelques indices quant à l’adoption de l’équipe feature et du type de changement organisationnel auquel vous pouvez vous attendre.

![Schéma d’adoption de l’équipe feature]({{ site.url }}assets/less/feature-team-adoption-map-fr.png)  
Schéma d’adoption de l’équipe feature


Le schéma présente quatre zones :

* Équipes composant - Toute équipe qui (1) se concentre sur des parties du produit plutôt que sur des features centrées sur le client, ou (2) qui se concentre sur la réalisation d’une tâche plutôt que sur la livraison d’un incrément produit est une équipe composant. Note ! … Plus l’appropriation du périmètre est réduite, plus stricte est la spécialisation et plus les problèmes de l’équipe composant sont importants.


* Équipe feature - Toute équipe qui se concentre sur la globalité du produit et qui est impliquée de la clarification des features centrées sur le client jusqu’aux tests est une équipe feature. Les équipes features existent à différentes échelles. Leur rôle peut se limiter à la seule implémentation de features prédéterminées ou elles peuvent être impliquées dans l’identification et la résolution des vrais problèmes des clients.


* Équipe fonctionnelle sur-spécialisée - Toute équipe qui s’occupe d’une tâche sur un large périmètre est probablement fonctionnellement sur-spécialisée. Cela conduit à de nombreux gaspillages à cause des multiples passages de relais. À éviter.


* Équipes composant étendu - Toute équipe qui a une responsabilité limitée sur un composant et qui est toutefois responsable de la vérification du bon fonctionnement de son travail sur l’ensemble du produit est une équipe composant étendu. Ayant la charge d’un “périmètre composant” et la charge d’un “périmètre sur l’ensemble du produit”, l’équipe est déchirée par un conflit interne. Ce conflit conduit soit (1) à la duplication de travail car plusieurs équipes créent les mêmes tests, ou (2) à un effort supplémentaire de coordination car les équipes doivent coordonner les tests “orientés produit”. Ce même conflit de périmètre s’applique également pour la clarification des besoins. Ces équipes représentent peut-être une amélioration par rapport aux équipes composant basiques, mais elles n’offrent pas tout le potentiel que peuvent offrir les équipes features.


## Schéma d’adoption de l’équipe feature

Une “équipe feature parfaite” est une équipe qui travaille sur l’ensemble du système et qui co-crée le produit avec de vrais utilisateurs. Cet objectif de perfection est très difficile à atteindre.

Avec cet objectif de perfection, nous pouvons utiliser le schéma précédent comme un schéma d’adoption d’équipe feature. Voici un exemple :
![Schéma d’adoption de l’équipe feature]({{ site.url }}assets/less/feature-team-adoption-map-telecom-fr.png)  
Schéma d’adoption d’équipe feature - Exemple dans les télécoms

Ce schéma d’adoption des équipes feature est tiré d’un cas d'adoption de LeSS Huge pour un produit. Au début de l’adoption, seules existaient les équipes composant traditionnelles. La stratégie d’adoption choisie a été d’étendre le périmètre fonctionnel des équipes et de créer des équipes composant étendu. L’objectif à court terme pour les années à venir est d’aller vers des équipes feature intervenant sur l’ensemble du produit. Toutefois, certains composants partagés ont été créés par un groupe produit de référence qui rend ces composants difficiles à intégrer car cela exigerait des changements organisationnels plus importants. Ils sont donc exclus pour le moment de l’objectif en cours.


---
Auteur : The LeSS Company B.V.  
Source : [Feature Team Adoption Map - Large Scale Scrum (LeSS)](http://less.works/less/adoption/feature-team-adoption_map.html)  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 25/01/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

---
layout: post
title:  "Un nouveau cadre de travail de développement logiciel : quelques idées"
date:   2017-07-26 00:00:01
published: true
tags: 
- agile
- nouveau cadre de travail de développement logiciel
---

Voici quelques notes portant sur un nouveau cadre de travail que j’aimerais approfondir. Je les mettrai à jour de temps à autre et je modifierai peut-être la date de cet article à ce moment-là. Nous verrons.

## Principes et valeurs du manifeste

C’est là où tout à commencé, et pour moi, c’est là où est la quintessence de toutes choses. Nous essaierons de nous référer au manifeste lorsque cela s’avèrera approprié, et j’écrirai peut être quelques articles en partant de là.

## Pratiques (tirées de XP)

![Pratiques XP]({{ site.url }}assets/ron_jeffries/circles-fr.jpg)  

### Équipe en entier

L’idée principale, c’est commencer par avoir au moins toutes les compétences de développeurs et de testeurs nécessaires dans l’équipe. Cela comprend également les concepts de Product Owner / Client présents dans Scrum et XP. L’idéal, toutefois, est d’avoir une _équipe_ pluri-disciplinaire, auto-organisée ayant une responsabilité et une autorité complète sur la réalisation du produit souhaité. Prenez par exemple une équipe dans un garage ou une organisation fonctionnant en mode lean startup.

### Le jeu du planning

Il y a deux aspects à considérer à minima : la planification du sprint ou de l’itération, et la planification de la livraison. Cette dernière est-elle nécessaire ? Si oui, comment devrait-elle être se dérouler ? Quelle responsabilité une équipe auto-organisée peut-elle avoir pour réfléchir à long terme, pour dire ce qu’elle pense, pour s’engager sur le calendrier ?

### Petites livraisons

C’est fondamental ! Mettez cela tout en haut de la pile avec le concept d’_incrément_ et faites-en un élément central. Notez-bien que le manifeste indique la mention “logiciel opérationnel” au moins 300 fois.

### Tests clients

Bonne idée, mais trop spécifique ? [^1]. Ceci dit,  c’est une bonne manière de s’assurer que nous avons bien compris et que nous sommes d’accord sur la prochaine story. C’est une bonne manière de communiquer lorsque le client est (d’une manière ou d’une autre) séparé de l’équipe de developpement. C’est une bonne manière d’être sûr, à chaque itération, que le produit fonctionne toujours. C’est toutefois insuffisant en tant que tel, ou avec les tests faits par le développeur, mais c’est souvent mieux que ce que la plupart des équipes ont aujourd’hui.

### Propriété collective

Voir _l’équipe en entier_. Cela inclut le concept-clé de profil de personne “en forme de T” ou [“en forme de coulure de peinture”](https://www.facebook.com/notes/kent-beck/paint-drip-people/1226700000696195/), des personnes ayant ce type de profil ont plus de valeur que des spécialistes isolés.

N’importe quel “pair” peut améliorer le code, à n’importe quel moment. Voir _Programmation en binôme_.

### Norme de codage

Ce point est trop spécifique, mais il s’agit un point clé : nous essayons tous de coder de la même manière afin que nous puissions tous comprendre tout ce que nous avons fait.

### Rythme soutenable

Est-ce qu’il y a beaucoup d’idées qui se cachent par là ? La pression du [Dark Scrum](http://www.les-traducteurs-agiles.org/scrum/2016/11/20/dark-scrum.html), la théorie du “deux fois plus de travail”, des inquiétudes sur l’engagement, les prévisions, les estimations.

L’idée fondamentale ici est de travailler à un rythme tel que l’avancement réel est constant, homogène et prévisible, et que les personnes ne craquent pas. Considérer les valeurs humaines comme … avoir une vie.

### Métaphore

Cela va avec l’idée d’une compréhension commune au sein de l’_équipe en entier_ sur la manière dont fonctionne le produit. Pas seulement le style du code, ou l’architecture, mais également l’ensemble de la cohérence conceptuelle qu’il peut y avoir au niveau de l’idée et de la conception du produit.

### Intégration continue

C’est trop spécifique. L’intégration continue fait partie de l’_incrément_. C’est avec l’intégration continue que vous obtenez la capacité à construire un incrément à chaque itération : si vous n’intégrez pas tous les jours, vous foncez tête baissée vers un vendredi atroce et un long week-end de travail.

### Développement piloté par les tests

C’est trop spécifique, mais c’est là encore une compétence clé à avoir. Cela fonctionne bien, lorsque vous êtes suffisamment bon, mieux que tout le reste, tout spécialement en équipe. L’ancien nom _tests développeur_ était probablement plus approprié. L’idée fondamentale est sans doute ici la _confiance_, une certitude grandissante que le produit fonctionne réellement, qu’il fait ce que vous voulez, qu’il ne régresse pas, et qu’il va là où vous pensez que vous voudriez qu’il aille.

Notez bien que la _confiance_ est un bon endroit pour mettre le test “intelligent”, le test utilisateur, le test client, et ainsi que d’autres tests du même genre (pour lesquels je n’y connais presque rien).

### Refactoring

Là aussi, c’est trop spécifique, mais c’est absolument critique. Voir _nature_, le besoin pour une conception incrémentale implique du refactoring qui implique des tests automatisés.

### Conception simple

S’agira t’il plus probablement _une conception simple partagée_ ? L’un des points essentiels ici c’est que nous devons nécessairement faire évoluer la conception et que nous devrions ainsi commencer avec une conception la plus simple possible sur laquelle nous puissions travailler, et nous devrons faire preuve d’un très grand savoir-faire dans l’évolution de cette conception, en faisant usage du _refactoring_, des _tests développeur_ et des _tests clients_ pour être en _confiance_ que tout continue à bien fonctionner.

### Développement en binôme

C’est une pratique qui est vraiment formidable et difficile. En comparaison avec le développement en groupe, qui est peut être moins difficile et qui est dans le même ordre d’idée que le développement en binôme. Cela a pour effet de renforcer _l’équipe en entier_, _l’appropriation collective_, la résilience de l’équipe par rapport au changement et la flexibilité lorsque les priorités bougent.  

## Scrum

Sans aucun doute, nous parlerons de Scrum, et il se peut ou pas que certains de mes prochains articles prendront comme base de départ Scrum.

## Mise à l’échelle

Oui, eh bien, je suis contre. Nous aborderons plus en détails ce que je veux dire par là.

## Modèle agile courant[^2]

C’est un modèle intéressant auquel je pourrais peut être faire référence.

## Variantes

D’autres formes “connues” existent. SAFe, qui est politiquement 
correct pour le moins. Modern Agile, FASTagile, DaD, LeSS, etc etc. Nous pourrions trouver cela intéressant de nous comparer à eux mais nous allons essayer d’éviter de tomber dans le piège de l’homme de paille [^3].

## Etc

Il y aura, sans aucun doute, d’autres aspects qui verront le jour avec le temps. Nous verrons.

[^1]:Je parie que c’est quelque chose que je vais dire souvent. Je veux simplement dire que c’est une bonne idée mais qu’elle se révèle être trop détaillée pour une pratique de haut niveau. Nous voudrons trouver un sujet plus général ou un autre endroit plus adapté pour qu’une idée “trop spécifique” puisse s’épanouir.

[^2]:NdT : Traduction temporaire à défaut de mieux pour l’instant de l’expression Agile Fluency Model.

[^3]:”une idée peut sembler être bonne si on la compare à un homme de paille”  
![Homme de paille]({{ site.url }}assets/ron_jeffries/strawman.jpg)  

---
Auteur : [Ron Jeffries](http://ronjeffries.com/about.html)  
Source : [A New Software Development Framework: Ideas](http://ronjeffries.com/articles/017-02ff/new-framework-0/)  
Date de parution originale : 25 Juin 2017  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 26/07/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



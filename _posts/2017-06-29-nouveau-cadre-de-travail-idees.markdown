---
layout: post
title:  "Un nouveau cadre de travail de développement logiciel : quelques idées"
date:   2017-06-28 00:00:01
published: true
tags: 
- agile
- nouveau cadre de travail de développement logiciel
---

Here are some notes about where I might like to go in considering the [New Framework](http://ronjeffries.com/categories/new-framework) idea. I’ll update this from time to time and maybe bump its date when I do. We’ll see.

Voici quelques notes portant sur un nouveau cadre de travail que j’aimerais approfondir. Je les mettrai à jour de temps à autre et je modifierai peut-être la date de cet article à ce moment-là. Nous verrons.

## Manifesto Principles and Values

## Principes et valeurs du manifeste

This is where it all began, and for me, it all comes back to this. We’ll try to refer to the Manifesto where it’s appropriate, and may write some articles starting from it.

C’est là où tout à commencé, et pour moi, c’est là où est la quintessence de tout choses. Nous essaierons de nous référer au manifeste lorsque ce sera approprié, et j’écrirai peut être quelques articles en partant de là.

## Practices (from XP)

## Pratiques (tiré de XP)

![Pratiques XP]({{ site.url }}assets/ron_jeffries/circles-fr.jpg))

### Whole Team

### Équipe entière

A central idea, beginning with having at least all the developer and testing skills you need inside the team. Includes the Product Owner / Customer notions from Scrum and XP. The ideal, however, is surely a cross-functional, self-organizing _Team_ with full responsibility and authority for building the desired product. Consider a team in a garage, or a Lean Startup.

Une idée centrale, commencer par avoir au moins toutes les compétences de développeurs et de testeurs nécessaires dans l’équipe. Cela comprend également les concepts de Product Owner / Client présents dans Scrum et XP. L’idéal, toutefois, est d’avoir une _équipe_ pluri-disciplinaire, auto-organisée ayant une responsabilité et une autorité complète sur la réalisation du produit souhaité. Prenez par exemple une équipe dans un garage ou une organisation fonctionnant en mode lean startup

### Planning Game

### Le jeu du planning

Two key aspects at least: iteration or Sprint planning, and “release planning”. Is the latter necessary? If so, how should it be done? What responsibility does a self-organizing team have to think long-term, reveal its thoughts, commit to schedule?

Il y a deux aspects à considérer à minima : la planification du sprint ou de l’itération, et la planification de la version. Cette dernière est-elle nécessaire ? Si oui, comment devrait-elle être se dérouler ? Quelle responsabilité une équipe auto-organisée peut-elle avoir pour réfléchir à long terme, pour dire ce qu’elle pense, pour s’engager sur le calendrier ?

### Small Releases

### Petites livraisons

This is fundamental! Bring this up to the top in the notion of _Increment_ and make it central. Note that the Manifesto refers to “working software” about 300 times.

C’est fondamental ! Mettez cela tout en haut de la pile avec le concept d’_incrément_ et faites-en un élément central. Notez-bien que le manifeste indique la mention “logiciel opérationnel” au moins 300 fois.

### Customer Tests

### Tests clients

Good idea, too specific?[^1] Good way to ensure we understand and agree on the meaning of the next story slice. Good way to communicate when Customer is (somewhat) separate from development team. Good way to be sure, every iteration, that the product still works. Not sufficient on its own, or with Programmer Testing, yet often better than many teams have today.

Bonne idée, mais trop spécifique ? [^1]. Ceci dit,  c’est une bonne manière de s’assurer que nous avons bien compris et que nous sommes d’accord sur la prochaine story. C’est une bonne manière de communiquer lorsque le client est (d’une manière ou d’une autre) séparé de l’équipe de developpement. C’est une bonne manière d’être sûr, à chaque itération, que le produit fonctionne toujours. C’est toutefois insuffisant en tant que tel, ou avec les tests faits par le développeur, mais c’est souvent mieux que ce que la plupart des équipes ont aujourd’hui.

### Collective Ownership

### Propriété collective

See _Whole Team_. Includes the key notion that “T-Shaped” or [“Paint-drip Shaped”](https://www.facebook.com/notes/kent-beck/paint-drip-people/1226700000696195/) people are more valuable than isolated specialists.

Voir _l’équipe en entier_. Cela comprend le concept-clé de profil de personne “en forme de T” ou “en forme de coulure de peinture”, des personnes ayant ce type de profil ont plus de valeur que des spécialistes isolés.

Any “pair” can improve any code, any time. See _Pair Programming_

N’importe quel “pair” peut améliorer le code, à n’importe quel moment. Voir _Programmation en _binôme_.

### Coding Standard

### Convention de codage

Too specific, but a key point: we all try to code alike so that we can all understand everything we have all done.

Ce point est trop spécifique, mais il s’agit un point clé : nous essayons tous de coder de la même manière afin que nous puissions tous comprendre tout ce que nous avons tous fait.

### Sustainable Pace

### Rythme soutenable

Many ideas hiding here? [Dark Scrum](http://ronjeffries.com/categories/dark-scrum) pressure, “twice the work” thinking, concerns about commitment, prediction, estimation.

Est-ce qu’il y a beaucoup d’idées qui se cachent par là ? La pression du [Dark Scrum](http://www.les-traducteurs-agiles.org/scrum/2016/11/20/dark-scrum.html), une pensée à la “deux fois plus de boulot”, des inquiétudes sur l’engagement, les prévisions, les estimations.

Fundamental idea is to work at a pace such that real progress is steady and consistent and predictable, and so that people don’t burn out. Consider human values like having a life.

L’idée fondamentale ici est de travailler à un rythme tel que l’avancement réel est constant, consistant et prévisible, et que les personnes ne craquent pas. Considérer les valeurs humaines comme … avoir une vie.

### Metaphor

### Métaphore

This goes to some idea of common understanding among the _Whole Team_ of how the product works. Not just the code style, or the architecture, but also the overall conceptual coherence of the product idea and design.

Cela va avec l’idée d’une compréhension commune au sein de l’_équipe en entier_ sur la manière dont fonctionne le produit. Pas seulement le style de codage, ou l’architecture, mais également l’ensemble de la cohérence conceptuelle qu’il peut y avoir au niveau de l’idée et de la conception du produit.

### Continuous Integration

### Intégration continue

Too specific. Part of _Increment_. This is how you get the ability to build an Increment every iteration: if you don’t integrate every day, you’re in for a hellacious Friday and a long weekend of work.

C’est trop spécifique. L’intégration continue fait partie de l’_incrément_. C’est avec l’intégration continue que vous obtenez la capacité à construire un incrément à chaque itération : si vous n’intégrez pas tous les jours, vous foncez tête baissée vers un vendredi atroce et un long week-end de travail.

### Test-Driven Development

### Développement piloté par les tests

Too specific, yet a key skill to have. Works, when you’re good enough at it, better than anything else, especially in a team situation. Former name _Programmer Testing_ was probably better. Perhaps the fundamental idea is _Confidence_, an increasing certainty that the product actually works, does what you intended, isn’t regressing, and is heading where you currently think you’d like to go.

C’est trop spécifique, mais c’est là encore une compétence clé à avoir. Cela fonctionne bien, lorsque vous êtes suffisamment bon, mieux que tout le reste, tout spécialement dans la situation d’une équipe. L’ancien nom _tests développeur_ était probablement plus approprié. L’idée fondamentale est sans doute ici la _confiance_, une certitude grandissante que le produit fonctionne réellement, qu’il fait ce que vous voulez, qu’il ne régresse pas, et qu’il ailler là où vous pensez que vous voudriez qu’il aille.

Note that _Confidence_ is a good place to put “sapient” testing, user testing, market testing, and the like. (About which I know almost nothing.)

Notez bien que la _confiance_ est un bon endroit pour mettre le test “intelligent”, le test utilisateur, le test de la concurrence du marché, et ainsi que d’autres tests du même genre (pour lesquels je n’y connais presque rien).

### Refactoring

### Refactoring

Again too specific, yet absolutely critical. See _Nature_, need for incremental design implies refactoring implies automated tests.

Là aussi, c’est trop spécifique, mais c’est absolument critique. Voir _nature_, le besoin pour une conception incrémentale implique du refactoring qui implique des tests automatisés.

### Simple Design

### Conception simple

Possibly _Shared Simple Design_? One aspect is that we must perforce evolve the design and should therefore start with the simplest design that can work, and must be very skilled at evolving that design, using _Refactoring_ and _Programmer Tests_, and _Customer Tests_ to have _Confidence_ that everything still works.

Plus probablement _une conception simple partagée_ ? L’un des aspect est que nous devons nécessairement faire évoluer la conception et que nous devrions ainsi commencer avec la conception la plus simple sur laquelle nous puissions travailler, et nous devons faire preuve d’un très grand savoir-faire dans l’évolution de cette conception, en faisant usage de _refactoring_, des _tests développeur_ et des _tests clients_ pour être en _confiance_ que tout continue à bien fonctionner.

### Pair Programming

### Développement en binôme

A marvelous and difficult practice. Compare with Mob Programming, which may be less difficult and is certainly in the same idea space as pairing. Helps with _Whole Team_ and _Collective Ownership_, helps to ensure team resilience under change, and flexibility as priorities shift.

C’est une pratique vraiment formidable et difficile. En comparaison avec le développement en groupe, qui est peut être moins difficile et qui est dans le même ordre d’idée que le développement en binôme. Cela renforce _l’équipe en entier_, _l’appropriation collective_, la résilience de l’équipe par rapport au changement et la flexibilité lorsque les priorités bougent.  

## Scrum

## Scrum

We’ll surely be talking about Scrum, and may or may not start articles from a look at Scrum

Sans aucun doute, nous parlerons de Scrum, et il se peut ou pas que certains de mes prochains articles prendront comme base de départ Scrum.

## Scaling

## Mise à l’échelle

Yes, well, I’m against it. We’ll talk about what I mean by that.

Oui, eh bien, je suis contre. Nous aborderons plus en détails ce que je veux dire par là.

## Agile Fluency Model

Modèle d’aisance agile 

An interesting model that may get referred to …

C’est un modèle intéressant auquel je pourrais peut être faire référence.

## Variants

## Variantes

Other “name brand” forms exist. SAFe, which is politically safe at least. Modern Agile, FASTagile, DaD, LeSS, etc etc. We might find it desirable to compare with these but we’re going to try to avoid the Strawman trope.[^2]

D’autres formes “connues” existent. SAFe, qui est politiquement 
correct pour le moins. Modern Agile, FASTagile, DaD, LeSS, etc etc. Nous pourrions cela intéressant de nous comparer à eux mais nous allons essayer d’éviter le trope de l’homme de paille [^2].

## Etc

## Etc

Doubtless there will be other angles showing up as time passes. We’ll see.

Il y aura, sans aucun doute, d’autres aspects qui verront le jour avec le temps. À voir.

[^1]:I’ll say this often, I bet. I just mean that this is a good idea but feels too detailed to be the top-level practice. We’ll want to find a suitable more general topic or place for a “too specific” idea to live.

[^1]:Je parie que c’est quelque chose que je vais dire souvent. Je veux simplement dire que c’est une bonne idée mais qu’elle se révèle être trop détaillée pour être une pratique de haut niveau. Nous voudrons trouver un sujet plus général ou un autre endroit ou une idée “trop spécifique” puisse s’épanouir.

[^2]:“Idea looking relatively good next to a straw man.” ![Strawman image](http://ronjeffries.com/xprog/wp-content/uploads/strawman.jpg)

[^2]:”une idée peut sembler être bonne si on la compare à un homme de paille”  
![Homme de paille]({{ site.url }}assets/ron_jeffries/strawman.jpg)  

---
Auteur : [Ron Jeffries](http://ronjeffries.com/about.html)  
Source : [A New Software Development Framework: Ideas](http://ronjeffries.com/articles/017-02ff/new-framework-0/)  
Date de parution originale : 25 Juin 2017  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Relecteur : [Claude Aubry](http://www.aubryconseil.com/pages/Auteur)  
Date de traduction : --/--/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



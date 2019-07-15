---
layout: post
title:  "Questions/Réponses à propos de la vélocité 5ème partie"
date:   2019-07-15 00:00
published: true
tags:
- vélocité
---

Au cours de la [4ème partie](http://www.les-traducteurs-agiles.org/2019/05/26/questions-reponses-a-propos-de-la-velocite-4eme-partie.html), nous avons abordé les confrontations plutôt épineuses qu'il peut y avoir entre la réalité des promesses, et la réalité du développement. Cet épisode revient sur certaines vérités au sujet de travailler plus dur et d'aller plus vite.

> A: Attendez une seconde ... Vous n'avez jamais parlé en fait que nous ne pouvons pas aller plus vite. Vous avez seulement dit qu'essayer plus dur ou d'ajouter davantage de personnes n'était pas la voie à suivre.  
>
> B: C'est vrai.  
>
> A: Donc nous _pourrions_ aller plus vite, c'est possible ?  
>
> B: Tout à fait.  

Pour parler franchement, nous n'avons aucune idée de la vitesse à laquelle des développeurs pourraient travailler. Un ami m'a appelé et m'a raconté avoir pris en charge un travail qui avait été estimé et de l'avoir réalisé en une matinée car le code était bien structuré, lisible et bien testé. Mon ami m'a dit "toutes les fonctions dont j'avais besoin avaient déjà été écrites et faciles à trouver"

Robert Martin dit toujours que la vitesse des travaux de développement de nos jours dépend principalement de la qualité du code sur lequel vous allez travailler. Du code de mauvaise qualité ? Vitesse réduite. Du code de très bonne qualité. Grande vitesse.

En plus, nous avons fouiné un peu partout et avons constaté que les développeurs passent environ 25% de leur temps en réunion (les plus séniors passant plus de temps). C'est 25% dès le départ.

La plupart des développeurs passent en partie le reste de leurs temps, environ 60 à 80% à corriger des anomalies. C'est un sacré bout de temps. S'ils pouvaient aller deux fois moins vite, mais en ne produisant aucune anomalie, ils iraient au moins 10% plus vite.

Par rapport au temps qu'il reste, le travail en silos, les mécanismes d'approbation dans le processus de travail et autres interruptions obligent les développeurs à passer une partie de leurs temps à attendre d'autres personnes. Le travail fait la queue dans une file d'attente.

Et bien sur, lorsque le travail d'un développeur attend dans une file d'attente, le programmeur consciencieux reste occupé en prenant du boulot supplémentaire supplémentaire dans sa propre liste de choses à faire, sa propre file d'attente.

Toutefois lorsque les travaux reviennent des tests, ou de la validation, ou d'une autre forme de revue, ces travaux doivent rejoindre une file d'attente attendre que le développeur soit à nouveau disponible pour les prendre en charge. Le développeur moyen type en entreprise que nous avons pu interroger a environ 5 tâches concurrentes (ou branches) ouvertes. Cela peut monter jusqu'à 15.

Vous pouvez voir le temps se réduire à peau de chagrin. Cela n'est en aucun cas surprenant qu'un petit bout de travail puisse prend un temps infini à être développé, même si le développeur est occupé et a beaucoup de tâches en cours à n'importe quel moment.

Les développeurs disent "Je ne suis pas bloqué, j'ai plein d'autres choses sur lesquelles travailler" et c'est vrai. Mais _**le travail lui en tant que tel**_ est bien bloqué. Le travail ne va pas aller suffisamment tôt en production _parce que_ les développeurs sont occupés à faire quelque chose d'autre. C'est pourquoi les pratiquants Lean disent "regardez le bâton, pas le coureur." L'efficacité du flux est lié au débit d'un système, non à la charge des employés.

C'est un système bordélique, rendu encore plus bordélique par des processus incluant de nombreux silos, d'efforts individuels, du travail bâclé, cycles d'approbations, de branches et je ne sais quoi encore.

**La plupart de nos systèmes semblent faire plus de la prévention   
logicielle plus que du développement logiciel**
{: style="text-align: center;"}

Mais toutefois, la qualité du code est le grand déterminant. Si le code est bien organisé, et qu'un bon outillage est utilisé, et que le développeur est familier avec le système, et que le changement n'introduit pas de réarrangements architecturaux majeurs; … eh bien, quelle vitesse surprenante pourrions-nous atteindre ?

Il serait facile d'aller plus file, mais arriver là peut s'avérer être un travail acharné du point de vue humain et pas uniquement pour les développeurs.

À ce sujet :

> A: Donc, comment pouvons-nous amener les développeurs à redoubler d'effort ?  
>
> B: Enlevez-leurs leur outils. Ajoutez plus de bureaucratie. Faites-leur utiliser des ordinateurs plus lents et d'anciens langages de programmation.  
>
> A: Et cela va ramener de la vélocité ?  
>
> B: Non. Vous avez demandé à comment les faire redoubler d'efforts.
 Ceci met en lumière un problème dans l'approche d'en faire plus. Dans la [deuxième partie](http://www.les-traducteurs-agiles.org/2019/01/29/questions-reponses-a-propos-de-la-velocite-2eme-partie.html), nous avons fait allusion à cela. Dans mon article de 2009 intitulé [Platitudes of Doom](http://agileotter.blogspot.com/2009/08/platitudes-of-doom.html)[^1], nous avons traité de cela en profondeur. Il y a ce postulat qui est que la raison pour laquelle le travail avance lentement c'est parce que les personnes ne travaillent pas avec assez d'acharnement.  

Être focalisé sur la charge et les efforts n'est d'aucune aide.

La conversation précédente est un peu ironique mais illustre le point que le problème n'est pas dans l'augmentation de la charge et dans des efforts accrus, mais dans les résultats obtenus. La plupart des programmeurs travaillent bien plus dur qu'ils ne le devraient et créent de cette manière bien moins de valeur.

Si nous insistons à mettre plus d'effort dans le travail, nous finissons par obtenir par quelque chose qui ressemble plus à de la force brute, et non avec de meilleurs résultats comme nous pouvons espérer. Cela sera abordé de manière plus approfondie lorsque je me mettrai à l'écriture de **The Journey**.

> A: Nous voulons qu'ils travaillent plus dur afin que nous puissions faire plus de choses.  
>
> B: Mais si vous voulez accomplir davantage, ne devriez-vous pas rendre le travail _moins dur_ ?  
>
> A: Nous voulons juste que le boulot soit fait.  
>
> B: Bien sûr, et eux aussi..  
Voici ce petit quelque chose de magique et d'intéressant. Si nous voulons que les gens puissent en faire plus, nous aurons probablement plus de chances de réussir en enlevant tout le superflu, l'incertitude, et le risque du processus, plutôt que d'y mettre de plus grand efforts et d'y mettre plus de pression.  

De nouveau, dans la [3ème partie](http://www.les-traducteurs-agiles.org/2019/04/08/questions-reponses-a-propos-de-la-velocite-3eme-partie.html), nous avons évoqué la formule de l'effort fourni pour faire une tâche par rapport à l'effort demandé. Allez jetez un coup d' œil juqu'au diagramme illustrant ce point et au texte associé puis revenez ici.

Cet extrait de la discussion a pour de but de simplement redire les points que vous avez déjà vu précédemment. Mais il y a une certaine probabilité que vous n'êtes pas un lecteur de longue date de ce modeste blog, perdu dans un coin sombres des vastes terres des bloggueurs, donc cela vous aidera peut être d'avoir davantage de choses à lire sur ce sujet.  
À savoir :

* La [3ème partie](http://www.les-traducteurs-agiles.org/2019/04/08/questions-reponses-a-propos-de-la-velocite-3eme-partie.html) aborde les sujets de l'incertitude, du risque et de l'effort. Cela peut s'avérer utile.

* Il peut être [dangereux d'accroître les efforts](https://agileotter.blogspot.com/2013/05/increasing-effort-is-unsafe-in-too-many.html)[^1].

* La présence d'[incertitude, de risque et d'efforts](https://agileotter.blogspot.com/2018/03/predictability-as-maturity-or-system.html)[^1] viennent contrecarrer la prévisibilité et doivent être pris en considération.

* Toutefois, ces éléments font partie de manière inextricable de la programmation, qui consiste [majoritairement à réfléchir](https://agileotter.blogspot.com/2014/09/programming-is-mostly-thinking.html)[^1].

* En tant que tel, nous ne savons pas si le boulot qu'on nous donne [est même possible](https://agileotter.blogspot.com/2014/10/preplanning-poker-is-this-story-even.html)[^1] certaines fois.

Peut être bien que la programmation n'est pas si lente que ça, si l'on considère l'état de la base du code et la présence du risque et de l'incertitude dans les exigences, la difficulté de prévoir l'effort intellectuel, etc.

**Peut-être que les estimations sont basses au lieu de dire que le travail est lent**

**Nous ne savons pas vraiment.**

Nous savons seulement qu'il existe une différence entre ce que nous nous attendons (et voulons) et ce que nous réalisons vraiment. Nous pouvons considérer cela comme d'une trahison, ou nous pouvons la considérer comme d'un [espace de curiosité](http://www.les-traducteurs-agiles.org/2016/10/16/espace-de-curiosite.html)[^2]

Je sais quels sont les choix qui mènent au blâme et à la frustration, et lesquels mène à l'alignement et à l'amélioration.

Mais je vais vous laisser méditer là-dessus jusqu'à la [6ème partie](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-vi.html)

[^1]: en vo
[^2]: en vf

---
Auteur : Tim Ottinger  
Source : [Q and A on Velocity, part V](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-v.html)  
Date de parution originale : 23 Octobre 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 15/07/2019  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

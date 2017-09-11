---
layout: post
title:  "Un nouveau cadre de travail : quelques termes"
date:   2017-09-11- 00:00:01
published: true
tags: 
- agile
- nouveau cadre de travail de développement logiciel
---

Une partie de cette idée du “nouveau cadre de travail” -- voire la totalité - c’est d’essayer de clarifier ma réflexion sur “Agile”, ce que cela signifie et comment l’exprimer. Cela m’amène à réfléchir sur certains termes abstraits que nous utilisons et à les décrire, des termes comme “Valeurs”, “Principes”, et “Pratiques”.

Mon principal intérêt réside dans “le développement agile de logiciels”, ce qui correspond à l’objectif premier du Manifeste. Mais nous devrons mettre cela dans le contexte, s’occuper des préoccupations managériales, des préoccupations liées au produit, des préoccupations administratives, et ainsi de suite. Pour l’instant, je ne suis pas certain à quel point j’irai dans chacune de ces directions, étant donné que je m’intéresse aux développeurs plus qu’à quiconque[^1].

## Pratiques

J’ai aimé le terme “Pratiques” pendant longtemps. Les pratiques sont les choses que nous faisons, et pour moi, rien n’arrive sans être le résultat de quelque chose que nous faisons. Et ce sont les choses que nous pratiquons, ce que je veux dire c’est que nous travaillons sur elles constamment, pour améliorer nos capacités à les appliquer. Mais ce mot pose quelques difficultés. 

Il est important de pratiquer et de travailler consciencieusement. Nous devons y prêter attention si nous voulons nous améliorer. Si le TDD[^2] est l’une de nos pratiques, nous devons prêter attention si nos tests sont trop gros, ou trop petits, ou trop faciles, ou trop difficiles. Nous devons apprendre de nos pratiques de TDD : comment mieux faire. Nous devons apprendre ce que le TDD nous dit de notre code, et comment notre style de codage affecte notre compétence à écrire des tests. Le TDD peut nous apprendre beaucoup, si nous prêtons attention.

Pour certaines personnes, les pratiques sont justes des choses que vous faites sans prêter attention. Par conséquent, ce terme pose peut être problème.

Pour certaines personnes, si quelque chose est une pratique, ils veulent que ce soit la meilleure pratique. Il ne fait pas de doute qu’il n’existe pas de “meilleures” pratiques, seulement des pratiques qui sont utiles quelque fois. Comment pouvons-nous savoir quand elles sont utiles ? Eh bien, mon avis c’est que nous devons les pratiquer suffisamment souvent, et suffisamment consciencieusement, pour être en capacité de décider.

Pour certaines personnes, si quelque chose est une pratique, cela signifie que vous devez le faire. Et je mets ici l’accent sur le mot _vous_ : elles sont enclines à _vous_ dire que _vous_ devez faire cette chose. Je me fiche de savoir si elles vous disent cela dans leur blog, ou si elles vous le disent de leur trône de responsables, ou de leur chaire de petit tyran de _ScrumMaster_. Pour moi, le boulot d’une équipe est de décider, en toute sagesse, quelles pratiques lui conviennet. Pour prendre ces décisions, ils doivent essayer beaucoup de choses, et de les essayer suffisamment minutieusement pour être en capacité de décider.

Donc, dans la mesure où le terme “pratiques” implique, à certaines personnes, une pratique aveugle, enfermer sur quelque chose au mieux, ou quelque chose qui est imposé, ce terme est un problème. De quoi pourrions-nous parler à la place ? Et si nous utilisions le terme de “compétences” ?

## Compétences

Une partie de la réflexion de ce nouveau cadre de travail semble aller dans la direction de grouper ou de généraliser certaines idées spécifiques. J’ai déjà écrit sur l’[équipe au complet](http://www.les-traducteurs-agiles.org/2017/08/27/nouveau-cadre-de-travail-equipe.html) y compris la notion d’équipe pluri-disciplinaire, ainsi que sur l’idée de _Client_ et de _Product Owner_. De manière similaire, je prévois de regrouper les _tests développeurs_ et les _tests clients_ dans un même groupe que je suis tenté d’appeler “Confiance”.

Peut être que le TDD est une _compétence_. Peut-être que les _tests développeurs_ sont une _compétence_ ou sans doute plus probablement, un vaste éventail de compétences.

Le terme _compétence_ semble convenir à merveille. Nous pouvons toujours améliorer une compétence : nous n’arriverons jamais à en atteindre le bout. Et nous pouvons toujours avoir de nouvelles compétences. 

La notion de _compétence_ pourrait nous amener à une appréciation d’un apprentissage tout au long de la vie, à une curiosité perpétuelle, ou à la fixation d’objectifs d’apprentissage puis à les atteindre.

J’apprécie le terme compétences, du moins pour l’instant

## Techniques[^1]

Mon ami et collègue [Joe Rainsberger](http://twitter.com/jbrains) a mentionné sur Twitter le terme “techniques”. Je pense qu’il s’agit d’un terme que nous pourrions ajouter et utiliser judicieusement.

Il existe une _compétence_, le _Refactoring_[^3], que tout à chacun doit apprendre afin de produire du logiciel de manière continue sans ralentir. Il existe des “modèles” de _refactoring_, tels que l’“Extraction de méthode”, la “Suppression d’Intermédiaire”, ou le “Remplacement du récepteur dynamique avec la définition automatique de méthode”[^4]. Quelque fois ces modèles se nomment simplement “_refactorings_”. Certaines personnes les appellent “_refactors_”. Je n’apprécie guère ce type d’individus.

Il serait peut être plus approprié que ces _refactorings_ soient décrits comme des techniques que tout à chacun devrait connaître comme faisant partie d’une compétence ayant un spectre plus large. Ceci dit, même si nous voyons apparaître une espèce de hiérarchie implicite ici, avec des compétences composées du moins en partie de techniques, la hiérarchie est assez profonde, et peut être ne s’agit-il pas de hiérarchie en tant que telle mais d’un réseau. Peut être ne devrions nous pas analyser ces termes trop précisément, mais il serait intéressant d’avoir une certaine manière d’exprimer que ceux-ci sont les composants de ceux-là. Mais …

* Livraison continue
  * Intégration continue 
    * Code propre
      * Refactoring
        * Extraction de méthode
          * Outils de refactoring de Visual Studio
            * Saisie au clavier
              * …

Cela peut continuer ainsi pendant longtemps. Je ne pense pas que cela nous apporterait grand chose de donner tous ces niveaux possibles. Toutefois, _technique_ et _compétence_ ont toutes les deux différentes connotations et leurs distinctions pourraient être utiles. Nous verrons.

## Valeurs

Je suis de plus en plus troublé par les méthodes ayant des “valeurs”. Il était correct pour le manifeste agile de mentionner des valeurs : il y avait quatre valeurs partagées par des hommes d’un certain âge dans ce moment particulier à cette époque. Nous n’avons pas dit que vous devriez avoir ces valeurs : nous avons dit que nous les avions.

Quand nous avons dit par exemple, que les valeurs d’XP sont la communication, la simplicité, le retour d’informations, le courage et le respect, que disons-nous ? Si nous voulons dire que l’inventeur d’XP avait ces valeurs en tête lorsqu’il a créé XP, alors c’est exact. Si nous voulons dire qu’XP a été conçu pour améliorer la communication, accroître la simplicité, donner de meilleurs retours d’informations, et permettre le courage, c’est exact. Si nous voulons ces choses, XP sera sans doute une des manière de les obtenir. Lorsque Kent Beck a ajouté “respect” à cette liste dans sa seconde édition, voulait-il dire que faire de l’XP permettrait d’accroître le respect des personnes les unes pour les autres ? Ou voulait-il dire que nous devions avoir du respect les uns pour les autres pour ne serait-ce qu’essayer XP ? Honnêtement, je ne sais pas.

Si toutefois, nous disons que pour appliquer les idées d’un cadre de travail donné, nous devons avoir ces valeurs, je pense que nous allons trop loin. Les gens ont les valeurs qu’ils ont, et ils ne peuvent pas changer pour ces nouvelles valeurs lorsqu’ils arrivent au bureau.

Je n’ai pas un meilleur terme pour _valeurs_ actuellement. Je pourrais continuer à l’utiliser, si j’en ai besoin, à moins que je ne trouve un meilleur terme, ou je pourrais couvrir les domaines que recouvre le terme d’autres manières. Pour l’instant, cela me pose un problème et pas de solution. Ça peut aller.

## Divers

J’ai vu et utilisé certains termes comme “Règles”, “Consignes”, “Standards, ainsi que d’autres du même genre. Et nous avons bien sûr des termes comme “Sprint”, “Itérations”, “Réunions” ou “Évènement”.

Je suis davantage préoccupé par les termes de “plus abstraits” mais les mots restent importants. Nous continuerons à creuser le sujet. 

## À suivre … 

Je suis certain que j’en aurai plus à dire à un moment ou à un autre. Mon plan actuel est de garder ces articles dans un certain ordre afin qu’ils soient lus comme dans un livre, j’y reviendrai donc certainement avec quelques mises à jours.


[^1]: Paragraphe ajouté le 05/07/2017 par l’auteur -- NdT additionnelle : même si vous n’êtes pas développeur, lisez quand même ça vaut le coup ;)

[^2]: NdT - TDD = Test Driven Development ou Développement piloté par les tests

[^3]: NdT - action de remanier un code existant, de l’améliorer, sans casser les services rendus par ce dernier. Le terme québécois “réusinage” ne s’est pas imposé en France.

[^4]: Je parie que vous n’avez jamais entendu parler du dernier. Moi non plus. Non je ne vous dirai pas. Cherchez un peu. :)

---
Auteur : [Ron Jeffries](http://ronjeffries.com/about.html)  
Source : [New Framework: Terms](http://ronjeffries.com/articles/017-02ff/new-framework-terms/)  
Date de parution originale : 25 Juin 2017  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 11/09/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}




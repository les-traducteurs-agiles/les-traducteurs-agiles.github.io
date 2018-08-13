---
layout: post
title:  "Est-ce que l'organisation compte ?"
date:   2015-05-05 22:01:53
tags:
- équipe
- développement
- refactoring 
---

> Je me demande s'il est même possible d'avoir les trois en même temps : la lisibilité, la facilité à être maintenu/modifié (ou bidouillabilité - NdT) et l'abstraction. -- Ben Kuhn, extrait de [Readability, hackability, and abstraction](http://www.benkuhn.net/rha)

Ben, la réponse courte est : Non. Ce n'est _pas_ possible. Mais à ce moment-là ... je ne réponds pas à la question que tu as _écrite_. Je réponds à la question que tu as _vraiment posée_. La question est :

> Je me demande s'il est même possible de faire un programme compliqué aussi lisible et modifiable qu'un programme simple.

Et bien sûr, la réponse est : _Non !_

Rentrons donc dans le vif du sujet sur pourquoi tu as posé la question ; et pourquoi tu l'as posée de cette façon.

Tu as noté que les programmes simples sont faciles à lire, et facile à modifier. C'est parfaitement exact. Ce programme est facile à lire et facile à modifier :

    void dial(modem, pno, quiet) {
      if (quiet) {
          modem.setVolume(0);
      } else {
          modem.setVolume(10);
      }
      modem.dial(pno);
    }

Ou pas ?

Bien que l'ensemble du programme tient en vingt lignes, tu peux voir toutes les interactions de toutes les variables alors, oui, il est facile à lire et facile à modifier.

Mais et si ce code faisait partie d'un programme de dix mille lignes ? Quelles sont les implications de cette boucle conditionnelle `if` ? Est-ce d'autres fonctions pourraient être embrouillées par le fait que la fonction `dial` modifie le `volume` du `modem`?

Au fur et à mesure que les programmes s’agrandissent, certaines parties commencent à dépendre d'autres parties. Les liaisons commencent à s'emmêler de plus en plus. Et le programme commence à se transformer en un _système_. Et un _système_ est toujours plus difficile à comprendre, plus difficile à lire, et plus difficile à modifier qu'un programme.

Mais en fait, tu posais une question très différente. Tu étais en train de demander si fractionner de grosses fonctions en petites fonctions, élimine la redondance, et si partitionner une application en objets polymorphiques rend les choses plus faciles à lire et à modifier. Tu étais en train de demander s'il serait mieux uniquement de tout laisser dupliquer, dans de grosses fonctions, sans aucun polymorphisme. Et la raison pour laquelle tu as demandé cela, c’est parce que tu as vu de petits programmes dans lesquels il y avait de la duplication, ainsi que quelques pseudo-grosses fonctions, dans lesquelles il n'y avait aucun polymorphisme et qui _restaient_ faciles à lire et à modifier.

La question que tu poses est une question essentielle. La question que tu poses est si l'organisation compte.

Pour répondre à cela, laisses-moi te montrer une photo de mon bureau :

![Bureau]({{ site.url }}assets/organisation_compte/UB_DESK.jpg)

Comme tu peux le voir, il n'est pas vraiment bien organisé. Oh, il y a une _espèce_ d'organisation. Mais il y a aussi beaucoup de chaos. Est-ce que cela signifie que l'organisation ne compte pas ?

En fait, le truc à propos de mon bureau est qu'il reste relativement simple. Il y a une pile sur ma droite. Et une autre pile sur ma gauche. La pile de droite contient les livres que je suis en train de lire ou auxquels je me réfère. La pile de gauche contient essentiellement un meli-melo de choses dont je ne veux pas m'occuper aujourd'hui mais que je devrai m'occuper certainement demain. Aucune des deux piles n'est particulièrement grande. Un rapide recherche linéaire dans l'une ou l'autre des piles me permet de retrouver ce dont j'ai besoin. Les dépendances sont limitées.

En d'autres termes, mon bureau est quelque peu désorganisé, mais il reste relativement simple. Et c'en est la clé. Les choses relativement simples peuvent tolérer un certain degré de désorganisation. Toutefois, au fur et à mesure que la complexité s'accroit, la désorganisation devient suicidaire. Essayez de trouver un livre ici :

![Bibliothèque mal rangée]({{ site.url }}assets/organisation_compte/badLibrary.jpg)

Ne penses-tu pas qu'il serait plus facile d'en trouver un là ?

![Bibliothèque bien rangée]({{ site.url }}assets/organisation_compte/goodLibrary.jpg)

_Beaucoup_ efforts ont été investis pour organiser cette deuxième bibliothèque. Et par conséquent, elle demande un certain effort pour apprendre son schéma d'organisation. Un nouveau venu ne peut pas juste se promener dans cette bibliothèque bien organisée et trouver tout de suite le livre qu'il souhaite. À la place, le nouveau venu doit d'abord apprendre quelques informations sur la [classification décimale de Dewey](http://fr.wikipedia.org/wiki/Classification_d%C3%A9cimale_de_Dewey), et sur la manière d'utiliser un catalogue de bibliothèque (sur fiches cartonnées - NdT), ou le catalogue informatisé. Cela demande au nouveau venu un peu de recherches et de réflexions avant qu’il puisse trouver le livre qu'il cherche.

Mais demandes à l'un des bibliothécaires de trouver un livre, et ils l'auront normalement entre les mains en quelques secondes.

Et nous arrivons là au coeur de la question que tu posais réellement. Tu étais en train de demander si le temps exigé pour apprendre le schéma de l'organisation du système en vaut la peine. Apprendre ce schéma d'organisation est _difficile_. Devenir compétent à lire et à modifier le code à l'intérieur de ce schéma demande du temps, des efforts et du travail. Et cela peut être ressenti comme du gaspillage lorsque tu le compares à comment la vie peut être simple lorsque tu as seulement 100 lignes de code.

Et voici que surgit alors un autre problème.

La structure d'organisation qui marche pour un programme de mille ligne, ne marche pas pour un programme de dix mille lignes de code. Et la structure d'organisation qui marche pour un programme de dix mille lignes ne fonctionne pas pour un programme de cent mille lignes.

Cela peut sembler presque intolérable. Parce que au fur et à mesure que le programme grossit, tu dois investir du temps, des efforts et en travail dans un schéma d'organisation voué à devenir obsolète.

Et donc la question que tu pose est si cela vaut le coup d'investir dans un quelconque schéma d'organisation  étant donné qu'il deviendra obsolète un jour.

La réponse à cette question devrait être évidente. Si tu décides qu'organiser ton système ne vaut pas les efforts investis, tu finiras par être
un [thésauriseur de code]({{ site.url }}equipe/developpement/refactoring/2015/05/05/les-thesauriseurs-de-code.html).

---
Auteur : [Uncle Bob](http://www.8thlight.com/team/uncle-bob)  
Source : [Does Organization Matter](http://blog.cleancoder.com/uncle-bob/2015/04/15/DoesOrganizationMatter.html)  
Date de parution originale : 15 Avril 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 05/05/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

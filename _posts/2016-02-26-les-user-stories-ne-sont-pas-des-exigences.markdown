---
layout: post
title:  "Les user stories ne sont pas des exigences"
date:   2016-02-27 11:15:55
published: true
categories: 
- user-stories
---

<div align="left" style="float:left; padding-right:30px" >
  <img title="Eléphants" src="{{ site.url }}assets/stories_sont_pas_exigences/elephants.jpg" />
</div>

_Les éléphants ne sont pas des girafes et les **user stories** ne sont pas des exigences. Elles partagent certaines caractéristiques et vous pouvez les trouver dans le même contexte, mais cela ne les rends pas semblables. En dépit de cela, beaucoup croient que les **user stories** sont les nouvelles exigences parce qu’il doit bien y avoir quelque part des exigences dans un projet, n’est-ce pas ? À cela, Je réponds deux fois non, elles ne sont pas des exigences et ce n’est pas quelque chose dont nous ayons vraiment besoin. Les **user stories** c’est être capable d’explorer les options et de saisir les opportunités. Les exigences c’est décider dès le début et s’y tenir._

Cet article est-il vraiment nécessaire ? Ne comprenons-nous pas déjà tout ce qui vient déjà d’être dit précédemment ? Non, je crois que des expressions comme “les exigences sont dans le backlog” est le reflet d’une ancienne manière de penser dans laquelle le document des exigences est désormais appelé backlog et les exigences appelées _user stories_. Et puis avec tout ça, vous pensez que vous êtes agile.

D’autres signes de cette idée fausse est de donner aux _user stories_ un identifiant unique et de les stocker dans une base de données. C’est peut être pratique mais c’est aussi un signe révélant un système de pensée orientée en terme d’exigences.

Mettre des _user stories_ dans un contrat c’est montrer sans ambiguïté cette manière de penser en tant d’exigences ; le plus dingue dans tout ça c’est qu’une _user stories_ n’est pas aussi précise qu’une exigence et qu’un tel contrat ne possède que peu de valeur. Et bien sûr les exigences restent sujet à interprétation malgré les techniques utilisées pour les écrire qui s’efforçent avec acharnement d’en lever toutes les ambiguïtés. Faisant donc partie intégrant des contrats pour les projets, les exigences sont aussi par nature résistantes à tout changement. Pour changer ou ajouter des exigences, vous devez les faire valider au CP, comité de pilotage. Pour en savoir plus sur cette partie contractuelle, reportez-vous à la section qui y est dédiée.

<div align="left" style="float:left; padding-right:30px" >
  <img title="Eléphants" src="{{ site.url }}assets/stories_sont_pas_exigences/girafes.jpg" />
</div>

Alors, que sont les _user stories_ ? Considérez-les comme des **instruments du planning**. L’agilité étant portée sur la livraison de la valeur, l’instrument du planning porte donc aussi sur la valeur. Nous priorisons par _user stories_, nous les estimons et nous décidons dans quel sprint nous les implémenterons. C’est tout ce qui a de plus naturel pour un instrument du planning, donc n’essayez pas de les transformer en quelque chose d’autre.

Le pouvoir de la _user story_ réside dans le dialogue qu’elle amorce. Au lieu d’avoir en main une spécification des exigences qui est interprétée par les développeurs et les testeurs, une communication à sens unique somme toute, dans la discussion que nous avons au sujet de chaque fonctionnalité que nous ajoutons, nous avons plusieurs compétences impliquées autour de la table.

Étant donné que les _stories_ ne convoient pas énormément de choses, une fois terminé nous pouvons après les jeter. Nous pouvons très bien garder quelques statistiques sur combien de points de story ont été réalisés mais c’est tout. 

Mais avons-nous besoin d’exigences ? Eh bien pas vraiment. Bien sûr, il y a des contraintes sur comment un système sera conçu et réalisé. Par exemple, les équipements médicaux doivent respecter les règlementations de la FDA[^1]. Mais appelons-les alors des contraintes.

Mais les exigences sont bien la description d’un système, et il y a sûrement quelque chose là-dedans, non ? Comment pouvez-vous dire que telle ou telle chose est une anomalie ou pas si vous n’avez pas des exigences d’une manière ou d’une autre ? Ici, je voudrais signaler la technique de la spécification par l’exemple. Une fois que vous avez décidé que telle fonctionnalité sera réalisée, vous écrivez les règles métiers sous la forme d’une série d’exemples dans un format qui soit lisible à la fois par un humain et par un programme. À À partir de ces spécifications, ce que fait le système devient clair et s’il venait à ne plus fonctionner correctement en raison d’un quelconque changement, les spécifications concernées apparaîtraient en rouge montrant ainsi exactement quelle règle métier a été transgressée. Et ce malheureux changement ne sera pas introduit dans les tuyaux de l’intégration.

[Comme j'ai pu l'écrire précédemment](http://blog.crisp.se/2015/03/24/perlundholm/too-small-for-a-user-story-bugs-fixes-and-support), une définition des anomalies devrait être simple et précise. Les anomalies sont des choses qui détruisent l’information, et ça c’est mal, peu importe qu’il s’agisse d’exigences ou non - c’est la seule définition qui convienne.

## Contrat

_(par Mattias Skarin)_

Alors qu’est-ce que nous utilisons à la place des exigences pour valider si ce que nous avons réalisé correspond à ce qui nous a été demandé ? Nous utilisons des contrats agiles. Les contrats agiles nous aident à nous concentrer sur ce qui compte, atteindre un objectif réel ensemble et répondre aux besoins de nos utilisateurs, à la place de nous perdre dans une forêt de détails.

Lorsque vous pensez à un contrat, prenez en considération ceci : dès l’instant où vous devez prendre votre contrat en main pour valider si votre partenaire a raté quelque chose, cela montre que quelque chose s’est très mal passé dans votre processus. Un contrat devrait permettre de bâtir la confiance entre le fournisseur et l’acheteur pour transcender tout ce qui cache dans les détails et non s’y perdre. 

## En résumé

* Bien que les éléphants et les girafes aient quatre pattes, ce sont des animaux différents
* Les _user stories_ ne sont pas des exigences, ce sont des instruments du planning
* Ce qui se rapproche le plus des exigences, c’est la spécification par l’exemple

## Références

Dans un [article de 2001](http://wiki.ayeba.fr/XP%2C+l%27essentiel+-+Carte%2C+Conversation%2C+Confirmation), Ron Jeffries indique : “… utilisez le jeu du planning pour sélectionner les _user stories_ …” 

“New to user stories” est un [article de la Scrum Alliance](https://www.scrumalliance.org/community/articles/2010/april/new-to-user-stories)
dans lequel William Nazzaro et Charles Suscheck comparent exigences et _user stories_.

Spécification par l’exemple :
Plus d’informations sur ce sujet dans cet article sur  [Wikipedia](https://en.wikipedia.org/wiki/Specification_by_example) et bien sûr [notre formation](https://crisp.se/kurser/kurstyper/specification-by-example) donnée par Gojki Adzic lui-même.


[^1]: FDA : Food and Drug Administration - Administration américaine responsable de la santé publique aux États-Unis

---  
Auteur : [Per Lundholm](https://www.crisp.se/konsulter/per-lundholm)  
Source : [User Stories Are Not Requirements](http://blog.crisp.se/2016/01/07/perlundholm/user-stories-are-not-requirements)  
Date de parution originale : 07 Janvier 2016  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 27/02/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

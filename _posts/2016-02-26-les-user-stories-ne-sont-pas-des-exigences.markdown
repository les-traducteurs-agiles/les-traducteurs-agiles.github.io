---
layout: post
title:  "Les user stories ne sont pas des exigences"
date:   2016-02-26 11:26:55
published: true
categories: 
- user-stories
---

![Elephants](http://blog.crisp.se/wp-content/uploads/2016/01/532397504_53698473c4_m.jpg)
_Elephants are not giraffes and user stories are not requirements. They share some traits and you may find them in the same context, but that does not make them the same. Despite that, many believe that user stories are the new requirements because there has to be requirements for a project, right? I give that a double “no”, they are not requirements and that is not anything we really need. User stories are about being able to explore options and seize opportunities. Requirements are about deciding up front and sticking with that._

<div align="left" style="float:left; padding-left:30px" >
  <img title="Eléphants" src="{{ site.url }}assets/stories_sont_pas_exigences/elephants.jpg" />
</div>

_Les éléphants ne sont pas des girafes et les **user stories** ne sont pas des exigences. Elles partagent certaines caractéristiques et vous pouvez les trouver dans le même contexte, mais cela ne les rends pas semblables. En dépit de cela, beaucoup croient que les **user stories** sont les nouvelles exigences parce qu’il doit bien y avoir des exigences dans un projet, n’est-ce pas ? À cela, Je réponds deux fois non, elles ne sont pas DES exigences et ce n’est pas quelque chose dont nous ayons vraiment besoin. Les **user stories** c’est être capable d’explorer les options et de saisir les opportunités. Les exigences c’est décider dès le début et s’y tenir._

Is this blog post really necessary? Don’t we all understand the above already? No, I believe that expressions like “the requirements in the backlog” reveals that old thinking where the requirements document is now called backlog and the requirements are called user stories. Then you think you are agile.

Cet article est-il vraiment nécessaire ? Ne comprenons-nous pas déjà tout ce qui vient déjà d’être dit précédemment ? Non, je crois que des expressions comme “les exigences sont dans le backlog” révèle une vieille manière de penser dans laquelle le document des exigences est désormais appelé backlog et les exigences appelées _user stories_. Et puis avec tout ça, vous pensez que vous êtes agile.

Other signs of the misconception is that user stories are given an unique id and stored in a database. This may be just convenient but can also be a sign of thinking in requirement terms.

D’autres signes de cette incompréhension est de donner aux _user stories_ un identifiant unique et de les stocker dans une base de données. C’est peut être pratique mais c’est aussi un signe révèlant un système de pensée orientée en terme d’exigences.

Putting user stories in a contract has to be a definitive sign of being requirements. The crazy part of it is that a user story is not as precise as a requirement and thus the contract is of little value. Requirements are of course open to interpretation but the techniques used to write them strive hard to remove any ambiguity. Requirements are also resistant to change, as they are used in project contracts. To change or add requirements, you need to take it through the CCB, Change Control Board. See below for more on contracts.

Mettre des _user stories_ dans un contrat c’est montrer sans ambiguïté qu’elles sont considérées comme des exigences ; Le plus dingue dans tout ça c’est qu’une _user stories_ n’est pas aussi précise qu’une exigence et qu’un tel contrat ne possède que peu de valeur. Et bien sûr les exigences restent sujet à interprétation malgré les techniques utilisées pour les écrire s’efforçant avec acharnement d’en lever toutes les ambiguïtés. Faisant partie intégrant des contrats pour les projets, les exigences sont aussi par nature résistantes à tout changement. Pour changer ou ajouter des exigences, vous devez les faire valider au CP, comité de pilotage. Pour en savoir plus sur cette partie contractuelle, reportez-vous à la section qui y est dédiée.

![Giraffes](http://blog.crisp.se/wp-content/uploads/2016/01/3185007560_3d2370cd5c_m.jpg)

<div align="left" style="float:left; padding-left:30px" >
  <img title="Eléphants" src="{{ site.url }}assets/stories_sont_pas_exigences/girafes.jpg" />
</div>

So what are user stories? Think of them as **planning instruments**. Since agile is about delivering value, the planning instrument is about values. We prioritize by user stories, we estimate them and we decide in which sprint we will implement them. All typical for a planning instrument, so do not try to make them into something else.

Alors, que sont les _user stories_ ? Considérez-les comme des **instruments du planning**. L’agilité étant portée sur la livraison de la valeur, l’instrument du planning porte aussi sur la valeur. Nous priorisons par _user stories_, nous les estimons et nous décidons dans quel sprint nous les implémenterons. C’est tout ce qui a de plus naturel pour un instrument du planning, donc n’essayez pas de les transformer en quelque chose d’autre.

The power of the user story is in the dialogue that it sparks. Instead of handing over a requirement specification that are interpreted by implementers and testers, a one-way communication, we have multiple skills involved in the discussion for each feature we add.

Le pouvoir de la _user story_ réside dans le dialogue qu’elle amorce. Au lieu d’avoir en main une spécification des exigences qui est interprétée par les développeurs et les testeurs, une communication à sens unique somme toute, dans la discussion que nous avons au sujet de chaque fonctionnalité que nous ajoutons nous avons plusieurs compétences impliquées autour de la table.

Since the stories do not carry much meaning, we can throw away them once done. We may very well keep statistics on how many story points we have done but that might be all.

Étant donné que les _stories_ ne convoient pas énormément de choses, une fois terminé nous pouvons les jeter après. Nous pouvons très bien garder quelques statistiques sur combien de points de story ont été réalisés mais c’est tout. 

But don’t we need requirements? Well, not really. There are of course constraints on how a system will be designed and built. E.g. medical equipment must respect regulation of the FDA. But let us call them constraints.

Mais avons-nous besoin d’exigences ? Eh bien pas vraiment. Bien sûr, il y a des contraintes sur comment un système sera conçu et réalisé. Par exemple, les équipements médicaux doivent respecter les règlementations de la FDA [^1]. Mais alors appelons-les des contraintes.

Still, requirements is a description of a system and surely there is value in that? How can you say that something is bug or not, unless you have requirements somehow? Here I would like to point to the technique of Specification by Example. Once you have decided that a feature shall be realised, you write the business rules as a series of examples in a format that is both human readable and executable. From those specifications, it is clear what the system does and should it go astray due to changes, the specifications will go red indicating exactly which business rule has been broken. That change will not slip through the build pipeline.

Mais les exigences sont bien la description d’un système, et il y a sûrement quelque chose là-dedans, non ? Comment pouvez-vous dire que telle ou telle chose est une anomalie ou pas si vous n’avez pas des exigences d’une manière ou d’une autre ? Ici, je voudrais signaler la technique de la spécification par l’exemple. Une fois que vous avez décidé que telle fonctionnalité sera réalisée, vous écrivez les règles métiers sous la forme d’une série d’exemples dans un format qui soit lisible à la fois par un humain et par un programme. À partir de ces spécifications, ce que fait le système devient clair et s’il venait à ne plus fonctionner correctement en raison d’un quelconque changement, les spécifications transgressées apparaîtront en rouge. Et ce malheureux changement ne sera pas introduit dans les tuyaux de l’intégration.

[As I have written before](http://blog.crisp.se/2015/03/24/perlundholm/too-small-for-a-user-story-bugs-fixes-and-support), a definition of bugs should be simple and precise. Bugs are things that destroy information and that is bad, regardless if there was a requirement or not, covering that exact case.

[Comme j'ai pu l'écrire précédemment](http://blog.crisp.se/2015/03/24/perlundholm/too-small-for-a-user-story-bugs-fixes-and-support), une définition des anomalies devrait être simple et précise. Les anomalies sont des choses qui détruisent l’information, et ça c’est mal, peu importe qu’il s’agisse d’exigences ou non - c’est la seule définition qui convienne.

## Contract

_(by Mattias Skarin)_

## Contrat

_(par Mattias Skarin)_

So what do we use instead of requirements to validate we are achieving what we asked for? We use Agile contracts. Agile contracts helps us focus on the thing that matter, achiving an effect goal together and solving user needs, instead on getting lost in a forest of details.

Alors qu’est-ce que nous utilisons à la place des exigences pour valider si ce que nous avons réalisé correspond à ce qui nous a été demandé ? Nous utilisons des contrats agiles. Les contrats agiles nous aident à nous concentrer sur ce qui compte, atteindre un objectif réel ensemble et répondre aux besoins de nos utilisateurs, à la place de nous perdre dans une forêt de détails.

When you think about a contract consider this: The moment you need to pick up your contract to validate if your partner has messed up something else has in your process has gone horribly wrong. A contract should build trust between provider and seller to transcend details, not get lost amontg them.

Lorsque vous pensez à un contrat, prenez en considération ceci : dès l’instant où vous devez prendre votre contrat en main pour valider si votre partenaire a raté quelque chose, cela montre que quelque chose dans votre processus s’est très mal passé. Un contrat devrait bâtir la confiance entre le fournisseur et l’acheteur pour transcender tout ce qui cache dans les détails et non s’y perdre. 

## Summary

## En résumé

* Although both elephants and giraffes have four legs, they are different animals.
* User stories are not requirements, they are planning instruments.
* The closest to requirements is Specification by Example

* Bien que les éléphants et les girafes aient quatre pattes, ce sont des animaux différents
* Les _user stories_ ne sont pas des exigences, ce sont des instruments du planning
* Ce qui se rapproche le plus des exigences, c’est la spécification par l’exemple

## References

## Références

[Ron Jeffries post from 2001](http://ronjeffries.com/xprog/articles/expcardconversationconfirmation/) where he says: “… uses the planning game to select user stories …”

Dans son [article de 2001](http://wiki.ayeba.fr/XP%2C+l%27essentiel+-+Carte%2C+Conversation%2C+Confirmation), Ron Jeffries indique : “… utilisez le jeu du planning pour sélectionner les _user stories_ …” 

[An article on Scrum Alliance](https://www.scrumalliance.org/community/articles/2010/april/new-to-user-stories) web “New to user stories” where William Nazzaro and Charles Suscheck compares requirements and user stories.

“New to user stories” est un [article de la Scrum Alliance](https://www.scrumalliance.org/community/articles/2010/april/new-to-user-stories)
dans lequel William Nazzaro et Charles Suscheck comparent exigences et _user stories_.

Specification by example: [Wikipedia](https://en.wikipedia.org/wiki/Specification_by_example) and [our course](https://crisp.se/kurser/kurstyper/specification-by-example) by the man himself: Gojki Adzic

Spécification par l’exemple :
Des informations sur ce sujet dans cet article dédié sur  [Wikipedia](https://en.wikipedia.org/wiki/Specification_by_example) et bien sûr [notre formation](https://crisp.se/kurser/kurstyper/specification-by-example) donnée par Gojki Adzic lui-même.


[^1] FDA: Food and Drug Administration - Organisme réglementant notamment l’activité médicale aux États-Unis

---  
Auteur : [Per Lundholm](https://www.crisp.se/konsulter/per-lundholm)  
Source : [User Stories Are Not Requirements](http://blog.crisp.se/2016/01/07/perlundholm/user-stories-are-not-requirements)  
Date de parution originale : 07 Janvier 2016  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 21/02/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

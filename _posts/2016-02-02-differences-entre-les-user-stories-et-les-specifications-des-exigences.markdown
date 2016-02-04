---
layout: post
title:  "La différence entre les user stories et les spécifications des exigences"
date:   2016-02-01 14:26:55
categories: 
- user story
---

It’s getting easier and easier to build unregulated software these days but it’s still pretty hard to create regulated/certified systems such as EHRs, medical device software, and government IT. To help create better systems we all know we need better user requirements; however, “heavyweight requirements” efforts have been shunned, especially in unregulated systems, over the past decade in favor of “user stories” and more agile specifications. But, are agile user stories the best way to go in regulated systems where requirements traceability and safety analysis is a must? I invited [Abder-Rahman Ali](http://www.productivecome.com/), currently pursuing his Medical Image Analysis Ph.D. in France, to come back and give us advice on whether there’s room for both user stories and SRSs in regulated industries or if we’re stuck with formal requirements specs. The following is Abder-Rahman’s third installment for this blog and I’m excited he’ll be tackling such an important topic. As always, he can be reached via [e-mail](abder-rahman.a.ali@ieee.org) or [twitter](http://www.twitter.com/abderhasan). Here’s what Abder-Rahman says about User Stories vs. Software Requirements Specifications:

_Aujourd’hui, il devient de plus en plus facile de créer des logiciels non soumis à un cadre réglementaire mais c’est toujours aussi difficile de créer des systèmes soumis à un cadre réglementaire ou certifiés tels que les logiciels de gestion des dossiers électroniques de santé, les logiciels embarqués dans les appareils médicaux, et les systèmes d’informations gouvernementaux. 
Nous savons que nous avons besoin de meilleures exigences fonctionnelles afin de nous aider à créer de meilleurs systèmes d’informations ; toutefois, ces dix dernières années“la grosse artillerie” des exigences a été rejetée, plus particulièrement pour les systèmes non certifiés où l’on préfère les “**user stories**” et les spécifications plus agiles. Mais, est-ce que les **user stories** agiles sont la meilleure voie pour les systèmes soumis à un cadre réglementaire où la traçabilité des exigences et l’analyse de la sécurité est une obligation ? J’ai invité [Abder-Rahman Ali](http://www.productivecome.com/), qui poursuit actuellement son doctorat d’analyse d’imagerie médicale en France, à venir et à nous donner son avis pour savoir s’il y a de la place à la fois pour les **user stories** et les spécifications des exigences dans les industries réglementées ou si nous devons en rester avec les spécifications formelles des exigences. L’article qui suit est la troisième intervention d’Abder Rahman sur ce blog et je suis content qu’il aborde un sujet aussi épineux. Comme précédemment, il peut être joint par [mail](abder-rahman.a.ali@ieee.org) ou sur [twitter](http://www.twitter.com/abderhasan). Voici donc ce que Abder Rahman dit à propos des **user stories** et des spécifications d’exigences de logiciel :_

It was on February, 2001, when seventeen practitioners formed what was called [The Agile Manifesto](http://agilemanifesto.org/). It seems that since then, we started to hear of the term User Story, although, as will be shown below, it seems that the term appeared before that date.

Ce fût en février 2001 que dix-sept praticiens ont accouchés de ce que l’on appelle le [manifeste agile](http://agilemanifesto.org/iso/fr/). Il semble que depuis lors nous avons commencé à entendre parler du terme _user story_, même si comme nous le montrerons plus loin, il semble que le terme soit apparu  bien avant cette date.

The questions that may pop-up on someone’s head are, is the User Story just a fancy name to the user requirement? Or, it is actually a new mindset of thinking in the way of dealing with user requirements?

Les questions qui peuvent surgir dans la tête de quelqu’un à propos des _user stories_ sont : est-ce que la _user story_ est-elle juste un nom fantaisiste pour exigence fonctionnelle ? Ou, est-elle vraiment un nouvel état d’esprit pour réfléchir à la manière de gérer les exigences fonctionnelles ? 

Referring to [Wikipedia](https://en.wikipedia.org/wiki/User_story) about the history of user stories, I found that user stories originated with Extreme Programming (XP), but, it wasn’t until 2001, when Ron Jeffries proposed the Three C’s formula: Card, Conversion, Confirmation, where the components of the user stories were captured.

En me référant à [Wikipedia](https://fr.wikipedia.org/wiki/R%C3%A9cit_utilisateur)  au sujet de l’origine des _user stories_, j’ai trouvé que celle-ci remontait à Extreme Programming (XP), mais, ce ne fut pas avant 2001 que les éléments constitutifs des _users stories_ furent réunis avec la formule des trois C proposée par Ron Jeffries : Carte, Conversation et Confirmation.

But, what are User Stories after all?

Mais, que sont les _user stories_ au juste ?

I really liked how [Mike Cohn](http://www.mountaingoatsoftware.com/agile/user-stories) described User Stories, when he said:

J’aime vraiment la manière dont [Mike Cohn](http://www.mountaingoatsoftware.com/agile/user-stories) décrit les _user stories_ lorsqu’il dit :

_User Stories are short, simple description of a feature told from the perspective of the person who desires the new capability, usually a user or customer of the system. They typically follow a simple template:_

_Les **user stories** sont des descriptions brèves et simples d'une fonctionnalité racontées du point de vue de la personne, généralement un utilisateur ou un client du système, désirant la nouvelle possibilité qui lui sera offerte par le logiciel. Les **user stories** suivent généralement un modèle très simple :_  

_As a \<type of user\>, I want \<some goal\> so that \<some reason\>._

_En tant que \<un type d'utilisateur\>, je veux \<réaliser un objectif quelconque\> afin de \<pour une certaine raison\>_

_User Stories are often written on index cards or sticky notes, stored in a shoe box, and arranged on walls or tables to facilitate planning and discussion. As such, they strongly shift the focus from writing about features to discussing them. In fact, these discussions are more important than whatever text is written._

_Les **user stories** sont écrites souvent sur des fiches cartonnées ou des notes adhésives, rangées dans une boîte à chaussures, et affichées sur les murs ou posées sur des tables pour faciliter la planification et la discussion. De cette manière, le centre de gravité est déplacé de l’écriture vers la discussion sur les fonctionnalités. En réalité, ces discussions sont plus importantes que le texte écrit._

Before moving ahead, and comparing User Stories with Software Requirements Specifications (SRS), let us see how SRS is defined. Based on [Chambers](http://www.chambers.com.au/glossary/software_requirements_specification.php), SRS describes the essential behavior of a software product from a user’s point of view, where the purpose of SRS is to be a basis for agreement between the customers and the suppliers on what the software product is to do; a basis for developing the software design; a basis for estimating costs and schedules; a baseline for validation and verification; reducing the development effort; facilitating transfer; and serves as a basis for enhancement.

Avant de continuer plus loin, et de comparer les **user stories** avec les spécifications des exigences, voyons comment les spécifications des exigences sont définies. D’après [Chambers](http://www.chambers.com.au/glossary/software_requirements_specification.php), les spécifications des exigences décrivent le comportement du logiciel d’un point de vue utilisateur, le but d’une spécification des exigences étant d’être la base d’un accord entre les clients et les fournisseurs sur ce que doit faire le logiciel ; une base pour développer la conception du logiciel ; une base pour l’estimation des coûts et les jalons ; une base pour la validation et la vérification ; pour réduire l’effort de développement ; pour faciliter le transfert ; et de servir comme d’une base pour l’amélioration.

After knowing what they mean, how can we compare User Stories with SRS? I saw that rather than bringing theory to this part, why not monitor some discussions related to this issue? I thus went through some discussions at a [Programmers Stack Exchange](http://programmers.stackexchange.com/questions/212834/user-story-vs-requirement) thread, and came up with the following:

Maintenant que nous savons ce qu’elles signifient, comment pouvons-nous comparer les **user stories** avec les spécifications des exigences ? Plutôt que parler encore de théorie sur cette partie, pourquoi ne pas regarder plutôt les discussions qui existent sur ce sujet ? J’en ai donc parcouru certaines dont une sur [Programmers Stack Exchange](http://programmers.stackexchange.com/questions/212834/user-story-vs-requirement), et j’y ai trouvé ceci :

One of the people involved in the discussion mentioned: _To be honest, after spending close to two years immersed in Agile development, I still think “User Story” is just a fancy term for “functional requirement”._ That person continues: _What User Stories almost never capture, in my experience, are non-functional requirements like performance and security. These kinds of requirements are very difficult to write properly and the format of the User Story simply isn’t very good for capturing them, because they’re more about general product quality and mitigating (but not eliminating) risks rather than meeting a specific user’s need. So, I really think of User Stories as a subset of requirements, with a specific formula, and still use the terms pretty much interchangeably. The one major advantage User Stories do have over requirements is that the word “requirement” suggests that a feature is required where it is often just desired. User Stories can in theory be prioritized and slotted in for any release, whereas requirements appear to be a prerequisite for every release._

L’une des personnes engagée dans cette discussion y mentionna la chose suivante : 

> Pour être honnête, après avoir passé deux ans en immersion en développement agile, je continue à penser que la “_user story_” est un juste un terme fantaisiste pour “exigence fonctionnelle”.

Puis elle poursuit :

> D’après mon expérience, ce que les “_user stories_” n’arrivent quasiment jamais à saisir, ce sont les exigences non fonctionnelles comme la sécurité ou la performance. Ces types d’exigences sont très difficiles à écrire correctement et le format utilisé par les _user stories_ n’est pas très adapté pour les saisir, parce qu’elles portent plus sur la qualité générale du produit et qu’elles atténuent (sans les réduire) les risques plutôt que satisfaire le besoin d’un utilisateur spécifique. Je pense donc vraiment que les _user stories_ sont un sous-ensemble des exigences, qui possèdent une formulation spécifique, et que les deux utilisent les mêmes termes de manière quasi interchangeable. L’avantage majeur que les _user stories_ peuvent avoir par rapport aux exigences est que le mot “exigence” suggère qu’une fonctionnalité est exigée là où elle est souvent seulement désiré. En théorie, les _user stories_ peuvent être priorisées et insérées dans n’importe quelle livraison, là où les exigences apparaissent comme un pré-requis pour chaque livraison.

Other opinions arise mentioning that SRS focuses on “how” the user interacts with the system, and “how” to implement the functionality. On the other hand, User Stories focus on “what” (interaction between user and system) purpose do features have, such that, the task of a User Story would be a functional requirement, and is the expected work product after the functional tasks have all been completed. Thus, they are completely different things.

D’autres soulèvent que les spécifications des exigences se focalisent sur le “comment” l’utilisateur interagit avec le système, et sur le “comment” la fonctionnalité est implémentée. D’un autre côté, les _user stories_ se focalisent sur le “quoi” (l’interaction entre l’utilisateur et le système) - le but que doit accomplir une fonctionnalité, et ainsi de suite, la tâche d’une _user story_ serait une exigence fonctionnelle, et elle est le résultat du travail attendu du produit après que toutes les autres tâches fonctionnelles aient été accomplis. Il s’agit donc de deux choses complètement différentes.

Requirements assume that the design of the application is done beforehand, and development is considering the implementation of that design.

Les exigences supposent que la conception de l’application est faite en amont et le développement est considéré comme l’implémentation de cette conception.

User Stories insist that the design of the product is done at the last minute, and is a collaboration between a product person and a developer person, and the details are decided during implementation.

Les _user stories_ insistent sur le fait que la conception du produit est faite en dernier [^1], qu’elle est le fruit de la collaboration entre une personne du métier et une personne du développement, et que les détails sont décidés pendant l’implémentation.

So, as can be noticed, the amount of details provided is different using the two approaches, such that, in the User Story for instance, there is a lot of information that is available not available in the requirement, namely, what is we are trying to achieve with the feature.

Comme nous avons pu le remarquer, la quantité de détails prodiguée est différente selon les deux approches, ainsi, dans le cas de la _user story_, il y a beaucoup d’informations disponibles non présentes dans les exigences, à savoir, ce que nous sommes en train d’essayer de réaliser avec cette fonctionnalité.

Others go and mention that a functional requirement is a formal specification that allows one to know exactly if the software works or not. Whilst a User Story is an informal way to describe a need of one of the User Stories, such that, it doesn’t specify a rigid specification to determine if the software is valid or invalid. Although you can test some part of the User Story, its real completion is when the user says : “Yes, this solves my problem”.

D’autres vont plus loin et indiquent qu’une exigence fonctionnelle est une spécification formelle qui permet à quelqu’un de savoir exactement si le logiciel fonctionne ou pas. Alors qu’une _user story_ est une manière _informelle_ de décrire le besoin, elle n’indique pas de manière stricte pour déterminer si un logiciel est valide ou non. Même si vous testez qu’une partie de la _user story_, elle sera vraiment terminée lorsque l’utilisateur dira : “Oui, cela solutionne mon problème”.

We thus realize that the User Story is a huge paradigm shift in the way to approach the work to be done. A contract here is not made, rather, you are trying to help your user to solve a problem. If you don’t see your user stories as discussion tools with a real user, then you are actually not using User Stories.

Nous prenons donc conscience que la _user story_ est un changement de paradigme énorme dans la manière dont le travail est à accomplir. Un contrat n’est pas établit ici, en lieu et place, vous êtes en train d’essayer d’aider votre utilisateur à résoudre un problème. Si vous ne voyez pas vos _user stories_ comme d’instruments de discussions avec un utilisateur et un vrai, alors vous n’êtes pas vraiment en train d’utiliser des _user stories_.

This post can grow bigger and bigger, and seems that when people attempt describe the notions “User Story” and “user requirement”, such descriptions come from their experience, and how they use each of them. Going through the comparisons above may not reveal clearly the differences between both terms. For that, we chose to interview Agile experts about this issue, for which answers will be shown in the next post.

Cet article peut grossir encore et encore, et il semble que lorsque les personnes tentent de décrire les notions de “_user story_” et d’“exigences utilisateurs”, elles les décrivent d’après leur expériences et d’après la manière dont elles les ont chacune utilisée. Examiner en profondeur ces différentes analyses ne permet pas de révéler clairement les différences entre les deux. Pour cela, nous avons choisi plutôt de poser des questions sur ce sujet à des experts agiles, dont vous trouverez les réponses prochainement.

Stay tuned until then, and don’t hesitate to share your views in this topic, and how you approach those two terms.

Tenez-vous au courant d’ici là, et n’hésitez à nous faire part de votre point de vue sur ce sujet [^2], et comment vous approchez ces deux termes.

[^1]: la traduction littérale “à la dernière minute” n’a pas été retenue pour éviter de donner un sens péjoratif au texte. Plus généralement on parle de _last responsible moment_ qui signifie (sans aller dans les détails) : éviter de prendre des décisions trop précocement ou d’attendre le meilleur moment- NdT

[^2]: ou dans votre réseau social préféré, notre site étant dépourvu de commentaires - NdT

---  
Auteur : [Abder-Rahman Ali](https://twitter.com/abderhasan)  
Source : [The difference between User Stories and Software Requirements Specifications (SRS), especially for regulated systems (part 1)](http://www.healthcareguy.com/2014/10/10/the-difference-between-user-stories-and-software-requirements-specifications-srs-especially-for-regulated-systems-part-1/)  
Date de parution originale : 10 Octobre 2014  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 03/02/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}
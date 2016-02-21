---
layout: post
title:  "La différence entre les user stories et les spécifications des exigences - Entretien avec Christiaan Verwijs"
date:   2016-02-21 11:26:55
published: true
categories: 
- user-stories
---

_This is the third post in the series in which I have interviewed several Agile experts to reveal the differences between user stories and software requirements and their application to regulated systems (i.e., health IT systems). You can find the previous post of this series [here](https://www.healthcareguys.com/?p=29726)._

Voici le troisième article de la série d’entretiens que j’ai réalisé avec plusieurs experts agiles pour montrer les différences entre les **user stories** et les spécifications des exigences ainsi que leurs applications dans les systèmes d’informations soumis à la réglementation (par exemple  dans le domaine médical). Vous pouvez lire le précédent article de cette série [ici](http://www.les-traducteurs-agiles.org/user-stories/2016/02/10/differences-entre-les-user-stories-et-les-specifications-des-exigences-par-johanna-rothman.html)_

Today’s interviewee is Christiaan Verwijs. Christiaan is the founder of Agilistic, a company that specializes in helping small businesses and startups on their journey toward Agile software development. He has been working with Scrum for more than three years, for a variety of companies and with a diverse group of teams. He enjoys writing about his Agile adventures in his personal blog: [http://www.christiaanverwijs.nl](http://www.christiaanverwijs.nl)

Je m’entretien aujourd’hui avec Christiian Verwijs. Christiian est le fondateur d’Agilistic, entreprise spécialisée dans l’accompagnement des PME et des startups le long de leurs périples vers l’agilité. Depuis plus de trois ans, il fait du Scrum au sein de différentes entreprises et avec différentes équipes. Il aime bien écrire à propos de ses aventures agiles sur son blog personnel : [http://www.christiaanverwijs.nl](http://www.christiaanverwijs.nl) 

**Do you think that “user story” is just a fancy name for SRS?**

**_Pensez-vous que “user story” soit juste un terme fantaisiste pour la spécification des exigences ?_**

The concept of a user story must be understood within the context of Agile software development. For me, a user story is mostly a vehicle to facilitate discussion and collaboration within the team. Some liken user stories to “unrealized product options,” and I like that idea. A user story is the simplest way to describe such options from the user’s point of view, “simplest” in the sense that it provides the team with just enough information to get started, test assumptions, and delivers something of value at the end of the sprint that can be reviewed. In a sense, you could describe a user story as a requirement. But it’s mostly just a “product option” that is either more or less desirable to the product owner.

Le concept de la _user story_ doit être compris à l’aune du contexte du développement agile de logiciels. Pour moi, une _user story_ est grosso modo un moyen pour faciliter la discussion et la collaboration au sein d’une équipe. Certains comparent les _user stories_ à “des options non réalisées du produit”, et j’avoue que j’apprécie cette idée. Une _user story_ est la manière la plus simple de décrire ce genre d’options d’un point de vue utilisateur, “la plus simple” dans le sens où cela procure à l’équipe suffisamment d’informations pour commencer, d’hypothèses pour tester, et pour livrer quelque chose ayant de la valeur en fin du sprint qui puisse être passée en revue. D’une certaine manière, vous pourriez décrire une user story comme une exigence. Mais il s’agit plus simplement “d’une option du produit” qui est plus ou moins désirable aux yeux du _product owner_.

**How do you compare a user story with SRS?**

**_Comment comparez-vous une user story avec une spécification des exigences ?_**

User stories are a form of specification, but a very limited one – by design. Within the context of Agile software development, we accept that projects are subject to frequent change and mistakes (in estimation, in assumptions, etc.). Instead of spending a lot of time on writing thorough specifications, we prefer to work with the least-extensive specifications to get us started. The problem with SRS is that they are mostly a bunch of assumptions about what users want, how functionality should work, and how to technically implement it. Until you’ve built the actual software and shown it to actual users, it’s all just speculation. And if your assumptions turn out to be wrong (as they often are), you have wasted a lot of time on specification. This makes it an expensive failure. Instead, I prefer to work with a method where I can fail early and quickly. Mistakes are less costly this way. And the best way to do this is by frequently delivering and reviewing (real) working software. So instead of focusing on specifications, we focus on building working software.

Les _user stories_ sont une forme de spécification, mais une forme - par nature - très limitée. Dans le contexte du développement agile, nous acceptons que les projets soient sujets à de fréquents changements et sujets aux erreurs (dans les estimations, dans les hypothèses de travail, etc). À la place de passer beaucoup de temps à écrire une spécification exhaustive, nous préférons travailler sur des spécifications moins détaillées pour commencer. Le problème avec les spécifications des exigences c’est qu’elles représentent tout un tas d’hypothèses sur ce que les utilisateurs veulent, sur comment les fonctionnalités devraient marcher, et sur comment les implémenter techniquement. Jusqu’au moment où vous les aurez construites et que vous aurez montré le vrai logiciel aux utilisateurs, tout cela est uniquement de la spéculation. Et si vos hypothèses s’avèrent être fausses (comme souvent cela peut être le cas), vous aurez perdu beaucoup de temps sur la spécification. C’est un échec qui revient cher. À la place, je préfère travailler avec une méthode qui me permet d’échouer de bonne heure et rapidement. Les erreurs coûtent moins chers de cette manière. Et la meilleure manière de le faire est en livrant et en passant en revue un (vrai) logiciel opérationnel. Par conséquent, à la place de se focaliser sur les spécifications, nous nous focalisons sur la réalisation d’un logiciel opérationnel.

This does not mean that you can’t extend user stories with more information, like acceptance criteria. For me, this is usually just a short checklist of what a user story must do. Like, “It must work in IE8,” or “The email uses the styling of [Brand X].” They can help to address nonfunctional requirements. Although I’m perfectly happy with backlogs that are not 100 percent made up of user stories. Nowhere in the Scrum Guide does it say that user stories are required or even needed. I prefer to write the acceptance criteria during sprint planning or when preparing the next sprint – just-in-time specification, in a sense. But very minimal, as I want to focus on writing working software instead of documents.

Cela ne signifie pas que vous ne pouvez pas ajouter des informations supplémentaires aux _user stories_ avec par exemple des critères d’acceptances. Pour moi, il s’agira plus généralement d’une simple liste de ce qu’une _user story_ doit faire. Comme par exemple “cela doit fonctionner sous IE8”, ou bien “le mail suit la charte graphique de la [marque X]”. Elles peuvent permettre de gérer des exigences non fonctionnelles. Je suis tout de même satisfait avec les backlogs qui ne comportent pas 100% de _user stories_. Il n’y a rien dans le guide Scrum indiquant que les _user stories_ soient obligatoires ou même nécessaires. Je préfère écrire les critères d’acceptances pendant la planification du sprint ou lors de la préparation du sprint suivant - d’une certaine manière, de la spécification en juste-à-temps. Mais c’est vraiment à minima, car je souhaite me focaliser sur l’écriture d’un logiciel opérationnel plutôt que sur celle de documents.

**Do you think that user stories replace “SRS”?**

**_Pensez-vous que les user stories remplacent les spécifications des exigences ?_** 

User stories serve a different need. They are not supposed to replace SRS. They are supposed to be part of a different way to build software. Instead of a planned approach, it suits an approach based on collaborative discovery.

Les _users stories_ répondent à un besoin différent. Elles ne sont pas supposées remplacer les spécifications des exigences. Elles sont supposés faire partie d’une manière différente de réaliser un logiciel.Elles conviennent plus à une approche basée sur la découverte collaborative plutôt qu’à une approche planifié.

**Which of the two do you prefer working with?**

**_Avec laquelle des deux, préférez-vous travailler avec ?_**

User stories. But not because of the stories themselves, but the different process they are a part of. I’m currently working on a large project with a team of six developers. We’ve completed about eight sprints now and have seen a major shift in what we’re building and how we’re building it. When we started the project, we had a lot of ideas and quite a detailed backlog (with user stories, but still). After only a few months, we’ve dropped a lot of supposed core features and replaced them with very different solutions that we discovered as we progressed. I really enjoy this approach because it fits with the discovery process and the unexpected stuff that happens in all projects. If we would’ve had to write software requirements, we would’ve spent months on that. And we would’ve still run into the same unexpected and unpredicted issues. It was a lot less painful to drop a few lightly detailed user stories than a bunch of specification documents.

Les _user stories_. Non à cause des _stories_ elles-mêmes, mais à cause du processus particulier dont elles font partie. Je travaille actuellement sur un grand projet au sein d’une équipe de 6 développeurs. Nous avons accompli environ 8 sprints et nous avons connu un grand changement sur ce que nous réalisons et sur comment nous le réalisons. Lorsque nous avons commencé le projet, nous avions beaucoup d’idées et un _backlog_ assez détaillé (avec des _user stories_ mais pas que). Après seulement quelques mois, nous avons abandonné un certain nombre de fonctionnalités soit disant essentielles et les avons remplacées avec des solutions très différentes, découvertes au fur et à mesure que nous avancions. 

**Which of the two methods do you recommend using for regulated systems (i.e., health IT systems, medical device software)?**

**_Laquelle des deux méthodes recommandez-vous dans le cadre de systèmes soumis à la réglementation (c’est-à-dire les systèmes d’informations dans le domaine de la santé, dans les logiciels embarqués d’appareils médicaux) ?_**

As for regulated systems, you may need more specifications on the software that you’ve written. But I’m not sure if you really need more specifications before you start building software. After all, why would the problems that non-health-IT projects are facing – constant change, different interpretations, difficulty with estimation – not affect these kinds of projects? This software is equally vulnerable to incorrect assumptions. Maybe even more so. What you will need is to very carefully describe how the software works and what happens under what conditions. I think that this kind of specification can be in the form of documentation, but I would actually prefer batteries of exhaustive automated tests – unit, regression, etc. This way, your “documentation” stays up-to-date as tests are adjusted when bugs are fixed, new features are implemented, etc.

Pour les systèmes d’informations soumis à la réglementation, vous pouvez avoir besoin de davantage de spécifications pour le logiciel que vous êtes en train d’écrire. Mais je ne suis pas certain que vous ayez vraiment besoin de plus de spécifications avant que vous ne commenciez à développer le logiciel.  Après tout, pourquoi est-ce que les problèmes auxquels les projets informatiques des domaines autres que la santé font face - changement constant, interprétations différentes, difficultés d’estimations - ne seraient-ils affectés eux aussi ? Ces logiciels sont tout autant vulnérables aux mauvaises hypothèses. Peut-être même plus. Ce que à quoi vous devrez faire très attention est la manière dont le logiciel doit fonctionner et ce qu’il se produit selon quelles conditions. Je pense que ce type de spécifications peut exister sous la forme d’une documentation, mais en fait, je préfèrerais que ce soit sous la forme d’une batterie de tests exhaustifs automatisés - unitaires, de régressions, etc. De cette manière, votre “documentation” reste à jour au fur et à mesure que les tests sont ajustés, que les anomalies sont corrigés, que les nouvelles fonctionnalités sont implémentées, etc.

Do you agree with Christiaan? Comments and discussion are welcome.

Êtes-vous d’accord avec Christiaan ? Tous les commentaires et les points de vue sont les bienvenus. [^2]

You can find the next post in this series, where I interviewed Per Lundholm, [here](https://www.healthcareguys.com/?p=29756).

Vous pourrez retrouver le prochain article de cette série qui sera l’entretien que j’ai eu avec Per Lundholm [ici](https://www.healthcareguys.com/?p=29731). [^3]

---  
Auteur : [Abder-Rahman Ali](https://twitter.com/abderhasan)  
Source : [The Differences between User Stories and Software Requirements Specification (SRS) – Interview with Christiaan Verwijs](https://www.healthcareguys.com/2015/07/23/the-differences-between-user-stories-and-software-requirements-specification-srs-interview-with-christiaan-verwijs/)  
Date de parution originale : 23 Juillet 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 21/02/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

---
layout: post
title:  "La différence entre les user stories et les spécifications des exigences - Entretien avec Ron Jeffries"
date:   2016-02-05 11:26:55
published: true
categories: 
- user-stories
---

_As mentioned in our post [The Difference between User Stories and Software Requirements Specification (SRS)](), we decided to interview some Agile experts on this topic in order to reveal some confusion that may be occurring in the industry. This will be a series of interviews, with one interview presented in each blog post._

Ainsi que nous l’avions mentionné dans notre article intitulé [La différence entre les user stories et les spécifications des exigences](http://www.les-traducteurs-agiles.org/user-stories/2016/02/04/differences-entre-les-user-stories-et-les-specifications-des-exigences.html), nous avons décidé de parler avec des experts agiles au cours d’une série d’entretiens afin de lever l’ambiguïté qui peut exister dans l’industrie informatique sur ce sujet. Chaque entretien de cette série fera l’objet d’un article à part entière.

The interviewee that we present now is [Ron Jeffries](https://en.wikipedia.org/wiki/Ron_Jeffries), one of the 17 authors and signatories of the [Agile Manifesto]((http://agilemanifesto.org/iso/fr/). He was the onsite XP coach for the original Extreme Programming project in 1996. He is the proprietor of [http://ronjeffries.com](http://ronjeffries.com) and senior author of _Extreme Programming Installed_ – the second XP book after Beck’s white book – and the author of _Extreme Programming Adventures in C#_.

L’invité du présent entretien est [Ron Jeffries](https://fr.wikipedia.org/wiki/Ron_Jeffries), l’un des 17 auteurs et signataires du [manifeste agile]((http://agilemanifesto.org/iso/fr/). C’était lui, le coach XP qui était présent sur site lors du projet originel Extreme Programming en 1996. Il est l’homme derrière le site [http://ronjeffries.com](http://ronjeffries.com), l’auteur principal d’_Extreme Programming Installed_ - le deuxième livre sur XP après le livre blanc de Kent Beck - et il est également l’auteur de _Extreme Programming Adventures in C#_.

Ron is a frequent speaker and trainer at Agile software-development conferences, including attending and speaking at all of conferences in the United States and some in Europe. He is a well-known independent consultant in XP and Agile methods.

Ron assiste et participe aux conférences sur le développement agile de logiciels aussi bien aux Etats-Unis qu’en Europe, dans lesquelles il intervient fréquemment en tant qu’orateur et formateur. Ron est également un consultant indépendant de renom sur XP et l’agilité.

Thus, I saw that Ron would be a great fit for the topic we are investigating. Without further ado, let us go ahead and see what Ron Jeffries had to tell us:

Par conséquent, il était tout indiqué que Ron soit la personne idéale concernant le sujet qui nous préoccupe. Sans plus tarder, poursuivons et voyons ce que Ron Jeffries a à nous dire :

**Do you think that “user story” is just a fancy name for SRS?**

**Pensez-vous que “_user story_” soit juste un terme fantaisiste pour la spécification des exigences ?**

No, they are quite different. User stories are small descriptions of single features, usually the smaller the better. SRS has no standard definition that I’m aware of, but generally refers to the set of all requirements, not to a single one. Even a single requirement spec is usually much much larger than a story.

Non, ces deux termes sont assez différents. Les _user stories_ sont des descriptions brèves de fonctionnalités prises individuellement, et généralement plus courtes, meilleures elles sont. À ma connaissance, les spécifications des exigences n’ont pas de définition, et elles se réfèrent généralement à l’ensemble des exigences, non à une seule. Même une seule spécification des exigences est généralement beaucoup beaucoup plus grosse qu’une story. 

**How do you compare a user story with SRS?**

**Comment comparez-vous une _user story_ avec une spécification des exigences ?**

I wouldn’t. I don’t see the need to do so. You may see a need, of course.

Je ne le ferais pas. Je ne vois pas le besoin de le faire. Vous pouvez en voir le besoin bien sûr.

**Do you think that user stories replace SRS?**

**Pensez-vous que les _user stories_ remplacent les spécifications des exigences ?** 

Certainly, products large and small can be and have been built without doing anything I’d call SRS. So the answer is clearly yes – user stories can replace SRS.

Certainement, de petits ou de grands produits  peuvent être ou ont été construits sans quoi que ce soit qui ressemble de près ou de loin à des spécifications des exigences. Donc la réponse est clairement oui - les _user stories_ peuvent remplacer les spécifications des exigences. 

**Which of the two do you prefer working with?**

**Avec laquelle des deux, préférez-vous travailler avec ?**

Stories. They are small, simple, and easy to use. Because they are focused more on conversation than on writing, they are far more collaborative. According to my explanation of stories, they explicitly include acceptance criteria and are also concrete enough for any purpose. Search for “Card, Conversation, Confirmation” for more on that thought.

Les stories. Elles sont petites, simples, et faciles à utiliser. Et parce qu’elles sont plus focalisées sur la conversation que sur l’écriture, elles sont beaucoup plus collaboratives. D’après mon explication sur les stories, elles incluent explicitement les critères d’acceptance et elles sont suffisamment concrètes pour n’importe quel objectif. Faites donc quelques recherches sur internet sur “Carte, Conversation, Confirmation” pour en savoir plus sur ce concept.

**Which of the two methods do you recommend using for regulated systems (i.e., health IT systems, medical device software)?**

**Laquelle des deux méthodes recommandez-vous dans le cadre de systèmes soumis à la réglementation (c’est-à-dire les systèmes d’informations dans le domaine de la santé, dans les logiciels embarqués d’appareils médicaux) ?**

I would use stories for everything at the team level. There might be some higher-level SRS that is parsed out into stories. There is some good work being done with regulated systems and every reason to believe that a lot of the mechanism that big organizations have built up could be trimmed down a lot. This might be seen as more of a job for Lean than for Agile.

J’utiliserais les _user stories_ pour tout ce qui relève de la responsabilité de l’équipe . Il pourrait y avoir des spécifications des exigences transverses aux stories. Il y a eut du bon boulot de fait avec les systèmes soumis à la réglementation et il y a beaucoup de raisons de croire qu’une majorité des mécanismes qui ont été bâtis par les grosses organisations pourraient être fortement réduits. C’est un boulot qui pourrait être pluspour le Lean que pour l’Agile.

Do you agree with Ron Jeffries? Comments and discussion are welcome.

Êtes-vous d’accord avec Ron Jeffries ? Tout commentaire et point de venue sont les bienvenus. [^1]

The next post in this series where I interviewed Johanna Rothman can be found [here](https://www.healthcareguys.com/?p=29726).

Le prochain article de cette série sera l’entretien que j’ai eu avec Johanna Rothman que vous pouvez retrouver [ici](https://www.healthcareguys.com/?p=29726). [^2]

[^1]: ou dans votre réseau social préféré, notre site étant dépourvu de commentaires - NdT
[^2]: traduit très prochainement - NdT

---  
Auteur : [Abder-Rahman Ali](https://twitter.com/abderhasan)  
Source : [The Differences between User Stories and Software Requirements Specification (SRS) – Interview with Ron Jeffries](https://www.healthcareguys.com/2015/07/23/difference-user-stories-software-requirements-specifications-srs-interview-ron-jeffries/)  
Date de parution originale : 23 Juillet 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 03/02/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

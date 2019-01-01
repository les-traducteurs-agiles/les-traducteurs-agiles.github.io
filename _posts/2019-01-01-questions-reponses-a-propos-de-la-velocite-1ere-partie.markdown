---
layout: post
title:  "Questions/Réponses à propos de la vélocité - 1ère partie"
date:   2019-01-01 00:01
published: true
tags:
- vélocité
---

Having had many conversations about velocity (and many blog posts here and at the Industrial Logic Blog) one day I decided to write up an example of the conversation as if it were happening between two characters named A and B.

Ayant eu de nombreuses conversations à propos de la vélocité (ainsi qu'un certain nombre d'articles de blog ici et sur le blog d'Industrial Logic), j'ai un jour décidé d'écrire une discussion fictive entre deux personnages appelés A et B comme si elle était en train de se dérouler.

The first question asked by A was the first question about story points that a younger agile otter asked in his first XP project.

La première question posée par A était la première question posée par une jeune loutre[^1] agile à propos des points de story lors de son premier projet XP.

Most of the questions were asked by my younger self at some point or asked by someone I have worked with.

La plupart des questions avaient été posé par une version plus jeune de moi-même à un moment donné ou par quelqu'un avec qui j'avais pu travailler.

By the same token, the answers came from myself and people I know too. I've internalized these conversations to the point that I'm not sure what questions were mine and which were asked of me, and which answers were original and which came from mentors (managers, coaches, developers, etc).

Du même coup, les réponses furent donné par moi et par les gens que je connais. J'ai internalisé ces questions au point que je ne suis même pas certains que ces questions sont bien les miennes ou qu'elles me furent posées, et quelles réponses sont mes propres réponses ou celles qui viennent de mes mentors (manageurs, coachs, développeurs, etc).

Suffice it to say that I'm represented (at various points in my journey) by both the questions and the answers. As such, the point of the dialog between A and B is not to humiliate or pillory either A or B. The questions are pretty reasonable (most of the time) and the answers are not only honest but reveal deeper truths about software development and agile methods -- most of which one cannot acquire except through years of experience or mentoring.

Il suffit de dire que je suis présent (à différentes étapes de mon parcours) que ce soit au niveau des questions que des réponses. À ce titre, je tiens à souligner que dans le dialogue entre A et B, il n'est aucunement question d'humilier ou de mettre au piloris A ou B. Les questions sont du reste plutôt raisonnables (la plupart du temps) et les réponses ne sont pas seulement honnêtes, elles révèlent également des vérités profondes à propos du développement logiciel et des méthodes agiles — la plupart d'entre elles ne peuvent être apprises si ce n'est qu'après des années d'expériences ou de mentorats.

At no time is it to be assumed by my publication of this series that I recommend using story points or velocity. I do not.  Even so, if people are using them, they should understand them at least until they realize that they are better off without.

À aucun moment, il est à prendre pour acquis dans la publication de cette série d'articles que je recommande l'utilisation des points de story ou de la vélocité

So, here is part 1, annotated.

Voici dont la 1ère partie annotée

    A: How long is a story point in real time?
    B: How many did you do in your last sprint?
    A: 23
    B: Then, for you, it's a 23rd of a sprint
    A: But the time before that it was 19
    B: At the time it was 1/19th of a sprint.
    A: But how long is it really?
    B: We've determined that.

    A: À combien d'heures correspondent un point de story ?
    B: Combien de points de story avez-vous réalisé lors de votre dernier sprint ?
    A: 23
    B: Alors pour vous, cela correspond à 1/23ème de sprint
    A: Mais la fois d'avant cela avait été 19
    B: À ce moment là cela correspondait à 1/19ème de sprint.
    A: Mais à combien de temps cela correspond-il ??
    B: C'est ce que nous venons juste de déterminer.

This was a major breakthrough for me early on. I didn't realize that roughly the same amount of work is done every week. Story points are a rough sizing of work, not a measurement.

Cela fût très tôt une découverte capitale pour moi. Je n'avais pas réalisé jusqu'alors que la quantité de travail réalisée est à peu près la même chaque semaine. Les points de story correspondent à une estimation grossière de la taille du travail, et non une évaluation.

I was once informed that every estimate involves not only effort but risk and learning. Risk and learning are often the larger part of each estimate. So when someone assigns a larger estimate, it is usually because they don't know how much they're going to have to learn to do the work or because they don't know what the risk is of it having wider unwanted effects on the schedule.

Une fois, Il m'a été dit que chaque estimation implique non seulement un effort donné mais aussi un risque et un apprentissage (une part d'inconnu). Les risques et l'apprentissage représentent souvent la part la plus grande de chaque estimation. Donc lorsque quelqu'un chiffre une grosse estimation, c'est généralement parce qu'il ne sait pas vraiment beaucoup de choses sur ce qu'il va devoir apprendre pour faire le boulot ou parce qu'il ne sait pas quel est le risque d'avoir des effets indésirables sur le planning.

Many developers and managers refer to stories "blowing up" -- where it was estimated as a 2, but in reality, it was more like an 8 or 13 or 21. It's hard to know where the risks and learning will occur.

Un certain nombre de développeurs et de manageurs reprochent aux _stories_ d'exploser — là où celles-ci étaient estimées à 2, alors qu'en réalité, cela correspondait plus à 8 ou 13 ou 21. C'est difficile de savoir lorsque les risques ou l'apprentissage va réellement se produire.

Sometimes a story assigned an 8 or 13 turns out to be easier and less risky than imagined, and the story is done in the time it would take to do one that would have been assigned a 2.

Parfois une _story_ chiffrée à 8 ou à 13 peut s'avérer plus facile ou moins risquée qu'initialement prévue, et la _story_ est faite comme si cela avait pu s'agir d'une story chiffrée à 2.

This doesn't mean that the team is doing a bad job, it really _reflects more on the variability of the work items instead of the lack of consistency of the team_.

Cela ne signifie pas que l'équipe a fait un mauvais boulot, en réalité _cela reflète davantage la variabilité des items à faire que du manque de cohérence de l'équipe_.

When the team is not familiar with the source code of the project,  it is more common for greater numbers to be assigned and it for the stories to "blow up" or have defects. That's what happens when you don't know your way around.

Lorsque l'équipe n'est pas familière avec le code source du projet, il est plutôt habituel de voir des chiffrages élevées et que _stories_ explosent ou aient des anomalies. C'est ce qu'il se passe quand vous n'êtes familier des lieux.

But either way, the size of a story point isn't very meaningful -- it's a guess to begin with, and its "real size" is not only knowable in arrears, but is also variable. It is a unitless unit of measure, a bit of nonsense that people sometimes find useful for capacity planning.

Mais quoi qu'il en soit, la taille d'un point de _story_ n'est pas vraiment significatif — c'est une supposition, quelque chose par laquelle commencer, et sa "vraie taille" ne sera vraiment connu que lorsqu'elle sera terminée, mais elle est aussi variable. C'est une unité de mesure sans unité, une espèce de non-sens que les gens trouvent parfois utile pour planifier la capacité à faire.

It's almost always misused. An option is to [stop using story points](https://www.industriallogic.com/blog/stop-using-story-points/).

C'est souvent quelque chose de mal utilisé. Une alternative possible est d'[arrêter d'utiliser les points de _story_](https://www.industriallogic.com/blog/stop-using-story-points/).

I'll see you in Part II.

Je vous revois pour la [2ème partie](https://agileotter.blogspot.com/2018/07/q-on-velocity-part-ii.html).

[^1]: le nom du site de l'auteur est Otter en anglais ou loutre en français et c'est aussi le surnom de l'auteur ;) - NdT

---
Auteur : [Tim Ottinger](https://plus.google.com/+TimOttinger)  
Source : [Q&A on Velocity, Part I](https://agileotter.blogspot.com/2018/07/q-on-velocity-part-i.html)  
Date de parution originale : 17 Juillet 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 01/01/2018  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

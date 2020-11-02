---
layout: post
title:  "Questions/Réponses à propos de la vélocité - 1ère partie"
date:   2019-01-01 00:01
published: true
tags:
- vélocité
---

Ayant eu de nombreuses conversations à propos de la vélocité (ainsi qu'un certain nombre d'articles de blog ici et sur le blog d'Industrial Logic à ce sujet), j'ai décidé d'écrire un jour une discussion fictive entre deux personnages appelés A et B comme si elle était en train de se dérouler.

La première question posée par A était la première question posée par une jeune loutre[^1] agile à propos des points de _story_ lors de son tout premier projet XP.

La plupart des questions ont été posées par une version plus jeune de moi-même à un moment donné ou par quelqu'un avec qui j'ai pu travailler.

Du même coup, les réponses ont été données par moi ou par les gens que je connais. J'ai internalisé ces questions au point que je ne suis même pas certains que ces questions sont bien les miennes ou qu'elles me furent posées, et quelles réponses sont mes propres réponses ou celles qui viennent de mes mentors (manageurs, coachs, développeurs, etc).

Il suffit de savoir que vous allez me retrouver (à différentes étapes de mon parcours) que ce soit au niveau des questions que des réponses. À ce titre, je tiens à souligner que dans le dialogue entre A et B, il n'est aucunement question d'humilier ou de mettre au pilori A ou B. Les questions sont du reste tout à fait acceptables (la plupart du temps) et les réponses ne sont pas seulement honnêtes, elles révèlent également des vérités profondes à propos du développement logiciel et des méthodes agiles — la plupart d'entre elles ne peuvent être apprises si ce n'est qu'après des années d'expériences ou de mentorats.

À aucun moment, il est à prendre pour acquis dans la publication de cette série d'articles que je recommande l'utilisation des points de story ou de la vélocité. Je ne le fais pas. Même si les gens les utilisent, ils devraient au moins en avoir la compréhension jusqu'à ce qu'ils réalisent qu'ils vivront mieux sans.

Voici dont la 1ère partie annotée

> A : À combien d'heures correspondent un point de story ?  
> B : Combien de points de story avez-vous réalisé lors de votre dernier sprint ?  
> A : 23  
> B : Alors pour vous, cela correspond à 1/23ème de sprint  
> A : Mais la fois d'avant cela avait été 19  
> B : À ce moment-là cela correspondait à 1/19ème de sprint.  
> A : Mais à combien de temps cela correspond-il ?  
> B : C'est ce que nous venons juste de déterminer.  

Cela fût très tôt une découverte capitale pour moi. Je n'avais pas réalisé jusqu'alors que la quantité de travail réalisée est à peu près la même chaque semaine. Les points de story correspondent à une estimation grossière de la taille du travail, et non une évaluation.

Une fois, Il m'a été dit que chaque estimation implique non seulement un effort donné mais aussi un risque et un apprentissage. Les risques et l'apprentissage représentent souvent la part la plus grande de chaque estimation. Donc lorsque quelqu'un chiffre une grosse estimation, c'est généralement parce qu'il ne sait pas vraiment beaucoup de choses sur ce qu'il va devoir apprendre pour faire le boulot ou parce qu'il ne sait pas quel est le risque d'avoir des effets indésirables sur le planning.

Un certain nombre de développeurs et de manageurs reprochent aux _stories_ d'exploser — pour celles qui étaient estimées à 2, alors qu'en réalité, elles correspondaient plus à 8 ou 13 ou 21. C'est difficile de savoir lorsque les risques ou l'apprentissage va réellement se produire.

Parfois une _story_ chiffrée à 8 ou à 13 peut s'avérer plus facile ou moins risquée qu'initialement prévue, et la _story_ est faite comme si cela avait pu s'agir d'une _story_ chiffrée à 2.

Cela ne signifie pas que l'équipe a fait un mauvais boulot, en réalité _cela reflète davantage la variabilité des items à faire que du manque de cohérence de l'équipe_.

Lorsque l'équipe n'est pas familière avec le code source du projet, il est plutôt habituel de voir des chiffrages élevés et que des _stories_ explosent ou voient apparaître des anomalies. C'est ce qu'il se passe quand vous n'êtes familier avec les lieux.

Mais quoi qu'il en soit, la taille d'un point de _story_ n'est pas vraiment significatif — c'est une supposition, quelque chose par laquelle commencer, et sa "vraie taille" ne sera vraiment connue que lorsqu'elle sera terminée, mais elle est aussi variable. C'est une unité de mesure sans unité, une espèce de non-sens que les gens trouvent parfois utile pour planifier la capacité à faire.

C'est souvent quelque chose de mal utilisé. Une alternative possible est d'[arrêter d'utiliser les points de _story_](https://www.industriallogic.com/blog/stop-using-story-points/).

Je vous revois pour la [2ème partie](http://www.les-traducteurs-agiles.org/2019/01/29/questions-reponses-a-propos-de-la-velocite-2eme-partie.html).

[^1]: le nom du site de l'auteur est Otter en anglais ou loutre en français et c'est aussi le surnom de l'auteur ;) - NdT

---
Auteur : [Tim Ottinger](https://plus.google.com/+TimOttinger)  
Source : [Q&A on Velocity, Part I](https://agileotter.blogspot.com/2018/07/q-on-velocity-part-i.html)  
Date de parution originale : 17 Juillet 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 01/01/2019  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

---
layout: post
title:  "Questions/Réponses à propos de la vélocité - 7ème partie"
date:   2020-04-15 00:00
published: true
tags:
- vélocité
---

Nous avons discuté dans la [6ème partie](http://www.les-traducteurs-agiles.org/2020/03/26/questions-reponses-a-propos-de-la-velocite-6eme-partie.html) des faux goulots d'étranglements et des reproches pouvant en être faits. Ces derniers sont souvent le résultat d'attentes non satisfaites, un phénomène que nous avons évoqué la dernière fois.

Reprenons la discussion à partir là :

> A : Je veux une vélocité de 30. Arrêtez de m'embrouiller et dites-moi comment y arriver.  
> B : Vous savez qu'un sprint de 19 points signifie qu'un point représente 1/19ème d'un sprint ?  
> A : Oui, je m'en rappelle très bien.  
> B : Si vous voulez des fonctionnalités qui représentent 1/30 d'un sprint, faitesen sorte qu'elles représentent 1/30ème de sprint au niveau de leur taille et de leur périmètre.

La personne A devient de plus en plus impatiente. Même si la question posée semble être très simple (comment augmenter la vélocité), le personne B semble esquiver en discutant des dynamiques humaines et systémiques, des méthodes d'estimation, et de la futilité d'améliorer la vitesse en changeant les unités d'estimation.  

Plutôt que d'aider A à bâtir un plan et un calendrier satisfaisant, B semble faire des ronds de jambe et semble dire que les plans et les calendriers ne sont ni importants ni réalistes. En bref, B n'est d'aucune aide (du moins du point de vue de A).

D'un autre côté, B est tout à fait conscient que A ne pose pas les bonnes questions. A est beaucoup trop focalisé sur l'utilisation des salariés, à vouloir faire correspondre la réalité à ses attentes, et sur la déconnexion des salariés au fait de respecter leurs promesses. Les bonnes questions commencent seulement maintenant à émerger.

B suggère à A que chaque semaine, qu'à peu de choses près, la même quantité de travail sera réalisée. Si vous voulez dénombrez plus de choses comme étant terminé, vous devez alors terminer plein de petites choses. Si vous voulez avoir terminé des choses de taille plus grande, vous devez en faire moins. Le périmètre du rectangle reste à peu près la même qu'il fasse 1x6 ou 2x3.

Dans la [2ème partie](http://www.les-traducteurs-agiles.org/2019/01/29/questions-reponses-a-propos-de-la-velocite-2eme-partie.html), B a voulu parler des manières d'accroître la zone de productivité du rectangle, en rendant plus facile l'exécution du travail. Cela, toutefois, a été esquivé par A dans la [4ème partie](http://www.les-traducteurs-agiles.org/2019/05/26/questions-reponses-a-propos-de-la-velocite-4eme-partie.html) car A voulait augmenter la quantité d'efforts à fournir plutôt que décroître la quantité exigée.

A continue à chercher une manière de faire grimper l'intensité pour un impact immédiat alors que B continue toujours de discuter sur le fait de travailler avec une plus grande régularité en vue d'obtenir un impact plus soutenable.

[![Vidéo Simon Sinek - Intensité vs Régularité]({{ site.url }}assets/tim_ottinger/miniature-video.png)](https://www.youtube.com/watch?v=y5OV3RmXhbg&hl=es&cc_lang_pref=fr%3Fcc_load_policy)  
_cliquez directement sur l'image pour lancer la vidéo sous-titrée en français directement sur Youtube_

À ce titre, B suggère de travailler à la manière d'un ["squelette qui marche", également connu sous la dénomination des "fines tranches verticales"](https://www.industriallogic.com/blog/evolution-cupcakes-and-skeletons/). Cette démarche permet de pouvoir achever des choses plus souvent, sur davantage d'éléments et de donner aux managers le pouvoir de décider lorsqu'une fonctionnalité est « suffisamment terminée ».

![Tweet Kent Beck]({{ site.url }}assets/tim_ottinger/Tweet-KentBeck-fr.png)

Voici la façon de faire agile de travailler, de petits morceaux bouts livrables individuellement (si cela est souhaité) et qui, tous ensemble, seront utiles à la fin aux utilisateurs finaux.

Chaque fonctionnalité pourrait atteindre ainsi le point d'équilibre des 20% de la loi de Pareto -- c'est-à-dire les 20% offrant 80% de la valeur de la fonctionnalité - à partir duquel il n'est plus tout aussi important d'en continuer le développement. Peut être qu'il y a une autre fonctionnalité qui est devenue plus importante sur laquelle il faut travailler et qui par conséquent rend caduque les 80% restant.

C'est bien ce que veut dire ce [principe du manifeste agile](https://agilemanifesto.org/iso/fr/principles.html) « La simplicité – c’est-à-dire l’art de minimiser la quantité de travail inutile – est essentielle. ». En faisant moins pour chaque fonctionnalité, nous obtenons plus de fonctionnalités « terminées ». En faisant moins, nous accomplissons davantage. En prenant en charge de plus petites unités de travail, nous terminons plus d'unités de travail.

L'hypothèse que les choses seront faites en intégralité parce qu'elles ont été imaginées et conçues dans leur ensemble, c'est bien ça ? C'est une idée non-agile. Il est très probable qu'une version « moindre » qui soit tout aussi satisfaisante puisse être fournie. Non seulement c'est vrai, mais avoir aussi une version « moindre » peut donner aux utilisateurs de la visibilité sur comment la fonctionnalité devrait se comporter en réalité -- une visibilité qu'ils n'avaient pas lorsqu'ils étaient au niveau de la base du cône d'incertitude[^1].  

L'informatique à tendance à travailler sur des [problèmes tordus (vo)](https://www.wickedproblems.com/1_wicked_problems.php) où apporter une solution à un problème change la nature du problème et où les problèmes s'entremêlent les uns aux autres. Dans ces conditions, avoir des _feedbacks_ rapides permet d'orienter les produits dans un certain sens là où le fait de travailler plus dur ne le fait pas.

> A : Ce serait donc alors de très petites fonctionnalités.  
> B : Oui.

Nous commençons à voir ici, nous l'espérons, une lumière commencer à apparaître, où A reconnait que B n'augmente pas la vitesse à laquelle l'équipe passe à dépiler le _backlog_, mais qui essayent à nouveau de faire face à la vitesse à laquelle les choses sont faites. La personne A rejette cette petite diversion à nouveau.  

> A : Mais je veux faire des choses ayant une taille importante.  
> B : Alors vous en ferez moins pendant un certain temps  
> A : Pourquoi ne puis-je pas avoir plus choses de taille plus importante terminées par itération ?  
> B : Combien peut-on mettre de litres dans un récipient de 15 litres ?  

Rejoignez-nous, A, B et moi-même dans la [8ème partie](http://www.les-traducteurs-agiles.org/2020/03/26/questions-reponses-a-propos-de-la-velocite-8eme-partie.html)

[^1]: NdT - Pour en savoir plus sur le cône d'incertitude : [http://www.les-traducteurs-agiles.org/2013/10/15/contrats-agiles.html](http://www.les-traducteurs-agiles.org/2013/10/15/contrats-agiles.html)

---
Auteur : Tim Ottinger  
Source : [Q and A on Velocity, part VII](http://agileotter.blogspot.com/2018/11/q-and-on-velocity-part-vii.html)  
Date de parution originale : 05 Novembre 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 15/04/2020  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

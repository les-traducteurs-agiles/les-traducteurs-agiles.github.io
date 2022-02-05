---
layout: post
title:  "Tester dans le sprint"
date:   2015-03-28 22:00
tags:
- test
- sprint
- scrum
---

Jeff Sutherland a dit aujourd'hui que ce n'est pas fini si ce n'est pas testé. Vous n'allez pas croire ce qui s'est passé par la suite !  

<div align="center">
  <img src="{{ site.url }}assets//tester_dans_le_sprint/sutherland-et-le-test.png" />
</div>

Jeff Sutherland est le créateur de Scrum. Depuis que je le connais, il a toujours dit que les pratiques à-la-XP sont nécessaires si les équipes Scrum qui élaborent les logiciels sont amenées à devenir, ce qu'il appelle, _hyper-productives_.  

Cet échange est typique : j'en vois et je participe à de semblables chaque jour. Paul Klipp affirme que si un gros problème survient, alors Scrum a échoué. Les gens adorent dire que Scrum a échoué, ou que Scrum devrait être [mourir sur un bûcher](http://ronjeffries.com/articles/2015-02-20-giles/). Eh bien, oui, et si l'on va dans ce sens, y compris chaque bonne idée qui aurait déjà échoué.  

La démocratie échoue lorsque des idiots ou des tyrans sont élus. La religion échoue lorsque des personnes font des mauvaises choses. La médecine échoue lorsque des gens ne prennent pas leurs médicaments. [Le baseball échoue](http://ronjeffries.com/xprog/articles/jatbaseball/) lorsque des personnes n'apprécient de jouer avec des chaussettes remplies de papier avec des bâtons trouvés par terre.  

C'est amusant de dire ce genre de choses. Et, à mon avis, c'est aussi d'une grande lâcheté. Il existe beaucoup de raisons expliquant pourquoi "Scrum ne marche pas", mais la question la plus importante est pourquoi ce qu'une équipe fait ne fonctionne pas. Il y a beaucoup de raisons, et généralement Scrum n'est pas l'une d'entre elles.  

Scrum est basé sur un principe très simple et très strict : inspecter et adapter. Cette idée a également d'autres noms, et comme Dave Snowden nous l'indique dans son [modèle Cynefin](http://cognitive-edge.com/), l'idée doit être appliquée différemment selon la situation. Mais toutes descendent du fait de regarder ce qu'il se passe, et de changer ce que nous faisons pour essayer de faire mieux.  

Passons en revue quelques points.  

Scrum ne dit pas " vous devez tester votre code dans un Sprint". Que dit-il ? Scrum dit qu'à la fin de chaque Sprint vous devez produire un incrément du produit. En ce qui concerne l'incrément :  

> L'incrément est la somme de l'ensemble des items du Product Backlog réalisés pendant un Sprint et de la valeur des incréments des Sprints précédents. À la fin d'un Sprint, le nouvel incrément doit être "fini", ce qui signifie qu'il doit être en condition opérationnelle et correspondre à la définition de "fini" de l'équipe Scrum. Il doit être utilisable que le Product Owner décide ou pas de le livrer réellement. ([Scrum Guide](http://www.scrumguides.org/scrum-guide.html)).  

Notez bien cette dernière phrase :  

> [L'incrément] doit être utilisable que le Product Owner décide ou pas de le livrer réellement.  

De plus, à la Définition de Fini, nous trouvons "tester à fond", ce qui implique peu ou prou cela :  

> Chaque Incrément est le complément de l'ensemble des incréments précédents et il est testé à fond, ceci afin d'être certain que tous les incréments fonctionnent ensemble.  

    L'incrément du produit doit fonctionner.

Il me semble que Scrum est plutôt clair là-dessus : à chaque Sprint, vous devez livrer un incrément d'un produit qui est testé, qui fonctionne réellement et qui peut être utilisé. Si nous ne faisons pas cela, nous ne suivons pas le conseil de Scrum. Et Scrum n'est pas du tout vague sur ce sujet. Vous ne pouvez pas prétendre que vous n'aviez pas remarqué que l'incrément devait être utilisable.  

    Les logiciels non testés ne fonctionnent pas.

Regardons les choses en face : un logiciel non testé ne fonctionne pas. Même si, par chance, il devait fonctionner, sans tester, nous ne pouvons pas être certain qu'il fonctionne. Si nous ne savons pas s'il fonctionne, nous ne pouvons pas certifier qu'il est utilisable. Donc, nous devons le tester. Le professeur Brehm avait pour habitude de nous dire “Punkt. Schluß. Neuer Absatz.” Et Papa avait pour habitude de dire : "Tout a été dit."  

# Rétrospective de Sprint

    Eh les gars ! Nous n'avons pas d'incrément du produit !
    Qu'est-ce qu'il se passe ?  

Supposons maintenant, que notre équipe Scrum soit joyeusement en train de ne pas produire un incrément utilisable du produit. Nous devons vraiment en prendre conscience : l'incrément est l'un des trois artéfacts obligatoires de Scrum, et il s'agit du plus important. Nous ne faisons pas ce que nous avions prévu de faire. C'est peu probable qu'il y ait quelque chose de plus important. Tout en haut de la liste des perversions devrait  simplement figurer "Pas de produit opérationnel".  

Scrum dit d'inspecter et d'adapter notre processus pour l'améliorer. Voici une amélioration cruciale qui est nécessaire. Que faisons-nous ?  

Eh bien, c'est évident, n'est-ce pas ? Nous décidons que pour nous un incrément opérationnel d'un produit n'est vraiment pratique, et comme il s'agit avant tout d'être pratique, nous laissons tomber cette exigence centrale de notre version de Scrum. Nous inspectons et adaptons cela en ne faisant pas de Scrum.  

Désolé, l'équipe, nous avons celui-là. Le conseil de Scrum est clair : produire un incrément opérationnel du produit. Pour savoir s'il fonctionne, nous devons le tester. Scrum rends ce problème visible et nous décidons de ne rien en faire. Cela vient de nous, pas de Scrum.  

# Ne pas faire du Scrum

Ainsi, d'un côté, si nous ne testons pas dans un Sprint, nous ne pouvons pas savons pas si l'incrément fonctionne, donc nous ne pouvons pas livrer un incrément opérationnel, et par conséquent nous ne faisons pas de Scrum. (Nous nous préparons aussi à échouer, mais cela nous le découvrirons bientôt.)  

Et c'est maintenant où nous sortons notre "Ce n'est pas un vrai écossais" ( [expression](http://en.wikipedia.org/wiki/No_true_Scotsman) exprimant une idée fausse - NdT) parmi d'autres excuses faisant paraître crédible que notre soi-disant projet Scrum n'ait pas livré un incrément opérationnel à chaque Sprint et ce n'est pas notre faute. Ouaaais. C'est la faute de Scrum !  

À quoi nous attendions-nous ? Que l'Inquisition de Scrum viendrait fondre sur nous dans leurs habits rouges et nous ferait passer cul par-dessus tête au sujet de notre incrément ? Même s'ils ne se montraient pas, nous aurions ressorti notre excuse : "Cela ne fonctionne pas pour nous. Notre situation est spéciale.".  

Eh bien, si l'Inquisition de Scrum s'était montrée dans leurs chouettes habits rouges, nous aurions pu mettre de faux badges du mérites Scrum sur nos chemises et retirer notre banderole "Cela fait 221 jours que nous n'avons pas fait de Scrum". Cela fait zéro jour de Scrum. Zéro !  

# Qu'est-ce que "Scrum" a fait pour rendre ceci clair ?

    Chaque projet a le Scrum qu'il mérite - non ~ Joseph de Maistre

Alors que je pense que nous avons le projet que nous méritons, en choisissant quoi faire (ou bien alors où aller travailler) je crois aussi que la communauté Scrum (quoi qu'elle puisse être) a une réelle responsabilité pour aider les gens à réussir avec Scrum. Ce travail n'a pas été fait parfaitement, et ne le sera jamais. Je suis enclin à dire qu'il pourrait être mieux fait, mais qu'il y a de nombreuses preuves qui indique que tester est central chez Scrum.  

* Jeff Sutherland, créateur de Scrum, a répété constamment que les pratiques à-la-XP, y compris tester, sont nécessaires pour réussir.
* La page sur les fondamentaux de Scrum de la Scrum Alliance indique que l'incrément doit être testé complètement.
* Le célèbre "Test ScrumButt" dit explicitement que les fonctionnalités doivent être testées et doivent fonctionner à la fin d'un Sprint.
* La Scrum Alliance offre son programme de développeur certifié scrum, enseignant aux équipes de développements les compétences nécessaires derrière la livraison d'un incrément de produit à chaque sprint.
* Beaucoup d'auteurs Scrum soulignent dans leurs écrits qu'une solide pratique technique est requise afin de livrer un incrément
* Beaucoup d'enseignants Scrum insistent aussi sur le besoin de pratiques techniques y compris le test.
* Beaucoup d'auteurs agiles et de coachs font les mêmes remarques, et offrent ces mêmes enseignements.

# Que devrions-nous faire de plus ?

Lorsque j'ai commencé cet article, je pensais parler de l'insistance constante de Jeff et les autres, puis le sujet devint plus abstrait et il était nécessaire de plus y travailler. Toutefois, il suffit que je regarde où que ce soit pour que je trouve des références explicites aux tests dans le sprint.  

Est-ce que tester pourrait être plus souligné ? C'est certain. Il devrait l'être au prix d'autre chose, bien sûr, mais on pourrait en dire plus. Si Jeff a raison en disant qu'il s'agit d'un des plus gros problèmes dans l'agilité, il faudrait sûrement insister plus. En même temps, je ne suis pas vraiment certain de ce qu'il "faudrait" faire.  

(Épargnez-moi les inévitables polémiques sur comment se fait-il que les scrum masters certifiés n'en savent pas assez sur ce sujet et que la certification est une arnaque, et ainsi de suite. La question a déjà été posée et répondue). Oui, il y a des problèmes. Les gens doivent en savoir plus. Tout le monde dans le domaine "Agile" travaille dur pour aider les personnes à comprendre ce qu'il faut faire et comment le faire.  

Revenons-en à nos moutons. Tout d'abord, qu'est que vous pourriez faire qui serait utile ? Je dirais qu'il n'est pas utile de faire sa petite rengaine cynique "Hahaha, vous voyez ? Scrum échoue". Même si c'était vrai, cela ne serait pas utile. Être utile serait de dire des choses comme "Tester est une partie vitale de Scrum. Vous ne pouvez pas faire de bon scrum sans cela.". Être utile serait d'écrire des articles sur comment tester dans un contexte agile, ou comment tester peut améliorer votre situation. Des choses comme cela.  

Aidez à rendre le monde meilleur. Offrez de meilleures idées, et pas des dénigrements aux bonnes idées. Est-ce que vous avez des idées qui pourraient aider ? Mettez-les sur la table. Vous pourriez même m'écrire une note avec vos suggestions.  

# TL;PL

Scrum dit que l'incrément doit être testé. Il l'a toujours dit. Oui, la communauté Scrum/Agile pourraient le dire plus et pourraient le dire plus fort. Mais il n'y a aucune excuse d'ignorer notre conseil, et pas plus d'excuse de ne pas tester dans chaque sprint.  


---
Auteur : [Ron Jeffries](http://ronjeffries.com/about.html)  
Source : [Testing inside the Sprint](http://ronjeffries.com/articles/2015-03-01-testing-in-sprints/)  
Date de parution originale : 1 mars 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 27/03/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

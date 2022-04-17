---
layout: post
title:  "Probablement tort"
date:   2022-03-30 00:01
published: true
tags:
- agile
- tdd
- scrum
---

> On pourrait croire que les développeurs savent qu'ils peuvent commettre des erreurs. Toutefois, nous avons tendance à avoir des opinions bien arrêtées bien plus que nous ne devrions en avoir. Du moins c'est mon avis.

Mon article le plus célèbre est sans doute : [Nous avons essayé le baseball et ça n'a pas marché](http://www.les-traducteurs-agiles.org/2022/03/21/nous-avons-essaye-le-baseball-et-ca-n-a-pas-marche.html).

Revenez quand vous l'aurez lu.

Heureux de vous retrouver. L'autre jour, j'ai entendu l'un de mes collègues grommeler sur le fait que dans la plupart des conversations, on finit par tomber sur quelqu'un qui va dire quelque chose du genre « Le développement orienté-objet a échoué » ou « le développement piloté par les tests a échoué » ou « Scrum a échoué ». J'ai alors répondu à son tweet par :

> Je connais la source de mes échecs, et il ne s'agit pas d'un paradigme ou d'un processus. Vous pouvez me citer.

Il m'est déjà arrivé par le passé d'avoir à vivre de mauvaises choses. Il m'a toujours semblé qu'il est possible d'accepter qu'il puisse arriver de temps en temps de mauvaises choses à des gens bien et de passer à autre chose, réconforté par le fait qu'il ou elle aille bien, ou qu'il est possible d'examiner les choses que l'on vient de faire pour voir si l'une d'entre elles a pu provoquer une mauvaise chose, ou s'il pourrait y avoir des choses à faire dans le futur qui pourrait diminuer les probabilités que ces mauvaises choses se reproduisent.

Ma propre personnalité a évolué de telle manière qu'elle me laisse plus encline à réfléchir et à agir comme si j'avais une influence substantielle sur ce qui a pu m'arriver et elle me pousse à essayer d'apprendre de nouvelles manières d'agir qui auront tendance à m'amener davantage de bonnes choses et moins de mauvaises choses.

Cela ne veut pas dire que je crois que nous pouvons tout contrôler. Tout au contraire, je pense que la vie est plutôt comme un radeau pneumatique, qui descend la rivière Youghiogheny à Ohiopyle en Pennsylvanie. Vous avez de grandes chances d'aller là où la rivière veut que vous alliez.

Et pourtant. Et pourtant. Vous trouverez que malgré tout votre pagayage, vos efforts ne vous conduiront certainement pas là où vous voulez aller, même si vous pouvez avoir une influence sur ce qui arrive et souvent de manière assez forte. Vous pouvez probablement faire en sorte d'éviter de chavirer. Vous pouvez presque toujours faire en sorte de garder l'avant du radeau dans le sens du courant.

Et alors … et alors … vos yeux tombent sur les guides assis dans leurs kayaks, immobiles sur l'eau, semblant à peine toucher l'eau avec leurs pagaies. Ils semblent à peine perturbés par cette même rivière qui manque de vous faire chavirer à chaque instant.

Sur l'eau, la manière dont vous pagayez est importante. Le type de bateau que vous avez est important. Oh, vous arrivez à suivre probablement le courant de la rivière et de temps en temps, vous vous retrouverez à l'eau, et vous pouvez être certain que vous serez complètement trempé. Mais la manière dont vous pagayez est importante.

## Qu'est-ce que cela à avoir avec le reste ?

Eh bien, la première chose, sur laquelle j'ai commencé à travailler, c'est l'attitude. Je choisis de me comporter comme si j'avais de l'influence sur ce qui m'arrive. Donc lorsque je fais face à un échec[^1], je regarde où est-ce que dans le passé j'ai pu faire fausse route, et je regarde vers l'avenir pour voir ce que je pourrais mieux faire la prochaine fois.

Je suppose que ce que je fais fait la différence. Il ne m'est pas possible d'imaginer vivre autrement, que ce que je fais n'ai pas d'importance. Ce serait horrible.

Passons un peu à de la programmation.

## Le TDD (développement piloté par les tests) a échoué

Qu'est-ce que cela peut bien vouloir dire ? Je suppose que nous devrions examiner les promesses de TDD. En réfléchissant, je pense que cela devrait donner quelque chose comme :

> (l'utilisation de) TDD mène à une conception simple et à un haut niveau de confiance sur ce que le programme fait par rapport à ce que nous nous attendons qu'il fasse.

Je ne pense pas que nous n'ayons jamais dit que TDD allait éliminer toutes les anomalies, même si certaines équipes ont réduit leur taux d'introduction d'anomalies de l'ordre d'un facteur deux en utilisant le TDD ainsi que d'autres types de pratiques.

Je ne pense pas que nous n'ayons jamais dit que TDD vous garantirait une conception parfaite, voire satisfaisante, même si lorsque vous regardez un expert en TDD produire du logiciel, il peut produire des conceptions d'une étonnante simplicité.

Je ne pense pas que nous n'ayons jamais dit que TDD garantirait quoi que ce soit, même si nous avons tendance à faire preuve d'enthousiasme sur les résultats que nous arrivons à obtenir avec.

Et je suis certain que nous n'avons jamais dit que TDD puisse être utilisé comme ça sans réfléchir tout en espérant en retirer un quelconque bénéfice.

Toutefois, supposons que le bien-nommé Alex Coder essaye le TDD et n'arrive pas à aboutir à une conception simple, et qu'il n'a pas une grande confiance dans le code produit. Supposons alors qu'Alex dise « TDD a échoué. Je ne suis pas arrivé pas à obtenir une conception simple et un grand niveau de confiance dans le programme produit. En fait, le programme fait en TDD s'est avéré vraiment hideux et truffé d'anomalies. »

Je pense que si nous devions poser à Alex quelques questions supplémentaires, nous obtiendrions quelques réponses intéressantes. Par exemple, si nous devions poser la question: Est-ce qu'il est facile ou difficile d'écrire des tests ? Je parierais qu'Alex nous dirait que c'était difficile, voire souvent très difficile. Si nous devions poser la question à quelle fréquence les tests changeaient, Alex nous répondrait très vraisemblablement qu'il devait changer les tests très souvent, à tel point que faire en sorte de continuer à faire tourner les tests lui générait plus de travail que le vrai programme.

Nous serions aussi tentés de lui rétorquer assez cruellement « Vous utilisez mal le TDD ». Bien assez vite, quelqu'un rétorquera « Aucun vrai écossais ! » ([expression](http://en.wikipedia.org/wiki/No_true_Scotsman) exprimant une idée fausse - NdT).

Qui a raison ? Qui a tort ? Eh bien, oui. Lorsque je pense au TDD, j'en suis venu à croire ce qui suit :

> TDD fonctionne très bien dès lors le développeur privilégie l'utilisation d'objets et de méthodes cohésives de petite taille, de telle sorte que la plupart des fonctions soient bien isolées et indépendantes. Et TDD fonctionne particulièrement bien lorsque les objets sont immutables, ou que les changements d'état sont petits et discrets. Le TDD fonctionne bien avec un style de développement du type « faites, ne posez pas de questions ».
>
> Le TDD ne fonctionne pas bien lorsque le développeur privilégie les fonctions en série qui racontent toute une histoire et en détail. TDD ne fonctionne pas bien lorsque les objets changent d'état souvent. TDD ne fonctionne pas si bien que ça avec des objets de taille importante ayant plusieurs membres changeant de manière indépendante.

Maintenant, il est « bien connu » que des objets, des procédures cohésifs de petite taille sont « mieux » que de longues méthodes et des objets massifs qui combinent tout ce qu'il y a besoin de savoir sur l'univers. Par « bien connu », je veux dire quelque chose d'un peu mieux que « Eh bien, Ron et Kent aime ça », mais certainement moins bien que « personne ne peut réussir avec des objets de grande taille et du code procédural ».

En sortant le jugement de valeur de l'équation, je voudrais dire que le TDD fonctionne bien avec des objets peu connectés, très cohésifs et des fonctions de petite taille, et non avec des objets qui ont une faible cohésion et un fort couplage, ni avec des fonctions de grande taille.

Est-ce que TDD « échoue » dans ces circonstances ? Je ne sais pas. Est-ce qu'un marteau échoue lorsque vous essayez de visser une vis avec ?

## OO (la programmation orientée objet) a échoué

Nous allons pouvoir passer plus rapidement l'OO. À quel moment la programmation orientée objet échoue-t-elle ?

La programmation orientée objet ne vous apportera pas grand-chose si vous préférez avoir une seule énorme classe contenant l'ensemble des données à gérer, et que le code qui doit manipuler ces données est dans une seule méthode géante.

Assez curieusement, les circonstances dans lesquelles l'OO fonctionne le mieux sont les mêmes que pour le TDD : c'est-à-dire lorsque le code que vous écrivez est très modulaire, très cohésif, avec des fonctions et des objets de petite taille.

Est-ce que la programmation orientée objet échoue lorsque vous préférez utiliser de grosses fonctions exploitant d'énormes blobs de données ? Est-ce qu'une débroussailleuse  échoue lorsque vous essayez de couper un chêne avec ?

## Scrum a échoué

Lorsque quelqu'un dit « Scrum a échoué », nous avons besoin de davantage d'informations. De quelle manière Scrum a-t-il pu « échouer » ?

- Est-ce que votre projet n'est pas arrivé dans les délais et dans le budget impartis ?
- Est-ce que vous n'avez pas accompli deux fois plus de travail en moitié moins de temps ?
- Est-ce que, dans votre rôle, vous avez haï Scrum ?

Scrum, si vous l'étudiez un tant soit peu, est assez explicite quant aux conditions nécessaires à sa mise en place. Cela commence par les valeurs.

> Une utilisation réussie de Scrum repose sur la capacité des gens à mieux maîtriser et mieux incarner les 5 valeurs que sont :
> l'Engagement, la Focalisation, l'Ouverture, le Respect et le Courage

Si je devais me retrouver face à face à une soi-disant démarche Scrum où les gens n'incarnent pas ces valeurs, je serais enclin à prendre mon sifflet et à signaler un sérieux problème.

> Scrum demande que le « **Product Owner** » ajoute le travail par ordre de priorité dans une liste qui s'appelle un **Backlog**.

Par conséquent, si nous nous retrouvons face à une soi-disant démarche Scrum sans _Product Owner_, ou sans liste ordonnée de chose à faire, ou si la liste change quotidiennement, nous devons demander si c'est vraiment du Scrum ou pas.

Si les gens n'ont pas d'autres choix que de travailler dans ces conditions, nous devons leur suggérer que Scrum n'est pas quelque chose qu'ils devraient utiliser. Ce n'est même pas quelque chose d'_envisageable_.

> Scrum demande que l'Équipe Scrum sélectionne la quantité de travail à faire à chaque Sprint.

Si dans une soi-disant démarche Scrum nous trouvons quelqu'un qui dit à l'équipe ce sur quoi elle doit travailler et la quantité de travail à produire, ce n'est pas du tout Scrum.

Si c'est la manière dont vous gérez le travail, Scrum n'est pas pour vous. Vous ne pouvez pas faire du Scrum de cette manière.

> Scrum demande que l'équipe produise un incrément de code testé opérationnel à chaque Sprint.

Si dans une soi-disant réussite Scrum, l'équipe ne produit pas un logiciel opérationnel à chaque Sprint, je vous demande humblement pardon, mais elle ne fait pas du Scrum. La règle suivante s'applique : vous devez trouver ce qui ne fonctionne pas[^2] et le corriger.

Si vous êtes en train de faire de votre mieux sans construire un logiciel opérationnel à chaque Sprint, Scrum n'est pas pour vous. Vous ne pouvez pas faire du Scrum de cette manière.

> Scrum demande que l'équipe et les parties prenantes inspectent les résultats et ajustent la manière dont ils travaillent pour le prochain Sprint.

Si sur une soi-disant démarche Scrum, les mêmes problèmes se reproduisent _Sprint_ après _Sprint_ et que des changements effectifs ne sont pas mis en place pour résoudre les problèmes, il n'y a que deux possibilités.

La plus probable, c'est que les membres de l'équipe n'essayent pas vraiment de les corriger. Peut-être que l'équipe ne fait pas assez preuve d'ouverture, de respect, et de courage pour les amener au grand jour. Peut-être que quelqu'un aux responsabilités à demander aux personnes de simplement essayer de manière plus acharnée. D'une manière ou d'une autre, ils choisissent de ne pas les corriger.

Il est pour ainsi peu probable que les problèmes puissent être corrigés.

Dans tous les cas, Scrum a fait son boulot, c'est-à-dire identifier les problèmes. Que l'équipe choisisse de les corriger ou pas, ou simplement de ne pas les corriger. Le boulot de Scrum dans le cas présent est fait.

### Cela dit …

Je ne dis pas que Scrum est parfait. Je ne dis même pas qu'il est bien. Je dis simplement qu'il est tout à fait explicite sur ce qu'il exige de vous à faire, et sur ce qu'il promet[^3], c'est-à-dire d'identifier les problèmes que vous devez résoudre.

Si vous faites Scrum de manière adéquate, je pense que vous êtes susceptible d'en tirer quelque chose. Et si vous faites mieux que l'utiliser de manière adéquate, je pense que vous évoluerez bien au-delà de ça et vers quelque chose de mieux.

## En résumé

En tant que développeur logiciel, vous devriez savoir que vous avez assez souvent tort. En tant qu'être humain, vous devriez savoir que vous avez assez souvent tort.

Lorsque les choses ne vont pas dans votre sens, vous pouvez blâmer l'OO, ou TDD, ou Scrum, ou vous pouvez penser sur ce qu'il se passe et voir si vous pouvez vous débrouiller ou pagayer autrement. Et peut-être même que vous aurez besoin d'un nouveau bateau.

Ou simplement vous laissez porter par le courant. C'est quelque chose de tout à fait correct. C'est votre[^4] choix.

[^1]: Je devrais dire « Lorsque j'échoue », mais j'essaie d'être diplomate, et d'amener à moi les lecteurs qui n'ont personnellement jamais échoué, mais qui ont seulement « rencontré l'échec ».

[^2]: De manière assez curieuse, une partie de ce qui ne va pas est lié au fait que probablement ils ne font pas du TDD, de _refactoring_, ou d'autres pratiques d'eXtreme Programming (XP) qui semblent tout à fait nécessaires pour faire du développement itératif et incrémental.

[^3]: À l'exception de cet odieux « faire deux fois plus de travail en moitié moins de temps ». Oui, si vous avez une équipe ordinaire et que vous faites du Scrum correctement, vous obtiendrez très probablement une meilleure productivité. Mais ce titre … c'est [donner des lames de rasoir à des bébés (VO)](https://ronjeffries.com/categories/razor-blades/)

[^4]: Comme la plupart des lecteurs réguliers de ce blog le savent, j'utilise rarement le « tu/vous », je préfère le « nous ». Ici le « tu/vous » me semble nécessaire. Je vous prie de m'excuser si cela … hum … vous ennuie.

---
Auteur : [Ron Jeffries](https://ronjeffries.com/about.html)  
Source : [Probably Wrong](https://ronjeffries.com/articles/-z022/0222ff/probably-wrong/)  
Date de parution originale : 14 Mars 2022  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 30/03/2022  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

---
layout: post
title:  "Le dernier moment responsable reconsidéré"
date:   2016-09-28 00:00:01
published: true
categories: 
- lean
---

>**Avant-propos du traducteur** : pour les lectrices et lecteurs les moins averti(e)s par rapport au concept du dernier moment responsable, nous vous proposons de lire au préalable notre traduction de l’article [le dernier moment responsable](http://www.les-traducteurs-agiles.org/lean/2016/06/28/le-dernier-moment-responsable.html) de Jeff Atwood (il est assez court, je vous rassure) qui vous permettra d’avoir des éléments d’informations pour comprendre et apprécier la présente traduction. 

Il est une phrase qui est citée de nos jours par beaucoup de concepteurs comme d’une espèce de recommandation en matière de gestion de projet :  “Décider au dernier moment responsable”.  Cela sonne bien, c’est marquant, mais est-elle de bon conseil ? 

J’ai décidé d’y regarder de plus près pour voir ce que cette phrase signifie vraiment et voir s’il s’agit vraiment d’un bon conseil.

En bref, il ne s’agit pas d’un bon conseil, en fait il ne s’agit même pas d’une phrase ayant du sens ; ce qui est encore pire, c’est que si celle-ci avait une quelconque signification, elle n’est pas actionnable ; et s’elle était actionnable, alors il ne s’agirait pas un bon conseil.

… vous êtes sceptique ? Poursuivez donc votre lecture, cher lecteur, et voyons ce que vous en penserez à la fin …

Mes partenaires dans cette étude sont les consultants de CRISP de Stockholm, les participants de mon [cours avancé Agile](http://alistair.cockburn.us/Advanced+Agile+class), et les personnes du [groupe de discussion agile de Salt Lake City](http://alistair.cockburn.us/Salt+Lake+City+agile+round+table+protocol) (c’est ce dernier groupe qui m’a donné bien sûr le plus de fil à retordre). Tous, avaient pris comme position que le DMR (Dernier Moment Responssable) est de bon conseil, ou du moins un bon heuristique.

Tout d’abord, cette expression n’a aucune signification. Pour être significative, nous devrions avoir un “moment” qui soit le “dernier” de quelque chose. Mais “responsable” — dans presque toutes les situations auxquelles vous pourriez penser — n’est pas une fonction [^1] connaissant un changement brusque. Sa pente est légère. Il y a des moments où choisir entre A et B est de toute évidence “responsable” (je vous laisserai même décider de la signification de ça) puis il y a un moment lorsque quelqu’un a annoncé que c’est le dernier moment responsable, où en réalité il ne le soit pas — il s’agit juste d’un moment que quelqu’un a annoncé. Le coût réel de retarder ou de revoir une décision se déplace légèrement vers le haut jusqu’à un certain moment, qui est clairement “hasardeux”, “coûteux” ou, pour garder un langage métaphorique, “irresponsable”.

Mais il n’existe pas de “dernier” de ces moments, seulement un déplacement léger et approximatif des coûts. Donc il n’existe pas de “dernier moment responsable” — cette phrase est simplement de la fiction.

Deuxièmement, elle n’est pas actionnable. Je veux dire par là que vous ne pouvez pas l’appliquer. Vous ne pouvez pas savoir lorsqu’arrive réellement ce dernier moment, si ce n’est qu’après, lorsqu’il est trop tard. Vous pouvez dire que vous l’avez raté, mais vous ne pouvez pas dire à l’avance quand est-ce qu’il arrivera. Donc vous ne pouvez pas vraiment appliquer ce conseil. Dans mon expérience le DMR est principalement utilisé pour atteindre quelqu’un en pleine tête lorsque vous souhaitez le blâmer pour ne pas avoir bien décidé. Bref, un mauvais outil.

Enfin, il ne s’agit pas vraiment d’un bon conseil. Si vous laissez toutes vos décisions ouvertes jusqu’à un DMR hypothétique, votre cerveau sera alors complètement encombré par ces décisions ouvertes et vous ne serez plus capable de toutes les suivre. Heureusement, beaucoup de décisions sont prises longtemps à l’avance, et vous n’aurez tout simplement plus à y penser après. Cela vous permet de bien dormir pendant la nuit — la décision a déjà été prise, et vous n’avez qu’à vivre avec les conséquences. D’autres décisions sont prises heureusement dans un “moment irresponsable à mi-chemin” — suffisamment tard pour avoir des conséquences fâcheuses, effrayantes ou avoir un certain coût, mais lorsque vous concluez finalement que (a) vous n’obtiendrez aucune information supplémentaire, et (b) que ce soit maintenant ou plus tard alors vous trouverez que le coût sera simplement trop élevé. Il ne s’agit donc pas du DMR, parce qu’il est profondément ancré dans le territoire effrayant/coûteux/ennuyeux.

Le DRM, s’il existe, se situerait à un point quelconque où la fonction coût commencerait à changer — suffisamment tard pour vous permettre d’obtenir plus d’information, suffisamment tôt pour vous permettre de clarifier la décision — là où il peut exister une espèce de sommet ou de point d’inflexion dans cette fonction coût complexe à plusieurs variables.

Voici les résultats j’ai eu des différents débats que nous avons eu :

1. Décider au plus tôt, puis dormir à poing fermé
2. Différer jusqu’à un certain point où le danger se fera sentir et viendra à menacer, pour obtenir plus d’information
3. Différer jusqu’à ce que vos alarmes personnelles “Danger ! Will Robinson” [^2] se déclenchent, et vous aurez donc le maximum d’information et au moins une chance décente pour mettre en œuvre celle de votre choix

… et derrière tout cela, il y a le concept des options réelles [^3], où vous payez tôt afin de ne pas avoir à décider du tout … Parler de la théorie des options réelles complique encore plus les choses.

Je vais continuer à écrire sur ce sujet, à ajouter des exemples, etc. mais pas aujourd’hui, je dois y aller maintenant.

Et vous, qu’en pensez-vous ?
Alistair

---

**Postscript 1**, quelques heures après, et après avoir trouvé des commentaires sympa ici et ailleurs sur Twitter : Karl Scotland et Chris Matts ont déjà commencé à descendre le long du chemin, Chris a écris le premier  [http://decision-coach.com/lean-and-real-options](http://decision-coach.com/lean-and-real-options), dans lequel il a écrit ces phrases très intéressantes :

> “Différer l’engagement” est une directive indiquant que l’engagement devrait être différer jusqu’au “dernier moment responsable”. Dans les options réelles, on ne dit pas autre chose (“Ne jamais vous engager trop tôt à moins que vous ne sachiez pourquoi”) par contre, vous pouvez vous engager de manière précoce si et seulement si vous avez l’information dont vous avez besoin pour prendre cet engagement. Bien que cela ne soit pas significatif, c’est quand même une nette amélioration par rapport à un “engagement différé” car cela nous oblige à trouver l’information qui nous permettra de prendre des engagements de manière anticipé. Prendre des engagements ainsi peut rendre les choses plus simples car nous n’aurons pas à gérer des options inutiles et que cela nous donne des informations dont nous avons désespérément besoin.

> Une des plus grandes différences entre le Développement logiciel lean et les options réelles est que lean parle du “Dernier Moment Responsable” alors que les options réelles parle de “l’expiration des options”. Le “DMR” devrait sembler aller de soi. Les défenseurs du lean parleront du “Point Optimal” pour prendre un engagement. L’“expiration des options” signifie qu’après un certain point, le moyen d’atteindre un objectif (ou une option) n’est plus disponible, il expire, ou meurt. Cet état de fait est déterminé par un processus clairement défini. Le problème avec le “DMR” est que, lorsque vous demandez à quelqu’un de différer un engagement, ou simplement de “différer l’engagement” jusqu’au “dernier moment responsable”, cela le plonge dans l’incertitude avec très peu de contrôle sur la situation.

puis Karl Scotland [http://availagility.co.uk/2010/04/06/defining-the-last-responsible-moment](http://availagility.co.uk/2010/04/06/defining-the-last-responsible-moment) écrivit

> Je définirai le Dernier Moment Responsable (DMR) en terme de coût du retard, tel qu’il est défini par Don Reinertsen, et de bénéfice du retard, un terme connexe employé conjointement avec Julian Everett lors d’un échange par messagerie électronique. En bref, le Dernier Moment Responsable intervient juste avant que le coût du retard ne dépasse le bénéfice du retard. Il n’est pas nécessaire d’être capable de quantifier les coût et bénéfices de manière très précise, toute évaluation étant meilleure qu’aucune !

Karl et Chris ont vraiment fait une superbe analyse, probablement meilleure que la mienne :) Je pense que le point de vue de Chris à prendre en compte concernant une prise de décision anticipée est la meilleure.

Je continue à ne pas aimer le terme “dernier” et je n’aime franchemant pas non plus le terme “responsable” , mais j’orienterai volontiers toute personne qui serait intéressée par prendre en considération les versions de Karl et de Chris. 

---

**Postscript 2**, hier, après la fin du tour de table, une personne a dit (à la surprise générale),

>”Les gars, vous rendez ça trop compliqué. C’est uniquement du bon sens — vous savez que vous vous ferez du mouron en attendant plus longtemps et vous savez que vous dormirez mieux en choisissant maintenant. Utilisez donc votre tête, bande de nazes.”

Merci Phil pour cette autre bonne réponse.

---

**Postscript 3**, l’exemple que j’utilise c’est la commande d’un déjeuner pour un groupe de stagiaires.

Au restaurant, il est indiqué : choisissez le menu 1 ou le menu 2 avant 10:30 pour le déjeuner de 12:30. Quand devons-nous demander aux personnes de faire leurs choix.

* A. Au moment où ils choisissent le stage
* B. Au début du stage le premier jour
* C. Au début de chaque journée de stage
* D. À 10:30
* E. À n’importe quelle moment entre 10:15 et 11:00
* F. À 11:00
* G. À 11:30
* H. À 12:30 lorsque nous arrivons pour déjeuner.

Le problème, c’est que les stagiaires peuvent être au milieu d’exercice ou d’une explication à 10:30.

Réfléchissez à quel pourrait être votre choix, et préparez vous à l’argumenter. Le DMR est, en théorie, 10:30, mais ce n’est pas vraiment un bon moment pour choisir. Personnellement je choisirai n’importe lequel des options C, E, F. E qui se rapproche le plus du DMR, tout en restant fidèle à mon avis sur le sujet : il n’y a pas de “moment” et il n’y a pas de “dernier”.

Le DMR reste à mes yeux une expression épouvantable, peu importe l’angle sous lequel je la regarde. À mon avis, la manière d’en parler de Chris Mattreste est celle ayant jusqu’à présent le plus de sens.

---

**Postscript 4**: Et nous avons continuer de débattre pendant le diner avec Cory Foy, Jonathan House et Ghennipher Weeks.

Cory introduisit l’idée du “goût du risque” pour parler des alarmes personnelles. Ghennipher rebondit sur cette idée, Jonathan exprima son désaccord. Après quelques échanges, je finis par conclure que la vision des courbes du risque et du coût permettent d’aborder de façons pseudo-scientifiques les peurs personnelles et les préférences risques/dégâts de chacun … ce qui conduit à l’idée que dans une équipe avertie, les membres discuteront explicitement de leurs goûts du risque respectifs, de leurs niveaux de peur, et apprendront à émettre des jugements sur le fait de savoir quand se prononcer pour prendre une décision basée sur leur compréhension respective des choses en question.

C’est un bel endroit pour s’asseoir et discuter — l’objet de notre discussion est de savoir si les gens deviennent conscients de leurs propres niveaux de risques/peur, s’ils les font partager aux autres, et s’ils prennent cela en compte dans leur prise de décision.

---

**Postscript 5**: Jonathan continue de maintenir que le DMR s’applique uniquement à un sous-ensemble de décisions et non à toutes les décisions.

Cet argument est tout à fait acceptable, sauf que maintenant nous avons de nouveaux problèmes : Quelles décisions ? Qu’est-ce que Responsable ? quel est le Dernier Moment ? Hmm, c’est bien pire qu’avant. 

---

**Postscript 6** : Dans la conversation, une personne (appelons-la A) ajouta “il s’agit du moment où vous avez tellement peur que vous pouvez presque sentir la pisse couler le long de votre jambe” (Bon d’accord, pendant la discussion, quelques bières sont passées par là). Un autre personne (appelons-la B) qui souhaite pour l’instant restée anonyme l’appelle le moment clé de négation de l’implémentation unique (vous êtes libre de changer tout ou partie des mots de cette phrase). La bande dessinée Calvin and Hobbes nous montre quelque chose qui s’en rapproche beaucoup : 
![À la dernière minute]({{ site.url }}assets/dernier_moment/ch_lm_panic_fr.png)

Je participe à cette discussion depuis 36 heures non-stop et je commence à être épuisé, mais je suis ravi d’avoir découvert beaucoup de choses. Le terme “Responsable” demeure à mon humble avis indéfinissable, le “Dernier … moment” n’existe
pas, donc le DMR reste un canular, mais aller au lit au bon moment pour BIEN DORMIR, aller aux toilettes au bon moment pour URINER a du sens, et il y a quelque chose d’intéressant sur la peur au niveau d’un groupe sur le bon moment (qui interagit avec la stratégie d’acquisition d’options réelles de Chris Matts, lorsque nous y regardons de plus près).
---

**Postscript 7** : Je joue désormais avec la notion de **périodes de temps où sont prises les décisions** plutôt qu’au les moments où sont pris les décisions, parce que je pense que le moment est un mauvais concept. Jusqu’à maintenant, il semble que tout soit lié à l’état émotionnel des personnes par rapport à la situation, rien qui soit objectif et utilisable. Donc cela donne en gros trois périodes comme ça :

* La période **Dormir tranquille** — prendre la décision maintenant et assumer toutes les conséquences qui s’ensuivront — J’en ai marre d’y penser et je ne veux plus continuer à me prendre la tête à ce sujet pour le reste de la journée.
* La période **être de plus en plus mal à l’aise** — les prises de décisions sont faites tardivement pour prendre en compte l’arrivée d’informations en continue — les décisions sont prises selon le “goût du risque” (merci Cory) et le niveau de peur acceptable des personnes.
* La période **en avoir des cauchemars** connu aussi sous le nom de “pisser dans mon pantalon” ou “connaître la panique à vous en tordre les boyaux” — vous vous retenez le plus longtemps possible jusqu’à ce qu’au moment critique où vous craquez et où vous décrochez le téléphone.

Que pensez-vous de l’utilisation de ces périodes de temps à la place des moments ?

Sans faire exprès, j’ai trouvé des noms bien meilleurs pour désigner ces 3 périodes :

* **Dormir tranquille**
* **Être de plus en plus mal à l’aise**
* **En avoir des cauchemars**

[^1]:Ici l’auteur prend comme métaphore, celle de la représentation graphique d’une fonction mathématique
[^2]:Phrase bien connue de la série Lost In Space - NdT
[^3]:Outil financier d’aide à la décision en matière d’investissement, voir cet [article](https://fr.wikipedia.org/wiki/Analyse_par_les_options_r%C3%A9elles) sur Wikipedia pour plus d’informations - NdT
---  
Auteur : [Alistair Cockburn](http://alistair.cockburn.us/)  
Source : [Last Responsible Moment Reconsidered](http://alistair.cockburn.us/Last+Responsible+Moment+reconsidered)  
Date de parution originale : 07 Octobre 2011  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 28/09/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}


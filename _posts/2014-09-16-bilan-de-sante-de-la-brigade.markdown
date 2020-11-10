---
layout: post
title:  "Bilan de santé de la brigade (modèle)"
date:   2014-09-16 00:01
published: true
tags:
- coaching
- dette technique
- équipe
---

![Vue générale du bilan de santé de la brigade]({{ site.url }}assets/henrik_kniberg/squad-health-check-model-overview.png)

(Téléchargez les cartes et les instructions en PDF (en [vo](https://spotifylabscom.files.wordpress.com/2014/09/squad-health-check-model2.pdf) et en [vf](https://www.dropbox.com/s/kljfbp9n22hnlmi/squad-health-check-model-fr.pdf?dl=0)) ou PPTX (en [vo](https://spotifylabscom.files.wordpress.com/2014/09/squad-health-check-model.pptx) et en [vf](https://www.dropbox.com/s/4j7as8ngxykg07i/squad-health-check-model-fr.pptx?dl=0))

## Qu'est-ce qu'un modèle de bilan de santé d'une brigade ?

Un grand nombre d'entreprises essayent de trouver des façons de mesurer et de visualiser comment s'y prennent leurs équipes. Ce qu'on appelle généralement des "modèles de maturité", et qui mettent en jeu une sorte de progression au travers de différents niveaux.

L'objectif de ce type de modèles est généralement bénin : ce sont par exemple des managers ou des coachs, présents dans de grandes organisations, qui souhaitent se faire une idée de là où ils devraient porter leurs efforts d'amélioration, repérer les problèmes systémiques, et aider les équipes à prendre davantage conscience de là où elles devraient également porter leurs efforts d'amélioration.

Nous préférons utiliser d'autres termes comme par exemple "le modèle du bilan de santé", car le terme "maturité" paraît un peu ... eh bien .... paternaliste. De plus, la plupart de nos modèles ne comportent pas de progression au travers de différents niveaux, sachant que le premier utilisateur concerné est l'équipe elle-même plutôt que le management.

Améliorer l'organisation ressemble plus à un jeu de devinettes (comment savez-vous ce qui doit être amélioré, et comment allez-vous savoir si ça s'améliore ?). Une approche systémique avec une visualisation claire peut aider à diminuer ce côté devinette.

## D'accord, mais est-ce que ce type de modèles fonctionne réellement ?

C'est variable. Parfois, un tel modèle peut être très utile. Parfois, c'est plus un "bof", les gens mènent consciencieusement des ateliers, des enquêtes, ... puis les données sont ignorées.

Attention quand même, dans certaines entreprises, nous avons vu des modèles de ce type devenir des monstres, des outils d'oppression systémique provoquant sous-optimisation et peur lorsque les managers utilisaient le "modèle de maturité" pour juger les équipes et les monter les unes contre les autres, les équipes cachant leurs problèmes pour faire illusion. Ce n'est pas génial !

Voici un camembert générique des "chances de succès" basé sur ce que nous avons constaté jusqu'à présent dans diverses entreprises :

![Chances de succès]({{ site.url }}assets/henrik_kniberg/chance-of-success.png)

Cependant, même si les dommages potentiels sont pires que les bénéfices potentiels, IL EXISTE un gain potentiel, et il existe des moyens pour éviter le scénario catastrophe.
Chez Spotify, nous avons mené des expérimentations rigoureuses pendant plusieurs années, et nous avons trouvé quelques moyens qui fonctionnent assez bien (plus de bénéfice que de douleur). Au mieux Utile (NdT : Helpful!), au pire Bof (NdT : meh...), et à ce jour jamais une Catastrophe (NdT : Disaster!). Nous avons aussi mis en place ce modèle de bilan de santé dans plusieurs autres sociétés et constaté des résultats similaires, et nous avons donc pensé qu'il était temps d'écrire un article :o)

## Pour qui est ce modèle de bilan de santé ?

Lors d'un bilan de santé d'une [brigade](https://labs.spotify.com/2014/03/27/spotify-engineering-culture-part-1/) (notre terme pour une petite équipe de développement auto-organisée et pluridisciplinaire), il ne subsistait plus que deux parties prenantes :

* **La brigade elle-même.** Tout en discutant des différents indicateurs de santé, la brigade prend progressivement conscience de ce qui fonctionne et de ce qui ne fonctionne pas. Le large éventail de questions aide à élargir leur point de vue. Peut-être étaient-ils bien au courant des problèmes de qualité du code, mais ils n'avaient pas vraiment réfléchi à la valeur perçue par le client, ou même à quelle vitesse ils apprenaient. Cela fournit également une vision équilibrée et objective des bonnes choses ainsi que des points de douleur.
* **Les personnes soutenant la brigade.** Les managers et les coachs qui travaillent à l'extérieur (ou en partie à l'extérieur) de la brigade, obtiennent une vue très synthétique de ce qui fonctionne ou non. Ils peuvent également voir apparaître des patterns entre plusieurs brigades. Si vous avez des dizaines d'équipes et que vous ne pouvez pas parler à tout le monde de tout, un résumé visuel vous aidera à comprendre où consacrer votre temps, et à qui en parler.

La première étape dans la résolution d'un problème est d'en être conscient. Et ce type de visualisation rend plus difficile pour tout le monde le fait d'ignorer le problème.

## Comment nous le faisons chez Spotify ?

Nous faisons trois choses de base :

1. Mener des **ateliers** dans lesquels les membres d'une brigade discutent et évaluent leur situation en se basant sur différents critères (qualité, plaisir, valeur, ...).
2. Créer un **résumé graphique** du résultat
3. Utiliser les données pour **aider les brigades** à s'améliorer

Nous avons plusieurs variantes, l'une est tout simplement appelée le "modèle de bilan de santé de la brigade", d'autres sont par exemple appelées "jeu facile@agile" et "réflexion trimestrielle" (peut-être de futurs sujets d'articles). Le modèle de bilan de santé est une version améliorée de l'ancienne enquête trimestrielle "brigades autonomes" mentionnée dans l'article de 2012 ["Agilité à grande échelle @ Spotify"](http://ayeba.wikispaces.com/Agilit%C3%A9%20%C3%A0%20grande%20%C3%A9chelle%20chez%20Spotify).

Voici un exemple réel de résultat d'un bilan de santé pour une tribu :

![Capture d’écran]({{ site.url }}assets/henrik_kniberg/screen-shot-2014-09-16-at-06-52-03.png)

Cela illustre la façon dont 7 brigades différentes d'une même tribu voient leur propre situation. La couleur est l'état actuel (vert = bon, jaune = quelques problèmes, rouge = très mauvais). La flèche montre la tendance (est-ce que cela s'améliore ou est-ce que ça se détériore ?).
Regardez ce graphique pendant une minute, et vous commencerez à voir des choses intéressantes :

* **Regardez chaque colonne,** et vous verrez des différences majeures entre les équipes. La brigade n°4 est contente sur à peu près tous les sujets. La brigade n°2 a beaucoup de problèmes, mais beaucoup de choses s'améliorent.
* **Regardez chaque ligne,** et vous verrez émerger des patterns systémiques. Chaque brigade est motivée (et est même en train d'améliorer les choses) ! La motivation est apparemment au beau fixe. Mais le processus de livraison est problématique, et le code source est globalement en mauvais état. Au fil du temps, cela aura probablement un impact négatif sur la Motivation.
* **Regardez le tableau d'ensemble,** et vous verrez que presque toutes les flèches sont orientées vers le haut, seules deux flèches sont orientées vers le bas dans le tableau d'ensemble. Cela signifie que le processus d'amélioration (le processus le plus important de tous) semble fonctionner.

Ceci, bien sûr, ne constitue qu'une approximation de la réalité ("tous les modèles sont faux, mais certains sont utiles" - George Box). Il vaut donc mieux vérifier deux fois les choses avant d'agir.

La brigade n°4 est-elle vraiment en si grande forme que cela, ou sont-ils juste optimistes et ils ne voient pas leurs propres problèmes ? La plupart des brigades pensent qu'elles livrent de la valeur à leurs clients, mais comment le savent-elles ? Est-ce fondé sur des vœux pieux ou sur les feedbacks de clients réels ?

Dans ce cas particulier, la brigade n°4 a effectivement été formée une semaine avant le bilan de santé et elle était vraiment dans une phase de constitution, ou de "lune de miel". Donc, les deux brigades n°2 et n°4 ont besoin de beaucoup de soutien.

La "Facilité à livrer" était clairement un problème majeur, c'est donc ce qui a conduit à mettre l'accent sur ​​des choses comme la livraison continue, et nous avons ainsi vu un progrès.

Notez que ceci est un modèle d'auto-évaluation, le tout basé sur l'honnêteté et la subjectivité des personnes dans les brigades. Donc, cela ne fonctionne que dans un environnement de haute confiance, où les personnes font confiance à leurs managers et collègues pour agir au mieux de leurs intérêts. Il est facile de se prendre au jeu des données, il est donc essentiel de s'assurer qu'il n'y a aucun intérêt / récompense à le faire.

Spotify met heureusement à disposition un environnement de très haute confiance et les managers et coachs prennent soigneusement le temps de montrer qu'il s'agit d'un outil pour aider, et non pas un outil pour juger.

## Comment nous collectons les données ?

Nous avons constaté que les sondages en ligne sont très mauvais pour ce genre de chose. Principalement parce qu'ils interrompent la conversation, alors que c'est là que réside la plus grande partie de la valeur. Les membres de la brigade acquièrent une meilleure compréhension pendant qu'ils discutent, et les coachs acquièrent une meilleure compréhension sur la façon d'aider efficacement les brigades. Les données seules vous donnent seulement une petite partie de l'histoire, ce qui pourrait induire en erreur.

Donc, nous (habituellement les coachs agiles) organisons des ateliers avec les brigades, en facilitant des conversations en face-à-face autour des différents indicateurs de santé. Une ou deux heures sont généralement suffisantes.

Pour faciliter cela, nous avons un paquet de cartes "Supers Cartes", chaque carte étant un indicateur de santé avec un "Exemple de ce qui est Super" et un "Exemple de ce qui est Nul".

![cartes du bilan de santé]({{ site.url }}assets/henrik_kniberg/squad-health-check-awesome-cards.png)

(Téléchargez les cartes et les instructions en [PDF](https://spotifylabscom.files.wordpress.com/2014/09/squad-health-check-model2.pdf) ou [PPTX](https://spotifylabscom.files.wordpress.com/2014/09/squad-health-check-model.pptx) - merci à Martin Österberg pour la conception)

Le paquet de cartes contient environ 10 cartes, voici un exemple de paquet complet :


|-------+-----------------------------+---------------------------|
| Sujet | Exemple de ce qui est Super | Exemple de ce qui est Nul |
|-------|-----------------------------|---------------------------|
| Facilité à livrer | Livrer est simple, sécurisé, indolore & essentiellement automatisé. | Livrer est risqué, douloureux, essentiellement manuel, et prend une éternité. |
| Processus adapté | Notre façon de travailler est parfaitement adaptée à nous. |Notre façon de travailler est nulle. |
| Qualité technique (code source en bonne santé) | Nous sommes fiers de la qualité de notre code ! Il est propre, lisible et a une bonne couverture de tests. | Notre code est un tas de m...rde, et la dette technique a pris le pouvoir. |
| Valeur | Nous livrons des trucs supers ! Nous en sommes fiers et nos parties prenantes sont très contentes. | Nous livrons de la m...rde. Nous sommes honteux de livrer cela. Nos parties prenantes nous haïssent. |
| Vitesse | Nous terminons rapidement les choses. Pas d'attente, pas de retard. | Il semble que nous ne terminions jamais quelque chose. Nous sommes toujours coincés ou interrompus. Les stories sont toujours bloquées par des dépendances. |
| Mission | Nous savons exactement pourquoi nous sommes ici, et nous sommes vraiment enthousiasmés par ce sujet. | Nous n'avons pas la moindre idée de pourquoi nous sommes là, il n'y a pas de vision d'ensemble ou de mise au point. Notre prétendue mission n'est absolument pas claire et ne nous inspire pas. |
| Motivation | Nous adorons aller au travail, et nous prenons notre pied lorsque nous travaillons ensemble. | Ennnnnuuuuyeuuux. |
| Apprentissage | Nous apprenons un tas de choses intéressantes tout le temps. | Nous n'avons jamais le temps d'apprendre quelque chose. |
| Soutien | Nous sommes constamment soutenus et avons de l'aide lorsque nous la demandons ! | Nous sommes constamment bloqués parce que nous n'avons pas de support et d'aide lorsque nous la demandons. |
| Pions ou joueurs | Nous maîtrisons notre destinée ! Nous décidons ce que nous allons fabriquer et comment nous allons le fabriquer. | Nous sommes juste des pions sur une échiquier, sans influence sur ce que nous fabriquons et sur la façon de le construire. |

Pour chacune des questions, la brigade est invitée à examiner si elle est plus proche de "Super" ou plus proche de "Nul", et nous utilisons des techniques de facilitation d'atelier (dotvoting, ...) pour les aider à parvenir à un consensus sur la couleur à choisir pour cet indicateur, et quelle est sa tendance (c'est stable, c'est en amélioration ou ça empire).

![atelier bilan de santé de la brigade]({{ site.url }}assets/henrik_kniberg/squad-health-check-workshop.png)

Nous préférons conserver trois niveaux (vert / jaune / rouge) pour que cela reste simple. La définition exacte des couleurs peut varier, mais cela peut être par exemple :

* Le vert ne signifie pas nécessairement que les choses sont parfaites. Cela signifie simplement que la brigade est satisfaite, et ne voit pas l'utilité de s'améliorer sur ce point en ce moment.
* Le jaune signifie qu'il y a des problèmes importants qui doivent être traités, mais ce n'est pas une catastrophe.
* Le rouge signifie que c'est vraiment nul et que ça doit être amélioré.


Effectivement, ce sont des données subjectives. En théorie, la brigade peut choisir d'y associer des données scientifiques (temps de cycle, nombre de défauts, vélocité, ...), mais peu le font. Parce que, même avec des données scientifiques, la brigade a besoin d'interpréter les données et de décider si cela constitue un problème ou non. Ainsi, à la fin de la journée, tout est finalement subjectif. Si quelque chose ressemble à un problème, alors c'est en soi un problème.

Parfois, nous combinons cela avec des rétrospectives, par exemple voter sur une carte et décider des actions pour améliorer ce sujet.

## Quelles sont les questions à poser ?

Si vous observez les différents exemples fournis ci-dessus, vous verrez que les questions varient un peu.
Principes directeurs :

* Les questions sont conçues pour couvrir un **large éventail de points de vue différents**.
* **Ces questions ne sont qu'un point de départ,** un choix par défaut. Les brigades sont libres de supprimer, ajouter ou modifier les questions si elles pensent à quelque chose de pertinent.
* Essayez de vous **limiter à une dizaine questions**. Si nous avons d'autres questions, certaines sont probablement en partie redondantes et peuvent être supprimées.


Nous nous assurons que les questions portent sur l'environnement dans lequel opère la brigade, et non sur une donnée scientifique (comme la vélocité). Cela rend l'enquête beaucoup moins intimidante, et renforce la notion que l'enquête porte sur le soutien et l'amélioration, pas le jugement.

Notre hypothèse (vrai ou non) est qu'une brigade désire fondamentalement réussir, et réussira aussi bien qu'elle le peut dans des circonstances données.

## A quelle fréquence mesurons-nous la santé de la brigade ?

Comme indiqué, nous avons un certain nombre de modèles différents en cours, donc cela varie beaucoup. Nous n'avons pas vraiment convergé vers un "intervalle de temps parfait" (et nous ne le ferons probablement jamais).

Une fréquence trimestrielle semble être cependant un bon point de départ. Une fréquence mensuelle semble exagérée (les personnes ont en vite marre, et les données changent trop vite pour être fiables). Une fréquence bi-annuelle semble trop faible (trop de choses se produisent dans ce délai). Mais, encore une fois, c'est variable.

## Conclusion - Choses à garder à l'esprit si vous le faites

Un tel modèle PEUT aider à stimuler et concentrer vos efforts d'amélioration. Mais il peut aussi foutre en l'air votre culture s'il est utilisé de façon inappropriée ! Donc, procédez avec une attention toute particulière.
Voici quelques lignes directrices pour améliorer vos chances de succès :

* **Soyez clair sur votre intention** pour introduire le modèle. Cela devrait concerner l'amélioration, pas le jugement.
* Recueillez des données principalement par la communication en **face-à-face**, et non via des enquêtes en ligne. Le processus de collecte de données doit être **intéressant et amusant**.
* **Impliquez les équipes** sur la façon d'appliquer le modèle, et laissez-les le modifier comme bon leur semble.
* **L'accord de l'équipe est plus important que la cohérence des données.** Si l'équipe A choisi un ensemble de questions légèrement différent de l'équipe B, c'est très bien (même si la synthèse sera moins simple à faire).
* Assurez-vous qu'il n'y a **pas d'incitation à déjouer le modèle**. Il ne devrait y avoir aucune raison pour qu'une équipe souhaite "faire illusion".
* Trouver un **moyen simple pour visualiser les données**. Plus le visuel est évident et intuitif, plus il a de chance d'être utilisé.
* **Méfiez-vous de comparer les équipes**. Si l'équipe A est majoritairement dans le vert et que l'équipe B est surtout dans le rouge, cela ne signifie pas que l'équipe A est "meilleure". Cela pourrait tout aussi bien signifier que l'équipe A a un contexte plus simple ou une prévision plus optimiste, ou que l'équipe B est plus honnête vis-à-vis de ses problèmes. Quoi qu'il en soit, il est probable que l'équipe B ait besoin de soutien. L'attitude du manager devrait être "comment puis-je vous aider ?" et non "les gars, pourquoi êtes-vous pire que les autres ?".
* **Suivez la mise en oeuvre**. Posez des questions aux personnes, par exemple "Est-ce que le modèle vous aide ?", "Si nous arrêtions de faire des bilans de santé, est-ce que ça vous manquerait ?", "Comment pourrions-nous rendre ce modèle plus utile ?". Le modèle lui-même (et votre façon de l'appliquer) doit s'améliorer en permanence.


Voir aussi le très perspicace [article de Martin Fowler sur les modèles de maturité](http://ayeba.wikispaces.com/Mod%C3%A8le%20de%20Maturit%C3%A9).

Voilà, c'est tout. Espérons que cet article ait été utile ! Avez-vous aussi expérimenté ce genre de choses ? S'il vous plaît, partagez vos expériences (positives ou négatives) en commentaire de ce blog !

_Henrik Kniberg et Kristian Lindwall, septembre 2014._

Cf. [Modèle d'Audit de la Santé d'une Brigade](http://ayeba.wikispaces.com/Mod%C3%A8le%20d%27Audit%20de%20la%20Sant%C3%A9%20d%27une%20Brigade)


---
Auteurs : Henrik Kniberg ([@henrikkniberg](https://twitter.com/henrikkniberg)) & Kristian Lindwall ([@klindwall](https://twitter.com/klindwall))  
Source : [Squad Health Check model – visualizing what to improve (Spotify Labs)](https://labs.spotify.com/2014/09/16/squad-health-check-model/)  
Date de parution originale : 16 Septembre 2014  

---
Traducteurs : [Fabrice Aimetti](http://www.fabrice-aimetti.fr/), [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/) (uniquement PDF et PPTX)
Date de traduction : 16/09/2014 - MàJ 14/11/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

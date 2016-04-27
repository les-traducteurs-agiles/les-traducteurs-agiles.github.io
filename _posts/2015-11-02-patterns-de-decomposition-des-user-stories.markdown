---
layout: post
title:  "Patterns de décomposition des user stories"
date:   2016-02-15 23:19:55
published: false
categories: 
- user-stories
---

> Ce fichier est et doit demeurer uniquement la source de la traduction publiée sur le site de l’auteur sur cette [page](http://agileforall.com/splitting-stories-in-french/). En effet, l’auteur souhaitant que la publication soit faite sur son site, le flag published est et doit être laissé à false

![Matryoshka](http://91.68.209.11/bmi/35qk152ejao6mi5pan29erbr9.wpengine.netdna-cdn.com/wp-content/uploads/2009/10/matryoshka.jpg)

De bonnes user stories suivent le modèle [INVEST](http://www.les-traducteurs-agiles.org/story/2015/02/23/investissez-dans-de-bonnes-stories-et-dans-des-taches-smart.html) de Bill Wake. Elles sont **I**ndépendantes, **N**égociables, de **Valeurs**, **E**stimables, **S**uffisamment petites, et **T**estables. Le critère _Suffisamment petites_ nous amène à décomposer les grosses stories. Mais les stories obtenues après décomposition doivent toujours suivre ce modèle.

Un certain nombre de nouvelles équipes agiles tentent de décomposer les stories d’après les couches d'abstractions : une couche pour l'IHM, une pour la base de données, etc. Cela peut satisfaire le critère _Suffisamment petites_, mais pas les critères _indépendantes_ et _de valeurs_. 

Au cours de mes années d'expérience en agilité, j'ai découvert 9 _patterns_ de décomposition des user stories en bonnes petites stories.

_(Note : Comme pour n'importe quel langage de pattern, je n’ai pas inventé ces patterns, je les ai juste observés et compilés. Par exemple, dans cet [excellent article](http://lassekoskela.com/thoughts/7/ways-to-split-user-stories/), Lasse Koskela met des noms sur certains de ces patterns que j'ai pu observer mais que je n'ai pas nommés dont notamment "Effort majeur".)_  

## Petites jusqu'à quel point ?

Jusqu'à quel point les stories devraient être les stories ? Je recommande entre 6-10 stories par itération, donc petites jusqu'à quel point  signifie _suffisamment_ petites par rapport à la vélocité de votre équipe. Avant votre prochaine réunion de planification, calculez le seuil de la valeur de l’estimation qui devrait déclencher la décomposition d’une story. Pour la plupart des équipes, il semble que cela soit 8 ou 13 points. Mais sur un projet récent dont je m’occupe, j’ai eu besoin de décomposer des stories à partir de 5 points.

Lorsque vous êtes en réunion de planification et que vous atteignez le seuil de la valeur de votre estimation déclenchant la décomposition, utilisez donc l’aide-mémoire présent en fin d'article et essayez quelques-uns des patterns jusqu’à ce que vous arriviez à une décomposition satisfaisante.

## Quel _pattern_ utiliser ?

Souvent, vous vous apercevrez que vous pouvez décomposer une story en utilisant plusieurs _patterns_. Quelle décomposition devriez-vous choisir ? Pour cela, j'utilise deux règles empiriques : 

1. **Choisir la décomposition qui vous permet de déprioriser ou de mettre à la poubelle une story.** La règle des 80/20 nous indique que la majeure partie de la valeur d’une story vient de la plus petite partie de la fonctionnalité. Lorsqu’une décomposition révèle une fonctionnalité de faible valeur et qu’une autre décomposition n’en révèle pas, cela suggère que cette dernière décomposition masque un gaspillage caché dans chaque petite story. Choisissez la décomposition qui vous permet de mettre à la poubelle les éléments de faibles valeurs.

2. **Choisir la décomposition vous donnant des stories petites et de taille sensiblement équivalente.** Une décomposition qui transforme une story de 8 points en quatre stories de 2 points est plus utile qu’une décomposition qui produira une de 5 et une de 3. Cela permet de donner au Product Owner plus de liberté pour prioriser séparément les différentes parties de la fonctionnalité.

## Pattern #1 : Étape du _workflow_

Voici une story issue de la création d'un système de gestion de contenu (CMS) pour l'un de mes clients.

> En tant que responsable de contenu, j'ai la possibilité de publier une actualité sur le site web d'entreprise.

Est-ce que cela ne semble t’il pas démesuré - de devoir approfondir jusqu’au workflow pour pouvoir publier une actualité ? Il s’avéra que pour avoir seulement quelques phrases écrites dans une actualité du site web d’entreprise cela exigeait à la fois une validation sur les aspects éditoriaux et juridiques et une dernière relecture sur un site de pré-production. Il n’y avait aucune chance que 6 à 10 stories de ce genre puissent tenir en une itération.

Dans un _workflow_ tel que celui-ci, la plus grosse valeur vient le plus souvent des étapes de début et de fin. Les étapes intermédiaires ajoutent de la valeur supplémentaire, mais elles ne sont pas auto-suffisantes. Cela peut donc valoir le coup de construire d’abord un cas simple de bout en bout puis d’ajouter les étapes intermédiaires et les cas à part.  

Les nouvelles stories furent :

> ... j’ai la possibilité de publier une actualité directement sur le site web d'entreprise  
> ... j’ai la possibilité de publier une actualité avec une validation sur l'aspect éditorial  
> ... j’ai la possibilité de publier une actualité avec une validation sur l'aspect juridique  
> ... j’ai la possibilité de voir une actualité sur le site de pré-production  
> ... j’ai la possibilité de publier une actualité du site de pré-production en production  

## Pattern #2 : Variations sur la règle métier

La story suivante dissimule en réalité plusieurs autres stories possédant un niveau de complexité équivalent accomplissant exactement la même chose mais avec des règles métiers différentes :

> En tant qu'utilisateur, je recherche des vols avec des dates flexibles.

En approfondissant sur ce que sont des “dates flexibles”, plusieurs règles métiers ont été révélées au grand jour, chacune pouvant donner sa propre bonne story : 

> ... comme "n jours entre x et y"  
> ... comme "un week-end en décembre"  
> ... comme "± n jours entre x et y"  

## Pattern #3 : Effort majeur

Quelques fois une story peut être décomposée en plusieurs parties. Et le gros de l’effort ira vers l’implémentation de la première d’entre elles. Prenons par exemple, cette story de traitement de carte de crédit

> En tant qu'utilisateur, j’ai la possibilité de payer mon vol avec une carte VISA, MasterCard, Diners Club, or American Express.

pourrait être décomposée en quatre stories, une pour chaque type de carte. Mais l’infrastructure du traitement des cartes de crédit sera construite uniquement pour la première story ; l’ajout d’autres types de cartes de crédit sera relativement trivial. Nous pourrions estimer la première story qui est plus grosse que les trois autres, mais alors nous devrons nous rappeler de changer nos estimations si plus tard le Product Owner change ses priorités. À la place, nous devrions différer la décision de savoir quelle type de carte de crédit devrait être implémenter en premier de la manière suivante :

> ... j’ai la possibilité de payer avec un seul type de carte de crédit (soit VISA, MC, DC, AMEX)  
> ... j’ai la possibilité de payer avec quatre types de cartes de crédit (VISA, MC, DC, AMEX) (étant donné un type de carte de crédit déjà implémenté).

Les deux nouvelles stories ne sont encore pas _indépendantes_, mais la dépendance est beaucoup plus claire qu’elle ne l’aurait été avec une story pour chaque type de carte.

## Pattern #4 : Simple / Complexe

Lorsque vous êtes en train de discuter d’une story en réunion de planification, et que la story semble devenir de plus en plus grosse (“Et à propos de x ?” ; “Avez-vous pensé à y ?”), arrêtez-vous et demandez-vous : “Quelle serait une version plus simple de cette story ?” Faites de cette version plus simple une story à part entière. Vous aurez probablement à définir quelques critères d’acceptations sur le vif pour conserver le caractère simple de la story. Puis, répartissez toutes les variantes et toutes les versions complexes dans leurs propres stories. Ainsi, par exemple, cette story,

> En tant qu'utilisateur, j’ai la possibilité de chercher les vols entre deux destinations.

restera simple en la décomposant ainsi,

> ... en spécifiant le nombre maximal d'escales  
> ... en incluant les aéroports à proximité  
> ... en utilisant des dates flexibles  
> ... etc.

## Pattern #5 : Variations dans les données

La complexité dans une story provient de la gestion des variations dans ses données. 
Par exemple, je travaille actuellement sur un système qui doit modéliser les zones géographiques desservies par les compagnies de transports urbains. Nous aurions pu dépenser tout le budget du projet uniquement pour gérer l’aspect géographique potentiellement très complexe. Lorsque j’ai discuté de cette story   

> En tant qu'utilisateur, j’ai la possibilité de rechercher les compagnies de transports urbains par lieu de départ et lieu d'arrivée.

avec notre Product Owner, j’ai découvert que, même si nous n’avions pas besoin d’un système d’information géographique complet, la modélisation de la géographique resterait tout de même assez complexe. Nous nous sommes arrêtés et nous nous sommes demandés, “Quelle est la manière ‘tout juste satisfaisante’ permettant de modéliser la géographie afin que nous puissions construire des fonctionnalités de forte valeur tout de suite ?”. Nous avons mis,

> En tant qu’utilisateur, j'ai la possibilité de rechercher les compagnies de transports selon le lieu de départ et d’arrivée dans les comtés.

Cela a fonctionné pendant un moment, jusqu’à ce que nous collections plus de données et trouvions quelques compagnies de transports desservant uniquement certaines villes et même leurs environs. Nous avons alors écris une nouvelle story :

> En tant qu’utilisateur, j'ai la possibilité de rechercher les compagnies de transports selon le lieu de départ et d’arrivée dans les comtés, les agglomérations, les villes et leurs environs.

En regardant les données de la nouvelle compagnie de transport, nous avons aussi découvert que certaines compagnies pourraient gérer des voyages en partance d’une seule ville tout en arrivant dans n’importe quelle ville environnante. Ceci nous a amené à cette story :

> Les compagnies de transports peuvent desservir différentes zones géographiques pour le lieu de départ et d'arrivée d'un voyage.

Chacune de ces trois stories sont le fruit de la décomposition de la story géographique d'origine. Les différences proviennent de l'ajout des stories en juste-à-temps après en avoir fait une version plus simple. Mais quelque fois vous connaissez dès le début les variations dans les données. L’exemple classique par excellence est la localisation :  

> En tant que responsable de contenu, j’ai la possibilité de créer de nouvelles actualités.  
> ... en anglais.  
> ... en japonais.  
> ... en arabe.  
> ... etc.  

## Pattern #6 : Méthodes de saisie des données

Quelques fois la complexité réside dans l’interface utilisateur plutôt que dans la fonctionnalité elle-même,. Dans ce cas, décomposez la story avec l’objectif de la construire avec l’interface utilisateur la plus simple possible puis mettez en place une interface utilisateur plus utilisable ou plus jolie. Ces stories ne sont pas, bien sûr, indépendantes - la deuxième story est bien entendu la story d'origine si vous la faites dès le début - mais cela peut toujours être une décomposition qui peut s'avérer utile.

> En tant qu'utilisateur, j’ai la possibilité de rechercher des vols entre deux destinations.  
> ... en faisant une simple saisie de dates  
> ... en utilisant un joli calendrier

## Pattern #7 : Ajournement de la performance

Quelques fois, une grosse partie de l’effort est mise dans la réalisation rapide d’une fonctionnalité - l’implémentation initial n’étant pas si difficile que ça à faire. Mais vous pouvez apprendre beaucoup de choses d’une implémentation plus lente et elle a bien une certaine valeur aux yeux du client qui autrement ne serait pas capable d’accomplir l’action décrite dans la story. Dans ce cas, fractionner la story en “faites-la fonctionner” et “faites-la vite”.

> En tant qu'utilisateur, j’ai la possibilité de rechercher les vols entre deux destinations  
> ... (lent -  jusqu'à son accomplissement, montrer une animation “rechercher en cours”).  
> ... (en dessous de 5 secondes)

## Patter #8 : Opérations (par exemple : Créer, Lire, Mettre à jour, Supprimer)

Le mot “gérer” dans une user story est un fourre-tout indiquant que la story recouvre plusieurs opérations. Le fractionnement de cette story se fait donc tout à fait naturellement. Par exemple :   

> En tant qu'utilisateur, j’ai la possibilité de gérer mon compte.  
> ... j’ai la possibilité de créer un compte   
> ... j’ai la possibilité d’éditer les paramètres de mon compte  
> ... j’ai la possibilité de supprimer mon compte  

## Pattern #9 : Lancer une expérience

Une story peut être grosse non pas parce qu’elle est forcément complexe, mais parce que son implémentation est mal comprise. Dans ce cas, aucune discussion au sujet de la partie métier de la story ne vous permettra de la décomposer. Faites une expérience limitée dans le temps pour résoudre l’incertitude tournant autour de l’implémentation. Ensuite, vous pouvez faire l’implémentation ou avoir une meilleure idée de comment la décomposer. Vous ne savez pas comment implémenter la story suivante ?  

> En tant qu'utilisateur, j’ai la possibilité de payer par carte de crédit.

Alors, décomposez-la en :

> Examiner le traitement de la carte de crédit.  
> Implémenter le traitement de la carte de crédit.  

Dans le segment “examiner” de la story, les critères d’acceptation devraient être des questions auxquelles vous devrez répondre. Faites suffisamment d’investigations pour vous permettre de répondre aux questions puis arrêtez-vous là ; c’est facile de se laisser emporter en faisant des recherches.

La décomposition de cet essai devrait se faire en dernier parce qu’il s’agit de votre dernière chance. Vous en savez probablement assez pour réaliser quelque chose. Faites donc cela et vous en saurez davantage. Donc, faites tout votre possible pour appliquer l’un des huit patterns précédents avant d’avoir recourt au pattern de l’expérience.

## Conclusion

Résistez donc à la tentation de fractionner une user story beaucoup trop grosse par couches d'abstractions. À la place, essayez ces patterns pour décomposer votre story en plus petites qui devront satisfaire toujours le modèle INVEST. Faites-moi savoir comment cela a fonctionné pour vous ou si vous êtes tombé sur des stories non décomposables (J’adore les défis !).

[Télécharger l'aide-mémoire sur le fractionnement des user stories](http://35qk152ejao6mi5pan29erbr9.wpengine.netdna-cdn.com/wp-content/uploads/2009/10/Story-Splitting-Cheat-Sheet.pdf)

Mis à jour de mars 2012 : Allez donc jeter un coup d’oeil sur l'article [Encore plus de manières de décomposer les user stories](http://www.richardlawrence.info/2012/01/27/new-story-splitting-resource/) que j’ai rédigé pour vous aider à appliquer ces patterns sur vos stories..

---  
Auteur : [Richard Lawrence](http://www.agileforall.com/author/richard/)  
Source : [Patterns for Splitting User Stories](http://www.agileforall.com/2009/10/patterns-for-splitting-user-stories/)  
Date de parution originale : 28 Octobre 2009  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 05/01/2016  
  
Relecteur : [Bruno Sbille](http://brunosbille.com/)
---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}




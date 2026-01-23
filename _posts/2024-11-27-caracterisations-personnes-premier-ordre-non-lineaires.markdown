---
layout: post
title: "De la nature non linéaire et de toute première importance des êtres humains dans le développement logiciel"
date:   2026-01-23 00:01
published: true
tags:
- agile
- facteur humain
---

> Préambule du traducteur : Même si le texte originel a été publié initialement en 1999 et malgré les avancées technologiques permettant de travailler à distance ainsi que dans d'autres domaines, il reste à mes yeux toujours d'actualité.

## Rapport technique - Humans and Technology - Mars 1999
Présenté à la 4ème International Multi-Conference on Systems, Cybernetics and Informatics, Orlando, Floride en juin 2000.

## Résumé

Nous autres, méthodologistes et concepteurs de processus avons pris l'habitude de concevoir des systèmes complexes sans toutefois prendre la peine de caractériser leurs composants actifs, bien que ceux-ci soient connus pour leurs caractères hautement non-linéaires et d'une très grande variété : les personnes.  

Dans ce rapport, je mets en exergue des théories et des projets à la lumière de cette prodigieuse et notable découverte ainsi que quatre éléments caractérisant les personnes, et qui impactent toute conception de méthode et le résultat de tout projet. J'ai découvert que ces caractéristiques sont de bien meilleures sources de prévisions sur le déroulement d'un projet et la réussite d'une méthode que tout autre facteur méthodologique.

Mots-clés : conception de méthodologie, processus, facteurs humains, facteurs collectif

## 1 - Introduction

Ce rapport compile l'étude et l'expérience acquise s'étendant sur une période de 20 ans d'environ trois douzaines de projets et de méthodes différentes. Pour faire court, pendant toutes ces années, nous avons conçu des systèmes complexes dont les composants actifs sont variables et hautement non-linéaires (autrement dit les personnes), sans avoir pris le temps de caractériser ces composants ou avoir caractérisé leurs effets sur le système en question. Après réflexion, cela peut sembler absurde, mais étonnamment peu de gens dans notre métier se sont investis suffisamment pour vraiment comprendre comment ces choses qu'on appelle les personnes influent sur le développement logiciel.

Parmi les exceptions notables, citons Gerald Weinberg \[Wei\] and Tom DeMarco \[Dm\], dont les ouvrages viennent d'être réimprimés en édition spéciale anniversaire. Leurs travaux dans ce domaine sont d'ailleurs reconnus et bien des consultants s'accordent à dire que le facteur humain est un aspect essentiel  dans le développement logiciel \[B99\], \[Hi\]. On pourrait s'attendre à trouver ici et ailleurs des recherches  pour poursuivre leurs travaux. Toutefois, la communauté du développement logiciel a grandement ignoré les caractéristiques des personnes comme sujet d'étude. Il s'agit d'un oubli significatif, aussi significatif que d'ignorer l'acier dans les murs en béton armé et de s'interroger par la suite pourquoi les expériences radiophoniques ne donnent pas les résultats attendus.

Comme beaucoup de gens, lorsque j'étais amené à évoquer des personnes dans des projets, je le faisais uniquement superficiellement et c'est bien après des années de recherches et de pratiques en méthodologie que j'ai commencé à m'interroger sur pourquoi mes recommandations en terme de méthodologie ne correspondaient pas à mes expériences dans les projets informatiques. Le problème n'était pas, ce que mes différentes équipes _faisaient_ (les projets en question avaient un fort taux de réussite). Le problème était que ce que j'écrivais ne correspondait pas à ce que nous faisions.

Ces cinq dernières années, j'ai découvert — et je continue à découvrir — combien il est difficile de déterminer "ce que je regarde". Peu à peu il m'est apparu évident qu'une chose ne collait pas dans mon équation méthodologique, ou en fait, dans l'équation de n'importe qui d'autre, aussi loin que je puisse voir, c'est-à-dire l'effet des « personnes » sur les méthodologies.

Du moment où j'ai commencé à comptabiliser ces faits, j'ai trouvé que mes prédictions méthodologiques et mes résultats commençaient à concorder avec mes expériences. Je considère aujourd'hui que les caractéristiques des personnes sont le facteur _dominant, de 1er ordre_ de tout projet.

En quoi cela diffère t'il de ce que DeMarco et Lister ont pu écrire dans leur ouvrage  _Peopleware_ ?

Dans leur ouvrage, DeMarco et Lister énoncent que les personnes sont déterminantes et nous livrent des clés de compréhension. De mon côté, je me suis plus particulièrement intéressé sur comment les caractéristiques des groupes et des individus influent sur la conception des pratiques de développement logiciel (autrement dit les méthodologies) au sein de différents groupes travaillant sur différentes sortes de missions.

Dans le chapitre « faire équipe » de l'ouvrage _Psychology of Computer Programming_, j'ai découvert quelque chose qui se rapproche de ce que je cherchais et plus particulièrement dans la partie gestion de « tâches » vs gestion de la « maintenance » à savoir : la notion de caractérisations et les recommandations qui découlent de celles-ci. Ces caractérisations et ces recommandations faites sur la bases d'entretiens dans les années 1960 s'avèrent toujours pertinentes et significatives 30 ans plus tard. Ceci valide la solidité et l'importance de ce type de question. Il est temps que nous étudiions ces questions qui sont au cœur de l'ingénierie logicielle et que nous arrêtions de les redécouvrir tous les 30 ans.

La rédaction de ce document, qui met en exergue l'ensemble de ces travaux, me permet d'affirmer que les « personnes » comme étant vraiment de toute première importance dans la réussite d'un projet et non de manière incidente ; j'en utilise les caractéristiques comme autant d'indicateurs prédictifs. Ce document est écrit à la première personne et non dans un style formel ou académique classique, parce qu'il relate une quête de quelque chose d'évident tout en restant non explicité, il me parait donc plus adapté de de la raconter sous la forme d'un récit. 

## 2 – Ce qui ne fonctionnait pas

En 1987, lors du développement en méthode formelle d'un logiciel de communication, j'avais été encouragé à traiter le sujet suivant : « le _problème_ lors du développement d'un logiciel, c'est qu'il y a trop d'ambiguïté dans l'explicitation du problème et dans la description de la conception. _Les choses iront mieux_ si nous faisons en sorte que les personnes adoptent un formalisme mathématique ». Après avoir travaillé quelques temps dessus sur ce domaine, j'ai découvert que :

- **Problème 1 :** Les personnes dans les projets ne sont pas intéressés par apprendre notre système
- **Problème 2:** Elles ont réussi à nous ignorer et à livrer du logiciel tout de même. 

J'ai arrêté le développement formel après avoir entendu l'un de mes collègues dans ce domaine dire : « En fait, le _problème_ réside dans la formation. _Les choses se passeraient mieux_ si nous commencions à donner aux étudiants une formation mathématique suffisante bien plus tôt — autrement dit dans le secondaire ». Compte tenu de ce que j'ai appris sur les personnes, je pense que son affirmation révélait en fait un désir frustré. Non pas que je doute de certains des avantages du développement formel, mais je doute de notre capacité à persuader 10**6 personnes à le maîtriser. La bonne question pourrait être : « En quelles circonstances et dans quel cadre, devrions-nous faire appel à un spécialiste en développement formel ? » 

Je suis donc passé à la place au développement d'outils, travaillant autant que possible de manière ethnocentrique. J'ai donc observé des concepteurs de protocoles de communication et j'ai discuté avec eux sur quels pourraient être les problèmes auxquels ils faisaient face. Mes collègues et moi avons alors décidé que « Le _problème_ est que les gens continuent de dessiner sur tableau blanc. _Les choses se passeraient mieux_ si nous leur donnions des outils spéciaux afin qu'ils puissent dessiner directement sur ordinateur et qu'ils puissent voir au plus tôt leurs conceptions devenir rapidement un exécutable.  »

Nous avons passé alors plusieurs années à développer un moteur d'inférence qui convertirait les diagrammes d'interactions en architecture logicielle et en système de règles \[Ci\]. Beaucoup d'équipes ont travaillé et travaillent encore sur des concepts similaires comme par exemple les machines à état fini exécutables de Harel \[Ha\].

Quelques années plus tard, nous avons terminé un prototype  et l'avons montré à notre groupe d'utilisateurs potentiels, et nous avons été estomaqués de les entendre nous dire « Non merci, en fait nous,  nous aimons dessiner sur les tableaux blancs. Nous ne voulons pas perdre du temps à mettre nos dessins sur ordinateurs. Hum, par contre pouvons-nous utiliser cette partie de l'éditeur de dessin de l'outil ? ».  Nous avons entendu ce même récit de la part d'autres éditeurs logiciels qui se terminait immanquablement par « ils utilisent juste l'éditeur de dessin ». Autrement dit

- **Problème 1.** Les personnes travaillant sur des projets n'étaient pas intéressées par apprendre notre système.
- **Problème 2.** Elles étaient très fortes pour nous ignorer et être en capacité néanmoins à livrer du logiciel.

Troublé par tout cela, je suis donc passé à des méthodologies de développement logiciel, et j'ai conçu la méthodologie orientée-objet pour IBM Consulting Group entre 1992 et 1994. Ne voulant pas répéter la même erreur une troisième fois, je me suis entretenu avec des personnes d'une douzaine de projets basés sur l'objet tout autour du monde, puis j'ai tout couché par écrit. En étudiant ces notes, j'en ai conclu différentes choses :

- Les équipes qui réussissent font du développement incrémental \[Co95\]
- Toute technique de conception qui s'avère plus compliqué que des « cartes CRC » \[B87\] semblent trop complexes pour être utilisée  
- Les équipes de conception ont le privilège d'ignorer tout outil ou toute technique qu'elles n'apprécient pas. Tout ce qu'elles ont à dire à leur patron c'est : « Cela me ralentit — je ne tiendrai pas les délais si je l'utilise » et leur patron les laisse alors ne pas les utiliser. À cette époque, cela ne paraissait pas important de l'écrire, mais je l'avais noté en tant que « contrainte de conception » au niveau méthodologique.

J'ai alors conçu la méthodologie la plus palpable, la moins cérémonielle possible et je l'ai utilisée sur un projet. J'ai documenté notre expérience sous le nom de projet Winifred  \[Co98\]. La technique de conception de base que j'y ai recommandé, que j'ai enseignée et sur laquelle j'ai guidée les gens sur ce projet se base sur les cartes CRC.

Quelques mois plus tard, j'ai enlevé mon chapeau de consultant pour le remplacer par celui d'ethnographe et j'ai étudié les manières dont une équipe se comporte réellement. Ce que j'ai pu observer m'a sidéré :

- Le processus que l'équipe suivait d'un instant à un autre était si intriqué qu'il m'était impossible de le mettre par écrit et même si j'avais été en mesure de le faire, personne n'aurait été capable de le suivre \[Co98p\]. Cela correspondait de manière très superficiel à mon propre processus.
- Pas une personne parmi la douzaine de concepteurs orienté-objets que j'avais accompagné n'utilisait les cartes CRC.

En d'autres mots, même si j'avais utilisé ce que je pensais être une approche ethnographique pour concevoir cette méthodologie :

- **Problème 1.** Les personnes travaillant sur les projets n'étaient pas intéressées par apprendre notre système.
- **Problème 2.** Elles étaient très fortes pour nous ignorer et livrer néanmoins du logiciel.

Ce processus s'est répété encore et encore plusieurs fois, jusqu'à que je sois contrarié de mon incapacité à « voir réellement ce qui se passait ». La meilleure chose que je pouvais dire était qu'il y avait des choses importantes sur le projet que nous n'avions pas su nommer. Pour résoudre cela, j'ai fait alors équipe avec un ethnographe pour avoir de l'aide pour mettre un nom sur ce qu'il se passait \[Ho\]. Un consultant plus un ethnographe, ça faisait un bon duo, mais à peine venions tout juste de commencer que nous nous sommes rendus compte que nous étions incapables de décrire ce que nous voyions et que nous ne pourrions le faire tant que nous n'aurions pas les mots pour ce que nous étions en train de voir. Et manifestement, notre vocabulaire actuel s'avérait inadéquate.

Depuis, j'ai discuté, et j'ai lu des récits détaillés provenant de trois douzaine de projets différents (certains d'entre eux sont évoqués dans le tableau 1). 

**Tableau 1 : Revue des projets et des méthodologies utilisées.** Le tableau ci-dessous liste l'ensemble projets passés en revue classés par ordre chronologique. Chaque projet comporte un index de référence bibliographique abrégé permettant de le retrouver dans le reste du rapport et pour certains d'entre eux des informations complémentaires.

* * *

  
**1980**. “CT5”. Réussite. 26 personnes, 3 ans (1 année de retard), projet stratégique. Montée en compétence par apprentissage, présence d'un processus macro bien défini, absence de processus micro.  

* * *

  
**1986**. Projets “Cleanroom”  \[Mi\]. Réussite. IBM Federal Sector, projets avec des équipes de taille importante. Succès répétés grâce à une méthodologie lourde et très rigoureuse.  
 
* * *

  
**1986**. “Projets de Sherr” \[Br\] Réussite. Processus du genre « faites que ça marche, mais ne faites pas d'heures supplémentaires » ayant forcé à trouver des solutions créatives, absence de processus défini.  

* * *

  
**1980**. “Broooklyn Union Gas” \[Co98\]. Réussite. Nouvelle technologie orienté-objet, 150 personnes, projet stratégique.  

* * *

  
**1992**. “Tracy” \[Co98\]. Échec. Petite équipe suivant aveuglément une méthodologie dite « modélisez le monde, puis codez-le ». Accès occasionnel aux utilisateurs et à du personnel non qualifié. 

* * *

  
**1992**. “BlackKnight”. Réussite. Petite équipe avec notes repositionnables reliées par des fils en laine.

* * *

  
**1992**. “Manfred” \[Co98\]. Échec. Petite équipe, peu rigoureuse. « Nous ferons la conception plus tard » — échec du prototypage en continu 

* * *

  
**1992**. “CSPITF”. Réussite. Petite équipe suivant scrupuleusement des itérations. Processus léger, assis les uns à côté des autres. Bonne synergie entre le responsable technique et le responsable projet. Le responsable technique est resté sur le projet pour restructurer la conception interne du code pour l'équipe ayant succédé à la sienne.

* * *

  
**1992**. “OTI” \[Co98\]. Réussite. Petites équipes. « Donnez aux bonnes personnes les bons outils, et laissez-les tranquille. » Réussites répétées avec une méthodologie légère centré sur l'humain.

* * *

  
**1993**. “Reginald” \[Co98\]. Échec. Une équipe de 2 personnes ayant grossi pour devenir 3 équipes réparties sur 2 comtés. L'une des équipes suivait aveuglement une méthodologie lourde à base de documentation papier, et n'a jamais produit un seul morceau de code avant que le projet ne soit annulé.

* * *

  
**1993**. “Ingrid” \[Co98\]. Réussite. 26 personnes, 2 ans. Présence d'un processus macro incrémental, absence de processus micro. Échec du premier incrément. L'ensemble des développeurs a été remplacé, passage à une méthodologie légère orientée communication au fil du temps.

* * *

  
**1993**. “Synon in NZ”. Réussite. Lors de notre entretien le responsable du projet a indiqué que la réussite était due au fait que « les 4 personnes travaillaient dans la même pièce en cycle itératif très rapide » et que dorénavant il ne prendrait plus en charge de projets dans lesquels les personnes ne pourraient plus se parler entre eux facilement.

* * *

  
**1994**. “Udall” \[Co98\]. Réussite. Le projet fut au départ un échec avec une équipe de taille importante. Le projet fut après une réussite en « recommençant tout depuis le début, en reprenant une partie des personnes de l'équipe précédente pour former une petite équipe performante » .

* * *

  
**1995**. “Winifred” \[Co98\]. Réussite. Équipe de 45 personnes, durée de 20 mois. La réussite est due à la présence « d'une manière de réaliser incrémentale, d'une bonne communication, d'un nombre réduits de bonnes personnes ». Présence d'un processus macro et absence de processus micro. Méthodologie orientée communication.

* * *

  
**1996**. “Reel”. Échec. Équipe de 150 personnes à laquelle il avait été dit de documenter chaque changement de conception. Le projet fut abandonné. L'un des participants au projet le résuma de la manière suivante : « L'utilisation de mauvaises habitudes avec diligence reste quelque chose de mauvais » .

* * *

  
**1997**. “Caliper”. Échec. Équipe de 90 personnes, projet stratégique. Incapacité à faire une livraison majeure au bout de 6 ans : attentes élevées, nouvelles technologies, absence d'incréments, absence de personnel qualifiés à tous les niveaux.

* * *

  
**1997**. “NorgesBank”. Entretiens avec les 6 équipes projets. Une phrase revenait dans tous les entretiens : « le succès est au rendez-vous lorsqu'il y a de bonnes communications entre l'équipe et les utilisateurs ».

* * *

  
**1998**. “C3” \[C3\]. Réussite. Une équipe de 8 personnes remplaçant une équipe de 26 personnes après un premier échec. Extreme Programming \[EP\] : petite équipe, très rigoureuse, méthodologie orientée communication.

* * *

  
**1998**. “NB Banking”. Réussite. Initialement il s'agissait d'une équipe de 3 personnes pour un projet de 2 mois qui est passé du jour au lendemain à une équipe de 10 personnes sur 14 mois. Détestation de la visioconférence. Présence de processus macro et absence de processus micro. La réussite était due aux « aux incréments, aux bonnes personnes et à de la communication ».

* * *

  
**1998**. “M.A.D.” \[Ch\]. Réussite. Petite équipe ayant étudié les utilisateurs finaux dans leur contexte et ayant utilisé des prototypes. Utilisation réussie d'une méthodologie orientée communication et prototypage.

* * *

  
**1998**. “Insman”. Réussite. Équipe de 6 personnes utilisant « Crystal (Clear) »\[Co00\]. Réussite due à la « focalisation sur de la communication rapprochée, le moral de l'équipe, des incréments de 3 mois avec de l'auto-apprentissage au niveau de l'équipe ».

* * *

  
**1999**. “Cinch”. En cours. Équipe de 40 personnes colocalisées mais continuant d'exiger des livrables écrits formels. L'équipe reconnaissait le coût engendré par la rédaction d'écrits, mais elle était dans l'incapacité de passer sur un mode davantage informel (traits de caractère, habitudes, culturel ?)

* * *

  
**1999**. “Hill AFB TSP1” \[Web\]. Réussite. Équipe de 7 personnes ayant atteint le niveau 5 CMM en utilisant des processus logiciels individuels (PSP-Personal Software Process) et d'équipes (TSP — Team Software Process). La réussite de cette petite équipe était notamment due à l'utilisation d'une méthodologie très rigoureuse.orientée processus 

* * *


Ce que je trouve le plus étonnant dans ces projets est qu'ils démontrent que :

- presque n'importe quelle méthodologie peut faire fonctionner des projets
- n'importe quelle méthodologie peut faire échouer des projets
- les projets menés avec des méthodologies lourdes peuvent s'avérer être couronnés de succès
- les projets menés avec des méthodologies légères sont plus souvent couronnés de succès et plus important encore, que les personnes ayant travaillés sur ces projets créditent cette réussite à la légèreté de ces méthodologies.

Je n'ai trouvé aucune théorie pour expliquer ce taux élevé de réussite de projets ayant utilisés des méthodologies légères comportant peu de cérémonies, ni pour expliquer le faible taux de réussite de projets ayant utilisés des méthodologies comportant beaucoup de cérémonies à l'exception notable de Cleanroom et de PSP/TSP. Il m'apparait évident qu'un management médiocre est un facteur non-méthodologique qui y est pour beaucoup, mais même en essayant de normaliser ça, je me retrouve dans l'incapacité de donner des éléments de prévisions significatifs.

J'en ai finalement conclu qu'il y a quelque chose d'autre qui joue ici, qui est juste sous nos yeux à chaque instant et que nous ne voyons pourtant pas : les personnes. Les caractéristiques des personnes sont le facteur de réussite primordial de la réussite et non un facteur de second ordre. En fait, en renversant l'ordre des choses, je considère désormais les facteurs liés aux processus comme des éléments de second ordre.

D'après mon expérience tout peut être réduit à juste quelques caractéristiques essentielles concernant les personnes. En les appliquant sur des projets plus récents, j'ai pu prédire de manière plus pertinente leurs résultats et j'ai pu donner des recommandations plus pertinentes. Je crois que le temps est venu, de manière formelle et officielle, de conduire des recherches sur « quelles sont les caractéristiques des personnes qui peuvent impacter le développement logiciel et quelles sont leurs implications dans la conception des méthodologies ? ».

## 3 – Quatre caractéristiques

Les personnes, comme tout système actif, ont des modes de réussite et d'échec. Voici les principaux modes que j'ai pu trouver et dénommer jusqu'à présent :
  
1. Les personnes sont des êtres communicants, qui fonctionnent le mieux en face-à-face, avec des échanges en temps réel
2. Les personnes ont du mal à agir de manière constante au fil du temps
3. Les personnes sont très versatiles, d'un jour à l'autre et d'un lieu à l'autre
4. Les personnes veulent être de bons citoyens, sont plutôt bons pour percevoir leur environnement, prendre des initiatives et faire « ce qu'il faut » pour qu'un projet fonctionne.

Il existe d'autres caractéristiques sur lesquelles je ne m'étendrai pas ici :

- Les personnes ont besoin à la fois de temps de réflexion et d'opportunités de communication (cf. \[Co98\], \[Cs\], \[Dm\]).
- Les personnes travaillent mieux à partir d'exemples (un sujet à approfondir) (cf. \[J-L\]).
- Les personnes préfèrent échouer de manière conservatoire plutôt que de devoir risquer à réussir différemment \[Pi\]; elles préfèrent inventer plutôt que faire des recherches ; elles peuvent conserver seulement une faible quantité d'informations en têtes, elles font des erreurs et elles trouvent difficiles de changer d'habitudes.
- Des personnalités individuelles peuvent facilement dominer un projet.
- Le profil de personnalité d'un individu affecte fortement la réalisation de missions spécifiques

### Les personnes sont des êtres communicants

Le facteur unique et le plus significatif est la « communication ». Le diagramme 1 représente la courbe de l'information que j'utilise désormais pour évoquer mes réflexions en termes de méthodologie. Ce diagramme démontre que l'efficacité de la communication baisse en fonction des modalités de communication et de synchronicité. Quelques recherches sur ce sujet (cf. \[Pl\] et \[Si\]) corroborent les expériences relatées par Weinberg il y a plus de 30 ans (cf. \[Wei\].)

La manière la plus efficace de communiquer est la communication en tête-à-tête, face à face, à côté d'un tableau blanc. Si nous enlevons l'une de ces caractéristiques, nous voyons une baisse d'efficacité de la communication. Les caractéristiques que nous perdons sont :

- la proximité physique : je suis bien en peine d'expliquer pourquoi, mais se trouver proche physiquement d'une autre personne a un effet sur la communication. Que ce soit par l'aspect tridimensionnel, temporel, à l'odeur, ou bien encore par tout un ensemble d'éléments visuels, la proximité physique compte.
- la variabilité des modalités possibles. Les personnes communiquent aussi bien avec des mots qu'à travers des gestes, marquant souvent un point à l'aide d'un geste, avec les sourcils ou en montrant avec le doigt
- les inflexions de la voix et le débit. En accélérant, en ralentissant, en faisant des pauses ou en changeant le ton de la voix, l'intervenant accentue soit pour souligner l'importance d'une phrase soit pour surprendre son interlocuteur.
- les questions-réponses en temps réel. Les questions permettent de révéler les ambiguïtés dans le discours de l'intervenant ou dans la manière dont le discours n'atteint pas l'auditeur dans son contexte. La séquence des questions dessine un schéma de communication entre les interlocuteurs. 

![Variation de l'efficacité de la communication selon les canaux de communication utilisés]({{ site.url }}assets/alistair_cockburn/EffectivenessCommunicationForm-fr.png)


**Figure 1. Modes de communication**

Que se passe t'il quand nous enlevons ces caractéristiques l'une après l'autre ?

- Commençons par supprimer uniquement la proximité physique. Mettez deux personnes aux deux extrémités d'un échange vidéo. En principe, cet échange présente les mêmes caractéristiques qu'une présence physique. Toutefois, lorsque nous essayons, l'effet n'est pas exactement le même. Les membres d'une équipe travaillant respectivement à Oslo et à Lillehammer se sont aperçus après coup, que là où ils avançaient le mieux dans leurs travaux de conception, c'était lorsqu'ils étaient assis les uns à côté des autres dans le train. Même le fait de marcher ensemble en partant de la gare s'avérait plus efficace qu'une réunion en distanciel. 
- Puis supprimons la possibilité de voir les gestes, tout en conservant l'inflexion de la voix et le direct (par exemple en utilisant un téléphone). La plupart des gens parlent _tout en dessinant_. En effet, tout en dessinant une ligne reliant deux rectangles, une personnes pourra souligner oralement ce qui est important de retenir. Cette information simultanément visuelle et auditive permet d'ancrer l'information. Si vous avez deux personnes au téléphone, cet aspect de la transmission de l'information est supprimé, de même que les expressions faciales, les gestes dont celui de pointer quelque chose avec le doigt. 
- Ensuite en supprimant la voix et l'inflexion en direct, mais en conservant la capacité à poser des questions (courriel). Sans la voix en temps réel, il est impossible de faire une pause, de vérifier s'il y a besoin de s'interrompre, d'accélérer ou de ralentir pour préciser un point. Sans l'inflexion vocale, il est impossible d'élever notre ton ou la force de notre voix pour indiquer la surprise, l'ennui ou l'évidence d'une idée que nous souhaitons transmettre. 
- Après en supprimant la capacité à poser des questions (mais en laissant la possibilité de remettre en place une des caractéristiques précédemment supprimées). En l'absence de questions, la personne émettrice doit deviner ce que la personne destinataire sait, ne sait pas, ce qu'elle souhaiterait poser comme question, et quelle serait la réponse appropriée à cette question hypothétique sans avoir de retour si c'est pertinent ou pas. Dans ce cadre de communication, nous pouvons considérer l'ajout d'éléments visuels (enregistrement vidéo) ou vocaux (enregistrement audio). 
- Enfin en supprimant tout élément visuel, vocal, direct et de questionnement, et nous obtenons … une documentation papier. Dans le diagramme ci-dessus, la documentation se révèle être le moyen de communication le moins efficace. Le rédacteur doit faire des postulats par rapport à ses futurs lecteurs, et ne bénéficiera pas du direct, de signaux empathiques, de l'inflexion de la voix ou des gestes.

Si ce modèle s'avérerait être d'une quelconque utilité, il devrait nous suggérer comment mieux travailler. Et c'est bien ce qu'il fait, et nous nous apercevons d'ailleurs que les projets qui avancent le mieux utilisent d'ores et déjà ce que ce modèle suggère.

> « Mettez tout le monde dans une seule pièce. », « Je ne veux pas plus de 4 personnes, c'est le nombre de personnes maximum qu'il est possible de mettre dans une pièce pour qu'elles discutent ensemble dans de bonnes conditions. ». 

Ces recommandations, sont les recommandations habituelles des chefs de projets qui arrivent à faire avancer leurs projets. Dès le départ, ils prévoient d'utiliser le mode de communication ayant la bande-passante la plus élevée, c'est-à-dire des personnes en face-à-face.

> « Assurez-vous qu'il y ait des tableaux blancs et des espaces-café dans tout l'immeuble ». 

Très tôt, Hewlett-Packard et IBM ont pu observer l'efficacité des « lieux de réunions informels » ; cette expression de « lieux de réunions informels » et leurs mises en place est désormais bien répandue dans notre secteur d'activité à tel point qu'un environnement de travail bien conçu se doit d'encourager la possibilité pour des petits groupes de se réunir de manière _ad hoc_. Weinberg a documenté plusieurs cas où des conversations ayant pu se dérouler dans un cadre détendu ont eu un effet significatif sur la productivité générale \[Wei\]. On assiste à des avancées importantes lorsque des personnes « parlent simplement ensemble ».

Trois méthodologies récentes mettent en avant le fait de réunir les personnes dans une même pièce ou très proches les unes des autres : Adaptive Software Engineering \[Hi\], Extreme Programming \[B99\], \[EP\], Crystal(Clear) \[Co00\]

Le modèle que nous avons évoqué précédemment nous incite à faire la recommandation suivante quant à l'archivage de la documentation produite :

Demandez à un concepteur de faire une brève description (5 à 20 minutes) de sa conception à un ou deux collègues qui ne sont pas familiers du sujet. Ils agiront comme des médiateurs pour les futures spectateurs de la vidéo. Laissez-les simplement avoir une discussion sur la conception, avec ces collègues posant des questions et enregistrez-les en vidéo. À la fin de l'enregistrement, reproduisez les schémas des exemples ou les schémas de conceptions utilisés, lors de la discussion, pour servir d'ancres mémorielles à la discussion

J'ai été agréablement surpris d'apprendre que Lizette Velasquez de l'entreprise Lucent Technologies avait non seulement pu tirer bénéfice de cette technique mais que j'avais oublié d'évoquer également quelque chose d'important. Elle a dit qu'il était important de marquer et d'indexer les moments où « quelque chose d'intéressant se passe ». Même si la plus grande partie de la discussion se passe sur un rythme plutôt lent, il arrive de manière occasionnelle qu'une question déclenche tout un emballement au niveau des échanges, et il ne fait aucun doute que les spectateurs voudront se référer et retrouver ces moments-là. 

De nos jours, il est possible de mettre cet enregistrement vidéo en ligne accompagné de liens hypertextes.

Pour les personnes qui pensent qu'un livre est mieux, je les incite à lire cet excellent et difficile ouvrage qu'est celui des Design Patterns. Imaginez un instant qu'à la place de soutirer la signification du _pattern_[^1] « Decorator » du livre, vous pouviez cliquer sur la page et voir l'un des auteurs expliquer ce _pattern_ en vidéo. Bien entendu, cet auteur ou un autre devrait utiliser les inflexions de la voix, faire des gestes pour mieux transmettre l'idée. 

La leçon à tirer de cette caractéristique humaine est que nous devrions tirer les communications de l'équipe aussi haut que possible sur la courbe en fonction de la situation.

### Les personnes ont tendance à ne pas agir de manière constante

Nous devons être prudent lorsque nous évoquons les types d'échecs d'origine humaine. « Si vous donnez à un chien un mauvais nom, autant vouloir le tuer » est un vieux proverbe anglais. En effet, comme nous allons le voir dans les deux exemples suivants, changer simplement le style de management et la culture locale peut changer profondément les comportements. Et en même temps, en me référant à mes expériences sur les projets passés, il existe une espèce de fil rouge montrant à quel point il est difficile de s'attendre à de la cohérence en terme d'actions. Jim Highsmith l'a très bien écrit \[Hi\] :

> « … ce sont des personnes, pas des rouages, à l'intérieur de la boîte. Les gens peuvent faire des choses similaires de manière répétée, mais jamais la même chose. À l'aide d'un processus étape-par-étape, nous pouvons nous attendre aux même résultats à partir des mêmes éléments en entrée, mais la réaction des gens à ces éléments peuvent varier considérablement de jour en jour en fonction de tout un ensemble de conditions, dont certaines qui n'ont aucun rapport avec la tâche en cours. »

Les personnes se satisfont d'un certain degré de souplesse quant à leur propre comportement. Je me souviens d'une des deux demandes les plus difficiles qui ait pu m'être faite, à savoir rendre une personne capable de faire quelque chose soigneusement et de manière constante jour après jour (l'autre demande la plus difficile étant de demander aux gens de changer leurs habitudes). Voici ci-dessous l'extrait d'une conversation dont j'ai été témoin récemment qui illustre ce propos :

> « Comment est-ce que je peux gérer tout ce flux de paperasses qui arrivent sur mon bureau » a demandé une personne. Une autre personne répondit : « C'est facile. Garde ton bureau propre, net, sans rien dessus, avec 4 bannettes d'un côté et quelques dossiers dans des chemises dans le tiroir du haut …  » et sa réponse s'arrêta là. « Garder le bureau sans rien dessus !? » se sont écriées les personnes dans l'auditoire à l'unisson. « Je ne peux pas faire ça ! »

Remarquez que la suggestion de bureau net leur demandait de changer à la fois leurs habitudes _et_ d'appliquer cette nouvelle habitude de manière constante.

Si les personnes pouvaient agir simplement de manière constante, ils garderaient leurs bureaux nets, éviteraient les aléas, perdraient du poids, joueraient d'un instrument de musique, et pourraient même produire du logiciel de manière régulière et dans les délais.

Comme Karl Wiegers nous le souligne avec malice « Nous ne sommes pas en manque de _pratiques_, nous sommes en manque de _pratique_  ». En voici quelques unes. Dans son ouvrage « The Science of Programming »  \[Gr\], David Gries nous donne des consignes détaillées pour dériver[^2] correctement des programmes. Les cartes CRC (Classes-Responsabilités-Collaboration) sont un bon moyen d'exploration pour la conception \[B87\]. De son côté, Extreme Programming \[EP\] utilisent des pratiques connues et très efficaces : la programmation en binôme et les tests unitaires de régression automatisés \[Je\]. Les pratiques mises en avant par la méthode Cleanroom[^3] sont quant à elles bien connues et documentées \[Mi\]. Dans Personal Software Process[^4], Watts Humphrey nous donne des préconisations détaillées sur comment les programmeurs pourraient devenir plus efficients. Appliquer de manière constante toute ou partie des idées susmentionnées devrait permettre d'améliorer les projets que j'ai pu voir.

Tout le problème réside dans le mot « constant ». Les approches PSP et Extreme Programming perdent du sens si elles sont appliquées de manière sporadique. Un fragment de code à moitié dérivé n'est pas un fragment de code sans erreur. De la même manière que la technique du bureau propre et net, elles doivent être appliquées de manière complète, constante, quotidienne.

Le manque de constance est un _type d'échec_ répandu chez les humains. Certaines méthodologies exigent une constance dans l'action, je les appelle des méthodologies à « haute discipline ». Les entretiens que j'ai fait sur les projets, indiquent que les méthodologies à haute discipline sont fragiles, même si elles sont déjà présentes dans ces projets. Ce qui suit est extrait d'une entreprise de niveau 5 en CMM[^5] est assez instructif : 

> « Durant l'été 1996, TIS a introduit la méthode PSP chez un petit groupe d'ingénieurs informatiques. Même si la formation a été plutôt bien reçue, l'utilisation de PSP chez TIS a commencé à décliner dès la fin de la formation. Et peu après, il s'est avéré qu'aucun des ingénieurs qui avaient été formés aux techniques PSP ne les utilisaient pas dans leur travail. Lorsqu'il leur a été demandé pourquoi, la raison a été unanime : "La méthode PSP est une méthode extrêmement rigoureuse et si personne ne me demande mes données, c'est plus facile de faire comme avant.". »

Pour rester utilisée, une méthodologie à haute discipline se doit d'offrir une certaine forme de support aux gens pour qu'ils puissent agir de manière constante. La méthode Cleanroom comporte des règles dites de « non-compilation » qui s'accompagnent de pratiques de gestion de projets et d'ingénierie logicielle. Extreme Programming requière à ce qu'un coach soit présent pour maintenir la pratique des pratiques. PSP n'a pas de support aussi explicite, et il n'est pas surprenant que dans ces conditions PSP ne soit plus utilisée par le groupe de personnes susmentionné par manque de structure de support. L'adjonction de TSP à PSP est censée offrir ces éléments manquants \[Web\].

Nonobstant les commentaires précédents, il y a vraiment des gens qui sont très disciplinés, de manière constante et quotidiennement (ceci pour illustrer qu'il existe une grande variabilité dans les comportements des gens). Quelques fois le simple changement de responsable d'une équipe peut modifier la constance de leurs actions. Je tiens à remercier Trygve Reenskaug pour l'anecdote qui suit - elle permet d'illustrer à quel point le style de management et l'alchimie personnel comptent beaucoup :

> Ici, avant, il y avait une boutique assez affreuse qui vendait tout un bric-à-brac. L'endroit était en désordre, et les vendeuses étaient occupées soit à se faire les ongles soit à parler au téléphone, et elles n'accordaient que très peu de temps aux clients. La boutique ferma, et une autre boutique du même genre s'ouvrit au même endroit. Cet endroit était tout simplement merveilleux ! Elle était propre, organisée et les vendeuses étaient attentives aux clients. Le seul point commun entre ces deux boutiques étaient … les vendeuses … qui étaient les mêmes !

En effet, il est bien connu que le style personnel de management a un énorme effet. Le projet Chrysler Comprehensive Compensation[^6] s'est déroulé aux alentours de 1997 \[C3\]. Au départ, l'équipe valorisait le fait de « réfléchir à l'avance », de « faire de la conception de manière fine mais extensible » et « que mon code soit privé ». L'équipe, collectivement, mais largement sous l'impulsion de Kent Beck, s'est reconstruite autour de valeurs cœurs « faire les choses simplement et clairement, nous pourrons ajouter la finesse plus tard », « tout le code est public, n'importe quel binôme peut se constituer et peut changer n'importe quel bout de code ».  Ces mêmes personnes ont donc adoptées des valeurs cœurs différentes et sont passées du désarroi, de la non-communication, de la non-livraison à une application constante d'un ensemble de pratiques à haute discipline, à des livraisons régulières sur une période de trois ans.

### Être un bon citoyen[^7] et être bon à fouiller un peu partout 

Trois facteurs de réussites permettent de contrer le problème de constance :

- les personnes veulent, en général, être de « bons citoyens »,
- les personnes prennent l'initiative
- les personnes sont douées pour fouiller un peu partout

Lorsque je fais un entretien sur un projet, je pose toujours la question qu'est ce qui leur a permis de réussir en fin de compte. La seule réponse qui revient régulièrement : « Une poignée de bonnes personnes arrivent à points nommés et font ce qu'il faut pour que le travail soit fait ». C'est exactement une phrase similaire à celle-ci qui fût écrite dans le manuel de la NASA intitulé « Leçons apprises sur le logiciel de vol de désorbitage »  \[NASA\]:

> « \[L'élément\] peut être le plus important pour le long terme, pendant toute la durée du projet, est d'avoir une équipe cœur pour le développement rapide du nouveau système de guidage, navigation et contrôle (GN&C). Cela implique de trouver des personnes compétentes : de les former et de les faire monter en compétences sur les outils, sur les processus et les méthodologies, et de les intégrer dans une équipe soudée.  


> « Après les avoir fait travailler ensemble sur le langage de définition d'enregistrements (ou RDL pour Record Definition Language - NdT) pendant un an, les membres de l'équipe auront acquis l'expertise nécessaire sur les méthodes, outils et domaines. Une _atmosphère aidante, coopérative est encouragée_, ce qui a permis d'organiser des formations interdisciplinaires. Une volonté commune de la part des membres de l'équipe _d'affronter tous les problèmes de toute nature_ pendant le projet s'est avéré inestimable plus d'une fois … » (j'ai ajouté la partie en italique pour mettre en valeur cette partie de phrase).


> … cette équipe peut s'avérer être un atout sur le long terme que ce soit au niveau de sa division qu'à celui de l'agence. 

Qu'est ce qui provoque ce type de comportement chez les gens ? Une réponse possible est : « être de bons citoyens » en terme professionnel.

Il se peut que nous puissions augmenter le taux de réussite des projets en augmentant le « sentiment d'appartenance à une communauté et le sens civique associé » au sein d'une équipe. En réalité, je ne mets pas cette recommandation en haut de la liste parce que je trouve que le sens civique est généralement suffisamment élevé, et que certains managers profitent déjà trop de ce sentiment (voir par exemple, le texte Death March \[Yo\]).

Toutefois, cette idée révèle un élément rarement mentionné dans la conception de méthodologie.

_“Communité et citoyenneté professionnel”_

Cette activité devrait faire partie à part entière au sein des activités principales d'un projet et de ses indicateurs, au moins au même niveau que la « revue de code et le test ». Je suis heureux de dire que plusieurs des projets que j'ai pu voir ont ce type d'activité de manière explicite. Ils les utilisent pour garder des canaux de communication de personne-à-personne en bonne position (il est inutile de dire que ces projets maximisent aussi la communication en face-à-face). Toutefois, je ne l'ai pas encore vu mentionnée par écrit en tant que tel dans une quelconque méthodologie ou dans un quelconque processus. 

Le second facteur de réussite est lorsque les personnes prennent des initiatives. Cela va de concert avec la bonne citoyenneté et être _bon à fouiller un peu partout_, pour produire un facteur de réussite bien connu à savoir « une poignée de bonnes personnes arrivent à points nommés ». 

« Bon à fouiller un peu partout » est une phrase un petit peu vague mais qui comporte de grands effets. Les personnes qui trient des papiers créées souvent de petits tas non triés, avec la technique du tri par insertion. Ce qui est surprenant en les observant c'est qu'assez souvent elles ne trient jamais les petits tas. L'a-peu-près est suffisant. En effet, ces personnes savent qu'elles peuvent rapidement chercher dans ce tas à la demande et elles se rappellent souvent où est « approximativement » l'élément recherché (de futures études devraient traiter des techniques d'ancrage mémorielles).

Nous essayons généralement de créer des documents de conception qui soient bons, précis et à jour. Étant donné que la non constance en terme d'action est un facteur d'échec, nous pouvons prédire de manière quasi-certaine que la documentation ne sera pas à jour. En fait, je n'ai pas encore vu de projets ayant réussi qui ait une documentation à jour, à moins que le code ou la documentation ait été générée automatiquement. J'ai toutefois vu un projet échoué parce qu'il avait été demandé aux développeurs de mettre à jour tous leurs documents de conception chaque fois qu'ils devaient changer quelque chose. Le coût du développement s'avéra tout simplement trop élevé, et l'avancement du projet trop lent, et peu de temps après, le projet fût abandonné.

J'ai demandé aux personnes de la maintenance comment ils géraient la mise à jour des programmes informatiques avec de la documentation obsolète. Leur réponse a été qu'ils « fouillaient un peu partout » et qu'ils ne faisaient pas confiance à la documentation de toute façon — ils regardaient le code tout simplement.

J'en suis venu moi aussi à m'appuyer sur ce facteur humain de réussite « être bon à fouiller un peu partout » dans les projets ainsi que dans la conception de méthode.

La traçabilité des documents est très couteuse à mettre en place et à maintenir, particulièrement en raison de la faiblesse des humains en matière de constance comme évoqué plus haut, je recommande donc d'avoir un niveau de traçabilité et de documentation de conception « juste suffisant » afin que la personne qui cherche quelque chose soit en mesure de savoir approximativement où chercher. Leurs yeux et leur intelligence feront la suite. Même s'il est peu probable que le niveau de traçabilité et de documentation soit maintenu sur la plupart des projets (et cela n'est pas très important, parce que les gens font leur travail davantage à partir de ce qu'ils ont appris en discutant avec les personnes sachantes qu'à travers la lecture des documents). 

Trygve Reenskaug m'a donné un autre exemple. Il avait proposé un système de conception assisté par ordinateur à un ingénieur concevant des plate-formes d'extraction de pétrole en mer. Trygve lui a évoqué que le système pouvait apporter de la plus-value en retraçant tous les changements faits au niveau de la plateforme. L'ingénieur a répliqué « faites juste en sorte que votre système enregistre les numéros de téléphone des personnes qui ont travaillé sur chaque partie. Je les appellerai en cas de besoin pour en savoir plus ».

Le terme méthodologique officiel que j'utilise est « basse précision » (NdT - ou à grosse mailles à la préférence de la lectrice ou du lecteur) \[Co98\]. J'ai découvert que la plupart des projets fonctionnent correctement avec des descriptions de basses précisions : les plans projets de basse précision sont plus faciles à lire, à modifier et à négocier. Les diagrammes d'architecture de basse précision sont plus faciles à se souvenir, les tables d'exigence de basse précision sont plus faciles à prioriser et peuvent être évaluer plus tôt dans le projet, la documentation de conception de basse précision sont plus faciles d'accès pour un lecteur pour avoir uniquement une « idée » de la conception — puis en le laissant regarder autour.

Les artefacts de basse précision utilisent les forces des gens pour réduire les coûts de développement. Ils se basent sur leurs capacités à « fouiller un peu partout » et sur la communication en face-à-face, tout en étant permissif sur la non constance de mise à jour. Je les ai utilisés et j'ai obtenu de bons résultats dans les projets depuis 1994, et je les recommande désormais en tant qu'élément central méthodologique.

### De la variation des personnes

Certaines personnes aiment faire des listes et d'autres non. Certaines personnes travaillent mieux le soir, d'autres mieux le matin. Certaines personnes aiment les dates butoirs, d'autres non. Certaines cultures valorisent l'autocritique publique, d'autres protègent les gens de toute forme d'embarras, et ainsi de suite.

Les méthodologies sont grosso modo un ensemble de règles de coordination de groupe, et par conséquent, une recommandation qui s'avère appropriée pour une personne ou un groupe sera rejeté par un autre. Dans le même ordre d'idée, ce qui s'applique à un groupe habitué à faire des consensus pourrait ne pas s'appliquer à une culture dans laquelle les personnes attendent que le patron prenne position.

Parmi les projets listés dans le tableau précédent, j'ai remarqué que deux exemples réussis de processus à haute discipline avaient été faits au sein de IBM Federal Sector Division et dans l'Air Force. Je n'ai pas encore vu de réussite de processus à haute discipline dans des contextes marchands. Je suis tenté d'en conclure qu'il existe certains facteurs de réussite dans les contextes gouvernementaux ou militaires qui permettent à des méthodologies plus contraignantes de survivre. Il y a une phrase qui revient dans les quelques groupes que j'ai pu interroger dans ces contexte :« nous aimerions travailler de manière plus légère, plus efficace, mais … » suivi d'une référence soit à un processus militaire standard soit à une difficulté de pouvoir contrôler les prestataires. Il serait intéressant de savoir s'il s'agit de facteurs intrinsèques ou culturels qui « tolèrent » simplement cette lourdeur.

Les méthodologies actuelles sont écrites pour imposer des cultures professionnelles et des manières de travailler dans une organisation cible. Comme cela a pu être écrit précédemment, un groupe peut la rejeter, et souvent le fait purement et simplement.

Les variations sur le plan culturel sont souvent pour les méthodologistes encore plus difficiles à incorporer que les variations individuelles quotidiennes. Au jour d'aujourd'hui, il n'existe aucune méthodologie (y compris la mienne) à ma connaissance qui prennent en compte les problèmes culturels, même si je connais des personnes qui sont suffisamment sensibles aux cultures locales pour formuler des recommandations particulières dans les projets.

### Autres caractéristiques

Je me repose aussi sur certaines autres caractéristiques sur lesquelles je ne m'attarderai pas. Voici celles que je retiens en priorité :

> _**Apprentissage**_. Les gens apprennent en regardant et en faisant. C'est un principe social et cognitif bien connu de certains cercles \[La\], mais pas encore très bien utilisé en développement logiciel. J'ai cherché différentes occasions pour l'appliquer mais je n'ai pas encore créé une structure méthodologique pouvant le faire pour l'instant.

> _**Flux**_. Le « flux » dans un contexte de développement logiciel fait référence à un moment de production intellectuelle silencieuse et efficace \[Dm\], \[Cs\], \[Co98\]. Les temps de flux doivent être contrebalancés avec des moments de communication. Comment équilibrer ces différents moments dans un projet est au-delà de ma compréhension actuelle. Toutefois, un certain nombre de personnes interrogées l'ont signalé comme étant un facteur de réussite notable dans les projets.

> _**Travailler à partir d'exemples**_. Certains psychologues cognitifs affirment avec conviction que nos mécanismes déductifs se construisent à partir d'exemples de problèmes spécifiques \[J-L\]. Les cartes CRC et les cas d'utilisation sont deux mécanismes de développement logiciel orienté exemples qui sont cités systématiquement par leurs utilisateurs comme étant deux outils efficaces. Les « diagrammes d'instance » sont souvent les diagrammes préférés des nouveaux venus en conception orienté objet, et sont d'ailleurs toujours utilisés régulièrement par les concepteurs chevronnés. Par contre, la documentation basée sur des exemples n'a pas encore eu l'attention qu'elle mérite de la part des méthodologistes ; elle est l'objet d'un prochain travail d'études.

> _**Approche kinesthésique ou multi-sensoriel**_. Que ce soit les cartes CRC, les jeux de rôle, la conception sur tableau blanc, le prototypage papier d'interface utilisateur, toutes ces techniques tirent profit de l'aptitude des personnes de parler, de se mouvoir, ou de jouer un rôle tout en réfléchissant. Il y a peu ou pas de recherches sur ce sujet, mais je trouve l'utilisation de ces techniques comme étant très significative dans la conception logiciel.

> _**Type de personnalité**_. Nous avons vu précédemment qu'une non-communication de la part du concepteur en chef peut aliéner son équipe, et qu'en même temps, il est demandé de manière répétée aux programmeurs de développer leurs compétences en matière de communication. Nous avons rencontré des responsables de projets qui sont incapables de prendre des décisions. L'adéquation du type de personnalité d'un individu avec le poste qui lui est attribué a un large effet au niveau des résultats d'un projet. Cette adéquation devrait être ajustée par rapport à ce qu'il y a de mieux concernant le développement personnel de l'individu, mais il arrive souvent que se voir attribuer un poste de manager constitue la seule voie de progression de carrière pour une personne. 

>_**Échec conservateur**_. Il a été clairement établit que les gens préfèrent échouer de manière conservatrice plutôt que réussir en prenant un risque \[Pi\]. Ceci peut expliquer pourquoi le développement en cascade continue toujours à être utilisé après toutes ces décennies de problèmes et l'avènement progressif des techniques de développement en spirale, incrémental et itératif.

>_**Changement d'habitudes**_. Faire changer les gens d'habitudes est la chose la plus dure que je connaisse. Et en même temps, les gens peuvent changer d'habitudes quasi instantanément, et changer du tout au tout au niveau de leurs systèmes de valeurs. J'ai été témoin de tels changements, faits de manière délibérée et en toute conscience peut être deux fois en 20 ans, et c'est impressionnant. Nous aurions besoin de mieux connaître ce type de phénomène.

>_**Petites têtes**_. Même les concepteurs experts le répètent régulièrement « J'arrive uniquement à me souvenir d'une petite quantité d'informations ». Différentes techniques de documentation ont essayé de palier cette faiblesse, mais aucune n'est arrivée à combiner l'utilisation d'artéfact de basse-précision avec une communication interpersonnelle élevée.

Je suis certain qu'il existe d'autres caractéristiques relatives aux personnes qui affectent en profondeur à la fois la manière dont fonctionnent les projets et la manière dont nous devrions faire des recommandations. En tout cas, vous savez lesquelles j'utilise actuellement.

## 4 — Conclusion

Les caractéristiques fondamentales des « personnes » ont un effet de tout premier ordre sur le développement logiciel, pas un effet de second ordre. En conséquence, comprendre les effets de premier ordre devrait devenir un élément de recherche de première importance, et ne pas être négligé, relégué en sujet de moindre importance. Je propose que ce champ d'étude devienne un sujet primordial dans le domaine de « l'ingénierie logicielle » pour les 20 à 50 prochaines années.

J'ai présenté plusieurs caractéristiques qui ont des effets notables sur la conception de méthodologie. 

> La première est que nous sommes sensibles aux rythmes et aux modalités de communication. La prédiction que je fais est que la proximité physique et la facilité de communication a un effet majeur.

> La seconde est que les personnes ont tendance à ne pas faire preuve de constance. La prédiction que je fais est que les méthodologies exigeant une forme de constance disciplinée s'avèrent fragiles en pratique.

> La troisième est que les gens changent, pas simplement quotidiennement mais aussi lorsqu'ils passent de groupes en groupes. Les méthodologies ne prennent pas en compte les variations culturelles et elles devraient être en mesure de les gérer.

> La quatrième est que les personnes aiment être de bons citoyens, qu'elles sont douées à fureter partout et qu'elles prennent l'initiative. Le tout forme le facteur de réussite « une poignée de bonnes personnes arrivent à points nommés ».

Être bon en communication et à fureter partout permettent de contrebalancer l'inconstance, ce qui conduit à faire la prédiction que les méthodologies peuvent faire bon usage des artéfacts de basse précision dont l'imprécision est couverte par la communication personnelle. L'étude des projets évoquée dans ce rapport permet d'étayer cette prédiction, elle-même sujette à une certaine forme de montée en compétence du personnel, y compris la chaîne managériale.

Dans le titre de cet article, je fais référence aux personnes comme étant des « composants ». Effectivement, dans la littérature de conception de processus/méthodologie, c'est ainsi que les personnes sont qualifiées. L'erreur dans cette approche est que les « personnes » (au contraire d'un composant - NdT) font preuve d'une grande variabilité et d'une grande non-linéarité qui s'accompagnent d'une ensemble de facteurs-clés de succès et d'échecs uniques. Ces facteurs sont primordiaux et ne sont pas à négliger. Le fait de ne pas prendre en compte de ces éléments par les concepteurs de processus et de méthodologies expliquent en partie les trajectoires imprévisibles que nous pouvons constater sur certains projets.

Pour finir, il devrait être claire que nous pourrions faire davantage de recherches sur ce sujet. J'espère qu'il y aura davantage de chercheurs pour relever ce défi qu'il y en a eu depuis la rédaction, il y a 30 ans, par Weinberg de sa version du présent article. J'attends avec impatience, en particulier, de nouvelles recherches en psychologie et en ethnographie pour découvrir d'autres effets de premier ordre que ceux mentionnés ici. 

## Références

\[B87\] Beck, K. and Cunningham, W., “A laboratory for teaching object-oriented thinking”, Proceedings of the OOPSLA Conference, 1987, ACM Sigplan Oct., 1987, pp.1-7.

\[B99\] Beck, K., Extreme Programming Explained: Embrace Change, Addison Wesley Longman, 1999.

\[Br\] Britcher, R., The Limits of Software, Addison Wesley, 1999.

\[Ch\] Christensen, M., _et al._, “The M.A.D. experience: multiperspective application development in evolutionary prototyping”, in the ECOOP’98 proceedings, Lecture Notes in Computer Science, Vol. 1445, Goos, G., Hartmanis, J, van Leeuwen, J., eds., 1998, pp. 13-41.

\[Ci\] Citrin, W., Cockburn A., von Kaenel, J., Hauser, R., “Using formalized temporal message†‘flow diagrams,” Software Practice and Experience, 1995.

\[Co94\] Cockburn A., “In search of methodology,” Object Magazine, July 1994.

\[Co95\] Cockburn A., “Unraveling incremental development,” Object Magazine, Jan. 1995.

\[Co98\] Cockburn A., Surviving Object-Oriented Projects, Addison Wesley, 1998.

\[Co98p\] Cockburn A., Position statement for “Software development and process” panel, ECOOP ‘98, online at [http://members.aol.com/acockburn/papers/Ecoop98panel.htm](https://web.archive.org/web/20140329203655/http://members.aol.com/acockburn/papers/Ecoop98panel.htm)

\[Co00\]Cockburn A., Crystal(Clear): A human-powered software development methodology for small teams, Addison Wesley, in prep. Online at [http://members.aol.com/humansandt/crystal/](https://web.archive.org/web/20140329203655/http://members.aol.com/humansandt/crystal/) clear.

\[Cs\] Csikszentmihalyi, M., Flow: The Psychology of Optimal Experience, Harper Perennial, 1990

\[C3\] The C3 Team, “Chrysler goes to ‘Extremes’”, in Distributed Object Computing, October, 1998, pp. 24-28.

\[Dm\] DeMarco, T., Lister, T., Peopleware 2nd Edition, Dorset House, 1999.

\[EP\] Extreme Programming, web notes, start from www.extremeprogramming.com.

\[Gr\] Gries, D, The Science of Programming, Springer Verlag, 1987.

\[Ha\] Harel, D., Politi, M., Modeling Reactive Systems with Statecharts, McGraw-Hill, 1998.

\[Hi\] Highsmith, J., Adaptive Software Development, Dorset House, 1999.

\[Ho\] Hovenden, F., “An ethnographic account of writing use cases on an IT project”, Humans and Technology Technical Memo, 1999.10.30, online at [http://members.aol.com/humansandt/papers/ethno1.htm.](https://web.archive.org/web/20140329203655/http://members.aol.com/humansandt/papers/ethno1.htm.)

\[Hu\] Humphrey, W., A Discipline for Softwrae Engineering, Addison Wesley, 1995.

\[Je\] Jeffries, R., “Extreme testing”, in Software Testing and Quality Engineering, March/April, 1999, pp. 23-26.

\[J-L\] Johnson-Laird, P. and Byrne, R. Deduction, Lawrence Erlbaum Associates, 1991.

\[La\] Lave, J., Situation Learning: Legitimate Peripheral Participation, Cambridge Press, 1991.

\[Mi\] Mills, H., Dyer, M., Linger, R., “Cleanroom Software Engineering,” IEEE Software Vol 2 (1984) No. 9, 19-24.

\[NASA\] JSC38609, “Deorbit flight software lessons learned”, NASA Johnson Space Center, Jan 19, 1998 online at

\[Pi\] Piatelli-Palmarini, M., Inevitable Illusions : How Mistakes of Reason Rule Our Minds, Wiley & Sons, 1996.

\[Pl\] Plowman, L., “The interfunctionality of talk and text”, Computer Support of Cooperative Work, vol. 3, 1995, pp.229-246.

\[Si\] Sillince, J.A., “A model of social, emotional and symbolic aspects of computer-mediated communication within organizations”, Computer Support of Cooperative Work vol. 4, 1996, pp. 1-31.

\[Web\] Webb, D., Humphrey, W., “Using TSP on the TaskView Project”, in _CrossTalk, The Journal of Defense Software Engineering_, Feb 1999, pp. 3-10, online at [http://www.stsc.hill.af.mil/crosstalk/1999/feb/webb.asp](https://web.archive.org/web/20140329203655/http://www.stsc.hill.af.mil/crosstalk/1999/feb/webb.asp)

\[Wei\] Weinberg, J., The Psychology of Computer Programming, Silver Edition, Dorset House, 1998.

\[Yo\] Yourdon, E., Death March Projects, Prentice Hall, 1997.

[^1]: Les _design patterns_ ou patron de conception sont un ensemble de solutions standards ou de bonnes pratiques pour répondre à des besoins récurrents en terme de programmation - pour en savoir plus, vous pouvez consulter cet [article Wikipedia](https://fr.wikipedia.org/wiki/Patron_de_conception)
[^2]: L'expression est difficile à rendre en français. Le terme original est "for deriving correct programs"  fait référence, via l'ouvrage de David Gries, à une méthode préconisée par Edsger W. Dijkstra d'obtenir un exécutable à travers la dérivation d'une spécification écrite avec un langage formel (c'est-à-dire utilisant une notation mathématique) d'un programme informatique en spécification technique - NdT
[^3]: La métaphore dont s'inspire cette méthodologie est celle de la salle blanche en électronique où tout est fait en terme de prévention des anomalies, pour en savoir davantage, vous pouvez consulter cet [article](https://en.wikipedia.org/wiki/Cleanroom_software_engineering) Wikipedia 
[^4]: Le Personal Software Process ou Processus personnel informatique est un processus de développement logiciel 
[^5]: Il s'agit du projet qui fût le terrain de jeu d'Extreme Programming, qui consistait à refondre la gestion de la paye de l'entreprise Chrysler
[^6]: CMM - Capability Maturity Model est un modèle permettant de mesurer le degré de maturité d'un projet en terme de compétences, processus et techniques 
[^7]: le concept de « bon citoyen » en entreprise va au-delà de la conscience professionnelle. La dénomination complète du concept est celle de « comportement de citoyenneté organisationnelle », pour en savoir plus, vous pouvez consulter cet [article Wikipedia](https://en.wikipedia.org/wiki/Organizational_citizenship_behavior) en anglais ou [cet autre c'est par ici](https://status.net/articles/what-is-organizational-citizenship-behavior-ocb-types-examples/) en anglais ou [par là](https://shs.cairn.info/revue-rimhe-2018-2-page-3?lang=fr) en français

---
Auteur : [Alistair Cockburn](https://alistaircockburn.com/Bio)  
Source : [Characterizing people as non-linear, first-order components in software development](https://web.archive.org/web/20140329203655/http://alistair.cockburn.us/Characterizing+people+as+non-linear,+first-order+components+in+software+development)  
Date de parution originale : 21 octobre 1999  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 23/01/2026  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

Traduction faite main sans IA.  
![Logo Fait (Hu)Main]({{ site.url }}assets/lta/FaitHuMain_hor_N_2.png)

Logo « Fait (Hu)Main » par [Lazar Baruk](https://lazarbaruk.itch.io/pack-de-logos-fait-humain)

{% include share_buttons.html %}

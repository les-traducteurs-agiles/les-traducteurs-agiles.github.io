---
layout: post
title:  "Less - Approche systémique"
date:   2020-04-10 14:46
published: false
tags:
- tag1
- tag2
---

# Systems Thinking

# Approche systémique

I took a speed reading course and read “War and Peace” in twenty minutes. It involves Russia.
—Woody Allen

J'ai pris un cours de lecture rapide et j'ai lu « Guerre et Paix » en vingt minutes. Cela parle de la Russie.

“No matter what we do, the number of defects in our backlog remains about the same,” a manager told us; this for a 15 MSLOC C and C++ product with several hundred developers where we were working. What’s going on? Systems thinking may help. In small groups the forces at play are more quickly seen and informally understood, but in large product development—or any large system—it’s tough. Gerry Weinberg highlights two decisive factors in this situation:

« Quoi que nous fassions, le nombre d'anomalie dans notre _backlog_ reste le même. » nous a dit un jour un manager en évoquant un produit de près de 15 millions de lignes de code sur lequel plusieurs centaines de développeurs étaient en train de travailler. Que pouvait-il bien se passer ? L'approche systémique peut s'avérer utile dans ce cas comme dans d'autres. En petits groupes, les forces en présence peuvent rapidement être identifiées et comprises spontanément, mais dans le cadre du développement d'un gros produit ou de n'importe quel gros système, c'est difficile. Gerry Weinberg met en avant deux facteurs décisifs dans ce genre de situation :

> **Weinberg-Brooks’ Law**: More software projects have gone awry from management’s taking action based on **_incorrect system models_** than for all other causes combined.
>
> **Causation Fallacy**: Every effect has a cause… and we can tell which is which. [[Weinberg92]](http://www.amazon.com/Quality-Software-Management-Systems-Thinking/dp/0932633226/ref=sr_1_1?ie=UTF8&qid=1413527418&sr=8-1&keywords=Quality+Software+Management%3A+Systems+Thinking)

> **Loi de Weinberg-Brooks** : De plus en plus de projets informatiques sont partis de travers après que l'encadrement ait pris des décisions basées sur des **modèles systémiques incorrects** plus que pour toutes autres causes combinées.
>
> **Erreur de causalité** : Chaque effet a une cause … et nous pouvons dire desquelles il s'agit. [[Weinberg92]](http://www.amazon.fr/Quality-Software-Management-Systems-Thinking/dp/0932633226/ref=sr_1_1?ie=UTF8&qid=1413527418&sr=8-1&keywords=Quality+Software+Management%3A+Systems+Thinking)

These reflect the impact of our **mental models** on the system, a subject that will be revisited later in this section.

Ces deux facteurs reflètent bien l'impact de nos **modèles mentaux** sur le système, un sujet que nous reverrons plus tard dans cette section.

Problems stemming from mental models and assumptions are one issue. Another is that large-scale adoption of Scrum, lean thinking, and agile principles is not isolated to the development group. It bumps into product management, budgeting, beta-testing, launch, and governance and HR policies. Accordingly, in large-scale agile adoption it is useful to be able to get together with colleagues and _effectively reason_ about the mental models, causal relations, feedback loops, and control mechanisms (or illusions of control) in a big system that is about to be seriously _perturbed._ Systems thinking is one of those reasoning tools.

Les problèmes résultant de nos modèles mentaux et de nos postulats sont un point à traiter. Un autre point est l'adoption à grande échelle de Scrum, de l'approche lean et des principes agiles en dehors du domaine du développement. Ce point a fait irruption dans la gestion de produit, les budgets, les tests, la commercialisation, la gouvernance et la politique RH. En conséquence, dans les adoptions agiles à grande échelle, il est utile de se réunir avec les collègues et de _réfléchir en profondeur_ sur les modèles mentaux, les relations causales, les boucles de _feedback_ et les mécanismes de contrôles (ou les illusions de contrôle) dans un gros système qui va être sérieusement _pertubé_. L'approche systémique est l'un de ces outils de réflexion.

In 1958, the _Harvard Business Review_ published [“Industrial Dynamics: A Major Breakthrough for Decision Makers,”](https://kupdf.com/download/industrial-dynamics-a-major-breakthrough-for-decision-makers_5902479bdc0d603940959ed5_pdf) a landmark paper by Jay Forrester, MIT Sloan School professor. This paper spurred the movement of systems thinking in business education, and the MIT Sloan School of Management became known for educating people in **system dynamics**. System dynamics is sometimes treated as a synonym for **systems thinking** , though the latter is a more general term.

En 1958 la _Harvard Business Review_ a publié un article de Jay Forrestor, professeur au MIT Sloan School, qui a fait date [“Industrial Dynamics: A Major Breakthrough for Decision Makers,”](https://kupdf.com/download/industrial-dynamics-a-major-breakthrough-for-decision-makers_5902479bdc0d603940959ed5_pdf). Cet artcile a lancé le mouvement de l'approche systémique dans le domaine des formations de gestion d'entreprise et la MIT Sloan School of Management devient célèbre pour former les gens à à la **dynamique systémique**. La dynamique systémique est quelques fois vu comme étant synonyme d'**approche systémique**, même si ce dernier est un terme beaucoup plus général.

MIT also attracted other system-dynamics-oriented researchers such as Peter Senge.<sup>[1](https://less.works/less/principles/systems-thinking.html#footnote-1)</sup>

Le MIT a également attiré d'autres chercheurs intéressés par la dynamique systémique tel que Peter Senge<sup>[1](https://less.works/less/principles/systems-thinking.html#footnote-1)</sup>

Consistent with _Weinberg-Brook’s Law_, Forrester’s research showed that decision makers who were given dynamic models of a business system and asked to improve their output performance, _usually made them run worse_ [[SKRRS94]](http://www.amazon.com/The-Fifth-Discipline-Fieldbook-Organization/dp/0385472560/ref=sr_1_fkmr0_3?ie=UTF8&qid=1413528034&sr=8-3-fkmr0&keywords=The+Fifth+Discipline+%EF%BF%BCFieldbook). The observation was that most people have weak judgement on how to fundamentally improve systems, usually applying incorrect “common sense” and quick-fix ‘solutions’ that do not create long-lasting systemic improvement.

En corrélation avec la loi de _Weinberg-Brook_, Jay Wright Forrester a montré que les décideurs à qui il avait été donné des modèles dynamiques de systèmes opérationnels et à qui il avait été demandé d'améliorer la performance opérationnelle, _n'avaient fait  généralement qu'empirer les choses_ [[SKRRS94]](https://www.amazon.fr/guide-lorganisation-apprenante-d%C3%A9velopper-lintelligence/dp/2212568711/). Il en est ressorti que la plupart des personnes évaluaient mal la manière dont il faut améliorer les systèmes, et appliquaient généralement leur « bon sens », en mettant en place des solutions de fortune qui n'apportent aucune amélioration systémique à long terme.

Why is the behavior of a large development group (a system) not understood or guided skillfully? The answer lies, in part, in the behavior of stochastic systems with queues and variability, as explored in the [Queueing Theory](https://less.works/less/principles/queueing_theory.html) LeSS principle. And the same answer lies in _control theory_: Most systems of interest—such as a product development group—have complex positive and negative feedback loops and nonlinear behavior. The behavior of these systems defies our gut instinct. And then there is the minor issue of _people_.

Pourquoi le comportement d'un grand groupe de développement (un système) n'est-il pas compris ou guidé de manière compétente ? La réponse réside, en partie, dans le comportement de systèmes stochastiques avec les files et les variabilités comme nous avons pu l'évoquer avec le principe LeSS de la [théorie des files d'attentes](http://www.les-traducteurs-agiles.org/2017/01/29/less-theorie-des-files-d-attente.html). Et la même réponse est présente aussi dans la _théorie du contrôle_ : la plupart des systèmes d'intérêt - tel qu'un groupe de développement de produit - ont des boucles de retours d'informations positives et négatives ainsi qu'un comportement non linéaire. Le comportement de ces systèmes défient notre instinct. Et puis il y a la problématique mineure des _gens_.

In summary, reasons for not being skillful in fathoming or guiding a big system include (but are not limited to):

En résumé, les raisons expliquants l'incompétence à maîtriser ou à guider un gros systèmes sont (liste non exhaustive) :

* lack of knowledge about the system dynamics, feedback loops, nonlinear systems behavior, and unintended consequences in workplace systems

* un manque de connaissance des dynamiques du système, des boucles de retours d'informations, du comportement non linéaire des systèmes, et des conséquences inattendues dans les systèmes sur le lieu de travail.

* not understanding root causes of problems (and how to find)

* une incompréhension des causes racines des problèmes (et de comment les trouver)

    * _causes,_ not cause; in systems thinking one sees that there are multiple, indirect, and dynamic causes to problems

    * _les causes_, non la cause ; en approche systémique, nous savons que les causes des problèmes sont multiples, indirectes et dynamiques

* not knowing if or why quick-fix or local-department decisions degraded overall delivery performance.  

* l'incapacité à savoir si ou pourquoi une solution de fortune ou une décision locale dégrade la performance globale opérationnelle.

In short, not being systems thinkers.<sup>[2](https://less.works/less/principles/systems-thinking.html#footnote-2)</sup>

En bref, ne pas être des théoriciens/penseurs/pratiquants systémiques.<sup>[2](https://less.works/less/principles/systems-thinking.html#footnote-2)</sup>

These reasons are consequential at the intersection of management and large-scale adoption of lean and agile principles. The leadership team is part of the system being perturbed; if they do not apply systems thinking, they could _really_ perturb it—and not in a good way!

Ces raisons sont la conséquence de l'intersection du management et de l'adoption des principes lean et agile. L'équipe de direction fait partie du système qui est pertubé ; si elle n'applique pas l'approche systémique, elle pourrait _vraiment_ le perturber - et pas de la bonne façon.

As a summary of systems thinking insight, we like the [11 ‘laws’](https://en.wikipedia.org/wiki/The_Fifth_Discipline#The_11_Laws_of_the_Fifth_Discipline) described in [The Fifth Discipline](http://www.amazon.com/Fifth-Discipline-Practice-Learning-Organization-ebook/dp/B000SEIFKK/ref=sr_1_1?ie=UTF8&qid=1413531002&sr=8-1&keywords=the+fifth+discipline):

Les points-clés à retenir de l'approche systémique peuvent être résumé dans les [11 lois](https://en.wikipedia.org/wiki/The_Fifth_Discipline#The_11_Laws_of_the_Fifth_Discipline) décrites dans la [Cinquième discipline](https://www.amazon.fr/cinqui%C3%A8me-discipline-organisations-apprenantes-dexemplaires-ebook/dp/B017WSYAHG)

* Today’s problems come from yesterday’s ‘solutions.’
* The harder you push, the harder the system pushes back.
* Behavior will grow worse before it grows better.
* The easy way out usually leads back in.
* The cure can be worse than the disease.
* Faster is slower.
* Cause and effect are not closely related in time and space.
* Small changes can produce big results…but the areas of highest leverage are often the least obvious.
* You can have your cake and eat it too—but not all at once.
* Dividing an elephant in half does not produce two small elephants.
* There is no blame.

* Les problèmes d'aujourd'hui viennent des solutions d'hier
* Plus vous poussez, plus le système pousse en retour
* Le comportement empirera d'abord avant de s'améliorer
* La manière la plus facile de s'en sortir conduit souvent à faire quelques pas en arrière
* Le médicament peut être pire que la maladie
* Plus vite c'est plus lentement
* Les causes et les effets ne sont pas étroitement liés dans l'espace et le temps
* De petits changements peuvent produire de gros résultats … mais les zones où l'effet de levier est le plus important sont souvent les moins évidentes
* Vous pouvez avoir votre gâteau et le manger aussi - mais pas en une seule bouchée
* Couper un éléphant en deux ne produit pas deux petits éléphants
* Il n'y a aucun reproche à faire

Toyota’s internal motto is [“Good **thinking**, good products.”](http://www.toyota-global.com/company/toyota_traditions/quality/may_jun_2005.html) Systems thinking is a set of _thinking_ tools to help…

La devise de Toyota en interne est [« Une bonne **réflexion**, de bons produits »](http://www.toyota-global.com/company/toyota_traditions/quality/may_jun_2005.html). L'approche systémique est un jeu d'outils de réfexion pour aider …

* **see system dynamics**—a development organization is a system of people and policies with subtle feedback loops and unintended consequences

* **à voir les dynamiques de systèmes** - une organisation de développement est un système de personnes et de règles avec de subtiles boucles de retours d'informations et des conséquences inattendues

    * we can learn to see and thus improve the system with **causal loop diagrams** created in a workshop

    * nous pouvons apprendre à voir et ainsi à améliorer le système avec des **diagrammes de boucles causales** faits lors d'un atelier

* **see mental models**—one reason behind suboptimal decisions is mistaken assumptions and faulty reasoning

* **à percevoir les modèles mentaux** - parmi les raisons derrière des décisions sous-optimales se trouvent des hypothèses erronées et des raisonnements incorrects

    * causal loop diagramming and Five Whys expose these

    * les diagrammes de boucles causales et les cinq pourquoi permettent de révéler tout ça

* **see local optimization**—another source of suboptimal decisions is **local optimization** , making the ‘best’ decision from the viewpoint of a person or department, rather than **global optimization** for the lean systems-level goal of _deliver value fast with high quality and high morale_ .  

* **à voir les optimisations locales** - une autre source de décisions sous-optimales est **l'optimisation locale**, autrement dit prendre la « meilleure » décision du point de vue d'une personne ou d'un département, au détriment d'une **optimisation globale** qui est l'objectif au niveau système _lean_ que de pouvoir _livrer la plus grande valeur possible de très grande qualité avec un moral d'acier_

This introduction is organized around the following areas in systems thinking: Learning to see (1) _system dynamics_ , (2) _mental models_ , (3) _root causes_ , and (4) _local optimization_ .

Cette introduction à l'approche systémique est présenté autour des domaines suivants : Apprendre à voir (1) _les dynamiques du système_, (2) _les modèles mentaux_, (3) _les causes racines_, et (4) _l'optimisation locale_.

## Seeing System Dynamics: Introduction

## Voir les dynamiques du système : Introduction

### Static versus Dynamic Complexity

### Complexité statique versus complexité dynamique

Many of us, especially in engineering and finance, are educated to master **complexity of static details**—learning to analyze and manage information (requirements, financial analysis, …), decompose complex structures into simpler ones, and so forth. That is, complexity of a static, information, or structural nature.

La plupart d'entre nous, notamment les ingénieurs et les financiers, ont été formés pour maîtriser la **complexité de détails statiques** - en apprenant à analyser et à gérer l'information (exigences, analyses financières, …), à décomposer des structures complexes en structures simples, et ainsi de suite. C'est-à-dire, la complexité d'une information qui est par nature structurellement statique.

Why do big software systems tend to degrade, with more and more time spent on defects? What might happen if the USA invades Iraq? Seeing the dynamics behind these questions involves analysis of the **complexity of dynamics** .

Pourquoi les gros systèmes informatiques ont-ils tendance à se dégrader avec de plus en plus de temps passé surles anomalies ? Qu'est-ce qui pourrait bien se passer si les États-Unis d'Amérique envahissait l'Irak ? Voir les dynamiques derrière ces questions implique d'analyser la **complexité des dynamiques**.

In contrast to static-details education, many of us receive no _formal_ education in analyzing _dynamics_ complexity<sup>[3](https://less.works/less/principles/systems-thinking.html#footnote-3)</sup>, especially workplace dynamics. Perhaps there is a belief it is sufficient to rely on common sense in the workplace. Forrester demonstrated that “common sense” is just not so in complex systems, and showed it is possible to formally educate people to become better system dynamics thinkers in the workplace using _dynamic system models_ visualized in _flow diagrams_ [[Forrester61]](http://www.amazon.com/Industrial-Dynamics-Jay-Wright-Forrester/dp/1614275335/ref=sr_1_1?ie=UTF8&qid=1413582840&sr=8-1&keywords=Industrial+Dynamics).

En contraste avec une formation sur les systèmes statiques que nous avons tous suivie, peu d'entre nous ont reçu de formation sur l'étude des systèmes dynamiques et complexes[^3] et notamment en milieu professionnel. Peut-être parce que nous avons la croyance qu'il est suffisant de s'appuyer sur le bon sens dans le milieu professionnel. Jay Wright Forrester a démontré que le « bon sens » n'est pas suffisant dans des systèmes complexes et qu'il est possible de former des personnes pour leur permettre de mieux appréhender les systèmes dynamiques en milieu professionnel en utilisant notamment des _diagrammes de flux_ [[Forrester61]](http://www.amazon.com/Industrial-Dynamics-Jay-Wright-Forrester/dp/1614275335/ref=sr_1_1?ie=UTF8&qid=1413582840&sr=8-1&keywords=Industrial+Dynamics).

Flow diagrams encompass material, financial, and information flows, stocks (variables with a quantity, such as cash or number of defects), the impact of decisions and policies, and cause-effect relations. A popular simplification is the **causal loop diagram** that focuses on cause-effect relationships and feedback loops in a system [[Sterman00]](http://www.amazon.com/Business-Dynamics-Systems-Thinking-Modeling/dp/0071179895). There are a variety of similar notations; they all show stocks (variables), causal links, and delay. In [[Weinberg92]](http://www.amazon.com/Quality-Software-Management-Systems-Thinking/dp/0932633226/ref=sr_1_1?ie=UTF8&qid=1413527418&sr=8-1&keywords=Quality+Software+Management%3A+Systems+Thinking) this is called the _diagram of effect_ .

Les diagrammes de flux peuvent s'appliquer aussi bien aux flux matériels, financiers, d'informations, de stocks (n'importe quel type de stock quantitatif comme de l'argent ou des anomalies), aux conséquences des décisions et des politiques et des relations de causes à effet. Lorsque nous pensons aux diagrammes de flux, nous pensons souventau seul diagramme de boucle causale dédié aux relations de cause à effets et aux boucles de rétroaction dans un système [[Sterman00]](http://www.amazon.fr/Business-Dynamics-Systems-Thinking-Modeling/dp/0071179895). Il existe une grande variété d'autres diagrammes qui peuvent faire figurer les stocks (quels qu'ils soient), les liens de causalités, et les retards. Dans son ouvrage,  [[Weinberg92]](http://www.amazon.com/Quality-Software-Management-Systems-Thinking/dp/0932633226/ref=sr_1_1?ie=UTF8&qid=1413527418&sr=8-1&keywords=Quality+Software+Management%3A+Systems+Thinking) Gerald Weinberg appelle cela un _diagramme d'effet_.

### The First Law of Diagramming: Model to Have a Conversation

### La première loi de la réalisation d'un diagramme : nous modélisons pour avoir une conversation

A tool to learn to see system dynamics is a causal loop diagram, ideally sketched on a whiteboard in a LeSS Overall Retrospective with colleagues. Before going further, here is the _First Law of Diagramming_

Un outil très utile pour apprendre les dynamiques d'un système est le diagramme de boucles causales - nous vous recommandons de l'utiliser notamment lors des Rétrospectives Globales LeSS sur un tableau blanc. Mais avant d'aller plus loin, voici la _première loi de réalisation d'un diagramme_.


> **The primary value in diagrams is in the discussion while diagramming—we model to have a conversation.**

> **La première valeur d'un diagramme c'est la discussion qui se déroule lors de la réalisation du diagramme - nous modélisons pour avoir une conversation.**

When a group gets together to sketch a causal loop diagram on a whiteboard (See it is the the acts of discussing and thinking that are most important when diagramming, Valtech India.), the primary value is the conversation and shared understanding they arrive at while creating the model. Its visualization as an easy-to-see diagram _is_ important to make concrete and unambiguous (on the whiteboard) the ideas—the mental models people have—because words alone can be fuzzy and misunderstood. But still, the diagram is secondary to what people take away: learning and a revised understanding through a discussion.

Lorsqu'un groupe se rassemble pour dessiner un diagramme de boucles causales sur un tableau blanc (« C'est l'acte de discuter et de réfléchir qui est le plus important lorsque nous dessinons », Valtech India.), la première valeur d'un diagramme c'est la conversation et la compréhension commune à laquelle les personnes arrivent lors de la création du modèle. Ce qu'il en résulte à savoir un diagramme facile à comprendre est important pour rendre les idées et les modèles mentaux concrets et non ambigües (sur le tableau blanc) parce que les mots seuls peuvent être imprécis et mal compris. Toutefois, le diagramme est secondaire par rapport avec ce que les gens repartent : ils ont appris quelque chose et ont revu leur compréhension du monde à travers une discussion.

<figure>![group%20cld%20modeling.jpg](https://less.works/img/systems-thinking/xgroup,P20cld,P20modeling.jpg.pagespeed.ic.lirKMzwWbD.webp)

![group%20cld%20modeling.jpg](https://less.works/img/systems-thinking/xgroup,P20cld,P20modeling.jpg.pagespeed.ic.lirKMzwWbD.webp)

<figcaption>Doing system thinking. Sketching a causal loop diagram together—modeling to have a conversation.</figcaption></figure>

Un atelier d'approche systémique : réalisation d'un diagramme de boucles causales à plusieurs - modéliser pour avoir une conversation.

_Concrete modeling tip_ : We start by writing on sticky notes to define _variables_ . A note might read “feature velocity” or “# defects.” We place these on a whiteboard. Then we sketch causal link lines between the sticky notes. There will be (or should be) lots of rewriting, erasing, and redrawing during the modeling session. The most meaningful outcome is _understanding_ ; in addition, some participants will want to take a digital photo of the whiteboard sketch.

_Trucs et astuces de pro pour modéliser_ : Nous commençons par écrire sur des petits papiers repositionnables les noms des _variables_, par exemple « vélocité des _features_ » ou « nombre d'anomalies ». Nous les plaçons ensuite sur le tableau blanc. Puis nous dessinons les liens de causalités entre les papiers . Il y aura (ou il devrait y avoir) beaucoup de réécriture, d'effaçage, de redessinage lors de la session de modélisation. Le résultat le plus important d'une telle session est la _compréhension_ - il se peut qu'à l'issue de cet atelier, certains participants voudront prendre une photo du dessin du tableau blanc.

## Seeing System Dynamics: Causal Loop Diagrams

## Voir les dynamiques d'un système : les diagrammes de boucles causales

Causal loop diagrams are used regularly in introductions to LeSS, to help see the dynamics of what is going on in large-scale development. It is useful to understand them for that reason alone. And more useful to you, we recommend you do these together with colleagues at a whiteboard. Model to have a conversation. When? Probably during a LeSS Overall Retrospective.

Les diagrammes de boucles causent sont souvent utilisés en introduction à LeSS pour aider à voir les dynamiques de ce qu'il se passe dans du développement à grande échelle. C'est donc utile de les comprendre pour cette seule et unique raison. Et cela s'avèrera encore plus utile pour vous, si vous le faites avec vos collègues devant un tableau blanc. Vous modélisez pour avoir une conversation. Quand ? Plus probablement pendant une rétrospective globale LeSS.

The practical aspect of this tip is more important than may first be appreciated. It is vague and low-impact to suggest “be a systems thinker.” But if you and four colleagues get into the habit of standing together at a large whiteboard, sketching causal loop diagrams together, then there is a concrete and potentially high-impact practice that connects “_be_ a systems thinker” with “_do_ systems thinking.”

L'aspect pratique de cet exercice est bien plus important que ce qu'il peut paraître au premier abord. Notre conseil peut sembler vague et n'avoir que peu d'impact que de vous suggérez d'« être un pratiquant systémique ». Mais si vous et quatre de vos collègues prenez l'habitude de vous réunir devant un grand tableau blanc, en dessinant des diagrammes de boucles causales ensemble, alors vous arriverez à faire la connexion entre « _être_ un pratiquant systémique » avec « _faire_ de l'approche systémique ».

The following examples seem sterile when presented in a book. But imagine you were at a whiteboard with other people and the diagrams were being sketched during a lively conversation. That’s the way we suggest ‘doing’ systems thinking.

Les exemples suivants peuvent paraître stériles car présentés dans un livre. Mais imaginez-vous à côté d'un tableau blanc avec d'autres personnes dessinant ensemble des diagrammes au cours d'une conversation animée. C'est de cette manière-là que nous suggérons de ' faire ' de l'approche systémique.

###### Notation and Examples

###### Notation et exemples

Causal loop diagrams contain many elements; the following common useful subset is explored through a scenario.

Les diagrammes de boucles causales contiennent beaucoup d'éléments ; les éléments suivants sont les plus communément utilisés et sont vus en détail tout au long du scénario qui va suivre

* variables
* causal links
* opposite effects
* constraints
* goals
* reactions; quick-fix reactions
* interaction effects
* extreme effects
* delays
* positive feedback loops

* variables
* liens de causalité
* effets opposés
* constraintes
* objectifs
* réactions; réactions corrections rapides
* effets d'interaction
* effets extrêmes
* retards
* boucles de rétroaction ou de retours d'informations positives

_The following simplified scenario is for a particular organization. It is not a generalization._

_Le scénario qui suit est un scénario simplifié pour une organisation spécifique. Il ne s'agit pas d'une généralisation._

**Variables**—Causal loop diagrams include _variables_ (or stocks) such as the _velocity (rate of delivery) of software features_ and _number of defects_ . Variables have a measurable quantity.

**Les variables** - Les diagrammes de boucles causales comportent des _variables_ (ou des stocks) telle que la _vélocité (taux de livraison) des features_ et le _nombre d'anomalies_. Les variables ont une quantité mesurable.

![systems thinking-4.png](https://less.works/img/systems-thinking/xsystems,P20thinking-4.png.pagespeed.ic.WpO9GKmuZP.webp)



**Causal links**—An element can have an effect on another, such as if feature velocity increases, then the number of defects increase; that is, more new code, more defects.

**Les liens de causalité** - Un élément peut avoir un effet sur un autre, comme par exemple si la vélocité des _features_ augmente alors le nombre d'anomalies augmente ; autrement dit, plus de code, plus d'anomalies.

![systems thinking-5.png](https://less.works/img/systems-thinking/xsystems,P20thinking-5.png.pagespeed.ic.oPRro2SqND.webp)



Now it is time to bump into _Weinberg-Brook’s Law_ and the _Causation Fallacy_ . It is easy to sketch a diagram; it is something else to model with insight. For example, consider the relationship between the _number of developers_ and _feature velocity._

Il est temps désormais de se jeter à corps perdu dans la _loi de Weinberg-Brooks_ et dans la _causalité fallacieuse_. C'est facile de dessiner un diagramme, ça l'est moins que de modéliser en faisant preuve de clairvoyance comme par exemple, la relation entre le _nombre de développeurs_ et la _vélocité des features_.

The nature of any cause-effect relationship is actually not obvious, though it is common for people to jump to conclusions such as more developers means better velocity. Adding people late in development may _reduce_ velocity (a sub-element of “Brooks’ Law” [Brooks95]). Or, _more_ bad programmers could really slow you down. An argument can be made that _removing_ terrible developers can _improve_ velocity.

Toute relation de cause à effets est par nature obscure, même si les gens ont l'habitude de sauter sur la première conclusion venue comme par exemple plus de développeurs égale plus de vélocité. Ajouter des personnes tard au cours du développement peut _réduire_ la vélocité (il s'agit d'une composante de la « loi de Brooks » [Brooks95]). Ou, _davantage_ de mauvais développeurs pourrait vraiment vous ralentir. Il pourrait être objecté qu'_enlever_ des développeurs exécrables peut permettre _d'améliorer_ la vélocité.

![systems thinking-6.png](https://less.works/img/systems-thinking/xsystems,P20thinking-6.png.pagespeed.ic.6XIYl7Vm3_.webp)



**Opposite effects**—A causal link effect may be the same or opposite direction; if A goes up then B goes up, or vice versa. Opposite effect is shown with an ‘O’ on the line. Suppose defects going up puts a drag on the system, lowering the velocity of new features because people spend more time fixing or working around bugs.

**Effets opposés** - L'effet d'un lien de causalité peut aller dans la même direction ou dans la direction opposée. Si A monte alors B monte ou vice versa. L'effet opposé se souligne à l'aide d'un '0' sur la ligne. Supposons que les anomalies ralentissent grandement le système, réduisant la vélocité des nouvelles _features_ parce que les gens passent plus de temps à corriger ou à trouver des solutions de contournement aux anomalies.

![systems thinking-7.png](https://less.works/img/systems-thinking/xsystems,P20thinking-7.png.pagespeed.ic.DPGMJyX2Qf.webp)



**Constraints**—Unless you can find people to work for free, there is a constraint on the number of developers, based upon cash supply.

**Contraintes** - À moins que vous ne trouviez des personnes prêtent à travailler gratuitement, il y a une contrainte sur le nombre de développeurs basé sur l'argent disponible.

Constraints are _not_ causal links. As cash supply goes up, it is not the case that the number of developers goes up.

Les contraintes ne sont _pas_ des liens de causalité. Lorsque la quantité d'argent disponible augmente, ce n'est pas le cas du nombre de développeurs/

![systems thinking-8.png](https://less.works/img/systems-thinking/xsystems,P20thinking-8.png.pagespeed.ic.gbgAIK-IsZ.webp)



**Goals and Reactions**–People, departments, and systems have goals, such as _higher feature velocity_ . Goals often generate pressure for people to react (or act), with the intent of achieving the goal. But since there is _Causation Fallacy_ and _Weinberg-Brooks’ Law_ to contend with, people should be cautious about assuming what actions will help. Now a goal and pressure for reaction is shown:

**Buts et réactions** - Les personnes, les départements et les systèmes ont des buts, comme avoir une _vélocité des features plus grande_. Les buts génèrent souvent de la pression pour que les gens réagissent (ou agissent) dans l'intention de leur faire atteindre le but. Mais étant donné qu'il y a la _causalité fallacieuse_ et la _loi de Weinberg-Brooks_ à laquelle il faut faire face, les gens devraient être prudents quant aux actions pertinentes à entreprendre. Voici un diagramme modélisant un but et la pression à réagir :

![systems thinking-9.png](https://less.works/img/systems-thinking/xsystems,P20thinking-9.png.pagespeed.ic.yVcHbh4_-i.webp)



Not only does a goal with a _reward_ create pressure to act, but also it creates pressure to _appear_ to be acting and achieving, due to the **measurement dysfunction** generated by rewards. And the measurement dysfunction can be proportional to the perceived value of the reward because people are being motivated to get a reward, not to improve the system [[Austin96]](http://www.amazon.com/Measuring-Managing-Performance-Organizations-Dorset-ebook/dp/B00DY3KQX6/ref=sr_1_1?ie=UTF8&qid=1413596674&sr=8-1&keywords=measuring+and+managing+performance+in+organizations). Notice how rewards can actually degrade system performance. Visually, the system dynamics may be…

Non seulement un but avec une _récompense_ créé une pression à agir, mais cela créé aussi une pression à _faire semblant_ d'agir et à atteindre le but, à cause du _dysfonctionnement de ce type d'indicateurs_ généré par les récompenses. Et le dysfonctionnement de l'indicateur peut être proportionnel à la valeur perçue de la récompense parce que les personnes sont motivées par avoir la récompense, non pour améliorer le système [[Austin96]](http://www.amazon.fr/Measuring-Managing-Performance-Organizations-Dorset-ebook/dp/B00DY3KQX6/ref=sr_1_1?ie=UTF8&qid=1413596674&sr=8-1&keywords=measuring+and+managing+performance+in+organizations). Remarquez bien comment et de quelle manière les récompenses peuvent dégrader en fait la performance du système. De manière visuelle, les dynamiques d'un tel système pourrait être …

![systems thinking-10.png](https://less.works/img/systems-thinking/xsystems,P20thinking-10.png.pagespeed.ic.39CLFp-g_9.webp)



It is quite interesting that all these dynamics have been added by introduction of reward, and yet there is no necessary connection between the top part of this model and the bottom.

Il est assez interessant que toutes ces dynamiques ont été ajouté par l'introduction d'une récompense et qu'il n'y pas de connexion entre le haut et le bas de cette modélisation.

There is no guarantee that feature velocity has improved—or even been worked on.

Il n'y a aucune garantie que la vélocité des features s'améliore ou même que l'on y travaille.

Removing the reward system is a root-cause solution to the dysfunction. Another (lesser) surface countermeasure is the lean-thinking _Go See_ (go see physically at the place of real work) principle and management behavior:

Enlever le système de récompense est une solution à la cause racine de ce dysfonctionnement. Une autre contremesure de surface est le principe et le comportement managériale _Aller voir_ (aller voir physiquement sur le lieu où le travail s'effectue) de l'approche lean.

![systems thinking-11.png](https://less.works/img/systems-thinking/xsystems,P20thinking-11.png.pagespeed.ic.NU8SjnJkUY.webp)



**Quick-fix reactions**—One difficult and slow solution toward the goal of higher velocity is to hire great developers, to increase coaching and education of existing staff, and to remove terrible workers. The alternative is called a _quick fix_ , a reaction that is hoped to achieve the goal quickly and with less effort. Sometimes a quick fix works well both in the short and long term, really strengthening the system. Sometimes not…hence, “faster is slower.” For example, people may _believe_ that increasing the number of developers increases the feature velocity. And they may thereby hope that hiring more developers will most quickly and easily solve the velocity problem. ‘QF’ indicates the quick fix:



![systems thinking-12.png](https://less.works/img/systems-thinking/xsystems,P20thinking-12.png.pagespeed.ic.x8IJWKprUx.webp)



**Interaction effects**—There is the constraint of cash supply on hiring. One hard and slow solution is to get more cash. A quicker fix is to hire _much_ cheaper developers. In this case, the level of cash supply now has an _interaction effect_ with other causal links. Low cash tends to strengthen the hire rate of much cheaper developers when there is pressure to increase hire rates.



One could simply draw an (opposite) causal link directly from _cash supply_ to _hire rate of very cheap developers_ , but that merely says that less cash leads to more hiring of extremely cheap developers. That is not quite what we want to say; rather, we want to show the interaction effect—that effect A influences _effect_ B. This is done by showing a causal link entering another causal link. For example, from _cash supply_ to the quick-fix line going into _hire rate of very cheap developers_ :



![systems thinking-13.png](https://less.works/img/systems-thinking/xsystems,P20thinking-13.png.pagespeed.ic.LvAE8ewRFJ.webp)



**Extreme effects**—We have worked with some very inexpensive developers with excellent skill and some very expensive developers that are terrible, but on average, you get what you pay for—when you hire from a large pool of very cheap labor, the average skill level is lower. In the model we want to show that the impact of hiring very cheap labor on the _number of low-skilled developers_ is a significantly greater effect than average.



To show an _extreme effect_ in the model, use a thick line:



![systems thinking-14.png](https://less.works/img/systems-thinking/xsystems,P20thinking-14.png.pagespeed.ic.JYkqz8Qe24.webp)



**Delays**—One problem in hiring in software development is the _fallacy of mild programmer variance_ —the mistaken belief that programmer variance (in terms of productivity, code quality, etc.) is relatively small. However, programmer variance studies suggest an average of four times faster in the top versus bottom quartile [[Prechelt00]](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.43.4788). Rather significant. Also, the COCOMO model—based on large and longitudinal studies—shows that the capability of the development personnel is by far the most important factor for productivity [[Boehm00]](http://www.amazon.com/Software-Cost-Estimation-Cocomo-II/dp/0130266922/ref=sr_1_1?ie=UTF8&qid=1413597244&sr=8-1&keywords=Software+Cost+Estimation+with+Cocomo+II). And, on average, very weak programmers create poor-quality code (poor design) and more defects, creating another drag on the system.



But the impacts of these effects are not immediately obvious. For example, it takes a relatively long time after hiring a large pool of weak programmers before the impacts of more and more bad code/design start to be felt. Similarly, the average _decrease_ in feature velocity (because of the powerful impact of programmer variance) will not show up immediately.



To show these _delayed effects_ in the model, use a double-line through the effect line:



![systems thinking-15.png](https://less.works/img/systems-thinking/xsystems,P20thinking-15.png.pagespeed.ic.0fwliLJm6G.webp)



Delay has an intriguing influence on the _educational_ or corrective power in a system. If an impact or unintended consequence is long delayed, one does not feel the effect (pain or gain) and so does not clearly see how A influenced B, or more subtly how _A influenced B influenced A_ .



Therefore, one does not learn from or correct mistakes—in policy, management actions, tools, and so forth. Likewise, gradual improvement through the lean thinking practice of _kaizen_ can take a long time; patience and insight are needed to see if and how things improve.



**Positive feedback loops**—Negative or positive feedback loops<sup>[5](https://less.works/less/principles/systems-thinking.html#footnote-5)</sup> and delays are where things start to get more subtle in a system—and in understanding a system. For example, how does one become a better programmer? In part, by mentoring from great programmers and seeing lots of examples of great code. But an office with a lot of low-skill developers does not generate a lot of great code examples, nor does it attract or retain the small pool of great programmers who could act as mentors. They would rather work somewhere else.



Now the development group starts to enter a self-reinforcing downward spiral—a set of _positive feedback loops_ . Fortunately, the downward trend is constrained by the supply of cash.



More great programmers—who could craft great code and mentor others—leave. So there is less and less quality code to look at and to learn from. The percentage of weak programmers grows even larger and feature velocity drops further. Code becomes more messy, awkward, and duplication-riddled, so the capacity to swiftly implement features declines. Since feature velocity is dropping further, there is more pressure to hire yet more very cheap programmers. All this leads to multiple positive reinforcement loops in the system, for example:



![systems thinking-16.png](https://less.works/img/systems-thinking/xsystems,P20thinking-16.png.pagespeed.ic.ONFuUmJHSE.webp)



_Tip_ : You can find positive feedback loops by finding cycles with an _even number_ of ‘Opposite’ effect relationships. There are several examples in the model above.



##### Conclusion



The example scenario is only that—an example. A causal loop diagram can visualize rich dynamics in a workplace system. These are best created by a group at a whiteboard.



## Seeing Mental Models



The previous causal loop diagrams reflect people’s mental models of causation, which may be wrong. It is interesting to note that people’s models of causation are influenced by the timeliness (delay) and quality of feedback in the system.



The implication of “mental models” is to improve our meta-cognitive skill to see and question our own assumptions and chains of reasoning. Are we making faulty leaps of logic? It also implies when working with others to discuss (inquiring rather than abusing) the mental models of our colleagues.



_Seeing_ these mental models is step one; _changing_ them is the even harder part of step two. That art is beyond the scope of this introduction, though a successful LeSS adoption must involve changes in mindset and insight among many groups.



A tip to better _see_ the mental models (beliefs, chains of inference, …) playing out in the system dynamics is to ask the following question during a modeling workshop and then sketch the answers. “Let’s talk about the assumptions behind this model. What do we _believe_ or assume in terms of facts and effects that led us here?”



Answers are sketched on the whiteboard model, for example:



<figure>![systems thinking-17.png](https://less.works/img/systems-thinking/xsystems,P20thinking-17.png.pagespeed.ic.5UIqBnJfK1.webp)



<figcaption>Visualizing the assumptions in our heads... our mental models.</figcaption></figure>



### Example: The “Faster is Slower” Dynamic



With the vocabulary of quick fixes, delays, positive feedback loops, and mental models, it is fascinating to see that there can be a short-term apparent improvement in a variable as the result of a quick fix, but a _delayed degradation_ of the very same variable—the “faster is slower” dynamic. This is a recurrent dynamic in the workplace and a cause of weakness. So it is worth another illustration.



_The story of Microsoft Word and the_ **_secret developer toolbox_** : A classic example of the short-term ‘improving’ but long-term degrading dynamic is the story of the first release of Microsoft Word for Windows [[Spolsky04]](http://www.amazon.com/Joel-Software-Occasionally-Developers-Designers/dp/1590593898/ref=sr_1_1?ie=UTF8&qid=1413597951&sr=8-1&keywords=Joel+on+Software). It was released _years_ later than desired. Why? _Because managers tried to follow the original schedule and pushed developers to meet it_ .



The story illustrates why _wishful thinking_ is identified as one of the wastes in lean thinking. In this case the wishful thinking of insisting on (apparently) following a schedule, which implies the misconception or wishful thinking that development estimates are not estimates but are commitments—a common myth that propels degradation of a system.



[The next model](https://less.works/less/principles/systems-thinking.html#figure-1) illustrates a _summary_ of the dynamics of what happened when the managers pushed people to evidently keep to the original schedule, and why this quick-fix reaction to slow progress appeared to make things faster in the short term but actually even _slower_ in the long term. See the dynamic of schedule pressure and the secret toolbox. intentionally omits some deeper dynamics that are expanded and shown in See deeper dynamics of schedule pressure and the secret toolbox..



<figure>![systems thinking-18.png](https://less.works/img/systems-thinking/xsystems,P20thinking-18.png.pagespeed.ic.A7OSuu755I.webp)



<figcaption>The dynamic of schedule pressure and the secret toolbox.</figcaption></figure>



As a quick fix, the Microsoft managers exhorted, bribed (with potential rewards), and threatened the Word developers to keep to the original schedule. Consequently, the developers predictably pulled out their **secret developer toolbox** —the many practices related to hacking out dirty code (no tests, no reviews, ignore known defects, copy-paste programming, poor design, …) to apparently deliver a feature faster. You see, developers also have _quick-fix_ reactions for their problems.



The tactics seemed to have worked like magic. As the managers pressured the developers, ‘features’ were delivered quicker as people used the secret toolbox, which reinforced the belief that pressuring developers helps. But this apparent acceleration actually had a delayed effect to make things slower, which is explored next. Since management did not quickly see the delayed effect of the secret toolbox, and because they believed managers should not be frequently looking in detail at the source code or themselves be master programmers, they did not learn from this dynamic.



A closer exploration of the system dynamics shows why things went slower in the long term and why the first Word for Windows release was years later than desired, illustrated in this model…



<figure>![systems thinking-19.png](https://less.works/img/systems-thinking/xsystems,P20thinking-19.png.pagespeed.ic.D24dvGHzfu.webp)



<figcaption>Some deeper dynamics of schedule pressure and the secret toolbox.</figcaption></figure>



Naturally, lots of dirty code eventually slowed things down. More subtly, developers would _ignore_ the bug list of ever-increasing open defects to—instead—generate new features. This led to a long delay between the creation of a defect and its correction. It turns out that this significantly increases variability and time to fix a defect because of the compounding negative effect of a long-lived bug (for example, due to workarounds and coupling) and because developers have long forgotten the detailed context of code related to the defect and therefore need to slowly rediscover that context—with more and more dirty confusing code surrounding them.



The astute reader may also notice the several positive feedback loops that reinforce the degradation cycle; this is one reason the product was years later than intended.



Solution? The lean thinking _Stop and Fix_ and _Go See_ principles. _First_ , rather than trying to go faster when there are problems, manager-teachers encourage people to go _slower_ and help them learn to see system dynamics and root causes, and to fix these—to improve the _system_ of development. By going slower, Toyota—the masters of lean thinking—has become one of the fastest companies around. _Second_ , for managers to _go see at the real place of work_ to learn what is going on. The “real place” in software development is the code, which suggests that first-level managers are master programmers who are frequently evaluating the code.



Microsoft people did not reflect on the situation until after release. When they did finally hold a retrospective, it led to a _zero-defects_ policy, meaning that the first priority was to fix known bugs in the code under development—to drive down to zero the open-defects list before writing more new-feature code.



## Seeing (and Hearing) Local Optimization



“Everyone is doing their best yet overall systems throughput is degrading. How can that be?” This is the paradox of **local optimization** —when a person or departmental decision maker optimizes for the local view or self-interest. The party making the decision frequently _believes they are making the best decision_ , but because ‘best’ is a local optimization, in fact it sub-optimizes overall system throughput. This is a result of “silo mentality,” misunderstanding, fear, limited information, delayed feedback, ignorance, careerism, avarice, and other common _organizational learning disorders_ .



A small product group of 30 people does not have the time or money to engage in much nonsense or waste. But large companies, with large product groups, centralized process and tool groups, a centralized “project management office,” and so forth, seem to have raised local optimization and waste to an art form. Government bureaucracies are the quintessential example, of course. As such, when you serve as a guide in large-scale agile adoption, _seeing_ (or _hearing_ ) and dealing with local optimization is singularly vital.



For example, the legal and corporate security departments put in place a policy that seems terribly important from their perspective. In the aim of preventing loss of intellectual property (IP), the legal department decrees “no one shall put any information on the walls.” Or, in response to cost-cutting pressure, the facilities management says, “It is important to ensure our walls are not dirty or damaged.” And thus they shut down a practice in lean thinking, visual management (which is usually done on walls), and they inhibit a well-known innovation practice, group whiteboard work. The lawyers may succeed in reducing loss of IP (actually, that is questionable), and the facilities people will succeed in keeping the walls clean—at the cost of inhibiting the product development group from innovating and collaborating. Finally, the company falls behind with less and less IP even worth protecting because tools for innovation and delivering fast have been disallowed, but the lawyers have successfully fulfilled their mandate from the executive team to “ensure our IP is protected.” And the _furniture police_ have clear walls. _They have done their best_ .



The following is a real e-mail quote from the _FURNITURE POLICE_ in one organization that dissallowed visual management on the walls. Can you identify the local optimizations and mental models driving this?



> _Individual work cubic partition can be personalized. But things obvious higher than the partition or harming the office environment’s harmony are restricted._



We also see local optimization in centralized groups that make software tool choices for others. The common mindset is to choose a tool that is best at reducing some supposed cost (curiously, these groups seldom recommend free open source tools) or best at doing something complicated or best for the work of one specialized worker role (even though _everybody_ has to use the tool), rather than maximizing the global goal of faster system throughput of value to customers.



In large-scale adoption of Scrum or agile principles, most of the “Yes, but …” issues that are raised are examples of local optimization, such as, “_Yes, but…what about management reporting_?” or more generally, “*Yes, but…what about
<special case="">*?” Then, policies and practices are twisted around, serving the goal of reporting or some other secondary aim rather than the primary goal of optimizing for fast value throughput. Sometimes we see *local optimization for the extreme or rare case* . For example, a person responsible for making a centralized tool choice for the enterprise presents a scenario for a complex or rare case of use, and then chooses the tool that fits that, sub-optimizing for a 5 percent case instead of optimizing for ease and speed for the 95 percent case.</special>



Other local optimizations are due to ignorance of new ways of working. This is especially common in large-scale product groups. For example, we once helped a large networking product group in Europe adopt Scrum and the practice of _continuous integration_ (CI) combined with a CI system that continually integrated, built, and automatically tested the product. After some time, an outside traditional manager inspected what was going on, and recommended the integration practices should be changed—because there was no written integration plan for how a human integration manager should manually integrate all the software, and of course, there was no integration manager. They wanted to ‘optimize’ around the work of an integration manager that was no longer needed. They could not see that their entire old-fashioned model of work had been eliminated with CI. This story repeats in all the departments of a large established product: local optimization around the _existing_ ways of work, such as manual test, a separate architecture department, component teams, and so on. A coach working to introduce large-scale Scrum at the enterprise level has a _mountain_ of similar local optimization thinking to deal with.



In lean thinking and agile methods, the focus is on global systems goals: Deliver value fast with high quality and morale—**global optimization** . Try to consider decisions in light of this goal. To develop an “optimize the whole” culture, challenge all decisions and policies with the question:



> **Does this decision or policy focus on delivering value to the external customer fast, or does it focus on the interests of a department, person, internal policy/practice, or rare case?**



In LeSS, the Product Owner is responsible for choosing high-value goals that **could lead to potentially shippable product (at the end of the Sprint) and that maximize the desired impacts and that delight the customer, while maintaining a sustainable pace and high engineering quality**. That explicit goal is meant to orient the system toward global rather than local optimization.



## Conclusion



In addition to becoming a systems thinker yourself, encourage others to learn more about this topic. We suggest you to try getting together at a whiteboard with colleagues to sketch a causal loop diagram, so that _being_ systems thinkers and _doing_ systems thinking are connected at the workplace.



<figure>![group%20cld%20modeling.jpg](https://less.works/img/systems-thinking/xgroup,P20cld,P20modeling.jpg.pagespeed.ic.lirKMzwWbD.webp)



<figcaption>Doing system thinking. Sketching a causal loop diagram together—modeling to have a conversation.</figcaption></figure>



## Recommended Readings

* W. Edwards Deming’s [_Out of the Crisis_](http://www.amazon.com/Out-Crisis-W-Edwards-Deming-ebook/dp/B00653KTES/ref=sr_1_1?ie=UTF8&qid=1413601625&sr=8-1&keywords=out+of+the+crisis) is a master work by arguably the most well-known systems thinker and quality expert. It opens with the modest goal, “The aim of this book is transformation of the style of American management… It requires a whole new structure, from foundation upward.” Deming also advocates the _System of Profound Knowledge_ in which managers (1) appreciate there is a _system_ , (2) understand common-cause and special-cause variation (queueing theory is related to variation), (3) understand limitations of knowledge and reasoning mistakes, and (4) know credible psychology and social research results so that behavior- or motivation-related policies are _not_ based on “common sense.” The core of the book centers around his famous _14 Points for Management_ , including (for example), “_Eliminate management by objective. Eliminate management by numbers, numerical goals. Substitute leadership_ .”   
* Jay Forrester’s [_Industrial Dynamics_](http://www.amazon.com/Industrial-Dynamics-Jay-Wright-Forrester/dp/1614275335/ref=sr_1_1?ie=UTF8&qid=1413601681&sr=8-1&keywords=industrial+dynamics) is the classic text on system dynamics—well written and insightful. Although written in the early 1960s, it is as relevant today as when published. It goes beyond cause-effect modeling to also model the flow and inventories of information, money, and material in systems. The book includes formal mathematical modeling but this is not obligatory to appreciate system dynamics.
* Weinberg’s _Quality Software Management: Systems Thinking_ and _An Introduction to General Systems Thinking_ are worthwhile. Written from the perspective of an experienced consultant in systems development.    
* Senge’s [_The Fifth Discipline_](http://www.amazon.com/Fifth-Discipline-Practice-Learning-Organization-ebook/dp/B000SEIFKK/ref=sr_1_1?ie=UTF8&qid=1413601715&sr=8-1&keywords=the+fifth+discipline) is a classic that advocates the need for leadership to apply systems thinking (it is the _fifth_ discipline) and other key disciplines for a great, sustainable enterpise. The others include leaders with (1) personal mastery and (2) reflection on their beliefs and faulty reasoning, the (3) definition and communication of a meaningful shared vision, and (4) the ability of teams to learn. We recommend ignoring—at least during the first few years of practice—the ‘archetypes’ notion presented in the book. It was well meant as a learning aid but has been observed to distract and intimidate people from learning and applying basic system dynamics modeling. The ‘archetypes’ are not part of original system dynamics.    
* [_The Fifth Discipline Fieldbook_](http://www.amazon.com/Fifth-Discipline-Fieldbook-Strategies-Organization-ebook/dp/B00JTCJEO8/ref=sr_1_1?ie=UTF8&qid=1413601809&sr=8-1&keywords=The+Fifth+Discipline+Fieldbook) is an in-depth resource, written from the viewpoint of many practitioners and consultants.    
* The organizational-learning writings from Argyris, Putnam, McLain, and Schön. Important concepts include _double-loop learning_ and _high-advocacy/high-inquiry dialogue_. Classic works include [_Action Science_](https://actiondesign.com/resources/readings/action-science) and [_Organizational Learning_](http://www.amazon.com/Organizational-Learning-Addison-Wesley-Organization-Development/dp/0201001748/ref=sr_1_11?ie=UTF8&qid=1413601940&sr=8-11&keywords=organizational+learning).    
* The publications and resources available through the [_Society for Organizational Learning_](https://www.solonline.org/).

---

##### Notes:

1. Senge wrote _The Fifth Discipline_ , on systems thinking and learning organizations, named “one of the seminal management books of the last 75 years” by the _Harvard Business Review._ See** [Senge94].  
2. Another reason: Believing more control is possible than actually is. Complexity science suggests fundamental limits on predicting and controlling semi-chaotic social systems [Stacey07]. This is a rather large can of worms that will remain unopened in this book.  
3. Macroeconomics, psychology, sociology, and biology are exceptions, among many others.  
4. ‘Basic’ does not mean trivial or easy to solve. For example, ‘motivation’ and ‘quality’ are basic but not easy issues.  
5. _Feedback loops_ is occasionally used in this book in the colloquial sense of feedback, rather than this system dynamics sense.


---
Auteur : [Prénom_Nom](url_bio)  nbsp
Source : [Titre_article_en_vo](url_article_en_vo)  nbsp
Date de parution originale : jj_MMMM_yyyy  nbsp

---
Traducteur : [Prénom_Nom](url_bio)  nbsp
Date de traduction : jj/mm/yyyy  nbsp

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

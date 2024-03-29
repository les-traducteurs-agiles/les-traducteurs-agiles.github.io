---
layout: post
title:  "INVEST est-il suffisant pour créer de bonnes stories ? Non !"
date:   2021-09-22 00:01
published: false
tags:
- user story
---

I developed the INVEST model years ago to help someone (and then many people) think about the user stories they were creating. Is INVEST all you need to create good stories? Unfortunately, no.

Il y a plusieurs années, j'ai développé le modèle INVEST afin d'aider une personne (et par la suite plusieurs autres) à bien réfléchir sur les _user stories_ qu'elle était en train de créer. Est-ce qu'INVEST est suffisant pour que vous puissiez créer de bonnes _stories_ ? Malheureusement, non.

## **INVEST**

## Le modèle INVEST

Briefly, INVEST (see [References](https://xp123.com/articles/all-you-need-is-invest-no/?utm_source=rss&utm_medium=rss&utm_campaign=all-you-need-is-invest-no#references)) is an acronym for qualities of good user stories:

En résumé, INVEST est un acronyme décrivant les caractéristiques d'une bonne _user story_ :

**I – Independent** – Stories are (mostly) independent capabilities.

**I – Indépendante** – Les _stories_ représentent (pour la plupart d'entre elles) des fonctionnalités indépendantes les unes des autres.

**N – Negotiable** – Stories are not specifications, but solution ideas we explore together.

**N – Negotiable** – Les _stories_ ne sont pas des spécifications, mais des idées de solution à explorer ensemble.

**V – Valuable** – Stories are valuable to those who care about the product.

**V – (de) Valeur** – Les _stories_ doivent apporter quelque chose d'utile, de valeur à ceux ayant de l'intérêt pour le produit

**E – Estimable** (yes, it also means “can be estimated”:) – Stories can be estimated in terms of the work required for a particular team to implement them. (I don’t emphasize this one too much; estimates are over-used, and often unnecessary; Small and Testable capture most of what I care about there.)

**E – Estimable** (oui, cela signifie aussi « peut être estimé ») — les _stories_ peuvent être estimées en terme de travaux à effectuer pour les implémenter par une équipe donnée. (Je n'insiste pas trop sur ce dernier point ; les estimations sont sur-utilisées, et souvent inutiles ; les éléments _Suffisamment petite_ et _Testable_ qui suivent reflètent beaucoup mieux ma pensée sur ce point.).

**S – Small** – Stories are on the scale of hours to days, not months to years.

**S – Suffisamment petite** — Les _stories_ se mesurent à l'échelle de quelques heures à quelques jours, pas à l'échelle de quelques mois ou de quelques années.

**T – Testable** – Stories are well enough understood that we can describe examples and behaviors.

**T – Testable** – Les stories sont suffisamment compréhensibles pour que nous puissions les décrire sous la forme d'exemples d'utilisation et de comportements.

That’s the original formulation. I tend to have a couple other criteria too. (But no, I won’t change the acronym.)

Cette formulation d'INVEST, est la formulation originelle. J'ai tendance à y ajouter deux critères supplémentaires (mais non, il n'est pas question pour autant que je change l'acronyme).

- **End-to-End** – Focus on a story as a full capability (from a user’s perspective), not a piece of a capability. (I’ve seen many places where teams have pieces of the puzzle, but nobody owns the end to end flow or capability.) 

- **De bout-en-bout** – Une _story_ se doit d'être considérée comme étant une fonctionnalité pleine et entière (du point de vue utilisateur), et non comme une simple fraction de celle-ci. (J'ai vu plein )

- **Scalable** (rather than just Small) – A story’s headline can be fulfilled in many ways – a manual solution, a minimal solution, or a full-featured solution. (Yes, this overlaps with the idea of negotiation through possible solutions). 

- **extenSible** (plutôt que Suffisamment petite) — Le libellé d'une _story_ peut être fait de plusieurs manières qu'il s'agisse d'une solution manuelle, d'une solution minimale, ou d'une solution complète. (Oui, j'en conviens, cela recoupe l'idée de devoir négocier entre plusieurs solutions).

## Story Templates

## Modèles de _story_

Some teams like to use templates for their story headlines. The most common one is the “Connextra” format –  
As a role, I want to do something, so that some goal is met

Certaines équipes aiment bien utiliser des modèles pour le libellé de leur _story_.  Le modèle le plus connu est celui qui suit le format dit « Connextra ».
En tant que _un rôle_, je veux _faire quelque chose_, afin d'_accomplir un certain but_.

Another template, suggested by Industrial Logic, is –  
Role Action Context

Un autre modèle, proposé par Industrial Logic, est —
Rôle Action Contexte

The advantage of templates is that they prompt you to think about which users you’re addressing and what capabilities they need. They push you to use a vocabulary your customers/users would understand. And they encourage you to rise above the details to think about why you want this.

L'avantage des modèles est qu'ils vous obligent à penser quels sont les utilisateurs à qui vous vous adresser et quelles sont fonctionnalités dont ils ont besoin. Ils vous poussent à utiliser un vocabulaire que vos clients/utilisateurs comprendront; Et ils vous encouragent à vous hisser au-dessus des détails du pourquoi vous voulez cela.

But, like INVEST, the templates are easy to see, but they aren’t the point.

Mais, tout comme INVEST, les modèles sont faciles à lire, mais là n'est pas l'essentiel.

## **The Context of Stories**

## **Le contexte des _stories_**

Criteria and story templates are great, and may nudge you in a better direction, but effective use of stories requires that you create a context that can leverage them. 

Les modèles de _story_ et de critères d'acceptation, et peuvent vous pousser dans une bonne direction, mais pour que l'utilisation des _user stories_ soient efficaces, vous devez créer un contexte autour d'elles pour en exploiter la substantifique moëlle.

Ron Jeffries described stories as “Card, Conversation, and Confirmation”, where Conversation is the most important part. On XP teams, a story (card) is treated as “a token of a conversation”, in Alistair Cockburn’s words. \[I’ve also heard “ticket” or “promise”, but I don’t have a reference.\] That is, the card exists because the team had a conversation about a possible future capability, and wrote a few words on a card to remind them of it. 

Ron Jeffries décrit les _stories_ sous la forme d'un triptyque « Carte, Conversation et Confirmation », dans lequel la Conversation représente la partie la plus importante. Dans les équipes XP, une _story_ (une carte) est considéré comme étant « un gage pour une conversation » d'après ce que rapporte Alistair Cockburn. (J'ai aussi entendu les termes de « ticket » ou de « promesse » mais je n'ai pas pu trouver la référence.). Autrement dit, une carte existe parce que l'équipe a eu une conversation sur une possible future fonctionnalité, et a écrit quelque mot pour s'en souvenir.

How much work could you manage effectively this way? If it were only three stories, you wouldn’t need to bother. But 5, 10, maybe 50? (I doubt I could keep 20 deep conversations in my head, though 50 “headlines” is manageable.)

Quelle quantité de travail pouvez-vous gérer efficacement de cette manière ? S'il ne s'agit que de trois _stories_, vous ne devriez pas avoir de soucis. Mais 5, 10, ou 50 ? (Mais je doute d'être capable de garder 20 conversations dans ma tête, mais 50 « libellés » cela reste gérable).

I can recall one legacy replacement project that had 100+ story cards and used them well. A handful at a time were active, but the cards helped track progress against the whole replacement. 

Je me rappelle d'un projet visant à remplacer un vieux système existant avec plus de 100 cartes de _story_. Seule une poignée d'entre elles étaient actives à un instant _t_, mais les cartes dans leur totalité permettaient aussi l'avancée du projet.

However, most times I’ve seen a hundred stories, or even hundreds, the teams weren’t collaborating deeply or well. Rather, they seemed to use the set of stories (held in a tool) to _avoid_ conversations and let analysis “get ahead”.  (For the record, dumping lots of stories in a tool is _not_ collaboration.)

Toutefois, la plupart du temps lorsque je vois une centaine de _stories_, ou même des centaines, les équipes ne collaborent pas bien ou de manière suffisante. À la place de cela, elles smeblent utilisés l'ensemble des _stories_ (souvent contenues dans un outil) pour _éviter_ les conversations et laisser l'analyse « mener la danse ».

Instead, agile teams _limit_ work in progress (WIP). They’ve found it better to have the conversation, and move on to implementing and deploying while it’s still fresh in everybody’s minds. You may then be able to get feedback, ideally from real use, and adjust future directions based on what you learn. 

Au lieu de cela, les équipes agiles limitent le travail en cours (TEC). Elles ont découvert qu'il est mieux d'avoir une conversion, puis d'aller faire l'implémentation et le déploiement tant que c'est toujours frais à l'esprit.  Vous pourrez alors être en mesure d'avoir des retours d'informations, idéalement issus après une utilisation réelle et d'ajuster les orientations futures en fonction de ce que vous avez appris.

> Stories replace documentation and handoffs with a dynamic interplay of conversation, experiments, implementation, and feedback.

> Les _stories_ remplace la documentation et les multiples passages de relais par une dynamique de conversations, d'expérimentatons, d'implémentations et de retours d'informations.

Stories replace documentation and handoffs with a dynamic interplay of conversation, experiments, implementation, and feedback. Rather than the old mostly-stable context, Agile teams recognize that most work now takes place in a constantly-evolving environment, and they must respond accordingly.

Les _stories_ remplacent la documentation et les multiples passages de relais par une dynamique de conversations, d'expérimentatons, d'implémentations et de retours d'informations. Plutôt que l'ancien contexte plutôt stable la plupart du temps, les équipes agiles reconnaissent le fait que travail se déroule désormais la plupart du temps dans un environnement en constante évolution et qu'elles doivent y réagir de manière adaptée.

## **A Product Isn’t a Bunch of Stories – or a Bunch of Code**

## **Un produit n'est pas un paquet de _stories_ — ou un paquet de code**

Stories can help in development, but there’s more to a product than stories or the code that implements them. A software product is not just software – it participates in and creates a whole ecosystem. 

Les _stories_ peuvent être d'une grande aide au cours du développement d'un produit, mais un produit c'est bien plus que des _stories_ ou du code. Un produit logiciel n'est pas que du logiciel — il participe à tout un écosystème et à le créer.

Especially early on, a team may have a lot of learning to do: users, customers, capabilities needed, architecture, etc. You may need to do experiments to learn where your ideas are useful or valuable. 

En particulier au début, une équipe a beaucoup de choses à apprendre : utilisateurs, clients, compétences nécessaires, architecture, etc. Vous pouvez avoir besoin d'expérimenter pour apprendre si vos idées sont utiles ou ont de la valeur.

Some developers resent the “folderol” and think somebody should somehow just know and tell them what to do – never backtracking, or even changing direction. They may get to work as if that were true, but the best teams instead accept the instability and leverage it to make even better products. 

Certains développeurs peuvent être agacés par « tout ce cirque » et pensent que quelqu'un devrait d'une manière ou d'une autre tout savoir et leur dire simplement ce qu'il faut faire — sans jamais revenir en arrière, ou sans jamais changer de direction. Ils peuvent se mettre au travail comme si tout était déjà acquis, mais les meilleures équipes acceptent cette instabilité des choses et la met à profit pour réaliser des produits encore mieux.

Product management has its own practices; product managers must balance outside and inside forces. To learn more deeply about this role, I look to Jeff Patton, Marty Cagan, Melissa Perri, and others (see [References](https://xp123.com/articles/all-you-need-is-invest-no/?utm_source=rss&utm_medium=rss&utm_campaign=all-you-need-is-invest-no#references)). Writing stories may be a small or even non-existent part of a product manager’s job. 

La gestion de produit a ses propres pratiques ; les responsables produits doivent trouver un équilibre entre les forces internes et externes. Je me suis tourné vers  Jeff Patton, Marty Cagan, Melissa Perri, ainsi que bien d'autres pour en apprendre davantage sur ce rôle (cf. [References](https://xp123.com/articles/all-you-need-is-invest-no/?utm_source=rss&utm_medium=rss&utm_campaign=all-you-need-is-invest-no#references)). La rédaction des _user stories_ peut s'avérer être une petite partie voire même ne rien représenter du quotidien du responsable produit.

## **Leveraging Agility**

## **Mettre à profit l'agilité**

A key aspect of agility is that we don’t just lock in on some idea and head there, but rather we adjust both our direction and our target as we learn. 

Un des aspects clés de l'agilité est que nous ne restons pas simplement bloqué sur la même idée, mais plutôt que nous ajustons à la fois notre trajectoire et notre cible au fur et à mesure que nous en apprenons davantage.

If your habit is to define a large project, load a bunch of stories in a tool, head there, and measure “conformance to plan”, you’re missing a chance. 

Si votre habitude est de définir un grand projet, de mettre un paquet de _stories_ dans un outil, de vous y jetez dedans tête la première, et de mesure « la conformité par rapport à un plan », vous râtez votre chance.

Agility is instead built around an evolutionary approach: ship something simple (but end to end), try it, learn, and repeat – a little better each time around. User stories support this as a lightweight way of reminding us what to do. 

L'agilité est plutôt construite comme une approche évolutionaire : livrez quelque chose de simple (mais de bout en bout), essayez-la, tirez-en des leçons, et répéter l'opération — un petit mieux à chaque fois. Les _user stories_ favorisent ça car elles sont une manière simple et légère de nous rappeler quoi faire.

## **Making Stories Work**

## **Pour des _stories_ bien huilées**

- Take a whole-product perspective.
- Build in learning and feedback – part of everything you do.
- Use an evolutionary approach that supports that. 
- Keep WIP low – focus on completing things more than starting them. 
- Have conversations about capabilities – and implement them soon after. 
- Use a tool if needed (e.g., remote), but don’t let stories become a “pile of leaves” (Jeff Patton’s great metaphor). 
- Use CCC, INVEST, story templates, or whatever else will help you sustain a context where the above works well. 

- Adoptez une approche globale produit
- Intégrez-y des boucles d'apprentissages et de rétroactions — cela fait partie de votre boulot
- Adoptez une approche évolutionnaire qui soutient cela
- Ayez peu de travail en cours — concentrez-vous à finir des choses avant d'en commencer de nouvelles
-



I’m happy that INVEST has helped some teams create better stories, but it’s a small tool. Flexible learning and an evolutionary approach are key to making Agile work. Stories are only a means to support that flexibility. 



## **References**

##Bibliographie

Cagan, Marty. Follow [@cagan](https://twitter.com/cagan) on Twitter. Most recent book: [Empowered: Ordinary People, Extraordinary Products](https://www.amazon.com/EMPOWERED-Ordinary-Extraordinary-Products-Silicon-ebook/dp/B08LPKRD5L/ref=sr_1_1?dchild=1&keywords=empowered&qid=1627962103&s=books&sr=1-1&tag=xp123com) (2020). 

Jeffries, Ron. “[Essential XP: Card, Conversation, Confirmation](https://ronjeffries.com/xprog/articles/expcardconversationconfirmation/)”. Retrieved 2021-08-02. 

Patton, Jeff. Follow [@jeffpatton](https://twitter.com/jeffpatton) on Twitter. Website: [https://www.jpattonassociates.com](https://www.jpattonassociates.com)

Perri, Melissa. Follow [@lissijean](https://twitter.com/lissijean) on Twitter. Website: [https://melissaperri.com](https://melissaperri.com)

Wake, Bill. “[INVEST in Good Stories, and Smart Tasks](https://xp123.com/articles/invest-in-good-stories-and-smart-tasks/)”. Retrieved 2021-08-02. (See its Related Articles section for more details on this.)


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

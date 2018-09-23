---
layout: post
title:  "Un nouveau cadre de travail ? XP revisité ? Non ..."
date:   2018-09-20 00:01
published: true
tags:
- tag1
- tag2
---

I’m really not going to “Revisit XP”, and really not going to define a new framework, but I have been thinking a bit about what I currently believe and feel about Agile, XP, Scrum, and all that jazz. One thing I did was to post this sketch, done at the BAR [^1] on Saturday:

Je ne vais pas vraiment "Revisiter XP", et je ne vais pas vraiment définir un nouveau cadre de travail, toutefois j'ai réfléchi sur ce que je crois et sur ce que je ressent à propos d'Agile, XP, Scrum et tutti quanti. L'une des choses que j'ai faite a été de poster ce dessin, fait au BAR dimanche :

Now this picture just represents some random notes, and I do not claim that my views day after tomorrow will be consistent with it, nor even that it reflected my views as of last Saturday. But here are some thoughts about it:

Maintenant, ce dessin ne représente que quelques notes prises sur le vif, et je ne garantis en rien que mon point de vue après-demain sera en cohérence avec ce dessin, ni même que ce dernier reflète exactement mon points de vue de samedi dernier. Mais, voici quelques réflexions à ce sujet :

## Main Topics

## Sujets principaux

Well, right then, I’ve come up with four headers, so far, under which to group ideas: Product, People, Time, and Spirit.

Donc, pour l'instant, j'ai trouvé quatre titres jusqu'à présent sous lesquels regrouper certaines idées : produit, personnes, temps et esprit

## Product

## Produit

Product is probably the central idea in my view. Kent Beck once said that all methodologies are based on fear, and my big fear is that we’ll be doing good work, that deserves understanding, support, and guidance, and that no one will know it.

Le produit est probablement l'idée centrale dans ma vision des choses. Un jour, Kent Beck a dit que toutes les méthodologies sont basées sur la peur, et ma plus grande peur est, bien que nous allons faire du bon travail, qui mérite compréhension, soutien, et conseils, que personne ne soit au courant.

So my preferences are arranged around producing a “Product Increment” frequently, and showing it to everyone who matters. We focus on frequent small releases, and continue to drive the interval between releases toward zero.

Donc mes préférences vont à ce qui permet de produire fréquemment un "incrément du produit", et de le montrer à toutes personnes intéressées. Nous nous focalisons sur de petites livraisons fréquentes, et nous nous efforçons de tendre vers zéro l'intervale entre deux livraisons.

For that to work, we need to rely on and work toward simple design, which is supported by, indeed requires, as far as I know, Test-Driven Development and Refactoring. Since the system is changing all the time, I believe that it needs to be supported by automated “checks” (née “tests”). Some of these show our stakeholders that the system still works. Some of them are used to help us find defects when they do inevitably crop up. The programmer tests mostly fall out of the TDD process: we just keep them.

Pour que cela marche, nous devons nous appuyer sur une conception simple et travailler dans cet objectif, celle-ci est épaulée par, et exige d'ailleurs pour autant que je le sache, le développement piloté par les tests [^1] et du _refactoring_. Étant donné que le système change tout le temps, je crois qu'il a besoin d'être épaulé par des "vérifications" (nées tests) automatisées. Certaines d'entre elles vont montrer à nos parties prenantes que le système fonctionne toujours. Certaines autres sont utilisées pour nous aider à trouver les anomalies lorsqu'elles finiront par arriver inévitablement. La plupart des tests des développeurs sont faits en dehors du processus TDD, par conséquent nous gardons aussi ce type de tests.

## People

## Personnes

People are more important than Product, even though my view centers on the product as the focus of our work, attention, and communication. We’ll follow the XP Practice _Whole Team_, or the Scrum dictum that the “Dev Team” includes all the skills necessary to build the desired product increment.

Les personnes sont plus importantes que le Produit, même si ma vision est tournée sur le produit comme étant le centre d'intérêt de notre travail, de notre attention et de notre communication. Nous allons suivre la pratique XP de _Toute l'Équipe_, ou la maxime Scrum de l'"Équipe de Développement" dans lesquelles toutes les compétences nécessaires pour construire l'incrément du produit désiré sont présentes.

We’ll surely move beyond that. We’ll want to address a connected business-side responsible person, where that’s needed. (XP _Customer_, Scrum _Product Owner_) In most companies, that’s always needed. We’ll want to address the need for real customer contact, a close connection to the real people who need to use the product or who will be impacted by it in important ways.

Nous irons certainement au-delà de ça. Nous voudrons nous adresser à une personne du côté métier, lorsque cela s'avère nécessaire (Le _Client_ dans XP, le _Product Owner_ dans Scrum). Dans la plupart des entreprises, c'est quelque chose qui est toujours nécessaire. Nous voulons gérer le besoin d'avoir le contact avec un vrai utilisateur, une relation étroite avec les vraies personnes qui ont besoin d'utiliser le produit ou qui seront impactées par le produit de manière importante.

There’s no inherent limit to who needs to be on the team, nor to who needs to be connected. Does the product have medical implications, tax implications, legal implications? Then we need medical, tax, and legal expertise on hand. Are they in the team or auxiliary to the team? You get to decide that. There will be issues of availability, delay, the need for the team to understand details, and so on. In principle, closer is better. In practice, we can’t all marry a doctor, a lawyer, and a tax expert.

Il n'y a pas de limite en tant que telle par rapport à qui doit être l'équipe, ni avec qui il est nécessaire d'être en contact. Est-ce que le produit a des implications médicales, des implications fiscales, des implications juridiques ? Si oui, alors nous aurons besoin d'expertise médicale, fiscale et juridique sous la main. Sont-elles dans l'équipe ou en complément de l'équipe ? Vous avez à décider cela. Il y aura des problèmes de disponibilités, de retard, le besoin pour l'équipe de comprendre les détails, et ainsi de suite. En principe, plus les contacts sont étroits, mieux c'est. En pratique, nous ne sommes pas mariés à un docteur, un avocat ou un fiscaliste.

The _People_ share _Collective Ownership_ of the product, as collectively as possible. Within the team, the developers share the code responsibility. No “my code / your code”: all “our code”. Everyone can and should improve everything that needs it, when it needs it.

Les _Personnes_ partagent la _Propriété Collective_ du produit, aussi collectivement que possible. À l'intérieur de l'équipe, les développeurs partages la responsabilité du code. Ce n'est pas "mon code / ton code" : c'est "notre code" à tous. Tout le monde peut et devrait améliorer tout ce qui doit l'être, lorsque ça a besoin de l'être.

Naturally, for this to work, we need an approach to working that keeps us from standing on each others’ feet. _Pair Programming_ and _Mob Programming_ surely come into this. We may need a _Coding Standard_ of some kind, maybe written, maybe just de facto.

Naturellement, pour ce travail, nous avons besoin d'une approche de travail pour éviter de nous marcher sur les pieds les uns les autres. La _Programmation en binôme_ et la _Programmation en groupe_ rentre très clairement dans ce cadre. Nous pouvons avoir besoin de _Convention de Codage_ d'une sorte ou d'une autre, peut être écrite, peut être de fait.

## Time

## Temps

On the one hand, our _Small Releases_ focus aims to drive the delay between having an idea and having it in the hands of the users down to zero.

D'un côté, nos _Petites Livraisons_ se focalisent pour faire tendre le délai entre la génération d'une idée et sa le fruit de sa concrétisation dans les mains des utilisateurs vers zéro.

But time, someone said[^1], is what keeps everything from happening at once. To keep everything from happening at once in my never-to-be-written framework, I recommend _Cadences_. We humans use days, weeks, months and so on, as markers of events. In our framework, we’ll use those intervals for _Daily Coordination, Product Review, Planning, Retrospectives,_ and so on.

Par temps, quelqu'un a dit [^1], c'est ce qui évite que tout arrive en même temps. Pour éviter que tout arrive en même temps dans mon cadre de travail qui-ne-sera-jamais-écrit, je recommande les _Cadences_. Nous autres, humains, nous utilisons les jours, les semaines, les mois et d'autres choses encore comme marqueurs d'évènements. Dans notre cadre de travail, nous utiliserons ces intervalles pour _la Coordination Quotidienne, la Revue du Produit, la Planification, les Rétrospectives_ et ainsi de suite.

What about _Iterations_ (Scrum’s “Sprint”)? I personally believe that a time box, used well, provides some important learning, especially in early days. I’ve often said that if a team can’t get a solid release done in two weeks, they should do it in one week. If they can’t do it in a week, they should do it in a day. If they can’t do it in a day, they should go home and rethink their life. Well, maybe not that last thing, but the point is, learning to complete a small bit of work, really complete, inside a time box, can be a valuable way to learn.

Et au sujet des _Itérations_ (les "Sprints" dans Scrum) je crois personnellement qu'un intervalle de temps [^2], bien utilisé, offre l'opportunité d'apprendre des choses importantes, tout spécialement dans les premiers jours. Je dis souvent que si une équipe n'arrive pas à faire une livraison sérieuse en deux semaines, elle devrait le faire en une semaine. Si elle ne peut le faire en une semaine, elle devrait le faire en une journée. Si elle ne peut le faire en une journée, les membres de l'équipe devraient retourner chez eux et repenser à leur vie. Euh, peut-être pas pour la dernière partie de la phrase, mais l'élément important ici, est d'apprendre à finir une petite quantité de travail, vraiment terminé, dans l'intervalle temps imparti, est une bonne manière d'apprendre.

That said, a time box surely has waste associated with it. Not everyone wants to go out drinking at noon on Friday if they’re done, and not everyone wants to start something new either. I believe, but do not know, that the right thing to do about _Iterations_ is perhaps to start with them, but to drive them to zero length, so that folks are just pulling the next story, getting it done, and releasing it, day in and day out.

Ceci dit, à un intervalle de temps est sûrement associé du gaspillage. Tout le monde ne veut pas sortir boire un coup à midi le vendredi s'ils ont fini, et tout le monde ne veut pas commencer quelque chose d'autre non plus. Je crois, mais ne sait pas, si la bonne chose à faire avec les _Itérations_ est de commencer avec elles peut-être, mais de faire tendre leur durée à zéro, afin que les personnes aient juste à tirer la prochaine _story_, la faire, et la livrer, jour après jour.

However, that grind will probably get really boring. We’ll use our _Cadences_ for the necessary punctuation that keeps us all from going bats.

Toutefois, il est probable que ce boulot deviendra vraiment ennuyeux. Nous utiliserons nos _Cadences_ pour avoir la ponctuation nécessaire qui nous empêchera de devenir maboules.

## Spirit [^3]

## Esprit

To me, “Agile” isn’t a set of practices. It’s what we described in the Manifesto, using Values and Principles. It’s a way of thinking, a spirit or manner of behaving. It focuses on letting responsibility and authority reside where the work is done, with support and true leadership coming from “above”. (We can debate elsewhere whether there should even be an “above”. For now, in these times, there is an above, and will be, most places, for a long time.)

Pour moi, "Agile" n'est pas un ensemble de pratiques. Pour moi, c'est ce que nous avons décris dans le Manifeste, avec les Valeurs et les Principes. C'est une manière de penser, un état d'esprit ou une manière de se comporter. Il se focalise sur le fait de laisser la responsabilité et le pouvoir de décider là où le travail est fait, avec le soutien et le véritable leadership qui vient "d'en-haut". (Nous pouvons débattre de ceci ailleurs si un en-haut devrait même exister. Pour l'instant, par les temps qui courent, il y a un en-haut, et il y en aura, dans la plupart des entreprises, encore pour un long moment).

For other views on this, we can look in part to Alistair Cockburn’s [Heart of Agile](http://heartofagile.com/), and Joshua Kerievskys [Modern Agile](http://modernagile.org/).

Pour avoir d'autres points de vue là dessus, nous pouvons jetons un coup d'œil au Cœur d'Agile d'Alistair Cockburn et au Modern Agile de Joshua Kerievskys.

Heart of Agile:
https://ronjeffries.com/articles/018-01ff/new-framework-xp/heart.png

Modern Agile:
https://ronjeffries.com/articles/018-01ff/new-framework-xp/modern.svg

Heart of Agile :


Modern Agile :


I note here the difference between these two names, and it is one that troubles me. To me, _Heart of Agile_ says “Hey, amid all the confusion, here’s what it’s all about”, while _Modern Agile_ says “Hey, Agile’s old hat, here’s a new hat”. I prefer the former. That said, both of these ideas bring out some important issues.

Je remarque ici une différence entre ces deux noms, et je suis troublé. De mon point vue, le _Cœur d'Agile_ dit "Hé, parmi tout ce brouhaha que vous pouvez entendre au sujet d'Agile, voici ce dont il s'agit", alors que _Modern Agile_ dit "Hé, Agile c'est un truc un peu vieillot, voici un nouveau truc tout neuf". Je préfère le premier. Ceci dit, ces deux idées mettent en lumière certains éléments importants.

Of those eight items, I want to emphasize “Make Safety a Prerequisite”, as I think it is by far the most important recent addition to the spirit of Agile, and I commend Joshua and his people for it. If an organization is going to become effective using Agile approaches, people have to be safe. (Not SAFe, by the way. Just safe.)

De ces huit items, je veux mettre en avant "Faire de la sécurité un pré-requis", car je pense qu'il est de loin la chose nouvelle la plus importante dans l'esprit Agile, et je suis reconnaissant à Joshua et à ses amis pour cela. Si une organisation se veut devenir plus efficace dans son utilisation des approches Agiles, les gens doivent se sentir _safe_, en sécurité. (Pas SAFe au fait. Simplement _safe_)

But I digress … where we we? Oh, Style …

Mais je m'égare … où en étions-nous ? Oh l'esprit …

There’s more to say about “Spirit”, to draw out XP’s notion of “Sustainable Pace”. There’s of course a great deal we could say about collaboration, how to review progress and process in an environment of safety, and so on. Perhaps, in due time, if I decide to define a framework [^3], I’ll have more to say about “Agile Spirit”. I’ll probably have more to say even if I don’t. For now, that’s all for “Spirit”.

Il y auriat encore beaucoup à dire à propos de l'"esprit", pour arriver à la notion de "Rythme Soutenable" d'XP.  Il y aurait beaucoup à dire à propos de la collaboration, sur comment nous passons en revue l'avancement et le processus dans un environnement sûr, et ainsi de suite. Peut-être en temps et en heure, si je me décide à définir un cadre de travail [^4], j'en dirai sans doute plus sur "l'Esprit Agile". J'aurai sans doute beaucoup plus de choses à dire que je ne le ferai. Pour l'instant, ce sera tout sur "l'Esprit"

## All The Rest

## Tutti quanti

What about how to estimate value, what about how to predict when you’ll be done, what about how to test your code, what about how to lead people, what about 300 ways to run a retrospective, what about remote programmers, what about diversity, what about compassion, what about people who want anchovies on their pizza, what about the ten thousand details that are part of being effective? I have in mind that on some magical four-dimensional diagram, we might fit them all in. We might connect these to specific skills that the team may need, and we should certainly always address the Style needed to apply those skills. Let me sketch one example here, not definitively but just to start us thinking:

Et qu'en t'il de comment évaluer la valeur, qu'en de comment prédire quand vous aurez fini, qu'en est-il de comment tester votre code, qu'en est-il de comment guider les gens, qu'en t'il des 300 manières de conduire une rétrospective, qu'en est-il des développeurs distants, qu'en est-il de la diversité, qu'en est-il des personns qui veulent des anchois sur leur pizza, qu'en est-il des dix mille détails qui font partie de devenir efficace ? J'ai en tête cela dans un diagramme magique à quatre dimensions, nous pourrions tout mettre dedans. Nous pourrions les connecter aux compétences spécifiques dont l'équipe peut avoir besoin, et nous devrons toujours prendre en compte l'esprit nécessaire pour appliquer ces compétences. Laissez-moi vous donnez un exemple, ce n'est qu'une esquisse mais c'est juste pour pouvoir démarrer notre réflexion :

Our company has someone from Marketing whom they’ve placed “in charge” of the product. This person has a role called “Product Owner”, because we are Scrummish. How should they interact with the development team?

Notre entreprise a nommé quelqu'un du Marketing pour "être en charge" du produit. Cette personne endosse un rôle dénommé "_Product Owner_" parce que nous sommes des Scrummistes. Comment devrait-elle interagir avec l'équipe de développement ?

First of all, this expertise should be part of the team, not separate from it. The PO’s main job should be to help everyone on the team begin to understand what the PO does, in terms of user needs and desires. The PO should bring actual users, with real needs, to visit with the team as often as possible, so that the team can begin to understand what’s really needed. While the PO may have the authority to tell the team what to do, they should never use it. Instead, they should build a common understanding of the needs, and help the team devise valuable and creative solutions to those needs.

Tout d'abord, cette expertise du Marketing devrait faire partie intégrante de l'équipe, et non se trouver en dehors. Le boulot principal du PO est d'aider les personnes de l'équipe à commencer à comprendre ce que le PO fait, en terme de besoins et de desirs utilisateur. Le PO devrait faire venir de vrais utilisateurs, avec de vrais besoin, afin qu'ils rendent visite à l'équipe aussi souvent que possible, afin que l'équipe comment à comprendre ce qui est vraiment voulu. Même si le PO peut avoir l'autorité pour dire à l'équipe quoi faire, ils ne devraient jamais l'utiliser. À la place, ils devraient développer une compréhension commune des besoins, et aider l'équipe à élaborer des solutions valables et créatives de ces besoins.

## Summing Up - For Now …

## En résumé - pour l'instant …

I just wanted to say a few words about the picture I tweeted last Saturday. I can’t boil down “Agile” to four bullet points, and frankly I don’t want to. I think it is more rich than that, more nuanced. But it’s not all about practices and canned methods, either.

je voulais juste dire quelque mot à propos d'une image que j'ai tweeté samedi dernier. Je ne peux réduire "Agile" à quatre points, et franchement je ne le souhaite pas. Je pense que c'est plus riche que cela, plus nuancé. Mais il ne s'agit que de pratiques et de méthodes en boîte non plus.

For now, it’s about People, Product, Time, and Spirit. Tomorrow, who knows? Stay tuned!

Pour aujourd'hui, c'est les Personnes, le Produit, le Temps et l'Esprit. Demain, qui sait ? Tenez-vous au courant.

[^1]: BAR : Brighton Agile Roundtable

    “Someone” is likely Ray Cummings, published in Argosy in 1921. The quote has been attributed to Einstein, Feynman, Wheeler, and even Woody Allen.” ↩

[^2]: Ce "quelqu'un" c'est sûrement Ray Cummings, publié dans Argosy en 1921. La citation a été attribué à Einstein, Feynman, Wheeler et même Woody Allen.

[^3]: NdT : Time box si vous préférez le terme anglo-saxon

    This used to be called “style”. I think I like “spirit” better. ↩

[^4]: Avant, ça s'appelait "style". Je pense que je préfère "esprit".  

    I won’t. Probably. ↩

[^5]: Je ne le ferais pas. Du moins probablement.

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

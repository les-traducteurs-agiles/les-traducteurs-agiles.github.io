---
layout: post
title:  "Un nouveau cadre de travail ? XP revisité ? Non ..."
date:   2018-09-20 00:01
published: true
tags:
- nouveau cadre de travail de développement logiciel
- agile
- xp
---

Je ne vais pas vraiment "Revisiter XP", et je ne vais pas vraiment définir un nouveau cadre de travail, néanmoins j'ai réfléchi sur ce que je crois et sur ce que je ressent à propos d'Agile, XP, Scrum et tutti quanti. L'une des choses que j'ai faite a été de poster ce dessin, réalisé au BAR [^1] dimanche :

![Pratiques XP revisitées]({{ site.url }}assets/ron_jeffries/revis_spirit_fr.jpg)

Toutefois, ce dessin ne représente que quelques notes prises sur le vif, et je ne garantis en rien que mon point de vue après-demain sera en cohérence avec ce dessin, ni même que ce dernier reflète exactement mon points de vue de samedi dernier. Mais, voici quelques éléments de réflexions sur ce dessin :

## Sujets principaux

Donc, là-bas, j'ai trouvé quatre rubriques, jusqu'à maintenant, sous lesquelles regrouper certaines idées : Produit, Personnes, Temps et Esprit

## Produit

Le produit est probablement l'idée centrale dans ma vision des choses. Un jour, Kent Beck a dit que toutes les méthodologies sont basées sur la peur, et ma plus grande peur est que, bien que nous allons faire du bon travail, travail qui mérite compréhension, soutien, et conseils, que personne ne soit au courant de ce travail que nous effectuons.

Donc mes préférences vont à ce qui permet de produire fréquemment un "incrément du produit", et de le montrer à toutes personnes intéressées. Nous nous focalisons sur des livraisons petites, fréquentes, et nous nous efforçons de tendre l'intervalle entre deux livraisons vers zéro.

Pour que cela marche, nous devons nous appuyer sur une conception simple et travailler dans ce sens, cette conception simple est soutenue par, et exige d'ailleurs pour autant que je le sache, un développement piloté par les tests [^2] et du _refactoring_. Étant donné que le système change tout le temps, je crois fermement qu'il doit être soutenu par des "vérifications" (_nées_ [^3] tests) automatisées. Certaines d'entre elles vont montrer à nos parties prenantes que le système fonctionne toujours. Certaines autres sont utilisées pour nous aider à trouver les anomalies lorsqu'elles finiront par arriver inévitablement. La plupart des tests des développeurs sont faits en dehors du processus de , par conséquent nous gardons aussi ce type de tests.

## Personnes

Les personnes sont plus importantes que le Produit, même si ma vision est tournée vers le produit comme centre d'intérêt de notre travail, de notre attention et de notre communication. Nous allons suivre la pratique XP de _l'Équipe En Entier_, ou la maxime Scrum de l'"Équipe de Développement" dans lesquelles toutes les compétences nécessaires pour construire l'incrément du produit désiré sont présentes.

Nous irons certainement au-delà de ça. Nous voudrons nous adresser à une personne du côté métier, lorsque cela s'avère nécessaire (Le _Client_ dans XP, le _Product Owner_ dans Scrum). Dans la plupart des entreprises, c'est quelque chose qui s'avère être toujours nécessaire. Nous voulons gérer le besoin d'avoir un contact avec un vrai utilisateur, une relation étroite avec les vraies personnes qui ont besoin d'utiliser le produit ou qui seront impactées par le produit de manière importante.

Il n'y a pas de limite en tant que telle sur qui doit faire partie l'équipe, ni avec qui il est nécessaire d'être en contact. Est-ce que le produit a des implications médicales, des implications fiscales, des implications juridiques ? Si oui, alors nous aurons besoin d'avoir sous la main une expertise médicale, fiscale et juridique. Ces expertises, font-elles partie intégrante de l'équipe ou dans un cercle plus élargi ? Vous devez décider de cela. Il y aura des problèmes de disponibilités, de retard, le besoin pour l'équipe de comprendre les détails, et ainsi de suite. En principe, plus les contacts sont étroits, mieux c'est. En pratique, nous ne sommes pas mariés à un docteur, un avocat ou un fiscaliste.

Les _Personnes_ partagent la _Propriété Collective_ du produit, aussi collectivement que possible. À l'intérieur de l'équipe, les développeurs partagent la responsabilité du code. Ce n'est pas "mon code / ton code" : c'est "notre code" à tous. Tout le monde peut et devrait améliorer tout ce qui doit l'être, lorsque ça a besoin de l'être.

Naturellement, pour que cela fonctionne, nous avons besoin d'une approche de travail pour éviter de nous marcher sur les pieds les uns les autres. La _Programmation en binôme_ et la _Programmation en groupe_ rentre très clairement dans ce cadre. Nous pouvons avoir besoin d'une _Norme de Codage_ d'une sorte ou d'une autre, qui peut être écrite, qui peut être de facto.

## Temps

D'un côté, nos _Petites Livraisons_ se focalisent pour faire tendre le délai entre la génération d'une idée et le fruit de sa concrétisation dans les mains des utilisateurs vers zéro.

Mais quelqu'un a dit [^4], "le temps ... est ce qui évite que tout arrive en même temps". Pour éviter que tout arrive en même temps dans mon cadre de travail qui-ne-sera-jamais-écrit, je recommande les _Cadences_. Nous autres, humains, nous utilisons les jours, les semaines, les mois et d'autres choses encore comme marqueurs d'évènements. Dans notre cadre de travail, nous utiliserons ces intervalles pour la _Coordination Quotidienne_, la _Revue du Produit_, la _Planification_, les _Rétrospectives_ et ainsi de suite.

Et au sujet des _Itérations_ (les "Sprints" dans Scrum) je crois personnellement qu'un intervalle de temps [^5], bien utilisé, offre l'opportunité d'apprendre des choses importantes, tout spécialement dans les premiers jours. Je dis souvent que si une équipe n'arrive pas à faire une livraison sérieuse en deux semaines, elle devrait le faire en une semaine. Si elle ne peut le faire en une semaine, elle devrait le faire en une journée. Si elle ne peut le faire en une journée, les membres de l'équipe devraient retourner chez eux et reconsidérer leur vie. Euh, peut-être pas pour la dernière partie de la phrase, mais l'élément important ici, c'est qu'apprendre à finir une petite quantité de travail, vraiment terminée, dans l'intervalle de temps imparti, est une bonne manière d'apprendre.

Ceci dit, il y a sûrement du gaspillage ici et là dans un intervalle de temps. Tout le monde ne veut pas sortir boire un coup le vendredi midi quand il a fini, ni commencer quelque chose d'autre non plus. Je crois, mais ne sait pas, si la bonne chose à faire avec les _Itérations_ ce serait de commencer avec, mais de faire tendre leur durée vers zéro, afin que les personnes n'aient qu'à tirer la prochaine _story_, la faire, et la livrer, jour après jour.

Toutefois, il est probable que ce boulot pourrait devenir vraiment ennuyeux. Nous utiliserons donc nos _Cadences_ pour avoir la ponctuation nécessaire qui nous empêchera de devenir maboules.

## Esprit [^6]

Pour moi, "Agile" n'est pas un ensemble de pratiques. Pour moi, Agile est ce que nous avons décris dans le Manifeste, avec les Valeurs et les Principes. C'est une manière de penser, un état d'esprit ou une manière de se comporter. Il se focalise sur le fait de laisser la responsabilité et le pouvoir de décider là où le travail est fait, avec le soutien et le véritable leadership qui vient "d'en-haut". (Nous pouvons débattre de ceci ailleurs si un en-haut devrait d'ailleurs même exister. Pour l'instant, par les temps qui courent, il y a un en-haut, et il y en aura, dans la plupart des entreprises, encore pour longtemps).

Si nous voulons avoir d'autres points de vue sur le sujet, nous pouvons jeter un coup d'œil au [Cœur d'Agile](http://heartofagile.com/) d'Alistair Cockburn et à [Modern Agile](http://modernagile.org/) de Joshua Kerievskys.

Cœur d'Agile :
![Cœur d'Agile]({{ site.url }}assets/ron_jeffries/Heart_of_Agile_logo_fr.png)

Modern Agile :
![Modern Agile]({{ site.url }}assets/ron_jeffries/Modern_Agile_logo_fr.png)

Je remarque ici une différences entre ces deux noms, et c'est une différence qui me trouble. De mon point vue, le _Cœur d'Agile_ dit "Hé, parmi tout le brouhaha que vous pouvez entendre [^7], voici vraiment ce dont il s'agit", alors que _Modern Agile_ dit "Hé, Agile c'est un vieux chapeau, voici un nouveau chapeau". Je préfère le premier. Ceci dit, ces deux idées mettent en lumière certains éléments importants.

De ces huit items, je veux mettre en avant "Faire de la sécurité un pré-requis", car je pense qu'il est de loin la chose nouvelle la plus importante dans l'esprit Agile, et je suis reconnaissant à Joshua et à ses amis pour cela. Si une organisation veut devenir plus efficace dans son utilisation des approches Agiles, les gens doivent se sentir _safe_ [^8], en sécurité. (Pas SAFe au fait. Simplement _safe_)

Mais je m'égare … où en étions-nous ? Oh l'esprit …

Il y aurait encore beaucoup à dire à propos de l'"esprit", pour arriver à la notion de "Rythme Soutenable" d'XP.  Il y aurait beaucoup à dire à propos de la collaboration, sur comment nous passons en revue l'avancement et le processus dans un environnement sûr, et ainsi de suite. Peut-être en temps et en heure, si je me décide à définir un cadre de travail [^9], j'en dirai sans doute plus sur "l'Esprit Agile". J'aurai sans doute beaucoup plus de choses à dire que je ne le ferai. Pour l'instant, ce sera tout sur "l'Esprit"

## Tutti quanti

Et qu'en est-il de comment évaluer la valeur, qu'en est-il de comment prédire quand vous aurez fini, qu'en est-il de comment tester votre code, qu'en est-il de comment guider les gens, qu'en t'il des 300 manières de conduire une rétrospective, qu'en est-il des développeurs distants, qu'en est-il de la diversité, qu'en est-il des personnes qui veulent des anchois sur leur pizza, qu'en est-il des dix mille détails qui font partie de devenir efficace ? J'ai en tête tout cela dans un diagramme magique à quatre dimensions, nous pourrions tout mettre dedans. Nous pourrions les connecter aux compétences spécifiques dont l'équipe peut avoir besoin, et nous devrions toujours prendre en compte l'esprit nécessaire pour appliquer ces compétences. Laissez-moi vous donnez un exemple, ce n'est qu'une esquisse mais c'est juste pour pouvoir démarrer notre réflexion :

Notre entreprise a nommé quelqu'un du Marketing pour "être en charge" du produit. Cette personne endosse un rôle dénommé "_Product Owner_" parce que nous sommes des Scrummistes. Comment devrait-elle interagir avec l'équipe de développement ?

Tout d'abord, cette expertise du Marketing devrait faire partie intégrante de l'équipe, et non se trouver en dehors. Le boulot principal du PO est d'aider les personnes de l'équipe à commencer à comprendre ce que le PO fait, en terme de besoins et de désirs utilisateur. Le PO devrait faire venir de vrais utilisateurs, avec de vrais besoin, afin qu'ils rendent visite à l'équipe aussi souvent que possible, afin que l'équipe commence à comprendre ce qui est vraiment voulu. Même si le PO peut avoir l'autorité pour dire à l'équipe quoi faire, il ne devrait jamais l'utiliser. À la place, il devrait développer une compréhension commune des besoins, et aider l'équipe à élaborer des solutions valables et créatives de ces besoins.

## En résumé - pour l'instant …

Je voulais juste dire quelque mot à propos d'une image que j'ai tweetée samedi dernier. Je ne peux réduire "Agile" à quatre points, et franchement je ne le souhaite pas. Je pense que c'est plus riche que cela, plus nuancé. Mais il ne s'agit pas uniquement de pratiques et de méthodes en boîte non plus.

Pour aujourd'hui, c'est les Personnes, le Produit, le Temps et l'Esprit. Demain, qui sait ? Tenez-vous au courant.

[^1]: BAR : Brighton Agile Roundtable - NdT

[^2]: ou TDD (pour Test-Driven Development) si vous préférez le terme anglo-saxon - NdT

[^3]: en français dans le texte original - NdT

[^4]: Ce "quelqu'un" est probablement Ray Cummings dans le magasine Argosy en 1921. La citation a également été attribuée à Einstein, Feynman, Wheeler et même à Woody Allen.

[^5]: _Time box_ si vous préférez le terme anglo-saxon - NdT

[^6]: Avant, ça s'appelait "style". Je pense que je préfère "esprit".  

[^7]: Au sujet d'Agile - NdT

[^8]: En plus du terme traduit _en sécurité_, le terme original a été laissé sinon le jeu de mot avec SAFe (Scaled Agile Framework) n'aurait pas été compréhensible - NdT

[^9]: Je ne le ferais pas. Du moins probablement.

---
Auteur : [Ron Jeffries](https://ronjeffries.com/about.html)  
Source : [New Framework? XP Revisited? No ...](https://ronjeffries.com/articles/018-01ff/new-framework-xp/#fnref:style)  
Date de parution originale : 17 Septembre 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 23/09/2018  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

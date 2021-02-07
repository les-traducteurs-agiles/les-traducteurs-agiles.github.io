  ---
layout: post
title:  "Le triathlon du développement produit"
date:   2020-12-13 10:57
published: false
tags:
- tag1
- tag2
---

Republished from [the original](https://www.facebook.com/notes/kent-beck/the-product-development-triathlon/1215075478525314/) published on July 19, 2016.

Le présent article est la republication d'un [précédent article](https://www.facebook.com/notes/kent-beck/the-product-development-triathlon/1215075478525314/) datant du 19 juillet 2016.

25 March 2016. Because I keep careful notes these days I can identify the precise moment when I asked the question I should have asked twenty years ago: what if those waterfall folks aren’t wrong, what if they are solving a different problem than I’m solving? What problem is that?

25 Mars 2016. En raison du fait que je prends des notes méticuleusement ces derniers temps, je suis en capacité d'identifier le moment précis où je me suis posé la question que j'aurais dû me poser il y a 20 ans : et si les gars à l'origine de la gestion de projets en cascade n'avaient pas tort, et s'ils essayaient de résoudre un autre problème que celui que j'essaye de résoudre ? Mais de quel problème s'agit-il ?

![Image for post](https://miro.medium.com/max/50/0*9RQtH0oI3QejpfXn?q=20)

![Image for post](https://miro.medium.com/max/720/0*9RQtH0oI3QejpfXn)

![Image for post](https://miro.medium.com/max/1440/0*9RQtH0oI3QejpfXn)

![toutou]({{ site.url }}assets/kent_beck/kent-notebook.jpg)

The Moment of Insight

L'épiphanie

The past four months have been fecund beyond belief for me. I have changed how I approach software development but also life in general. Different risk profiles call for different approaches, but I can sometimes choose which risk profile I use in a situation.

Les quatre deniers mois ont été féconds au-delà de toute espérance en ce qui me concerne. J'ai changé quant à ma manière d'aborder le développement logiciel mais aussi la vie en général. Différents profils de risques exigent différentes approches.

Trying to communicate my insight has been frustrating. I feel like a puppy on a hike. I’ve run ahead, found an _awesome_ stick, brought it back, dropped it at my masters’ feet, and now I’m barking madly without anyone paying to attention to just how _awesome_ the stick really is.

Essayer de communiquer cette révélation s'est avérée plutôt frustrante. Je me sens comme un chiot en promenade. C'est comme si je courais devant, que je trouvais un _super_ bâton, que je le ramènais, que je l'apportais aux pieds de mon maître et que j'aboyais maintenant dans tous les sens sans que personne ne prête attention à ce bâton et à quel point il est vraiment _super_.

I awoke in the middle of the night with a new approach, a new metaphor to go with the new vocabulary I’m using. Here goes.

Je me suis réveillé au milieu de la nuit avec une nouvelle approche, une nouvelle métaphore avec un nouveau vocabulaire à utiliser. Le voici.

# Explore/Expand/Extract

# Explorer / Étendre / Extraire

![Image for post](https://miro.medium.com/max/667/0*-Df9CIHNkU1Pfvg_)

![explorer-étdendre-extraire]({{ site.url }}assets/kent_beck/note-rose-fr.png)


Explore/Expand/Extract


Explorer / Étendre / Extraire

Product development proceeds in three phases:

Le développement produit se déroule en trois phases :

1. Explore–the risky search for a viable return on a viable investment. Successful exploration is unpredictable, so the highest expected value strategy is to reduce the cost of experimentation and put a little investment into many, uncorrelated experiments. If you’re lucky, one of these experiments turns out to be unexpectedly successful, which leads to:

1. Explorer - en partant dans une quête difficile et risquée en vue d'obtenir un retour viable sur un investissement viable. Une exploration couronnée de succès est, par nature, complètement imprévisible, donc la stratégie pour obtenir la valeur attendue la plus élevée est de réduire le coût de l'expérimentation et de faire de petits investissements dans plusieurs expérimentations non corrélées les unes aux autres. Si vous êtes chanceux, et que l'une de ces expériences s'avère fructueuse cela nous conduit à :

2. Expand–now things are going nuts (think Pokemon Go or Facebook Live Video). Unanticipated bottlenecks appear. All you have time for is to eliminate the next bottleneck just before it derails you. Once growth becomes routine, it’s time to:

2. Étendre - maintenant les choses deviennent un peu folles (pensez à Pokemo Go ou à Facebook Live Video). Des goulots d'étranglements inattendus font leur apparition. Tout ce que vous pouvez faire c'est éliminer le goulot d'étranglement qui arrive juste avant qu'il ne vous fasse échouer. Une fois que la croissance est devenue routine, il est temps de :

3. Extract–now the shape of the problem and solution spaces are clear. One euro in equals three euros out. Playbooks emerge: here’s how you roll out the service in a new city. Economies of scale matter: delivering the service at lower cost is more profitable.

3. Extraire - maintenant la forme des espaces du problème et de la solution sont clairs. Un euro investi équivaut à 3 euros récupérés. Des stratégies émergent : par exemple voici comment mettre en place ce service dans une nouvelle ville. Les économies d'échelles sont aussi à prendre en compte : livrer le service à un coût plus bas s'avère davantage profitable.

There’s hours and hours of cool stuff implied by this model, but that’s the basics.

Bref, nous avons plein et plein d'heures cool devant nous en perspective pour creuser ce qu'implique ce modèle mais nous venons d'en voir l'essentiel.

# Lessons from the Triathlon

# Leçons apprises de ce Triathlon

* Each phases requires different equipment, different technique, different training. Software product development requires different tools, techniques, and value systems in the three phases. (The answer to the ??? in my notebook is “Efficient Extraction”.)

* Chaque phase requiert un équipement différent, une technique différente, une formation différente. Le développement d'un produit logiciel nécessite différents outils, techniques, et systèmes de valeur dans les 3 phases.

* You can’t mix the phases. Just because biking is the fastest phase in kilometers per hour doesn’t mean you can go faster by taking your bike into the water. (I was dealing with a project prematurely moving from explore to expand just yesterday.)

* Vous ne pouvez pas mélanger les phases. Ce n'est pas parce qu'aller en vélo est ce qui vous permet d'aller le plus vite possible en km/h que vous pouvez pédaler dans l'eau. (Je me suis occupé tout juste hier d'un projet qui est passé de la phase explorer à la phase étendre).

* The transitions are awkward, but they count. If a project goes from one phase to another and the team doesn’t notice, it’s like trying to swim on a bike. Not so good.

* Les transitions sont délicates, mais elles sont essentielles. Si un projet passe d'une phase à une autre et que l'équipe ne le remarque pas, c'est comme essayer de nager sur un vélo. Ça ne marche pas très bien.

* Only organizations that can execute all three phases can complete a race. If you just don’t feel like running, then it’s not a triathlon.

* Seules les organisations en capacité d'accomplir les trois phases peuvent terminer la course. Si vous n'avez pas envie de courir, alors ce n'est pas un triathlon.

* Unlike a triathlon, the same people don’t have to complete the phases. I specialize in exploration. As soon as expansion starts, I’m ready to start exploring again. As long as there is someone I can hand off to, this works fine.

* Au contraire d'un triathlon, il n'est obligatoire que tout le monde ait à accomplir toutes les phases. Je me spécialise en exploration. Dès que l'expansion commence, je suis prêt à explorer à nouveau. Tant qu'il y a quelqu'un à qui je peux passer le relais, ça marche.

* The relative progress of the three phases roughly maps. Exploration (swimming) seems slow. Experiment after experiment fails. False hopes are dashed. Repeatedly. Then comes the “overnight success” of expansion (biking). Progress that would have taken months now happens in days or hours, just like a mile on a bike is _way_ shorter than a mile swimming. Extraction (running) is more of a slog than expansion.

* La manière dont chacune des trois phases avance se recoupe peu ou prou. L'exploration (la nage) paraît lente. Les expériences échouent les unes après les autres. Les faux espoirs sont anéantis. Jour après jour. Puis vient le succès du jour au lendemain de l'expansion (le vélo). Les progrès qui auraient pris des mois se font en quelques jours ou quelques heures, tout comme un kilomètre en vélo est _un monde_ plus court qu'un kilomètre à la nage.

* ??? \[hoping for suggestions from actual triathletes or poets\]

* ??? \[j'espère avoir quelques suggestions de la part de tri-athlètes ou de poètes\]

# Application

# Application

A few highlights:

Quelques éléments à souligner :

* Choose exploration. If you’re extracting and starting to feel hopeless or burned out, deliberately switch to exploration.

* Choisir l'exploration. Si vous êtes en pleine extraction et que vous commencez à perdre espoir ou que êtes victime de surmenage, passez alors délibérément en phase d'exploration.

* Accelerate experimentation. If you’re following all the rules and your experiments aren’t getting anywhere, break the rules to experiment faster. If experiments aren’t likely to last, quick and easy won’t cost you in the long run.

* Accélérer l'expérimentation. Si vous avez suivi toutes les règles et que vos expériences ne mènent nulle part, brisez alors les règles pour expérimenter plus vite. Si ces expérimentations n'ont pas été faites pour durer, quelque chose de rapide et de facile ne vous coûtera pas alors grand chose à long terme.

* Transition. If things aren’t going smoothly, see if you’ve changed phases without noticing. If so, change the rules to match the phase you’re in.

* Transition. Si les choses ne se passent pas bien, regardez si vous avez changé de phases sans y prêter attention. Si c'est le cas, changez alors les règles pour qu'elles correspondent à la phase dans laquelle vous êtes.

I’m only four months in, so I’m sure there’ll be lots more to come. I hope I’ve convinced you that this really is an _awesome awesome_ stick.

Cela ne fait que quatre mois que je creuse le sujet, et je suis sûr qu'il y a beaucoup d'autres choses que je vais découvrir. J'espère vous avoir convaincu qu'il s'agit d'un _super super_ bâton.

![Image for post](https://miro.medium.com/max/60/0*dJX4T7elMoDeU_Y5?q=20)

![Image for post](https://miro.medium.com/max/522/0*dJX4T7elMoDeU_Y5)

![Image for post](https://miro.medium.com/max/1044/0*dJX4T7elMoDeU_Y5)

![toutou]({{ site.url }}assets/kent_beck/toutou.jpg)


Gratuitous Puppy Picture

Image tout à fait gratuite d'un toutou

---
Auteur : [Ken Beck](https://medium.com/@kentbeck_7670/about)  
Source : [The Product Development Triathlon](https://medium.com/@kentbeck_7670/the-product-development-triathlon-6464e2763c46)  
Date de parution originale : 20 Novembre 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : jj/mm/yyyy  nbsp

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

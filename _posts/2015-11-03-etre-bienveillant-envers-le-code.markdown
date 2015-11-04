---
layout: post
title:  "Être bienveillant envers le code"
date:   2015-11-03 21:00:55
published: true
categories: 
- developpement
---

As a programmer I spend a lot of time in front of the computer. But despite appearances, I am not there. I am not in front of a computer every day for 8 hours drying my eyes and weakening my muscles. I am somewhere else.

En tant que programmeur, je passe beaucoup de temps en face d'un ordinateur. Mais en dépit des apparences, je ne suis pas là, je ne suis pas devant un ordinateur 8 heures par jour m'abîmant les yeux et affaiblissant mes muscles. Je suis quelque part ailleurs.

I am in an amazing world of executable ideas, manipulating abstract artifacts made of concepts. I am assembling them to generate a meaningful structure in which a computer program can evolve. This world is like a city that grows as we add more behavior to it. This world has the neighborhood of repositories, the shopping cart markets, the fashion contests of views, controllers directing traffic, etc.

Je suis dans un monde spectaculaire d'idées exécutables, manipulant des artéfacts abstraits faits de concepts. Je les assemble pour générer une structure significative dans laquelle un programme d'ordinateur peut évoluer. Ce monde est comme une cité qui grossit au fur et à mesure que nous y ajoutons de nouveaux comportements. Ce monde a comme voisinage des dépôts, des marchés de paniers d'achats, des vues de concours de mode, de contrôleurs orientant le trafic, etc.

But this city is not mine alone. It’s built by all the people on my team. It’s a place shared with others, where our creations grow together. It starts small and simple like a village with just a few small classes, but as time passes it can evolve into a crowded city which abounds with components. Some of the neighborhoods are clean and artfully crafted with well decoupled skyscrapers, while others are rotting, under the pressure to “Deliver now!”

Mais cette cité n'est pas à moi tout seul. Elle est construite par toutes les personnes de mon équipe. C'est un endroit partagé avec d'autres, où nos créations grandissent ensemble. Elle commence simple et petite come un village avec juste quelques petites classes, mais le temps passant elle évolue en une cité bien peuplée et qui abonde de multiples composants. Une partie du voisinage est bien propre et délicatement ouvragé avec des grattes-ciels bien découplés, alors que d'autres sont en train de se détériorer, sous la pression de "Livrez maintenant !"

## The Broken Window Theory

## La théorie de la fenêtre brisée

The Broken Window Theory is based on a set of experiments on abandoned cars. Researchers left a car parked in Palo Alto, Calif., where it remained intact for more than a week. After a week, a researcher returned to the car and broke a window. Once the car seemed abandoned, rather than simply parked, it didn’t take long to be vandalized and destroyed. It only took one broken window to start the process.

La théorie de la fenêtre brisée est basée sur une série d'expériences sur les voitures abandonnées. Les chercheurs avaient laissé une voiture garée à Palo Alto en Californie, où elle resta intact pendant plus d'une semaine. Une semaine après, un chercheur retourna à la voiture et cassa une vitre. Une fois que la voiture sembla abandonnée, plutôt que simplement garée, il ne se passa pas beaucoup de temps avant qu'elle soit vandalisée et détruite. Il suffit d'une vitre brisée pour démarrer ce processus.

The theory, in a nutshell, states that social perception of how much the people around you “care” about something is an important factor in how much care you devote to the same thing. When you see litter in the streets, throwing one more wrapper doesn’t make a difference. When the streets around you are clean, you pause and question yourself.

La théorie, en quelques mots, indique que la perception sociale du degré de préoccupation que les gens autour vous montre à propos de quelque chose est un facteur important de votre propre degré de préoccupation pour cette même chose. Lorsque vous voyez des détritus dans la rue, jeter un papier sale de plus par terre ne fait pas beaucoup de différence. Lorsque les rues autour de vous sont propres, vous vous arrêtez et vous réfléchissez. 

The other part of the theory is that problems are easier to fix when they are small. What begins with a single broken window leads to more broken windows, and eventually to abandoned or bug-infested buildings. Small problems can easily become big problems if we don’t fix them quickly.

L'autre partie de la théorie est que les problèmes sont plus faciles à corriger lorsqu'ils sont petits. Ce qui commence avec une seule fenêtre cassée conduit à davantage de fenêtres cassées, et éventuellement à des bâtiments abandonnés ou infestés de vermines. Les petits problèmes peuvent devenir facilement de gros problèmes si nous ne les corrigeons pas rapidement.

## Are you contributing to the Broken Window Effect?

## Contribuez-vous à l'effet de la fenêtre cassée ?

As a good programmer, chances are that you are really good at finding errors, or better ways to implement another developer’s code. Sometimes I find myself wondering what the dev who wrote that code was thinking, or even calling it “crap” out loud. But what happens if I don’t actually change it?

En tant que bon développeur, il y a de fortes chances que vous soyez vraiment bon pour trouver des erreurs, ou que vous trouviez de meilleures façons d'implémenter le code d'un autre développeur. Quelques fois je m'aperçois que je m'interroge sur ce à quoi pensait le développeur qui a écrit ce code était en train de penser, ou même s'il l'appelait "tas de merde" à voix haute. Mais que se passe t'il si je ne le change pas ?

What’s the effect of highlighting something really wrong with the code, and not doing anything about it? It’s like pointing at a broken window and letting everybody know that vandalizing this neighborhood is acceptable.

Quel est l'effet de pointer du doigt quelque chose de vraiment mauvais dans le code, et de ne rien faire dessus ? C'est comme montrer une fenêtre cassée et laisser savoir à tout le monde que vandaliser le voisinage est acceptable.

Having broken code is not great, but the real danger lies in what happens when you and your team accept it as reality and nobody fixes it. Imagine the effect on new team members when everybody acts like that. It’s like an invitation to live in one of the worst parts of the city. Would you like to stay there? Would you have the courage to improve things if no one else does?

Avoir du code dégradé n'est pas génial, mais le réel danger repose sur ce qui se passe lorsque vous et votre équipe l'accepte en tant que réalité et que personne ne le corrige. Imaginez l'effet que cela peut avoir sur les nouvelles personnes de l'équipe quand tout le monde agit de cette manière. C'est comme une invitation à vivre dans l'une des pires parties de la cité. Aimeriez-vous vivre là ? Auriez-vous le courage d'améliorer les choses si personne d'autre ne le fait ?

If broken windows accumulate, then at some point the gradual decay in quality of your project gets out of control. As with the Broken Window Theory, the cost of refactoring entangled code is smaller up front, but if you delay it, it quickly becomes unaffordable.

Si les fenêtres cassées s'accumulent, alors au bout d'un moment la dégradation graduelle dans la qualité de votre projet sera hors de contrôle. Comme avec la théorie de la fenêtre cassée, le coût du _refactoring_ d'un code emmêlé est faible au début, mais si vous trainez, il deviendra rapidement inabordable.

The biggest difference-maker in the quality of a project is the development team’s attitude toward improving things.

Le plus gros marqueur de différence dans la qualité d'un projet est l'attitude de l'équipe vis-à-vis de l'amélioration des choses.

## The Boy Scout rule

## Le règle du scout

Good teams follow the Boy Scout rule: “Always leave the campground cleaner than you found it.” Good teams improve the environment, making it easier for the rest to add new code. Make your city better by slowly fixing one window at the time. Do it while you are adding a new feature nearby. There is no bad neighborhood for the Boy Scout rule.

Les bonnes équipes suivent la règle du scout : "Toujours laissé le terrain du campement plus propre que vous ne l'avez trouver." Les bonnes équipes améliorent l'environnement, rendant les choses plus faciles pour les autres pour ajouter du nouveau code. Rendre votre cité plus belle lentement en réparant une fenêtre à la fois. Faites-le pendant que vous êtes en train d'ajouter une nouvelle fonctionnalité dans le coin. Il n'y a pas de voisinage en mauvais état avec la règle du scout.  

One of the first steps for applying the rule is to stop ignoring the difficult code. By calling code bad, you are labeling it as code that is not worth rescuing. When you do so, you are reinforcing the idea that your neighborhood is a bad neighborhood. Being ‘crap’ is then an essential part of your code, and there is nothing you could do about it.

L'une des premières étapes pour appliquer cette règle est d'arrêter d'ignorer le code difficile. En nommant un code comme mauvais, vous êtes en train de l'étiqueter comme étant un code ne valant pas le coup d'être sauvé. Quand vous faites ça, vous êtes en train de renforcer l'idée que votre voisinage est un mauvais voisinage. Avoir "un tas de merde" devient alors une part essentielle de votre code, et il n'y a rien que vous pourriez faire pour empêcher ça.

Instead, treat it as “unattended.” This does not state that the code is good, but it expresses your willingness to improve it. It’s a piece of software that is actually working, but is waiting for (and deserves) some attention and care.

À la place, traitez-le comme "sans surveillance". Cela ne veut pas dire que le code est bon, mais cela exprime votre volonté de l'améliorer. C'est un morceau de logiciel qui fonctionne vraiment, mais qui attend d'avoir (et qui mérite) un peu d'attention et de soin.

## So, now what?

## Et, maintenant quoi ?

If you feel like you don’t know where to start improving your city... If you see a lot of broken windows... If you know your city needs to get better... Then start taking action now.

Si vous sentez que vous ne savez pas par où commencer pour améliorer votre cité... Si vous voyez beaucoup de vitres cassées... Si vous savez que votre ville a besoin d'aller mieux... Alors commencez à agir maintenant.

You can encourage people to take actions by just changing the words you use. Start talking about the state of the code in a time frame (e.g. “It’s unattended for now”) and take away the idea of code being “crap.” Doing so, you generate the proper environment to apply the Boy Scout rule. Start refactoring little pieces of software when you see the opportunity, and encourage your team to do the same.

Vous pouvez encouragez les personnes à agir simplement en changeant les mots que vous utilisez. Commencez en parlant de l'état du code dans une période donnée (par exemple "c'est sans surveillance pour l'instant".) et bannissez l'idée que le code est un "tas de merde". En faisant cela, vous générez un environnement propice à l'application de la règle du scout. Commencez par _refactorer_ des petits morceaux de logiciels lorsque vous en verrez l'occasion et encouragez votre équipe à faire de même.

Resources :

"Is the Broken Windows Theory Effective?" - SiOWfa13: Science in Our World: Certainty and Controversy. N.p., n.d. Web. 01 Oct. 2015.



---  
Auteur : [alexandru codreanu, dario garcia, lucas giudice](http://www.8thlight.com/team/)  
Source : [Caring about coding](https://blog.8thlight.com/alexandru-codreanu/dario-garcia/lucas-giudice/2015/10/30/caring-coding.html)  
Date de parution originale : 30 Octobre 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 03/11/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



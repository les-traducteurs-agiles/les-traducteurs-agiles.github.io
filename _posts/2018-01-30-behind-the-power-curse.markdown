---
layout: post
title:  "À l’opposé de la courbe de puissance"
date:   2018-02-08 00:00:01
published: false
tags: 
- agile
- équipe
- vélocité
---

I promise that this blog is about software. So bear with me for a bit.

J’avais promis que ce blog ne parlerait que d’informatique. Donc laissez-moi quelques minutes pour vous expliquer ce qui suit.

What happens when you increase the throttle in an airplane? You go faster, right? More power to the engine means more thrust which means more speed.

Que se passe t’il si vous poussez la manette des gaz dans un avion ? Vous volez plus vite, n’est-ce-pas ? Davantage de puissance dans le moteur signifie par plus de poussée donc par plus de vitesse.

Most of the time this is true; but there’s a different mode you can get the aircraft into which reverses this relationship. It’s called: the region of reversed command.

C’est vrai la plupart du temps ; mais il existe une situation où vous pouvez faire que cette relation s’inverse dans un avion. Cela s’appelle : `la zone de second régime

Remember the four forces that govern flight: gravity, lift, thrust, and drag. Lift opposes gravity, and thrust opposes drag. An airplane, in straight and level flight, balances all these forces perfectly.

Rappelez-vous, les quatre forces qui gouvernent le vol : la gravité, la portance, la poussée et la trainée. La portance s’oppose à la gravité, et la poussée à la trainée. Dans un aéroplane en vol linéaire et en palier, l’ensemble de ces forces s’équilibre parfaitement.

Thrust, of course, comes from the engine. Lift comes from the air flowing around the wings, and drag…? Well, drag comes from two different sources.

La poussée, bien sûr, vient du moteur. La portance vient de l’air circulant autour des ailes, et la trainée … ? Eh bien, la trainée a principalement deux origines.

Parasitic drag is simply the cost of plowing through the air. It is the air resisting the movement of the plane. But there’s another kind of drag called induced drag.

La trainée parasite est tout simplement le `coût` de pénétration dans l’air. C’est la résistance de l’air au mouvement de l’avion.  Mais il existe une autre type de trainée appelée trainée induite.

Induced drag is caused by the pilot. It happens when the pilot raises the nose of the aircraft. Raising the nose, changes the angle of the wings causing the lift vector, which is always perpendicular to the wings, to point a bit backwards, thereby opposing the forward motion of the aircraft.

La trainée induite est causée par le pilote. Cela arrive lorsque le pilote relève le nez de l’aéronef. Relever le nez change l’`incidence/assiette`des ailes provoquant le vecteur de portée, qui est toujours perpendiculaire à la surface des ailes, et qui pointe légèrement vers l’arrière et donc s’opposant au déplacement vers l’avant de l’avion.

If you raise the nose just a little, the induced drag is small, and so increased thrust still causes increased speed. But if you raise the nose a lot, then the induced drag can cancel out the thrust. This is called getting behind the power curve.

Si vous relevez le nez juste un peu, la trainée induite est limitée et donc l’augmentation de la poussée provoque toujours l’augmentation de la vitesse. Mais si vous relevez beaucoup le nez, alors la trainée induite peut annuler totalement l’effort de poussée. Cela s’appelle être à l’`opposé` de la courbe de puissance. 

The graph[1] shows an airplane in straight and level flight. To the right, you can see that the speed and power have a positive relationship. The more power, the more speed. But to the left, in the region of reversed command, it takes more and more power to go slower and slower.

L’illustration [1] montre un avion en vol linéaire et en palier. À droite, vous pouvez observer que la vitesse et la puissance ont une relation `positive`. Plus puissance égale plus de vitesse. Mais à gauche dans la `zone de second régime`, il est nécessaire d’avoir de plus en plus de puissance pour aller de plus en plus lentement. 

In other words, the pilot has the nose so high that the thrust vector is being defeated by the backwards pointing lift vector; and the plane is kind of mushing through the air on raw power, barely making any headway.

Autrement dit, le pilote a tellement relevé le nez que le vecteur de poussée est dépassé par le vecteur de portance qui le tire vers l’arrière ; l’avion lutte donc contre l’air à pleine puissance sans avancer le moins du monde

> Can you see where I’m going with this?

> Voyez-vous où je veux en venir ?

Except during the final moments of landing, pilots don’t usually operate their aircraft behind the power curve. It’s a bit dangerous back there. The slower you go, the more power you need. If you go slow enough, you’ll max out your power and descend with the stall warning screaming in your ears. So pilots stay in front of the power curve by watching their airspeed, and keeping it above the inflection point.

Sauf au moment final de l’atterrissage, les pilotes se gardent de mettre leur avion en second régime. C’est un moment un peu dangereux. Plus vous allez lentement, plus vous avez besoin de puissance. Au point qu’à un moment, vous aurez le maximum de puissance tandis que l’alarme de décrochage vous hurlera aux oreilles. Les pilotes doivent donc rester en premier régime en surveillant la vitesse-air[1], et en la gardant au-dessus du point d’inflexion. 

So what does this have to do with software? (As if you haven’t already guessed.)

Donc, qu’est-ce que cela à à voir avec l’informatique ? (dans le cas où vous n’auriez pas deviné.)

Too many software teams operate behind the power curve all the time. Rotten code is induced drag. These teams have created so much induced drag that it takes a huge effort to make any forward progress. The team mushes forward at full power, barely making any headway. Indeed, many teams have maxed out their power and are in a slow uncontrollable descent.

De trop nombreuses équipes informatiques travaillent au second régime tout le temps. La trainée induite correspond à du code pourri. Ces équipes ont généré tellement de trainée induite que cela demande un effort gigantesque pour faire la moindre avancée. L’équipe lutte pour aller de l’avant à pleine puissance, sans faire des avancées vraiment significatives. En effet, certaines équipes ont maximisé leur puissance et sont dans une lente descente incontrôlable.

How does a pilot get out from behind the power curve? By lowering the nose. This brings the lift vector to vertical allowing the thrust vector to dominate, and the plane screams off into the wild blue yonder.

Comment fait un pilote pour rester en dehors du second régime ? En baissant le nez. Cela amène le vecteur de portance à la verticale, permettant ainsi au vecteur de poussée de dominer, et l’avion de vrombir par un beau ciel dégagé

How does a software team get out from behind the power curve? By lowering their noses, cleaning up the messes, and reducing the induced drag. With that drag gone, and all the power they have, the wild blue yonder is theirs to explore.

Comment une équipe informatique se sort-elle du second régime ? En baissant le nez, en nettoyant leur bazar, et réduire la trainée induite. Une fois cette trainée disparue, et avec toute la puissance dont elle dispose, le beau ciel est désormais sien.

Wouldn’t it be great if we could invent an airspeed indicator and a stall warning horn for software teams? Oh, yeah, we did! It’s called the velocity chart. Good Agile teams operate in front of the power curve, because the velocity chart allows them to see their speed, and keep it in front of the inflection point. When the velocity starts going down, good agile teams increase their refactoring to eliminate the induced drag.

Ne serait-il pas génial si nous pourrions inventer un anémomètre ainsi qu’une alarme de décrochage pour les équipes informatiques ? Ah, oui, c’est vrai, nous l’avons déjà ! Cela s’appelle le diagramme de vélocité. Les bonnes équipes agiles travaillent au premier régime, parce que le diagramme de vélocité leur permet de visualiser leur vitesse, et d’être en mesure de la maintenir au-dessus du point d’inflexion. Lorsque la vélocité commence à descendre, les bonnes équipes agiles accroissent leur _refactoring_  pour éliminer la trainée induite.

Startup culture in the U.S. believes in operating behind the power curve. That’s where they think they want to be. They are so focussed on fast progress, and so convinced that high quality means low speed, that they abandon discipline and principles for the sake of the goal. This is a tragedy.

`La culture startup aux États-Unis est persuadée qu’il est obligatoirement nécessaire de travailler en second régime.`C’est là que les startups pensent vouloir être. Elles sont tellement focalisées sur des progrès rapides, et tellement convaincues qu’avoir de la qualité supérieure est indisociable de lenteur, elles abandonnent donc la rigueur et les principes au prétexte que la fin justifie les moyens. C’est une tragédie.

They start out believing that power and speed are related without paying any attention to drag. So they haul back on the yoke, put their noses into the sky, ram the throttle forward, and then burn fuel madly while going nowhere in a hurry. They don’t understand that when you make a mess, you induce drag, and you cancel out your power.

Elles ont commencé à croire que la puissance et la vitesse sont liées sans prêter attention à la trainée. Elles rétablissent le joug, pointent leurs nez vers le ciel, pousse la manette des gaz à fond, et brûle le carburant de manière irresponsable en allant nulle part à toute précipitation. Elles ne comprennent pas que lorsque vous faites de la m*, cela induit de la trainée, et cela annule votre puissance.


---
Auteur : [Uncle Bob](http://www.8thlight.com/team/uncle-bob)  
Source : [Operating Behind the Power Curve](http://blog.cleancoder.com/uncle-bob/2018/01/15/behindThePowerCurve.html)  
Date de parution originale : 15 Janvier 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : --/02/2018  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



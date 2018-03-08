---
layout: post
title:  "À l’opposé de la courbe de puissance"
date:   2018-03-08 00:00:01
published: true
tags: 
- agile
- équipe
- vélocité
---

En préambule, je vous assure que ce billet parle bien de développement logiciel. Je vous demande donc votre indulgence.

Que se passe t-il si vous poussez la manette des gaz dans un avion ? Vous volez plus vite, n’est-ce-pas ? Davantage de puissance dans le moteur signifie davantage de poussée donc davantage de vitesse.

C’est vrai la plupart du temps ; mais il existe une situation où vous pouvez faire en sorte que cette relation s’inverse. Cela s’appelle : _le second régime_

Vous le savez sans doute, quatre forces gouvernent le vol : la gravité, la portance, la poussée et la trainée. La portance s’oppose à la gravité, et la poussée à la trainée. Dans un aéroplane en vol rectiligne et en palier, l’ensemble de ces forces s’équilibre parfaitement.

La poussée, bien sûr, vient du moteur. La portance vient de l’air circulant autour des ailes, et la trainée … ? Eh bien, la trainée a principalement deux origines.

La trainée dite parasite est tout simplement l'effort de pénétration dans l’air. C’est la résistance de l’air au mouvement de l’avion.  Mais il existe une autre type de trainée appelée trainée induite.

La trainée induite est provoquée par le pilotage. Cela arrive lorsque le pilote relève le nez de l’aéronef. Relever le nez change l’angle des ailes par rapport au vent modifiant ainsi le vecteur de portée, qui est toujours perpendiculaire à la surface des ailes, et pointe légèrement vers l’arrière. Elle s'oppose donc au déplacement vers l'avant de l'avion.

Si vous relevez le nez très légèrement, la trainée induite est limitée et l’augmentation de la poussée provoque donc toujours l’augmentation de la vitesse. À l'inverse si vous relevez franchement le nez de l'avion, la trainée induite peut alors annuler totalement l’effort de poussée. Cela s’appelle être à _l’opposé de la courbe de puissance_. 

![courbe de puissance]({{ site.url }}assets/uncle_bob/region-of-reversed-command-fr.png)

L’illustration[^1] montre un avion en vol rectiligne et en palier. À droite, vous pouvez observer que la vitesse et la puissance ont une relation positive. Davantage de puissance égale davantage de vitesse. Mais à gauche en second régime, il est nécessaire d’avoir de plus en plus de puissance pour aller de plus en plus lentement. 

Autrement dit, le pilote a tellement relevé le nez que le vecteur de poussée est dépassé par le vecteur de portance qui le tire vers l’arrière ; l’avion lutte donc contre l’air à pleine puissance sans avancer le moins du monde

> Voyez-vous où je veux en venir ?

Excepté au moment final de l’atterrissage, les pilotes se gardent bien de mettre leur avion en second régime. C’est un peu dangereux. Plus vous irez lentement, plus vous aurez besoin de puissance. À un tel point, que vous finirez par vous retrouver en descente à pleine puissance avec l’alarme de décrochage vous hurlant aux oreilles. Les pilotes doivent donc rester en premier régime en surveillant la vitesse-air[^2], en la gardant au-dessus du point d’inflexion. 

Donc, quel le rapport avec le développement logiciel ? (dans le cas où vous n’auriez pas deviné.)

De trop nombreuses équipes de développement travaillent tout le temps en second régime. La trainée induite correspond à du code pourri. Elles ont généré tellement de trainée induite que cela demande un effort gigantesque pour arriver à faire la moindre avancée. Elles luttent pour aller de l’avant à pleine puissance, sans faire de progrès vraiment significatifs. En effet, ces équipes ont maximisé leur puissance et se retrouvent dans une lente descente incontrôlable.

Comment fait un pilote pour rester en dehors du second régime ? En baissant le nez. Cela amène le vecteur de portance à la verticale, permettant ainsi au vecteur de poussée de dominer, et l’avion de vrombir dans un magnifique ciel bleu azur.

Comment une équipe informatique se sort-elle du second régime ? En baissant le nez, en nettoyant leur bazar, et en réduisant la trainée induite. Une fois cette trainée disparue, et avec toute la puissance dont elle dispose, le magnifique ciel bleu azur est désormais sien.

Ne serait-il pas génial si nous pouvions inventer un anémomètre ainsi qu’une alarme de décrochage pour les équipes de développement ? Ah, oui, c’est vrai, nous l’avons déjà ! Cela s’appelle le diagramme de vélocité. De bonnes équipes agiles travaillent au premier régime, parce que le diagramme de vélocité leur permet de visualiser leur vitesse, et d’être en mesure de la maintenir au-dessus du point d’inflexion. Lorsque la vélocité commence à baisser, les bonnes équipes agiles augmentent leur _refactoring_  pour éliminer la trainée induite.

Les startups aux États-Unis sont persuadées de devoir travailler en second régime. C’est en second régime qu'elles pensent devoir être. Elles sont tellement focalisées sur l'obtention de progrès rapides, et tellement convaincues que l'atteinte d'une très bonne qualité est indissociable de lenteur, qu'elles abandonnent rigueur et principes au prétexte que la fin justifie les moyens. C’est dramatique.

Elles ont commencé à croire que la puissance et la vitesse sont liées sans prêter attention à la trainée. Elles tirent donc sur le manche, pointent leurs nez vers le ciel, poussent la manette des gaz à fond, et brûlent du carburant aveuglément en toute précipitation sans aller nulle part . Elles ne comprennent pas que lorsque vous faites de la m\****, cela induit de la trainée, et annule la puissance dont vous disposez.

[^1]: https://i2.wp.com/aviationglossary.com/wp-content/uploads/2015/08/region-of-reversed-command.png?ssl=1

[^2]: vitesse-air = vitesse d'un aéronef par rapport à l'air ([article Wikipedia](https://fr.wikipedia.org/wiki/Altitudes_et_vitesses_(a%C3%A9ronautique)#Vitesse_vraie_ou_Vv_ou_TAS))

---
Auteur : [Uncle Bob](http://www.8thlight.com/team/uncle-bob)  
Source : [Operating Behind the Power Curve](http://blog.cleancoder.com/uncle-bob/2018/01/15/behindThePowerCurve.html)  
Date de parution originale : 15 Janvier 2018  

---
Traducteurs : Cyril Morel, [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/).  
Remerciements à Paul Bricknell sur une expression spécifique.  
Date de traduction : 08/03/2018  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



---
layout: post
title:  "Le dernier moment responsable"
date:   2016-06-28 00:00:01
published: true
tags: 
- lean
---
Mary et Tom Poppendieck décrivent dans leur ouvrage [Lean Software Development: An Agile Toolkit](http://www.amazon.com/exec/obidos/ASIN/0321150783/codihorr-20), une technique qui est contre-intuitive pour amener à de meilleures prises de décisions :

> Faire du développement logiciel de manière concurrente signifie à la fois démarrer le développement lorsqu’on a seulement une partie des exigences qui est connue et développer en courtes itérations, cette manière de faire permet d’obtenir du _feedback_ qui permet de faire émerger le système. Le développement concurrent rend possible de **retarder l’engagement jusqu’au dernier moment responsable**, c’est-à-dire, le moment où ne pas prendre de décision permet d’éliminer une option importante. Si les engagements sont retardés au-delà du dernier moment responsable, alors les décisions prises le sont par défaut, ce qui n’est pas généralement une bonne approche pour prendre des décisions.

Paradoxalement, il est donc possible de faire de meilleures prises de décisions en _ne décidant pas_. Je suis un procrastinateur de niveau mondial, alors qu’est-ce qui m’empêche d’interpréter ceci comme étant d’avoir _carte blanche_[^1] ? Pourquoi faire aujourd’hui ce que je peux remettre à demain ?

Prendre des décisions au dernier moment responsable n’est pas de la procrastination ; c’est de la [paresse éclairée](http://www.codinghorror.com/blog/archives/000237.html)[^2]. C’est une stratégie solide et essentielle d’évitement du risque. **Des décisions prises trop tôt dans un projet sont beaucoup trop risquées**. Souvent, des décisions prisent précocement ont pour conséquence de faire faire du travail qui devra être mis ensuite à la poubelle. Cela peut être encore pire, ces décisions prises trop tôt peuvent avoir des conséquences inévitables et handicapantes pour tout le reste du projet.

Au début d’un projet, vous devriez prendre le moins de décisions structurantes possibles que vous aurez à gérer par la suite. Cela ne signifie pas, bien sûr, arrêter de travailler - cela signifie que vous vous adaptez à la nature hautement versatile du développement logiciel. Souvent, votre meilleure décision est d'[avoir les couilles de dire “Je ne sais pas”](http://www.codinghorror.com/blog/archives/000373.html)[^2]. Ce qui sera immédiatement suivie de “… mais nous y travaillons”.

Jeremy Miller a participé à une table ronde sur le TDD[^3] avec Mary Poppendieck et il a [recollé les morceaux](http://codebetter.com/blogs/jeremy.miller/archive/2006/01/18/136648.aspx)[^2] de manière tout à fait logique entre le dernier moment responsable et [YAGNI](http://www.codinghorror.com/blog/archives/000111.html)[^4] :

> **La clé est de prendre des décisions aussi tardivement que  vous pouvez attendre de manière responsable, parce qu’il s’agit du moment où vous avez le plus d’informations sur lesquelles baser votre décision**. En conception logicielle, cela signifie que vous renoncez à créer des solutions générales ou des structures de classes jusqu’au moment où vous savez qu’elles sont justifiées ou nécessaires. Je pense qu’il y a une tendance naturelle chez les humains de construire ou d’acheter des choses par anticipation de futurs besoins, même s’ils sont improbables. N’est-ce pas là la devise des [scouts](http://www.scouting.org/)[^2] - [Être toujours prêt](http://www.scouting.org/factsheets/02-503a.html)[^2] ?

En tant qu’ancien scout moi-même, je pense que nous devrions résister à notre tendance naturelle de trop préparer à l’avance. Mon atelier est rempli d’outils inutilisés dont je pensais avoir besoin. Pourquoi est-ce que j’ai ce compresseur à air ? Quand est-ce que j’ai utilisé mon aspirateur de chantier la dernière fois ? Est ce que j’ai déjà utilisé ce coffret de douilles ? C’est un vrai gaspillage d’argent et d’espace dans mon garage. Sans compter tout le temps que j’ai passé en atermoiement à sélectionner ces outils que je n’utilise pas. Depuis, j’ai adopté l’approche du dernier moment responsable pour mon atelier. Je me force à acheter seulement des outils que j’ai déjà utilisé ou des outils dont j’ai besoin spécifiquement pour un projet qui va bientôt démarrer.

Soyez prêt. Mais pour demain, pas pour l’année prochaine. Décider trop tard est dangereux, mais décider trop tôt dans ce monde du développement logiciel qui change rapidement peut être plus dangereux de manière tout à fait justifié. Laissez donc le principe du dernier moment responsable être votre guide.

[^1]: NdT - en français dans le texte
[^2]: NdT - article en VO non traduit
[^3]: NdT - développement piloté par les tests - plus d’informations dans cet [article](https://fr.wikipedia.org/wiki/Test_driven_development) sur Wikipedia
[^4]: NdT - acronyme de “you ain't gonna need it” traduisible par « vous n'en aurez pas besoin » - l’acronyme YAGNI en VO a donc été conservé car plus répandu (et moins beau/intelligible) que VNAPB - plus d’informations dans cet autre [article](https://fr.wikipedia.org/wiki/YAGNI) sur Wikipedia

---  
Auteur : [Jeff Atwood](https://blog.codinghorror.com/about-me/)  
Source : [The Last Responsible Moment](https://blog.codinghorror.com/the-last-responsible-moment/)  
Date de parution originale : 17 Octobre 2006  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 28/06/2016  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

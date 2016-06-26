---
layout: post
title:  "Le dernier moment responsable"
date:   2016-06-26 00:00:01
published: true
categories: 
- lean
---

The Last Responsible Moment

Le dernier moment responsable

In [Lean Software Development: An Agile Toolkit](http://www.amazon.com/exec/obidos/ASIN/0321150783/codihorr-20), Mary and Tom Poppendieck describe a counter-intuitive technique for making better decisions:

Mary et Tom Poppendieck décrivent dans leur ouvrage [Lean Software Development: An Agile Toolkit](http://www.amazon.com/exec/obidos/ASIN/0321150783/codihorr-20), une technique contre-intuitive pour amener à de meilleures prises de décisions.

> Concurrent software development means starting development when only partial requirements are known and developing in short iterations that provide the feedback that causes the system to emerge. Concurrent development makes it possible to **delay commitment until the last responsible moment**, that is, the moment at which failing to make a decision eliminates an important alternative. If commitments are delayed beyond the last responsible moment, then decisions are made by default, which is generally not a good approach to making decisions.

> Faire du développement logiciel de manière concurrente signifie démarrer le développement lorsque seulement une partie des exigences est connue et développer en courtes itérations, cela permet d’avoir du _feedback_ qui permet ainsi au système d’émerger. Le développement concurrent rend possible de **retarder l’engagement jusqu’au dernier moment responsable**, c’est-à-dire, le moment où ne pas prendre de décision permet d’éliminer une option importante. Si les engagements sont retardés au-delà du dernier moment responsable, alors les décisions prises le sont par défaut, ce qui n’est généralement pas une bonne approche pour prendre des décisions.

Paradoxically, it's possible to make better decisions by _not deciding_. I'm a world class procrastinator, so what's to stop me from reading this as carte blanche? Why do today what I can put off until tomorrow?

Paradoxalement, il est possible de faire de meilleures prises de décisions en _ne décidant pas_. Je suis un procrastinateur de niveau mondial, alors qu’est-ce qui m’empêche d’interpréter ceci comme étant d’avoir _carte blanche_ (en français dans le texte - NdT) ? Pourquoi faire aujourd’hui ce que je peux remettre à demain ?

Making decisions at the Last Responsible Moment isn't procrastination; it's [inspired laziness](http://www.codinghorror.com/blog/archives/000237.html). It's a solid, fundamental risk avoidance strategy. **Decisions made too early in a project are hugely risky**. Early decisions often result in work that has to be thrown away. Even worse, those early decisions can have crippling and unavoidable consequences for the entire future of the project.

Prendre des décisions au dernier moment responsable n’est pas de la procrastination ; c’est de la [paresse éclairée](http://www.codinghorror.com/blog/archives/000237.html). C’est une stratégie solide et de base d’évitement du risque. **Des décisions prises trop tôt dans un projet sont beaucoup trop risquées**. Souvent, des décisions prisent précocement ont comme conséquence de faire du travail qui devra être mis à la poubelle. Cela peut être pire, ces décisions prises trop tôt peuvent avoir des conséquences handicapantes et inévitables pour tout le reste du projet. 

Early in a project, you should make as few binding decisions as you can get away with. This doesn't mean you stop working, of course – you adapt to the highly variable nature of software development. Often, [having the guts to say "I don't know"](http://www.codinghorror.com/blog/archives/000373.html) is your best decision. Immediately followed by "... but we're working on it."

Au début d’un projet, vous devriez prendre le moins possible de décisions structurantes que vous aurez à gérer par la suite. Cela ne signifie pas, bien sûr, arrêter de travailler - cela signifie que vous vous adaptez à la nature hautement versatile du développement logiciel. Souvent, votre meilleure décision est d'[avoir les couilles de dire “Je ne sais pas”](http://www.codinghorror.com/blog/archives/000373.html). Suivie immédiatement par “… mais nous y travaillons”.

Jeremy Miller participated in a TDD panel with Mary Poppendieck last year, and he logically [connects the dots](http://codebetter.com/blogs/jeremy.miller/archive/2006/01/18/136648.aspx) between the Last Responsible Moment and [YAGNI](http://www.codinghorror.com/blog/archives/000111.html):

Jeremy Miller a participé à une table ronde sur le TDD (développement piloté par les tests - NdT) avec Mary Poppendieck et il a [recollé les morceaux](http://codebetter.com/blogs/jeremy.miller/archive/2006/01/18/136648.aspx) de manière tout à fait logique entre le dernier moment responsable et [YAGNI](http://www.codinghorror.com/blog/archives/000111.html) : 

> **The key is to make decisions as late as you can responsibly wait because that is the point at which you have the most information on which to base the decision**. In software design it means you forgo creating generalized solutions or class structures until you know that they're justified or necessary.
I think there's a natural human tendency to build or buy things in anticipation of future needs, however unlikely. Isn't that the [Boy Scout](http://www.scouting.org/) motto – [Be Prepared](http://www.scouting.org/factsheets/02-503a.html)?

> **La clé est de prendre des décisions aussi tardivement que  vous pouvez attendre de manière responsable, parce qu’il s’agit du moment où vous avez le plus d’informations sur lesquelles baser votre décision**. En conception logicielle, cela signifie que pouvez oublier de créer des solutions générales ou des structures de classes jusqu’au moment où vous savez qu’elles sont justifiées ou nécessaires. Je pense qu’il y a une tendance naturelle chez les humains de construire ou d’acheter des choses par anticipation de futurs besoins, même s’ils sont improbables. N’est-ce pas là la devise [scouts](http://www.scouting.org/)- [Être toujours prêt](http://www.scouting.org/factsheets/02-503a.html) ?

![Emblême Boy Scout]()
 
As a former Scout myself, I think we should resist our natural tendency to prepare too far in advance. My workshop is chock full of unused tools I thought I might need. Why do I have this air compressor? When was the last time I used my wet/dry vac? Have I ever used that metric socket set? It's a complete waste of money and garage space. Plus all the time I spent agonizing over the selection of these tools I don't use. I've adopted the Last Responsible Moment approach for my workshop. I force myself to only buy tools that I've used before, or tools that I have a very specific need for on a project I'm about to start.

En tant qu’ancien scout moi-même, je pense que nous devrions résister à notre tendance naturelle de trop préparer à l’avance. Mon atelier est remplit d’outils inutilisés dont je pensais avoir besoin. Pourquoi est-ce que j’ai ce compresseur à air ? Quand est-ce que j’ai utilisé mon `wet/dry vac` la dernière fois ? Est ce que j’ai déjà utilisé cet ensemble de règles de mesures ? C’est un vrai gaspillage d’argent et d’espace de mon garage. Sans compter tout le temps que j’ai passé en atermoiement à sélectionner ces outils que je n’utilise pas. Depuis, j’ai adopté l’approche du dernier moment responsable pour mon atelier. Je me force à acheter seulement des outils que j’ai déjà utilisés ou des outils dont j’ai besoin spécifiquement pour un projet qui va démarrer prochainement.

Be prepared. But for tomorrow, not next year. Deciding too late is dangerous, but deciding too early in the rapidly changing world of software development is arguably even more dangerous. Let the principle of Last Responsible Moment be your guide.

Soyez prêt. Mais pour demain, pas pour l’année prochaine. Décider trop tard est dangereux, mais décider trop tôt dans ce monde du développement logiciel qui change rapidement peut être plus dangereux de manière tout à fait justifié. Laissez donc le principe du dernier moment responsable être votre guide à partir d’aujourd’hui..

---  
Auteur : [Jeff Atwood](http://jpattonassociates.com/about-jeff-patton/)  
Source : [User Story Mapping Presentation](http://jpattonassociates.com/user-story-mapping-presentation/)  
Date de parution originale : 28 Janvier 2008  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 17/10/2006  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}



regarder le lien vers le texte chickens pigs  
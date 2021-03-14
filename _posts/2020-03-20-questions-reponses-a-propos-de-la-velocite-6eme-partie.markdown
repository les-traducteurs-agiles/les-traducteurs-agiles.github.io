---
layout: post
title:  "Questions/Réponses à propos de la vélocité - 6ème partie"
date:   2020-03-26 00:00
published: true
tags:
- vélocité
---

Dans la [5ème partie](http://www.les-traducteurs-agiles.org/2019/07/15/questions-reponses-a-propos-de-la-velocite-5eme-partie.html) de cette série d'articles, nous avons examiné la lien entre travailler davantage et aller vite. J'espère que le message que vous avez retenu a été que nous voulons que les personnes travaillent moins et de manière durable afin qu'elles soient en capacité de livrer davantage, même s'il y a certaines conditions qui doivent être mises en place si nous voulons être plus productif sur une période donnée.

Reprenons donc à partir de là :

> A : Donc comment pouvons-nous livrer des fonctionnalités vraiment plus vite ?  
>
> B : Ah, voici une question intéressante. Combien de temps cela vous prend-il pour livrer une fonctionnalité en ce moment ?  
>
> A : Bien trop longtemps. Nous avons besoin que les développeurs aillent plus vite.  
>
> B : Quel est le % du temps de traversée représentant le temps de cycle des développeurs ?  
>
> A : Pourquoi parlez-vous du temps de traversée ? Je vous parle de développement.  
>
> B : Le temps de traversée représente la mesure (d'avancement - NdT) de la livraison. Le temps de cycle du développement n'est qu'un élément du temps de traversée.
Cette partie de la conversation illustre le manque de curiosité quant aux processus. La personne A a ostensiblement décidé que le goulot d'étranglement c'était le développement et elle n'est pas du tout intéressée de connaître comment le reste du processus pourrait restreindre ou ralentir la livraison.  

Ceci n'est pas inhabituel.

Le problème des longs temps de traversée sera fréquemment imputé au développement ou lorsque des tests sont faits après les développements, à l'assurance qualité (AQ).

Un de mes amis a fait partie d'un grand projet de développement comportant de fortes contraintes de délais en tant que testeur professionnel. Il a été convoqué devant les directeurs de l'entreprise au motif de « mettre en retard de la livraison ». Le directeur du développement informatique (dont l'assurance qualité ne fait pas partie) a reproché au département de l'assurance qualité de « ne pas faire passer les tests assez vite ».

Cela n'a pas été dit bien sûr de manière ironique. Le fait est que le département de l'AQ trouvait un nombre exceptionnel d'anomalies (en partie, sans doute parce que le directeur du développement avait décrété pas de tests, pas de conception, pas de _refactoring_, et pas de tests pendant le développement afin « d'accélérer les choses »). Le département de l'AQ renvoyait donc le code pour être retravaillé ce qui ralentissait les nouveaux développements.

Le problème ? Eh bien, la file d'attente et l'accumulation du travail à faire apparaissait du côté de l'AQ, par conséquent les personnes de l'AQ devaient être forcément fautifs pour ne pas faire bouger les choses plus vite, n'est-ce pas ? Ce n'était certainement pas les développeurs qui, eux, avaient produits scrupuleusement des quantités de code défectueux aussi vite que possible pendant des mois.

Dans une autre entreprise, nous avons vu les équipes de développements se voir reprocher par le marketing des fonctionnalités non réalisées, le marketing attendant qu'il y ait assez d'éléments produits pour faire une grande annonce publicitaire sur la livraison. Tant bien même de la valeur aurait pu être déjà livrée aux clients, l'idée de faire «un grand coup» faisait bien trop partie de la culture de l'organisation. Le développement prenait généralement quelques jours par _story_ -- assez vite en réalité. Mais ces fonctionnalités restaient en attente pendant des mois. En conséquence, certaines personnes dans l'organisation avaient décidé que c'était les équipes de développement qui «prenaient des mois pour écrire du code». Dans ce cas précis, un des architectes a refusé, par exemple, de prendre en compte les statistiques, les chiffres et les indicateurs. « Je ne suis pas d'accord »  a dit l'architecte à qui avait été présenté ces statistiques, « les développeurs doivent aller plus vite.»

Pourquoi cela ? Parce que le développement et l'AQ sont au plus près de la réalité, comme la roue qui colle à l'asphalte. Dans la [3ème partie](http://www.les-traducteurs-agiles.org/2019/04/08/questions-reponses-a-propos-de-la-velocite-3eme-partie.html) de cette série d'articles, nous avons dit :
> « _La durée que cela prend de faire les choses … c'est ça la réalité.
Les estimations sont des constructions de toutes pièces._ »  

Lorsque des plans (qui semblent) parfaitement corrects ne sont pas en phase avec la réalité, la plupart d'entre nous ont tendance à répondre à la déception par le reproche. Les personnes se trouvant entre la réalité du travail à accomplir et les attendus deviennent les plus faciles à blâmer.

Là où nous devrions voir un espace de curiosité[^1], nous avons tendance à voir un « problème ».

![espace de curiosité]({{ site.url }}assets/tim_ottinger/Screenshot-2018-10-29-17.35.20-fr.png)

Si nous voyons la différence comme un problème, plutôt que comme un espace de curiosité, nous avons tendance à considérer les personnes qui se trouvent **au** niveau du goulot d'étranglement comme **étant** le goulot d'étranglement. C'est une erreur qui devrait être évidente pour les personnes qui sont au minimum au fait de l'approche systémique, mais la plupart des personnes sous pression sont plutôt sujettes à une réaction émotionnelle qu'à une approche systémique rigoureuse.

Ne faisons pas de reproche aux gens pour ne pas voir ce qui nous paraît évident. Mettre au piloris les gens pour leur ignorance n'est guère utile. Ce ne serait que reproches après reproches. Comment cela peut-il être utile ?

Au lieu de ça, si nous pouvons réfréner notre impulsion, nous pouvons approcher le problème avec le cœur plus léger, et chercher des solutions plutôt que renforcer la suspicion et les reproches. La curiosité (et nos sens) pourrait donner un bien meilleur résultat dans ce cas-là.

> A: _Je n'ai pas envie de m'occuper du temps de traversée_. Pouvons-nous juste nous focaliser juste sur le temps de cycle du développement ?  
>
> B: Bien sûr, mais vous pourriez du coup ne pas travailler sur le goulot d'étranglement, ça va être du gaspillage.  
>
> A: Je veux seulement parler des développeurs.  
>
> B: OK. Tant que vous savez que cela ne sert rien.  

Et voici la vérité au cœur de cet article faisant écho à la théorie des contraintes :

> Si vous ne travaillez pas sur le goulot d'étranglement,  
> nos efforts pour améliorer le flux seront sans effets.  

Cela signifie qu'il est possible d'aller au-delà de nos hypothèses irréfragables. Avec toute une série de phrases comme « c'est les devs », « c'est l'AQ », « vous ne travaillez pas assez », « vous prenez pas les choses au sérieux » -- qui [supposent toutes, que les problèmes sont liés à la motivation](https://agileotter.blogspot.com/2015/09/confirmation-bias-and-twelve-day.html) plutôt qu'à des éléments techniques.

Si une personne fait face à un tel mur de briques, qu'est-ce qu'elle peut faire ? Eh bien c'est ce que nous verrons dans la [7ème partie de cette série d'articles.](http://www.les-traducteurs-agiles.org/2020/04/15/questions-reponses-a-propos-de-la-velocite-7eme-partie.html)

[^1]: NdT - Pour en savoir plus sur l'espace de curiosité, c'est par [ici](http://www.les-traducteurs-agiles.org/2016/10/16/espace-de-curiosite.html)

---
Auteur : Tim Ottinger  
Source : [Q and A on Velocity, Part VI ](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-vi.html)  
Date de parution originale : 29 Octobre 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 26/03/2020  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

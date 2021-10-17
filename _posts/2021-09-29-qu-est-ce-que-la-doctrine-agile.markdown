---
layout: post
title:  "Qu'est-ce que la doctrine Agile ?"
date:   2021-10-17 00:01
published: true
tags:
- agile
---

## De l'insuffisance de la stratégie et des plans

Mark Bonchek et Chris Fussel expliquent dans leur article éponyme [pourquoi la stratégie et les plans s'avèrent insuffisants (vo)](http://blogs.hbr.org/cs/2013/02/use_doctrine_to_pierce_the_f.html) :

> « Une stratégie ne donne pas suffisamment d'éléments aux employés d'une entreprise pour les guider quant à la manière de passer à l'action, et les plans s'avèrent trop rigides pour s'adapter à des changements de situation. Dans des environnements en constante évolution, vous avez besoin de balises anti-brouillard pour savoir si vous vous rapprochez du sol. »

… où les « balises anti-brouillard » représentent la doctrine.

> « Une doctrine permet de créer un cadre de référence commun à l'intérieur duquel les individus peuvent prendre des décisions rapides justifiées compte tenu des circonstances dans lesquelles elles sont prises … Si la stratégie permet de définir les objectifs et que les plans préconisent les comportements, alors la doctrine permet de guider les décisions. »

Autrement dit, **la doctrine nous permet de décentraliser, en toute sécurité, la prise de décision par la mise en place d'une logique de décision cohérente**.

[L'OTAN définit la doctrine](https://en.wikipedia.org/wiki/Military_doctrine#Defining_doctrine)[^1] de la manière suivante …

> _**Principes fondamentaux guidant** les forces militaires **dans leurs actions en appui des objectifs**. Bien qu'autorisés, **ces principes demandent à faire preuve de discernement dans leur mise en application**_  

… je m'interroge …

## Quelle pourrait être la doctrine Agile ?

Quels sont les principes fondamentaux qui devraient guider les actions des praticiens Agile en appui de leurs objectifs, qui seraient autorisées mais qui demanderaient de faire preuve de discernement dans leur mise en application ?

### S'agit-il uniquement du Manifeste Agile ?

Le candidat naturel pour une doctrine Agile est le [Manifeste Agile](http://agilemanifesto.org/iso/fr/manifesto.html).   

J'ai quelques problèmes avec cette proposition pour les raisons suivantes :

- **Ce n'était pas vraiment l'intention du Manifeste Agile d'être une doctrine** en dépit du fait que de nombreux nouveaux agilistes le considèrent comme tel.
- **Le Manifeste Agile est le résultat d'un compromis**, c'est-à-dire que l'ensemble des valeurs et des principes du Manifeste est le résultat du plus petit dénominateur commun sur lequel un groupe de personnes s'est mis d'accord.
- **Le Manifeste Agile n'a pas été mis à jour depuis 2001** (c'est-à-dire il y a 12 ans au moment où je rédige ces lignes). Pour citer John Boyd : « Ne considérez pas le Manifeste Agile comme étant une doctrine parce que beaucoup de choses affreuses se sont produites ces 12 dernières années. ».
- **12 principes cela fait beaucoup à retenir dans notre mémoire de travail …** et je préférerais une doctrine que les gens pourraient se rappeler sans avoir à la lire et à la relire … tout du moins dans sa version de base.

### Qu'en est-il d'Extreme Programming ?

J'ai tendance à préferer plutôt une méthode Agile concrète. En raison de mon histoire personnelle, j'aurais tendance à préférer [Extreme Programming](http://jchyip.blogspot.com.au/2011/05/listen-test-code-refactor-learn-target.html) :

> « Le logiciel est quelque chose de bien trop difficile pour passer du temps sur des choses qui ne valent pas le coup. Donc, si nous recommencions tout depuis le début, quelles sont les choses qui comptent absolument à nos yeux ? … **Écouter, Tester, Coder, Réusiner**. C'est tout ce qui compte pour (faire) du logiciel. Toute personne qui vous dit quelque chose de différent est en train de vous vendre quelque chose. »
>
> Kent Beck

Écouter, Tester, Coder, Réusiner - ces 4 verbes semblent bien trop orientés développement logiciel pour s'apprêter à une doctrine Agile généraliste, poussons donc un peu plus loin …

## Une proposition de doctrine Agile

### 1. Réduire la distance entre les problèmes et les solutionneurs de problèmes

J'ai entendu pour la première fois cette phrase de la part de [John Sullivan](http://www.linkedin.com/profile/view?id=8685792), mais il l'évoquait dans le contexte de réduire la distance entre les clients et les développeurs.

Je fais ici référence à deux types de distance :

1. **La distance physique**
2. **La distance conceptuel**, c'est-à-dire, de quelle manière le problème est-il conceptuellement accessible aux personnes qui vont résoudre le problème. Cela nous mène à des choses comme rendre les problèmes visibles, avoir de meilleures techniques pour modéliser le problème, etc.

### 2. Valider chaque étape

- Quel est le résultat souhaité ?
- Pourquoi passez-vous par cette étape ? Est-ce que cela vous rapproche du résultat souhaité ?
- Comment saurez-vous que cette étape a été faite et franchie avec succès ?

En d'autres termes, en utilisant les termes mêmes de tout professionnel Agile un temps soit peu efficace :

> **Est-ce que vous avez un test pour ça** ?

### 3. Faire de plus petites étapes

> « … parmi toutes les améliorations les plus importantes de ces dernières années en terme de développement produit, certaines comme l'ingénierie concurrente, le prototypage rapide et les méthodes agiles ont comme caractéristique que de participer à **la réduction de la taille des lots**. »
>
> Extrait du livre [The Principles of Product Development Flow](http://www.amazon.com/gp/product/B007TKU0O0/ref=as_li_ss_tl?ie=UTF8&camp=1789&creative=390957&creativeASIN=B007TKU0O0&linkCode=as2&tag=youdthinwitha-20) de Don Reinertsen

Il en découle alors des lots de travaux plus petits, des livraisons plus petites, etc.

Et parce qu'éviter les coûts de transaction est généralement la raison principale expliquant l'existence d'étapes plus longues, réduire ces mêmes coûts de transaction en fait également partie.

### 4. S'améliorer au fur et à mesure

> « Quittez ce monde en le laissant un peu meilleur qu'il ne l'était quand vous l'avez trouvé. »
>
> Robert Baden-Powell   

« S'améliorer au fur et à mesure que l'on avance » c'est être conscient et être en capacité de gérer la [dette technique (vo)](http://martinfowler.com/bliki/TechnicalDebt.html) et d'essayer de laisser les choses dans un état un peu meilleur que dans celui dans lequel vous les avez trouvées afin de traiter de manière incrémentale l'entropie. Tout système technique laissé sans maintenance se dégrade avec le temps, il en est de même pour les systèmes humains

## Alors ?

Est-ce que cette doctrine est un concept utile ?

Est-ce qu'il s'agit de la bonne doctrine ?

Comparé à d'autres principes existants, est-ce que cette doctrine sera plus facile à établir, plus facile à maintenir, et plus efficace à venir appuyer des prises de décision appropriées et qui fasse clairement référence à Agile ?

[^1]: NdT - la définition de la doctrine donnée dans la [version française de la page Wikipedia](https://fr.wikipedia.org/wiki/Doctrine_militaire) n'est pas celle citée dans l'article d'origine. Le lien vers la page anglaise a donc été conservé pour la présente traduction.

---
Auteur : [Jason Yip](https://jchyip.medium.com/about)  
Source : [What is Agile doctrine?](http://jchyip.blogspot.com/2013/03/what-is-agile-doctrine.html)  
Date de parution originale : 03 Mars 2013  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 17/10/2021  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

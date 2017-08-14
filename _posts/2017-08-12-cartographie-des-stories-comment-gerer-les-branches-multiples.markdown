---
layout: post
title:  "Comment gérer les branches des cartographies des user stories"
date:   2017-08-14 00:00:01
published: true
tags: 
- user stories
---

## This question recently came from Douglas Ferguson (but I get asked a lot)

## Voici une question reçue récemment de Douglas Ferguson (mais qui m’est posée souvent)

[In User Story Mapping], how do you typically handling multi-user processes that create branches?
Do you create different maps for different users and different flows?

Dans une cartographie de user stories, comment gérez-vous les processus multi-utilisateurs pouvant engendrer plusieurs branches ?
Créez-vous différentes cartographies pour les différents utilisateurs et les différents flux ?

## My response:

## Ma réponse :

I get asked this often, and do my best to avoid answering the question because I want to see what people come up with.

C’est une question que l’on me pose souvent, et je fais de mon mieux pour éviter de répondre à cette question car je veux voir ce à quoi les gens vont arriver par eux-mêmes.

The only rules for me about mapping are that:

Pour moi, les seules règles valables pour faire la cartographie sont :

1. I can tell a story – and I usually tell it left to right
2. I can break the story down into options and details – and I usually do that top to bottom

1. Je suis en mesure de raconter une histoire - et je la raconte habituellement de gauche à droite
2. Je peux décomposer une histoire en alternatives ou en détails - et je le fais habituellement de haut en bas

That’s it. No more rules. And you can even break those if you have a good reason.

Voila, c’est tout. Pas d’autres règles. Et vous pouvez même violer ces règles si vous avez une bonne raison.

If we were writing a book here, the characters have options, but it’s a book, so they only do one thing. But, if we’re telling a story about an interactive product, people use the product differently at different times, they may do things in different orders, and they may make a decision that changes all the “steps” they’d do after that decisions. They won’t behave like characters in a book. That makes it messy. And, because people can do things in a variety of different ways, it makes any modeling process painful. So I avoid a lot of that pain by reminding myself that:

Si nous étions en train d’écrire un livre ici, les personnages auraient la possibilité de faire différentes choses options, mais comme c’est dans un livre, ils font une seule chose. Mais, si nous étions en train de raconter une histoire à propos d’un produit interactif, les gens pourraient utiliser le produit différemment à différents moments de la journée, ils pourraient faire les choses dans un ordre différent, et ils pourraient prendre une décision changeant toutes les “étapes” qu’ils pourraient faire après cette décision. Ils ne se comportent pas comme les personages d’un livre. Ça fait un peu foutoir. Et, parce que les personnes peuvent les choses dans une variété de différentes manières, cela rends la modélisation du processus pénible. Donc je m’évite pas mal de peine en me remémorant la chose suivante :

> A story map is not a precise model of user’s workflow. It’s a tool that helps us work together to tell users’ stories.

> Une cartographie n’est pas un modèle précis de flux de travail d’un utilisateur. C’est un outil qui nous aide à travailler ensemble à raconter les stories des utilisateurs

## Flatten the flow

## Aplatir le flot

So when someone says to me: “In this process the user does steps A and B, but in step C they make a decision. Then they might branch to steps D, E, and F, or they might take the other branch and do steps G, H, and I. How do I map that?”

Aussi lorsque quelqu’un me demande : “Dans ce processus, l’utilisateur fait les étapes A et B, mais à l’étape C, il prend une décision. Il pourrait prendre ensuite la branche vers les étapes D, E et F, ou il pourrait prendre l’autre branche et faire les étapes G, H, et I. Comment est-ce que je cartographie cela ?”

In a flowchart it would look like this:

Dans un logigramme, cela pourrait ressembler à cela :

![flowchart](http://jpattonassociates.com/wp-content/uploads/2015/07/flowchart-1024x435.jpg)

![logigramme]({{ site.url }}assets/jeff_patton/logigramme.jpg)

I usually tell them I’d put all those options in a left to right flow: A, B, C, D, E, F, G, H, and then I. It would look like this as a map:

Je leur réponds que généralement je mets toutes les alternatives dans un flux de gauche à droite :  A, B, C, D, E, F, G, H, et puis I. Sur une cartographie, cela ressemblerait à ceci :

![flattened branches](http://jpattonassociates.com/wp-content/uploads/2015/07/flattened-branches.jpg)

![branches aplaties]({{ site.url }}assets/jeff_patton/branches-aplaties.jpg)

Basically I put the options in the order someone tells the story. I use the telling of the story to add in the extra language like “users would make a decision in step C and they’d they continue at D, or jump over here to G. I don’t show the branches in a map the way I would in a flow chart. I use conversation to communicate the branches.

De manière générale, je mets les alternatives dans l’ordre dans lequel l’histoire a pu m’être raconté. J’utilise le récit de l’histoire pour ajouter les éléments de langage supplémentaire comme “les utilisateurs pourraient prendre une décision lorsqu’ils arrivent à l’étape C et ils pourraient vouloir continuer en D, ou sauter ici en G. Dans une cartographie, je ne montre pas les branches comme je le ferais dans un logigramme. J’utilise la conversation pour communiquer les branches.

## Roll it up

## Enroulemnt

As I see that very long story mapped out the way I just drew it, it looks long to me. I might roll it up into 3 basic columns: the first stuff I do that leads to making a decision, the stuff I do in the first branch, and the stuff I’d do in the second branch. That map might look like this:

Voyant cette très longue histoire se dessiner, avec la manière dont je venais de l’esquisser, elle m’a paru tout d’un coup très longue. Je pourrais l’enrouler en 3 colonnes : le travail que je fais d’abord et qui conduit à prendre une décision, le travail que fais dans la première branche, et le travail que je ferais dans la seconde branche. La cartographie pourrait ressembler à cela :

![branches rolled up](http://jpattonassociates.com/wp-content/uploads/2015/07/branches-rolled-up.png)

![branches enroulées]({{ site.url }}assets/jeff_patton/branches-enroulees.jpg)

**If you’re trying to hand off a story map without conversation** to explain what’s going on inside it, then none of this works. And that’s when I remind you that Agile stories get their name from the action of story telling, not act of story documenting. If you really can’t use conversation to explain things, then you’ll need a workflow diagram, flow chart, use case, or some other model to do it.

**Si vous essayez de transmettre une cartographie dans avoir une conversation** pour expliquer comment cela se passe dedans, alors rien de cela marchera. Et c’est là que je dois vous rappeler que les _stories_ agiles tirent leur nom de l’action de raconter une histoire, et non l’acte de documenter une histoire. Si vous ne pouvez vraiment pas utiliser la conversation pour expliquer les choses, alors vous aurez besoin d’un diagramme de flux de travail, d’un logigramme, d’un cas d’utilisation, ou d’une autre modélisation pour pouvoir le faire.

**If you think you might forget details about the branching**, then It’s a good idea to annotate the stories or around the stories in the map. Write just enough to help you remember how to tell the story.

**Si vous pensez que vous pourriez oublier des informations détaillées au sujet des différentes branches**, alors c’est une bonne idée d’annoter les _stories_ ou à côté des _stories_. Écrivez juste assez pour vous aider à vous souvenir de la manière dont il faudra raconter l’histoire.

## Flatten the flow across users

## Aplatir le flux de plusieurs utilisateurs

In a back and forth with Doug, he got back to me with this:

En échangeant avec Doug, il revint vers moi

>“Image this flow
> 
>merchant enters new product to catalog – user navigates catalog – user opens product detail – user presses order – production receives order – shipping ships product – user receives tracking info 
>
> Here the flow has multiple actors. My flows are a bit more complex and specific to my use case and can create branching, but from your FAQ it seems that I could just flatten it all out without much worry.”

>”Imaginer ce flux
> 
> un marchand ajoute un nouveau produit à son catalogue — l’utilisateur parcoure le catalogue — l’utilisateur consulter les informations détaillées sur le produit — l’utilisateur passe commande — le service production reçoit la commande — le service livraison expédie le produit — l’utilisateur reçoit des informations de suivi de livraison
>
> Voilà donc le flux avec les différents acteurs. Mes flux sont un petit peu plus complexe et spécifique à mon cas d’utilisation et qui peut avoir des branches, mais d’après ton FAQ il paraît que je pourrais l’aplatir sans trop de difficulté.


Yup, you’ve got it. And you can see the map is embedded in the way you told the story.

Eh oui, Doug, tu as tout compris; Et tu pourras voir que la carte a été dessinée selon ton récit 

> Map the product flow across types of users

> Cartographier le flux du produit selon les différents types d’utilisateur

If you do that given the example above, you might end up with something like this:

Si vous faites cela en suivant l’exemple précédent, vous pourriez arriver à quelque chose qui pourrait ressembler à ceci :

![whole product map](http://jpattonassociates.com/wp-content/uploads/2015/07/whole-product-map.jpg)

![cartographie de l’ensemble du processus produit]({{ site.url }}assets/jeff_patton/carto-processus-produit.jpg)

I haven’t written in the details on the cards, but you get the idea I think. It’s now a map that tells lots of user’s stories inside the whole product.

Je n’ai pas écrit le détails sur les cartes, mais vous avez l’idée générale. C’est maintenant une cartographie qui en raconte beaucoup sur les _stories_ utilisateurs au sein de l’ensemble du processus produit.

## Don’t map everything if you don’t have to

## Ne cartographiez pas tout si vous n’avez pas à le faire

I’ve got to tell you I don’t build whole product maps like this unless I’m rebuilding a whole product. I usually work with companies that have a product on the market, and they’d like to introduce new features or capabilities into that product. One mistake they sometimes make is thinking they need to map the whole thing.

Je dois vous dire  que je ne construis pas toutes les cartographies produit ainsi sauf si je suis amené à reconstruire complètement un processus produit. Je travaille généralement avec des entreprises qui ont déjà un produit sur le marché, et qui aiment ajouter des nouvelles fonctionnalités ou de nouveaux éléments à leur produit. Quelques fois, elles font l’erreur d’imaginer qu’elles doivent cartographier l’ensemble de leur processus produit. 

Don’t do that. It takes a lot of time. And the only reason to do it is to help others understand your whole product if they don’t already.

Ne faites pas cela. Cela prend beaucoup de temps. Et la seule raison pour le faire c’est d’aider les autres à comprendre votre processus produit s’ils ne le comprennent pas encore.

>“Instead, just map the change.”

> “À la place, cartographiez juste ce qui change.

For example if I want to add a capability that lets a merchant add a special sale price to their product, I’d map the merchant’s part of the experience where they put the product on sale, and the shopper’s part of the experience where they see the product is on sale.

Par exemple, si je veux ajouter la possibilité à un marchand d’ajouter un prix de vente spécial pour son produit, je cartographierais la partie de l’expérience du marchand où il met le produit en vente, et la partie de l’expérience du client où il voit le produit en vente.

That small map might look like this:

Ce fragment de carte pourrait ressembler à ceci :

![map a capability](http://jpattonassociates.com/wp-content/uploads/2015/07/map-a-capability.jpg)

![Cartographier une possibilité]({{ site.url }}assets/jeff_patton/carto-une-possibilite.jpg)

## Do what makes sense to you

## Faites ce qui a du sens pour vous

I strongly suspect that if I’d given you no advice at all, you’d have figured this out on your own. So, if this saves you a little time, that’s cool.

Je suspecte fortement que si je ne vous avais pas donné de conseil du tout, vous auriez trouver de votre côté. Donc si cela vous a permis de gagner un peu de temps, c’est cool.

And, even better, if you figure out something different that helped you in your situation, please share it back!

Et mieux encore, si vous êtes arrivés à quelque chose de différent qui vous aide dans situation, alors je vous en prie de bien vouloir le partagez avec nous.

---  
Auteur : [Jeff Patton](http://jpattonassociates.com/about-jeff-patton/)  
Source : [How do I handle branches in Story Maps?](http://jpattonassociates.com/qa_branches_in_maps/)  
Date de parution originale : 13 Juillet 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 15/08/2017  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}


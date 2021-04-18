---
layout: post
title:  "Séquencement en 3X"
date:   2021-04-18 10:03
published: false
tags:
- tag1
- tag2
---

Sequencing in 3X

Part of [Comparing Explore, Expand, and Extract](https://www.facebook.com/notes/kent-beck/comparing-explore-expand-and-extract-topics-in-3x/1241983035834558).

Death, taxes, and sequencing. You are going to do something now and everything else later (even if the something you do now is nothing). How do you decide what to do now and what to defer?

Estimates of costs and benefits are one factor influencing sequencing. As described in [Estimates in 3X](https://www.facebook.com/notes/kent-beck/estimates-in-3x/1242012852498243), though, estimates vary in how useful they are in the different phases. In the absence of estimates, how do you choose?

## Explore

The bad news is that during exploration we don’t have the information we need to make optimal sequencing decisions. The good news is that sequencing doesn’t matter. Success is going to be a surprise. We’re going to roll the dice until we get double sixes. One dice roll is much like another.

We do have a balance question during exploration: what proportion of effort should go into experimenting and what proportion into making experimenting cheaper. This turns into a sequencing question–shall I experiment next or optimize experimenting?

A reasonable heuristic for balancing and sequencing is to optimize some aspect of experimenting when it has become tedious. I call this Frustration-Driven Development.

## Expand

The bad news about sequencing in expansion is that if you mess it up, you’ll fail. The margin for error is tight. You are trying to clear bottlenecks just before they ruin your product.

The good news is that sequencing decisions are mostly out of your hands. You’re trying to bend the supply curve of your rate-limiting resource up and bend the demand curve down so that they no longer cross in the foreseeable future. Once you’ve done that you are faced with the next bottleneck. And once there are no bottlenecks looming, you into extraction where you _can_ finally make informed sequencing decisions.

![](https://scontent-cdg2-1.xx.fbcdn.net/v/t31.18172-8/14086457_10154497380318675_7907348228576767704_o.jpg?_nc_cat=107&ccb=1-3&_nc_sid=abc084&_nc_ohc=y1U4CYH12lEAX81HP5A&_nc_ht=scontent-cdg2-1.xx&oh=9f2292bd7a99bee41379b3be4dc4ec2b&oe=60A1E9F5)

_Expansion: one damn bottleneck after another_

## Extract

In extraction you have reliable estimates of costs and benefits. Sort the tasks to be done by ROI, add a little randomness to avoid local minima, and pick whatever is next.

One heuristic is to keep the tasks small. In extraction, you have a lot to lose, so avoid making big changes. Small tasks are easier to estimate, and it’s easier to spot one that is going bad.

## Conclusion

The sequencing mistake is to obsess over sequencing decisions that don’t matter or can’t be made on the basis of data. All that energy would be better spent experimenting or improving experimenting.


---
Auteur : [Prénom_Nom](url_bio)  nbsp
Source : [Titre_article_en_vo](url_article_en_vo)  nbsp
Date de parution originale : jj_MMMM_yyyy  nbsp

---
Traducteur : [Prénom_Nom](url_bio)  nbsp
Date de traduction : jj/mm/yyyy  nbsp

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

---
layout: post
title:  "Les estimations en 3X"
date:   2021-04-18 10:01
published: false
tags:
- tag1
- tag2
---

Estimates in 3X

Part of [Comparing Explore, Expand, and Extract](https://www.facebook.com/notes/kent-beck/comparing-explore-expand-and-extract-topics-in-3x/1241983035834558).

If you had infinite resources, you’d just do everything. Infinite resources erase opportunity cost. In our universe, though, resources are always finite. Everything we do implies the loss of everything we didn’t do instead.

We can’t make these decisions perfectly, witness all the death-bed regrets. However, we can sometimes do better than a dartboard at deciding what to do and what not to do. That’s where estimates come in.

An estimate is a measure of some limited resource expected to be consumed in pursuing one course of action. We might expect to spend two months marketing a book, or ten thousand dollars, or two peoples’ time for a month. Whether the limited resource is time, money, or people, we would like to know beforehand how much of the resource will be consumed so we can wisely choose our course of action.

Estimates measure benefits as well as costs. Estimated benefits help decide between alternatives. Estimates of benefits are as subject to variability as estimates of costs, though, and are subject to path dependence (A or B might not be valuable but A & B are awesome).

Estimates behave differently in explore, expand, and extract. These sometimes-contradictory differences partly explain why estimating software development is so hard sometimes.

## Explore

Estimates of benefits are right out the window. The essence of exploring is that you don’t know where success will appear. You have some intuition or you wouldn’t be trying an idea, but some of the most valuable ideas are those attempted out of sheer cussedness.

Estimates of exploration costs are more of a challenge than a prediction. “I think I can answer this question for X dollars/hours/people.” “How about X/4?” This economy of scope is the game that makes exploring romantic. Instead of estimates, use timeboxes. “Once we’ve used X dollars/hours/people, we’re going to treat the question as answered and move on.”

You _can_ estimate in the large in exploration. Think of a startup selling equity for a round of funding. The amount of money may be based on some mythical “valuation”, but it’s really an estimate of how much exploration will cost times the probability of success times the value of success. You’d hate to run out of money/time/people just before succeeding, but you’d also hate to keep spending after failure is inevitable.

## Expand

In the expand phase you are seeing consistent growth. This makes it possible to estimate when you are going to run out of a resource, be it money, computers, or people. You can generally only see one bottleneck ahead. Whatever you’ve done to mitigate that bottleneck changes the location and form of the next bottleneck.

“According to these projections, on May 12 we will run out of disk space.” “Okay, do this and this and this to get more disks and that and that and that to use fewer disks.”

Estimates warn of trouble in expansion. If you see curves interest that you really don’t want to cross, you try to change things, and the curves remain stubbornly crossed, then it’s time to invoke plan B.

Estimates of cost during expansion are not usually important. You have a winner, provided you can ride the rocket all the way up. Burning a little money now to make sure you make it to orbit makes sense. (Burning so much money that the rocket crashes, not so good.) Keep an eye on the total available, but don’t worry about individual actions.

## Extract

Estimates become valuable in extraction. You have enough experience with costs and benefits to be accurate. Sequencing tasks correctly creates value. You want to realize the highest return on investment first.

The usual rules apply:

- Practice and reflect so you learn.
- Estimate small-ish things, so surprises remain small-ish.
- Notice when estimates suddenly go wonky. You may have re-entered exploration.

## Conclusion

“Estimate Sometimes” lacks the sensible ring of “plan the work, work the plan” and fails as a rallying cry beside “No Estimates!”. However, that’s the whole point of 3X. Each phase requires its own approach. Estimates are just one example.


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

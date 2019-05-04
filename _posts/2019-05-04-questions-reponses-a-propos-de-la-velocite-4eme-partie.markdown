---
layout: post
title:  "Questions/Réponses à propos de la vélocité 4ème partie"
date:   2019-05-04 00:01
published: true
tags:
- vélocité
---

In our [last installment, part III](https://agileotter.blogspot.com/2018/07/q-and-on-velocity-part-iii.html), we talked about the reality of reality and contrasted that to the made-up-ness of schedules and estimates and promises.  

Today we take a deeper look into one element of that dichotomy:  

> A: The schedule is a best-guess, but there is a real promise behind it.  
> B: How does that affect the rate at which things can be done?  
> A: Can I put more people on it?  
> B: Maybe, but cf Brook's Law  

There is a reality to the made-up-ness of schedules, too. In this exchange, person A is reminding person B of the fact.  

Promises are real. Trust is real. Keeping promises creates, sustains, and promotes trust. Real life organizations run on trust.  Plenty of business leaders (and one agile aquatic mammal) have spoken and written on this at length. One of my favorite authors on the subject is Stephen M. R. Covey (AKA "Covey the Lesser") with his book titled [The Speed Of Trust](https://www.amazon.com/SPEED-TRUST-Thing-Changes-Everything/dp/1416549005). Also, see economist[ Ronald Coase's](https://en.wikipedia.org/wiki/Ronald_Coase) work, where he explains the lower transactional costs of trust.  

And yet, for all of this, reality doesn't do what we want it to do. Things still also take as long as they take.  

Rock, meet hard place.  

If we were installing drywall or carpet, then the work would be partly skill and mostly effort. We could get more drywallers or more carpet-layers and we could do more rooms at the same time.  We might even be able to do one room at a time faster, provided on how well they coordinate.  

But no. This is different. Programming is a chain of logic that is fed by and feeds into many other chains of logic. The parts are not as independent as we think, and not understanding the larger context (and the flaws in the parts in the larger context) will lead to many defects.  

I once switched a bit of code from a bad way of doing work (building JSON strings by concatenation) to a more proper use of a JSON library, and took a system down for a little while. Sometimes the system depends on the work having been done the way it was -- the wrong way -- in order to function. Things stick together in a weird way.  

Bringing in developers who don't know the way that the code works doesn't help. Mob programming or pair programming with people who know more about the different parts of the code certainly does help. Adding knowledgeable people to the effort does lead to a better result, but doesn't necessarily make the work go faster.  

[Brooks' Law](https://en.wikipedia.org/wiki/Brooks%27s_law) is the observation that adding people to a late project makes it later. This has been studied and documented at length, and anyone wanting to try to accelerate a project by adding people should beware. It's not impossible to add people to a project, but often a flood of new workers who don't know the system will make it FAR worse.  

These are inconvenient truths, which press us to look into more promising alternatives if we want to see work delivered to an all-to-real schedule.  

Follow us to [Part V](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-v.html)


---
Auteur : Tim Ottinger  
Source : [Q and A on Velocity, Part IV](https://agileotter.blogspot.com/2018/10/q-and-on-velocity-part-iv.html)  nbsp
Date de parution originale : 15 Octobre 2018  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : jj/mm/yyyy  nbsp

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

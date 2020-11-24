---
layout: post
title:  "Du coefficient de charge à la vélocité aux points de story au décomptage de story au temps de traversée au …"
date:   2020-11-24 08:42
published: false
tags:
- vélocité
---

> The problem is that we’re over-optimistic



The problem is that when we estimate how long it will take us to build something, we tend to be over-optimistic. We tend not to take into account all the interruptions and overheads of the typical work day nor the inevitable complications that show up on any “straightforward” task.



I don’t remember anyone ever referencing this in the early days of Extreme Programming, but this is essentially the optimism bias that leads to the [planning fallacy](https://en.wikipedia.org/wiki/Planning_fallacy), proposed by Daniel Kahneman and Amos Tversky in 1979.



## This led to the idea of [Load Factor](http://c2.com/cgi/wiki?LoadFactor)



We estimated each task in Perfect Engineering Days or Ideal Days(no interruptions, perfect flow) and then we multiplied by a Load Factor (originally 2.5, eventually most teams started with 3) to determine a more likely duration in real days. In essence, we assumed that everything would take around 3x longer than we thought.



Over multiple iterations, we could refine Load Factor to better reflect the actual data from the team. In the teams I was on, it usually ended up being 2.something.



The problem was over-optimism. The solution was Load Factor. It roughly worked.



## Yesterday’s Weather is simpler than Load Factor



But wait. What if you could make this simpler? Instead of multiplying by Load Factor, just observe how many Ideal Days you did every iteration (aka observe the [Project Velocity](http://c2.com/cgi/wiki?ProjectVelocity)). Each iteration, you simply committed to what you completed in the last iteration. This was known as [Yesterday’s Weather](http://c2.com/cgi/wiki?YesterdaysWeather).



Velocity is the inverse of Load Factor and is simpler to understand. The practice of using Yesterday’s Weather to shape commitment theoretically gave the team a breather after tough iterations. In my experience, Yesterday’s Weather tended to be more of a guide than a rule.



The problem was still over-optimism. The simpler solution was Velocity and Yesterday’s Weather. It roughly worked.



## I’d rather not get into why real days aren’t the same as ideal days…



Even back when people were using Load Factor, there would always be managers who would be challenging why the Ideal Days were not equivalent to Real Days. To attempt to sidestep this discussion, many teams chose to adopt arbitrary size units (_e.g._, [Gummi Bears](http://c2.com/cgi/wiki?GummiBearsOfComplexity), [Nebulous Units of Time](http://c2.com/cgi/wiki?NebulousUnitOfTime), etc.). Eventually, most teams stabilised around the term [Story Points](http://c2.com/cgi/wiki?StoryPoints) as more palatable to most environments.



I also believe that around this time, people were arguing that relative estimation was easier for humans than absolute estimation. That is, it’s easier for you to say these two tasks are roughly comparable than to say how long each task will take in days.



[Planning Poker](https://en.wikipedia.org/wiki/Planning_poker) became popular but the fastest way to do Story Point estimation that I’m aware of is [Swimlane Sizing](http://theagilepirate.net/archives/109).



The problem was still over-optimism, but we also had the problem of over-optimism of managers and the difficulty of estimating. The solution was switching to Story Points. It roughly worked.



## Just count the Stories



When you break down work into Stories that are roughly 1–5 Story Points, you’ll begin to notice that they average out to 2.something. Many teams started to notice this and thought: “Instead of using Story Points, why don’t we just count Stories instead?”



The problem is still over-optimism and the difficulty of estimating. The solution is counting stories. It roughly works.



## Why are we grouping everything into big projects?



One of the key target attributes of a User Story is that it can be delivered independently. If that is actually the case, why are we grouping them together? Instead of asking how many Stories will get delivered after a period of time, why not ask, when will this Story be delivered? If we collect data on the start-to-done lead times of Stories, we can then use this data to estimate a range for when any particular story will get done. We can even do this for different Story sizes if necessary.



The problem is still over-optimism and the difficulty of estimation. The solution is measuring start-to-done lead time to support estimation. It roughly works.



---
Auteur : [Jason Yip](https://jchyip.medium.com/about)  
Source : [From “Load Factor” to “Velocity” to “Story Points” to “Counting Stories” to “Lead Time” to …](https://jchyip.medium.com/from-load-factor-to-velocity-to-story-points-to-counting-stories-to-lead-time-to-5f261707c76c)  
Date de parution originale : 29 Février 2016  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : jj/11/2020  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

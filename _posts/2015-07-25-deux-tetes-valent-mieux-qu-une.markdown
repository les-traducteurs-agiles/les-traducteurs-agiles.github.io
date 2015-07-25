---
layout: post
title:  "Deux têtes valent mieux qu'une"
date:   2015-07-25 21:59:53
published: true
categories: inspiration
---

To me, pair development is a no-brainer. It’s more fun than working alone, and you get a little of the benefit of the wisdom of the crowds but without the overhead of ineffective meetings and quality gates that method usually brings.

Pour moi, le développement en binôme va de soi. C'est plus amusant que de travailler tout seul, et vous bénéficiez d'une partie du savoir collectif mais sans les réunions inefficaces  et les contrôles qualités qui nous passent au-dessus de la tête qu'une méthode apporte habituellement.
 
Many people equate pair programming with XP. Ward Cunningham was excitedly telling me about pair programming at OOPSLA in 1993. I also ran into Paul Chisholm who had also been using it. Combined with my experience, that made three. Three occurrences make a pattern, and I wrote it down as a pattern after the conference. It was published at the first patterns conference in August 1994.

Pour la plupart des gens le développement en binôme égal XP. Ward Cunningham me parlait avec passion du développement en binôme à la conférence OOPSLA de 1993.  J'ai aussi discuté avec Paul Chisholm qui l'utilisait. Avec moi et mon expérience, nous étions trois. Trois occurrences fait un pattern et je l'ai couché par écrit après la conférence. Le pattern fut publié à la première conférence sur les patterns en août 1994.
 
Laurie Williams approached me in 1998 asking my suggestion for a PhD topic. I suggested Pair Programming, and her subsequent work led to a book on pairing (together with Robert Kessler) in 2002.
 
Laurie Williams entra en contact avec moi en 1998 pour me demander une idée de sujet pour un sujet de doctorat. Je lui suggérais le développement en binôme, et son travail par la suite conduisit à un livre sur le travail en binôme (co-écrit avec Robert Kessler) en 2002.  
 
Then in 2011 Joe Dager asked me about the origins of Pair Programming on behalf of author Karen Martin, who had traced Pair Programming’s origins to P. J. Plaugher (it amazed Joe that it came from the 1970s). So I sent out some inquiries in August. On August 27 Trygve Reenskaug replied:

Puis en 2011, Joe Dager me posa la question sur les origines du développement en binôme de la part de Karen Martin, qui avait retracé les origines du développement en binôme à P. J. Plauger (cela étonnait Joe que l'origine remonte aux années 1970). Alors j'ai lancé quelques recherches en août de cette même année. Le 27 août Trygve Reenskaug répondit :
 
Anne Lise Skaar and I did a large (75000 lines Smalltalk code) project combining literate programming and pair programming in the middle to late 80ties. The experience was reported in a talk at OOPSLA-89. We worked together sitting in front of a common screen for more than a year, possibly even more than two… Ward Cunningham and Kent Beck were mentioned in the paper. 

Anne Lise Skaar et moi avons fait un gros projet (75 000 lignes de code Smalltalk) combinant du développement ordinaire et du développement en binôme vers le milieu ou la fin des années 80. L'expérience fût relatée lors d'un exposé à la conférence OOPSLA de 89. Nous avons travaillé ensemble en face d'un seul écran pendant plus d'une année, voire pendant presque deux ... Ward Cunningham et Kent Beck étaient mentionnés dans cet exposé. 
 
In a reply from Ed Yourdon on the same day, the P. J. rumour gains ground:

Dans une réponse reçue de Ed Yourdon le même jour, la rumeur P. J. prenait de la consistence :
 
If anyone in my old company, YOURDON Inc, deserves any credit at all, it would have been PJ Plauger. He was instrumental in persuading me to get UNIX in our company (which had a $10,000 license fee at the time, a sum of money which Plauger lent the company, interest-free!). And even the dumb typewriter-like terminals at the time cost about $3,000 -- so we couldn't afford to get very many of them.

Si quelqu'un dans mon ancienne entreprise, YOURDON Inc, mérite un quelconque crédit, ce serait bien PJ Plauger. Il fût l'instrument qui me persuada de faire entrer UNIX dans notre entreprise (dont la licence à l'époque coûtait $10 000, une somme d'argent que Plauger prêta à l'entreprise sans aucun intérêt !). Et même les terminaux qui ressemblaient à des machines à écrire coûtait $ 3 000 -- et donc nous ne pouvions nous permettre d'en acheter beaucoup.
 
That forced programmers to work together on one Teleptype. But what capped it off was this reply from Jerry Weinberg later that day:

Cela força les développeurs à travailler ensemble sur un Teletype. Mais ce qui fit tout bousculé a été cette réponse de Jerry Weinberg plus tard dans la journée :
 
I learned to pair program (on paper — we didn't even have terminals back in the 1950s) in Los Angeles, from Bernie Dimsdale, who learned it from John von Neumann. I don't know if it has any history before then, but that's way back to Aberdeen Proving Grounds in the 40s.

J'ai appris le développement en binôme (sur papier - dans les années 50, nous n'avions même pas de terminaux) à Los Angeles de Bernie Dimsdale, qui l'avait appris de John von Neumann. Je ne sais pas s'il y a eu une histoire avant cela, mais cela remonte à Aberdeen Proving Grounds[^1] dans les années 40.
 
[^1]: Aberdeen Proving Grounds - terrain d'essai de l'armée américaine
 
There were some responses of a different color. On that same day Brian Kernighan wrote:

Il y eût quelques réponses d'une teneur différente. Ce même jour Brian Kernighan écrivait : 
 
I have no recollection of any of the history of pair programming, and I certainly have no involvement with it at all.  I definitely plead not guilty.

Je n'ai aucun souvenir d'une quelconque histoire du développement en binôme, et je n'ai certainement aucun rapport avec. Je plaide définitivement non coupable.
 
which Doug McIlroy confirmed the next day:

ce que me confirma Doug McIlroy le lendemain :
 
I'm not familiar with "pair programming” as a formal concept, but if it refers to having two pairs of eyes on every piece of code, it would apply to very little early Unix code. Ken and Dennis were a pair of programmers, but they split the work.

Je ne suis pas familier du "développement en binôme" en tant que concept formel, mais s'il se réfère au fait d'avoir deux pairs d'yeux sur chaque morceau de code, il ne pourrait s'appliquer qu'à une toute petite partie du code d'Unix, Ken et Dennis était un binôme de développeurs, mais ils se répartissaient le travail.
 
Last night over beers, I learned of a “new” variant on this theme called Mob Programming from Woody Zuill. It’s a good idea and many folks are embracing it. It, too has history. I remember that Joe Davison, Ricky Spiece and Martin Biernat were doing this in Bell Laboratories in the 1990s.

La nuit dernière après quelques bières, j'ai appris une "nouvelle" variante sur ce thème appelé le développement collectif de Woody Zuill. C'est une bonne idée et beaucoup de personnes l'adoptent. Elle, aussi a une histoire. Je me rappelle que Joe Davison, Ricky Spiece et Martin Biernat faisaient déjà cela dans les années 1990.
 
Pairing is great, and it’s not new. I’m sure Ada and Charles were doing it back in 1843. Learn to pair and have some fun.

Le binômage est génial et il n'est pas nouveau. Je suis certain qu'Ada et Charles le pratiquait en 1843. Apprenons à binômer et amusons-nous.

---
Auteur : [Jim ("Cope") Coplien](https://sites.google.com/a/gertrudandcope.com/www/jimcoplien)  
Source : [Two Heads Are Better than One](http://www.computer.org/web/agile-careers/content?g=8504655&type=article&urlTitle=two-heads-are-better-than-one)  
Date de parution originale : 09 Mars 2015  

---
Traducteur : [Nicolas Mereaux](http://www.les-traducteurs-agiles.org/traducteurs/)  
Date de traduction : 27/05/2015  

---

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Ce(tte) oeuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Licence Creative Commons Attribution - Pas d'Utilisation Commerciale - Partage dans les Mêmes Conditions 4.0 International</a>.

---

{% include share_buttons.html %}

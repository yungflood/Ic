# MY FINAL PERFORMANCE :D
## Where i started
- To begin i started with this strudel beat i began including the break sample and chopping it up
```haskell
setCpm (170/4)
_$mel:
s("supersaw").note("<d2 d4 d2 a3 c5 f3>").fast(8).adsr(".01:.01:.3:.2")
.penv(25).panchor(0).pdec(0.01).delay("0.25").crush("8")
.gain(.1).orbit(3)

_$perc:
s("alesissr16_cp:3").beat("1,7,8,12",16).lpf(2000).gain(0.2)

_$hh:
s ("spacedrum_hh").beat("0,1,2,3,4,5,6,7,8",8)
.gain(0.8)
.tremolosync("6")

_$breaks:
s ("brk").beat("<0,4,8>",16).slice(4, "<0 3 1 3>").iter(1).fast(2).crush(6).distort(2)
.gain(0.3)

_$kick:
s ("korgpoly800_bd").beat("0,4,8,12",16).lpf(200).distort(0.3).duckorbit(3).duckdepth(1)

_$mel2:
s ("rhodespolaris_misc").beat("5,13",16).delay(4).gain(0.2).crush(8)
```
- I then started my hydra code by using my idea from last time but playing with some different parameters and using the initScreen casting a video I made for my cousin's metal band lol and manipulating that in Hydra
```haskell
s0.initScreen()
src(o0).scale(1.01).blend(
  src(s0).luma(0.2).kaleid(2).colorama(3),0.04)
	.out(o0)
```
## Performance!!!
- In my performance I adjusted a few parameters in hydra such as .thresh() and .scale
- My strudel code worked perfectly in strudel but i forgot to test it in flok (sigh), so during my performance one of my main elements didn't work the drum break so this caused me to pivot my track a bit
- My track originally had more of jungle feel using the chopped break but i switched to more of a techno kind of route using the offbeat mel2 as a backbone for that transition
- I then added these two sounds during the performance to give my track even more of a footwork/ technoish feel
```haskell
_$clap:
s("cp").beat("0,3,5,8,15",16)

_$oh:
s("oh").beat("3,6,8,14",16).tremolosync("3")
```
## In Conclusion
- I loved this class and had an awesome time learning about live coding! Its a new part of my music making roster and had a great semester.
Have an awesome summer!!
All the best,
Isaac :D
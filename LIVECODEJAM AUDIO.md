# LIVECODE JAM AUDIO 
## MY PROCESS
- I started my process by just noodling around on strudel last night to prepare more or less what I would do for the audio side of things as I am a bit more comfortable with the visual side
- Firstly I started by creating the melody and playing around with the pitch envelope settings to create this melody layer
```haskell
$mel:
s("saw").note("<f a c e d a c d2>").fast(8)
.penv(48).panchor(0).pdec(0.03)
.gain(0.7) .lpf(6000)
```
- Then I began working on the drums using the 909 bank for more trancey ravey sounds and ended up with this drum pattern
```haskell
$kicks:
s("bd:1").bank("RolandTR909").beat ("0, 4, 8, 12",16).gain(1)
  .crush(10)
.lpf (800)

$hh:
s ("hh hh hh hh hh hh hh hh")
.gain(0.8)
.tremolosync("3")

$oh:
s("~ oh ~ oh ~ [oh ~ oh ~] ~ oh").bank("RolandTR909")
.adsr(".01:.08:.5:.2")
.gain(0.3)

$clap:
s("cp:1").beat("4,12",16).bank("RolandTR909")
.gain(0.6)
```
- I then finished up with a bass line that i created on the off beats
```haskell
$bass:
s("saw").note("< ~ f1 ~ f1 ~ f1 ~ f1>")
  .fast(8)
.gain(1)
.lpf(800)

_$bass:
s("saw").note("< ~ d1 ~ d1 ~ d1 ~ d1>")
  .fast(8)
.gain(1)
.lpf(800)
```
- My thought process with the bass was to mute the layer with the notes I dont want and switch it to the notes I do want every once in a while under my direct control 
## END THOUGHTS
- Overall this was an awesome excersise and I had a ton of fun creating a nice little beat to play with 



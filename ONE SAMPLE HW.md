# ONE SAMPLE HW
## My Process
- To begin this process I found an interesting kalimba sample within strudel and began to brainstorm how I would create different textures with the one sample
- Ultimatley I decided i was going to use the tremolo and the filters + gain structuing to create my layers and produce my whole idea
## First Layer
- My first layer I wanted to create a bassish backbone to build off of so I used the lpf with a q that is going from 0 - 20 over time with a gain of 1 to keep it on the top of the mix 

```haskell
$: s("[kalimba!4]kalimba ").gain (1) .lpf (500) .lpq ("<0 10 20>") 
```
## The Next Layer
- The next layer I began playing around with the tremolo that i found in the learning tab on strudel

```haskell
$: s("kalimba!8").gain (0.6).tremolosync("4").tremoloskew("<.5 0>").delay(.25).delayfeedback(".25")
```
## Anotha layer
- In this layer I tried messing around with the duckorbit for a pumping effect and didn't quite acheive the result I was looking for but kept it anyways I also have been playing around with the transpose but I don't think it is actually doing anything to the samples lol I just didn't delete it

```haskell
$: s("kalimba!16").gain (0.2).hpf(1500).transpose ("12").duckorbit("2:3").tremolosync("6").delay(.3)
```
## anotha 1
- More experementing with effects

```haskell
$: s("kalimba!2").gain (1.2).crush ("<16 14 12 10>").hpf ("<4000 3000 2500 2000 1000 500>") .hpq (15).transpose ("-10")
```
## The last two
- These last two I added just for more texture and to help build the space of the production + more experementing again

```haskell
$: s("kalimba!4").gain (1.2).lpf (200).lpq (20)
$: s("kalimba!10").gain(0.3).transpose ("-25").tremolosync("4").delay(.3)
```
## The Performance 
- In the actuall performing of this piece I would start with only the first layer unmuted and gradually add layers by unmuting channel with the _ so the code initally would appear like this 

```haskell
$: s("[kalimba!4]kalimba ").gain (1) .lpf (500) .lpq ("<0 10 20>") 
_$: s("kalimba!8").gain (0.6).tremolosync("4").tremoloskew("<.5 0>").delay(.25).delayfeedback(".25")
_$: s("kalimba!16").gain (0.2).hpf(1500).transpose ("12").duckorbit("2:3").tremolosync("6").delay(.3)
_$: s("kalimba!2").gain (1.2).crush ("<16 14 12 10>").hpf ("<4000 3000 2500 2000 1000 500>") .hpq (15).transpose ("-10")
_$: s("kalimba!4").gain (1.2).lpf (200).lpq (20)
_$: s("kalimba!10").gain(0.3).transpose ("-25").tremolosync("4").delay(.3)
```

## Final Product
```haskell
$: s("[kalimba!4]kalimba ").gain (1) .lpf (500) .lpq ("<0 10 20>") 
$: s("kalimba!8").gain (0.6).tremolosync("4").tremoloskew("<.5 0>").delay(.25).delayfeedback(".25")
$: s("kalimba!16").gain (0.2).hpf(1500).transpose ("12").duckorbit("2:3").tremolosync("6").delay(.3)
$: s("kalimba!2").gain (1.2).crush ("<16 14 12 10>").hpf ("<4000 3000 2500 2000 1000 500>") .hpq (15).transpose ("-10")
$: s("kalimba!4").gain (1.2).lpf (200).lpq (20)
$: s("kalimba!10").gain(0.3).transpose ("-25").tremolosync("4").delay(.3)
```

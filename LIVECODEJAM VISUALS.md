# LIVE CODE JAM VISUALS
## My Process
- Starting these visuals began with me exploring how to delay with a blend and create feedback
- I began with this code 
```haskell
s0.initCam()
src(o0).scale(1).blend(
  src(s0),0.01)
.out(o0)
```
- This bit of code was the basis for my whole performance and I added a few effects for the actual performance which led me to this my final code
```haskell
s0.initCam()
src(o0).scale(1).blend(
  src(s0).luma(0.3).colorama(3).scale(1),0.01)
.out(o0)
```
- :D this was so fun!
# HYDRA STUFF!!
## Where i started
- I began by using this bit of code i messed around with while learning the basics in class 
```haskell
s0.initCam()
src(s0).luma(0.6).thresh(0.2).colorama(20)
.out(o1)
```
- I then began experementing and tried to figure out a way to create a feedback loop
- I tried initally to work with the repeat but couldn't get it to actually trail behind to make trail sort of effect 
- I then used this video as a bit of inspiration 
[![videolink](https://www.youtube.com/watch?v=m-Q7b82Y9Mk)
- I ended up creating this which i still enjoy but need to put more effort into creating a trailing effect for future use
```haskell
s0.initCam()
src(s0).luma(0.6).thresh(0.2).colorama(20)
.out(o1)
```

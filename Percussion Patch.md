# Percussion Patch Isaac P
## My Thought Process
- I started this patch honestly by working on a different piece of code I was making that sounded cool but wasn't quite related to the project 
' fast 1.2 $ stack [
fast 4 $ s "new notes" # n (irand 15) #pan tri ,
n (run 8) # s "voodoo" 
] ' 
- This patch led me to messing around more with the stack function to make full drum loops and I then utilized this for my percussion patch
- Next I went and started working on my percussion patch 
- First I used a stack function and this bit of code from the class git hub 
'  s "hh!16?" '
- This line was my inspiration for my first line of the drum patch 
'  s " bd!8 hh!5 sd!3 ? ", '
- Next I wanted to add a more steady 4 on the floor groove and used the s " bd bd bd bd " to acomplish that i also added the extra gain to help it cut over the more accently kick underneath 
- Next I wanted a clap on every other beat and it to pan back and forth so I used the ~ to silence the beats I didnt want the clap and the # pan sine for a constant pan 
- The toms I just wanted to try something different and liked how this sounded repeating 4 times with random silence  
'  s "lt!4?", '
- Lastly I just wanted another accent hh so I added the extra one more spread out with more gain to cut above the other hats
- This led me to my final percussion patch code 
' stack [
s " bd!8 hh!5 sd!3 ? ",
s "bd bd bd bd" #gain 1.5 ,
s " ~ cp ~ cp" #pan sine, 
s "lt!4?",
s "~~hh~~~hh~" #gain 2
] ' 

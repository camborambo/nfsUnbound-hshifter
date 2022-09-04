# H-Shifter support for Need for Speed Heat

Since NFS Heat for some reason doesn't support shifters at all, this program makes it possible!  
You can use a shifter with up-to 8 gears.  

Since I didn't have the patience to find static pointer (offset) to the one memory address that's required for this (either Frostbite engine or Denuvo or both being difficult..), this program supports either manually supplying the memory address that you can easily find with Cheat Engine, or an automatic memory scanner that will do this for you easily.   

## Getting started

*This guide will cover the usage of built-in memory scanner for ease-of-use.*  

Since I own Logitech Driving Force Shifter, I will demonstrate how to use this with Logitech G HUB software, however, this program will work with any shifter that supports custom keymappings.  
What you'll want to do is map your shifter gears to keys 1 - 6 (not NUMPAD keys!) like this:  
| Key   | GEAR             |
|-------|------------------|
| Key 0 | REVERSE          |
| Key 1 | Neutral (UNUSED) |
| Key 2 | GEAR 1           |
| Key 3 | GEAR 2           |
| Key 4 | GEAR 3           |
| Key 5 | GEAR 4           |
| Key 6 | Gear 5           |
| Key 7 | Gear 6           |

![ghub](https://i.imgur.com/eTj3Fx6.png)

Once you've done all that, launch the game, set your transmission to manual in settings and hop into a session (you cannot be inside the garage).  

After you load into the game, launch `heat-shifter.exe`, type `s` and press `ENTER`.  

The program will ask you to shift into the 4th gear. Do as you're asked and `ALT-TAB` back into the program and press `ENTER`.  

The program will search NFS' memory for a short while (depending on your computing power).  

After it's done searching, it will ask you to shift into 3rd gear, `ALT-TAB` back and press `ENTER`.  

This step will repeat a few more times, until the program finds 18 results and print out found memory addresses.  

After that happens, you can go back to the game and try changing gears with your shifter.  

If the gear doesn't change on the speedometer, press the `+` key (numpad) and change to two different gears. If the gear changes inside the speedometer, you have the right address. So repeat the process of pressing the `+` key and shifting into two different gears, until it basically works :)  

**That's it, enjoy!**
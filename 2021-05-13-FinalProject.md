## Final Project Prospective

### Proposal

What a trip, if I do say so myself. For brevity's sake, I'll just go through the steps of my process and my own thoughts while making writing my code.

Starting from the beginning, as in, my proposal, I stated clearly that my inspiration was a tamagotchi. Mainly the idea of creating a "living" that you take care of, or interact with in some way.

My main desire was to create a flock of creatures. A group on tiny weird creatures that one can control; basically they follow the the player.

You could place food on the screen, and the creature, first starting at only one, can eat it and reproduce. Reproducing as in the creature multiplies in numbers. In time you would have a crowd of creatures, in varying sizes, since eating the food also increases size.

In addition, I was also envisioning an element of zooming in. wherein as the crowd increases so does the canvas. This is to create an effect of a camera pulling out as the group increases in size. So at the start, it would feel more intimate, but as more creature increase, it would create this abstract feeling, like the crowd becoming less of creatures and more like a blob.

This would have played into the inheritance and other feature of my program. The reason as to why I wanted to have my creatures flock and be in nurmbers is for the sake of a color effect.

I really wanted to play color in this project. As mentioned in my proposal, I was inpired by a project that involved inheretence in cells communicatig with each other. So I wanted to incorporate this aspect with that of color.

What this resulted was the idea of making it so that the creatures evolve in color. Starting with a specific color, which they pass on to their children, except with a bit of difference. The desired result would be a big group of colored creatures, but because of this color evolution, it would be a color mixture. And this paired up with the zoom out feature would result in a big blob of paint with this weird mixture of hue. Almost like a paint brush that the mouse controls.



### Attempt and Process

I started by simply doing what I did for my squirrel eat squirrel project, that is, start by creating a creature class. A class that created a simply circle that moved. In this case, though the movement would be dictated by the player. The object, aka, our creature, would simply follow the mouse.

I'm not very keen of the physics/forces that were reuqired to accomplish this movement. So I mainly looked at examples that accomplished this effect. I forget which example I used, I'm pretty sure it was from a processing example. But since I didn't end up using this code, I doesn't matter too badly. Explained a bit later.

After incorporting this simple code, I paused and starting creating the food class for creating food pellets that the creatures would eat.

This was also fairly easy since it's just a condensed duplicate of the creature class, albeit without the movement. Instead it had code that would create a new food object upon a mouse click. 

After finishing the food portion, I simply used some of the code from my squirrel code for eating and reproducing methods. I obviously tweaked it to fit this new context, and in the end, I managed to get it working.

So now I had a program that created a creaute, currently a simple circle, that followed the mouse. With the click of the mouse, a random food pellet would appear. And if the circle went over to it. The circle would increase in size and reproduce, which simply means creating another creature object. The eaten food pellet would obviously disappear, and the user could continue to creature food pellets and feed and reproduce the creatures. 

The problem now was the flocking.

Even though 

### Positives and Negatives




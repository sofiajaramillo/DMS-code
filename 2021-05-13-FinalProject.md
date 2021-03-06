## Final Project Prospective

### Proposal

For brevity's sake, I'll just go through the steps of my process and the thoughts I had while writing my code.

Starting from the beginning, as in, my proposal, I stated clearly that my inspiration was a tamagotchi. Mainly the idea of creating a "living" thing that you take care of, or interact with in some way.

My main desire was to create a flock of creatures. A group on tiny weird creatures that one can control; basically they follow the the player.

You could place food on the screen, and the creature, first starting with only one, can eat it and reproduce. Reproducing as in the creature multiplies in numbers. In time you would have a crowd of creatures, in varying sizes, since eating the food also increases size.

In addition, I was also envisioning an element of zooming out. Wherein as the crowd increases so does the canvas. This is to create an effect of a camera pulling out as the group increases in size. So at the start, it would feel more intimate, but as more creatures appear, it would create this abstract feeling, like the crowd becoming less of living things and more like a blob. This would have played into the inheritance feature of my program. 

The reason as to why I wanted to have my creatures flock is for the sake of a color effect.

I really wanted to play color in this project. As mentioned in my proposal, I was inpired by a project that involved inheritence in cells communicatig with each other. So I wanted to incorporate this aspect with that of color.

This resulted in the idea of the creatures evolving in color. Starting with a specific color, which they pass on to their children, except with a bit of a difference. The desired result would be a big group of colored creatures, but because of this color evolution, it would have this color mixture. And this paired up with the zoom out feature would result in a big blob of paint with this weird mixture of hue. Almost like a paint brush that the mouse controls.



### Attempt and Process

I started by simply doing what I did for my squirrel eat squirrel project, that is, creating a creature class. A class that creates a simply circle that moves. In this case, the movement would be dictated by the player. The object, aka, our creature, would simply follow the mouse.

I'm not very keen of the physics/forces that were required to accomplish this movement. So I mainly looked at examples that accomplished this effect. I forget which example I used, I'm pretty sure it was from a Processing example. But since I didn't end up using this code, it doesn't matter too much. Explained a bit later.

After incorporting this simple code, I paused and started creating the food class for creating food pellets that the creatures would eat.

This was also fairly easy since it's just a condensed duplicate of the creature class, albeit without the movement. Instead it had code that would create a new food object upon a mouse click. 

After finishing the food portion, I simply used some of the code from my squirrel code for eating and reproducing methods. I obviously tweaked it to fit this new context, and in the end, I managed to get it working.

So now I had a program that created a creature, at this point a simple circle, that followed the mouse. With the click of the mouse, a random food pellet would appear. And if the circle went over to it, the circle would increase in size and reproduce, which simply means creating another creature object. The eaten food pellet would obviously disappear, and the user could continue to create food pellets and feed and multiply the creatures. 

![Attempt](ProjectSketchgif.gif)

### Flocking

The problem now was the flocking. I needed to write code that would allow the creatures to crowd together, but not touch each other. So basically flock.

Again, I couldn't simply write my own code for this, since it would require a deep understanding of seeking and separation forces. So I sought to look for similar examples that accomplished a similar goal in order to implement this code into mine, with credit of course.

I landed on the example for separation forces in the "Nature of Code" book, chapter 6 section 8. It did exactly what I was intending for. And in a perfect world I would have simply taken some of the basic setup of the code and brought it over to my code, simply implementing it.

But I overestimated how complex the code was, and the fact that I both didn't have the time and understanding to make it work that way. 

After some thought, I reluctantly settled on the idea of using this code as my basis instead, basically dropping the movement code I already had and sort of starting from scratch with this new code.

Which is what I did, I used the example code, this separation sketch, as a base, and brought over my own code into it. I basically recreated my sketch over again.

### Positives and Negatives

After getting the flocking done, I had a pretty good setup. A program that created creatures that ate and reproduced, moved by following the mouse, and stayed flocked together.

Now the next part was including the rest of my features. Both successfully and not.

The first one, and probably the most important one, was the color feature. Basically make it so that the creatures evolve in color as they reproduce.

I first started by making it so that the first creature gets set with a random hue every run. Then I wrote code so that every time the creature, or any other creature reproduced, the creature would pass down their hue, but with a difference of 10. So the next creature would have a lighter hue, therefore evolving.

I also thought it would be cool for the hue to change in both directions, either add or subtract hue. So I created two types of food pellets, blacks and whites, that would do exactly that, subtract and add hue when eatten.

Apart from hue, there was also brightness and saturation. I didn't want to mess with these values too much, since they don't add too much to the color as much as hue. So after setting a set saturation and brightness level, I simply made it so that the user can control them via sliders on the screen, if desired. 

I also thought about functionality a bit, so I proceded to code a start/play screen and a pause screen to facilitate the program. It took some if statements, and despite that the pause screen is still a bit iffy, it works for it's purpose.

You would think that at some point I would implemement my important zoomnig out feature. But the sad reality is that I wasn't able to incorporate it. Mainly becuase of time and prioritizing other things, but also because if felt like a tricky thing to do and I wasn't exactly confident in a way to accomplish this effect. I already had a strong foundation, so I didn't want to rock the boat and potentially mess something up.

The good thing is that I was able to create a new feature that I didn't even think of at first. This comes in the form of the creatures actually leaving a trail behind, like a paintbrush. 

I thought about ways that I could make the program more fun, and I realized that I should utilize the fact that I have all these colorful creatures controlled by the player. So I thought that it would be cool to make them act like brushes. So I coded some if statements to stop the loop witht the press of a key, and I got just that. Now the creatures could leave long lines of "paint" behind on the screen.

Lastly, my creatures were a bit too simple. Like they were only colored circles, which might be fine for my simplistic self, but they don't really look like creatures. So I decided to look back at my previous project, where I created a pretty cool creature design, like a mutant squid. I liked what I did with the following eyes there, so I brought that code over. So they're still circles, but with a little googly eyes that follow the mouse when they move.

![CreatureProgram](CreatureProgram.gif)

*The Creature Program in essence*

![DrawingFlocking](DrawingFlocking.gif)

*The new drawing function I came up with*

Here's a quick link to the sketch:

https://editor.p5js.org/sofiajaramillo/sketches/seHsgQe7N

### Final Thoughts

So at the end of the day, I managed to produce a pretty solid program. One that creates these tiny living things that increase in numbers. That one can control, feed, and draw with.

My favorite part of this whole process was seeing my work slowly evolve, like my creatures. Adopting and leaving features, and thinking of new things to potentionally bring in. I'm very intrigued by all the different features that I could theoretically add in the future.

Honestly, this might be my favorite thing I've worked on this semester, and maybe in Processing as a whole. And I could totally see myself using some aspect of this program in future creative endeavors.

It's still a bit upsetting that that I can't completely call this work my own, since I am working from the code from someone else. But my main hope is that as I learn more and understand some of these trickier subjects, I could potentially come back and write it completely from my own knowledge, without someone else's influence.

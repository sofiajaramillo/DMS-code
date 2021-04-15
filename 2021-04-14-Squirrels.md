## Squirrel Eat Squirrel

The processing for coding a game for squirrels eating other squirrels was a bit of a fun struggle.

I mainly took the lead in this group project. Well, "lead" as in I did most of the actual coding, while the rest of group members did the design elements. I don't like to look at it as me doing most of the work, but more like I choose the option that allowed me to code the game the way I saw it fit.

The process began pretty simple. I first wrote a class for the player. This included a simple display function, which displayed a simple circle, as well as a move function that utilized the arrow keys to move the circle, with the user's input. Then I coded the enemy class, which also displayed a circle, and moved by being placed in random locations each run, as well as random sizes. The point was to create multiple enemy objects in an array, which would act as the random enemy circles the player either eat or get eatten by.

The difficult part here on out was finding a way to write the program so that these enemies and player could interact in the way they're supposed to. As in, actually eating each other. I was able to accomplish this by creating a method in the player class that checked the location of the player in relation to any enemy object/circle on the sketch. Based on this location, the player would either "eat" the enemy it came into contact on the basis that it's smaller in size, and increase in size. If it's bigger, than you would get hit and loose a "life", and after loosing 3 lives, you would lose overall. 

All of this was incapsulated in a method. Or two, as in, the other method that ended the sketch when all the lives were lost. Overall, I was able to create a sketch where a player circle, controlled by the user, could eat other circles that were smaller or get eatten by those that were bigger.

This method I would later within the enemy class itself so that the enemies could actually eat each other, not just the player.

I didn't get to take a screenshot, but here's a sketch of what my sketch looked like:

![Squirrel Sketch.jpg]({{site.baseurl}}/Squirrel Sketch.jpg)


# Implementations

The basics were down. Now my goal was to implement my member's contributions into my main code. 

First, the easiest implementation, was the enemy's movement which one of my members worked on. "Movement" as in the enemies didn't just sit in static locations but actually moved in an erratic way. I simply implemented this code into the move method of my enemy class.

The second was bit trickier. This involved implementing the grass, which was a background and grass blades which were procedurally generated. The background was fine enough, but the blades weren't working for some reason. Thankfully, my other member was able to fix it and get it working.

The last implementation was the difficult one. My team member worked on a sketch for the player and the enemy; two sketches of squirrels made up of ellipses and shapes. The sketches were fine on their own, but I knew that I had to have these squirrels as individual images, not just multiple lines of ellipses, for the code to avoid unnecessary problems. It was tricky, but I manage to export them as png with the save function, and import then as singular images with one x and one y. 


Overall, I implemented all my team members design elements into my code so that the game finally started to look like a "squirrel eat squirrel" game, not just circles eating circles.

Again, no screenshots, but here's a drawing:


# Advanced Stuff

After implementing my members code, I worked on adding the other features. I added a quick fullscreen option, I fixed the player lives since they weren't working, I made it so that a new squirrel could appear after 120 frames, and I added two buttons to toggle between two different speeds for the enemies. I also tried adding a button to reset the game, in case the random location/sizes of the enemies don't seem favorable.

Obviously, some of these are a bit iffy, or not working how I want it to work exactly, but I think they do their job well, especially considering my contraints.

I want to implement another button to make the squirrel player move on it's own, and maybe an "apple" that would add an extra life or increase the squirrel's size. But as of writing this, I'm not sure if I'll be able to, since I'm focusing on adding my other members new updated elements, but we'll see.
 
Here's how the game looks like as of now:






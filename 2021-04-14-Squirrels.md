## Squirrel Eat Squirrel

The processing for coding a game for squirrels eating other squirrels was a bit of a fun struggle.

I mainly took the lead in this group project. Well, "lead" as in I did most of the actual coding, while the rest of group members did the design elements. I don't like to look at it as me doing most of the work, but more like I choose the option that allowed me to code the game the way I saw it fit.

The process began pretty simply. I first wrote a class for the player. This included a simple display function, which displayed a simple circle, as well as a move function that utilized the arrow keys to move the circle, with the user's input. Then I coded the enemy class, which also displayed a circle, and moved by being placed in random locations each run. The point was for to create multiple enemy objects in an array, which would act as the random enemy circles the player either eats or gets eatten by.

The difficult part here on out was finding a way to write the program so that these enemies and player could interact in the way they're supposed to. As in, actually eating each other. I was able to accomplish this by creating a method in the player class that checked the location of the player in relation to any enemy object/circle on the sketch. Based on this location, the player would either "eat" the enemy it came into contact on the basis that it's smaller in size. If it's bigger, than you would get hit and loose a "life", and after loosing 3 lives, you would lose overall. All of this was incapsualted in a method. Or two, as in, the other method that ended the sketch 

This method I would later within the enemy class itself so that the enemies could actually eat each other, not just the player.

The basics were down. Now my goal was to implement my member's contributions into my main code. 

First, the easiest implementation, was the enemy's movement which one of my members worked on. "Movement" as in the enemies didn't just sit in static locations but actually moved in an erratic way. I simply implemented this code into the move method of my enemy class.

The second was bit trickier. This involved implementing the grass, which was a background and grass blades which were procedurally generated. The background


I didn't take screenshots as I worked, but here's a quick sketch of how my sketched looked like and how it looked like after:


After implementing my members code, I worked on adding the other features. I added a quick fullscreen option, 



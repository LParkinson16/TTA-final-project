# TTA-final-project
The last project for the training course with Generation UK as part of the Tech Talent Accelerator.

#Getting statrted
The final product for the first iteration of my project is currently being hosted by GDeveleop at the link :
https://games.gdevelop-app.com/game-04c58441-a35a-4392-baae-c81d95089248/index.html
From here the game may be played directly.

#Running tests
 
#Deployment

#Built with
For this project I relied on GDevelop 5 which is an open source cross-platform game engine that specialises in creating small 2D games. This engine makes use of many fundamental programming concepts such as the creation of variables and the use of comparrioson operators to determine how they will interact with one another. This also allows developers to use JavaScript in tandem with the tools that it provides in order to make a functioning product.

#Authors
Latiff Parkinson

#License
Games exported with GDevelop exist under the MIT license

#Acknowledgment
THE GEM TUTORIALS



#Process

##sprites
I began by loading in the sprites that I would be using throughout the process. I assigned these different behaviours that would allow them to be able to interact with one another appropriately when referenced later.

##pregame
Before the game begins to run I have created a condition that initiates the game to start running when the space bar is pressed. This condition also includes instructions to hide certain sprites such as the hitbox for the main character sprite that will collide with obstacles.

##movement speed
Here I have created a condition for when the game is running. Whilst the game is running the character will move across theground at a speed of four

##ground
whilst the game is running the ground sprite as well as the character hitbox will scroll across the screen. This happens bu detracting its x position on the screen from the 'scroll speed' variable that I created earlier

##clouds
As I wanted the clouds to travel at their own pace I created the variable 'cloudspeed' which is set to one. The clouds will travel at this pace until the game is stopped.

##obstacles
At the beginning of the scene the obstacles are placed into the game. The speed at which obstacles move across the screen by deducting their position in the x axis from the sroll speed. Obstacles are also set to a speed of one. The 'obstacle.width()' variable is set to space all obstacles 810 pixels apart when being placed in the game. There are a total of 8 different sprites that may appear when playing and the 'RandomWithStep()' variable allows me to select a random obstacle to be placed in the game.
On the condition that a collision occurs between the character and an obstacle the game is stopped and the charactersprie changes to a new animation when upon collision.

##score
the score variable is simply a text file with the "pixelmix" font that has one added to it every 0.15 seconds. The score will initally appear as a string of zeroes however as the score increases one zero is removed for every increase in the amount of digits on the screen

##gameover
when this condition is met the 'gamerunning' variable that keeps the game on is set to zero so that all objects stop running eg; the scroll speed. Once this happens the layer with the "GAMEOVER" text and restart button will appear. If clicked the restart button will change the scene to the beginning again. 



Stacking Game
=======================
In this assignment you will write learn some standard game making techniques. You will learn how to check for collisions, add different levels, keep score and add artwork to your game. Your game doesn't have to look or work like any other. Feel free to make modifications and add additional features. You may find the slides that start from 456 of the PythonProcessing.pptx PowerPoint slides helpful.

Suggested steps for completing this assignment.  
--------

### Create a paddle
* Start by creating a paddle that can be used to catch the falling squares. Create three variables for the Paddles: `paddleX`, `paddleY` and `movingRight`
* Then Create two functions `drawPaddle()` and `movePaddle()`
* Write a `mousePressed()` function to control the movement of the Paddle.
### Create a stacker
* Create two stacker variables `stackerX` and `stackerY`. Initialize `stackerX` randomly
* Write two stacker functions `drawStacker()` and `moveStacker()`. 
* Write a function that checks for a collision between the stacker and the paddle: `checkForCatch()`. It can use Processing's [`dist()`](http://py.processing.org/reference/dist.html) function. If the stacker is below a certain y coordinate and within a certain distance of the paddle, we can consider the stacker caught.
### Add a level
* Create a `level` vairable. If the stacker is caught increase `level` by one.
* Add an `if` statement to `drawPaddle()` so that when we reach level 1, we draw the blue stacker on top of the paddle
* Add code in `checkForCatch()` to randomize the position of the stacker above the screen so that the next stacker drops down from the top of the screen
### End the game is the stacker isn't caught
* Create a `gameOver` variable and initialize it to `True`
* In `draw()`, add an `if` statement. If the game is over, display an appropriate message and/or artwork. Run the program and make sure the it shows the game over message.
* Now go back and change the initializtion of `gameOver` to `False`
* Add an `if` statement at the bottom of `moveStacker()`. If the stacker reaches the bottom of the screen, set `gameOver` to `True`. Play your game to test that it works.

Samples of Student Work   
-----------------------   
None yet!  

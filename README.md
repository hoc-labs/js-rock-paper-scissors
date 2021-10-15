# Rock Paper Scissors

Rock paper scissors is a classic two player game. Each player chooses either rock, paper, or scissors. The items are compared, and whichever player chooses the more powerful item wins.

The possible outcomes are:
* Rock destroys scissors.
* Scissors cut paper.
* Paper covers rock.
* If there’s a tie, then the game ends in a draw.
  
Our code will break the game into four parts:
* Get the user’s choice.
* Get the computer’s choice.
* Compare the two choices and determine a winner.
* Start the program and display the results.

## Step 1 - create a function called userChoice that returns the word the user selected.

The first step is to prompt the user to ask whether they want rock, paper, or scissors.

Create a function that performs this task and returns the value in lower case.

Your function should check to make sure the user entered a valid value. If not, then you should write to the console log that there was an error and return null from the function.

Test your function by calling it and writing the return value to the console.

## Step 2 - create a function called computerChoice which will randomly select a word.

The function should use the Math.random and Math.floor methods to get a value between 0 and 2, where each number represents either rock, paper or scissors.

Here is a [reference](https://education.launchcode.org/intro-to-professional-web-dev/appendices/math-method-examples/random-examples.html#random-examples) for the Math.random.

Here is a [reference](https://education.launchcode.org/intro-to-professional-web-dev/appendices/math-method-examples/ceilfloortrunc-examples.html#floor) for Math.floor.

Test the function by calling it multiple times and logging the output to the console. Ensure that random answers are coming back.



The function should return the correct word that matches the selected value.

## Step 3 - create a function called determinWinner that determines who won.

Now it’s time to determine a winner.

Create a function named determineWinner that takes two parameters named userChoice and computerChoice. 

This function will compare the two choices played and then return if the human player won, lost, or tied.

Let’s deal with the tie condition first. 

Within the determineWinner() function, write an if statement that checks if the userChoice parameter equals the computerChoice parameter. If so, return a string that the game was a tie.

If the game is not a tie, you’ll need to determine a winner.

Begin by writing an if statement that checks if the userChoice is 'rock'. Inside the if statement’s block, write another if/else statement. The inner if/else should check if the computerChoice is 'paper'. If so, return a message that the computer won. If not, return a message that the user won.

Next, write another if statement for if the userChoice is 'paper'.
Inside this if statement, the computerChoice must be either 'scissors' or 'rock'. Write logic that will return a winner.

Next, write yet another if statement for if the userChoice is 'scissors'.

Inside of this if statement, the computerChoice must either be 'rock' or 'paper'. Write logic that will return a winner.

## Step 4 - create the playGame function

Everything is set up. Now you need to start the game and log the results.

Create a function named playGame.

Inside the playGame() function, create a variable named userChoice set equal to the result of calling getUserChoice(), passing in either 'rock', 'paper', or 'scissors' as an argument.

Create another variable named computerChoice, and set it equal to the result of calling getComputerChoice().

Under both of these variables, use console.log to print them to the console.

## Step 6
Finally, let’s determine who won.

Inside the playGame() function, call the determineWinner() function. Pass in the userChoice and computerChoice variables as its parameters. Make sure to put this function call inside of a console.log() statement so you can see the result.

Then, to start the game, call the playGame() function on the last line of your program.

## Extension

Make this game better by adding a secret cheat code. If a user types 'bomb' as their choice, then make sure they win, no matter what.








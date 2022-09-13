
author : fabiokrone<br>
mail-id : fabiokrone10@gmail.com<br>
project0 - Tic-Tac-Toe

# Activity: 
Using Minimax, implement an AI to play Tic-Tac-Toe optimally.
<br>
# Introduction
Tic-Tac-Toe is a two player game, X and O, who take turns marking the spaces in a 3x3 grid. Each player takes turns, first X, and then O. The player who succeeds in placing three of their marks in a horizontal, vertical, or diagonal row first wins the game. The game always ends with a win-lose or a draw situation. 
<br>

# Game play
Each player takes turns, first X, and then O. The goal is to get three in a row in a 3x3 board. Each player on their turn can mark only an empty cell with their corresponding mark (X or O). The game ends with a win-lose or a draw situation.
<br>

# Game in Numbers
So, how many Tic-Tac-Toe games are possible? This is a simple question solvable with a little brute force and basic combinatory techniques. It is quite obvious that the answer is towards the south of 9!. Total number of possible games is equal to the sum of the number of games that end on the 5th move, 6th move, 7th move, 8th move and the 9th move. A brief calculation of this sum results in 255,168. These calculations do not take symmetry of the board into consideration. It is also interesting to note that most games end in a draw (always, if both players play optimally).
<br>

# Game Environment
Tic-Tac-Toe is an adversarial environment. Adversarial environment refers to a competitive environment where each player’s goal is to minimize the opponent’s score and thereby maximize their own score. 
<br>
Hence, this game belongs to a class of adversarial search problems where our aim is to find a way (solution) to maximize our score in the presence of an adversary who is planning against us. In particular, Tic-Tac-Toe is a two player environment. It follows turn taking which means actions of a player are taken one followed by the other. Moreover, this game is a zero sum game, meaning, the sum of the utilities (scores) of the players at the end of the game is constant for every game.
<br>

![logo](https://github.com/fabiokrone/images/blob/main/game.png)


# The Minimax Algorithm
Let us call the two players MAX and MIN, for reasons that will soon become obvious. MAX wants to find a sequence of actions leading to a win, but MIN has something to say about it. This means that MAX’s strategy must be a conditional plan—a contingent strategy specifying a response to each of MIN’s possible moves. In games that have a binary outcome (win or lose), we could use AND–OR search (page 125) to generate the conditional plan. Infact, for such games, the definition of a winning strategy for the game is identical to thedefinition of a solution for a nondeterministic planning problem: in both cases the desirableoutcome must be guaranteed no matter what the “other side” does. For games with multiple outcome scores, we need a slightly more general algorithm called minimax search.


# References
Game in Numbers - <i>http://www.se16.info/hgb/tictactoe.htm</i><br>
Peter Norvig & Stuart Russell - Artificial Intelligence : A Modern Approach (4rd edition)<br> 

# UMBC CMSC 471.2 Spring 2021 HW3
### **NAME:** *your name here*
### **UMBC USERNAME:** *your user id here*


## 1. Minimax and Alphabeta

**1.1**  For the [first game tree on the HW3 page](https://www.csee.umbc.edu/courses/undergraduate/471/spring21/02/hw/HW3/mm0.png), use the minimax algorithm to compute a value for each non-leaf node. Squares represent max nodes and circles represent min nodes. Indicate which move the maximizing player should make. Edit game_trees.ppt via powerpoint or google docs and push the .ppt and .pdf versions of the result to your repo.

**1.2** Simulate the alpha-beta algorithm on the [second game tree on the HW3 page](https://www.csee.umbc.edu/courses/undergraduate/471/spring21/02/hw/HW3/mm1.png), crossing out the nodes that are pruned. For each non-leaf node that is not pruned, show the exact value (e.g., =3) or the last constraint (e.g., <= 2, >=8) that the alpha-beta algorithm determines. Edit game_trees.ppt via powerpoint or google docs and push the .ppt and .pdf versions of the result to your repo.


## 2. Game characteristics

For each of the following statements, say whether it is true or false and provide a short (e.g. one paragraph) justification for your answer.

**2.1** Given a two-player, turn-taking, zero-sum, fully observable game between two perfectly rational players, it does not help the first player's outcome to know what strategy the second player is using -- that is, what move the second player will make, given the first player's move.

*...your answer here ...*

**2.2** Given a two-player, turn-taking, zero-sum, partially observable game between two perfectly rational players, it does not help the first player to know what move the second player will make, given the first player's move.

*...your answer here ...*

**2.3** A perfectly rational backgammon-playing agent with unlimited resources never loses.

*...your answer here ...*


## 3. Answer the following questions for the game of NIM.

**3.1** For a NIM game with initial configuration [5,4,3], what is the shortest possible game in terms of plys?

*...your answer here ...*

**3.2** For a Nim game with initial configuration [5,4,3], what is the longest possible game in terms of plys?

*...your answer here ...*

**3.3** For a Nim game with initial configuration [H1, H2, ... Hn] where the Hi values are all positive integers greater than 0 and n is greater than 0, what is the initial branching factor of the game tree, i.e., how many initial moves are there?


**3.3** For a Nim game with initial configuration [H1, H2, ... Hn] where the Hi values are all positive integers greater than 0 and n is greater than 0, what is the shortest possible game in terms of plys?

*...your answer here ...*

**3.4** For a Nim game with initial configuration [H1, H2, ... Hn] where the Hi values are all positive integers greater than 0 and n is greater than 0, what is the longest possible game in terms of plys?

*...your answer here ...*

## 4. Answer the following questions about your Nim program

**4.1** Describe the heuristic you used to compute a static evaluation of a non-terminal game node

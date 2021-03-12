# UMBC CMSC 471.2 Spring 2021 HW3
### **NAME:** Kelly Snyder
### **UMBC USERNAME:** ks16


## 1. Minimax and Alphabeta

**1.1**  For the [first game tree on the HW3 page](https://www.csee.umbc.edu/courses/undergraduate/471/spring21/02/hw/HW3/mm0.png), use the minimax algorithm to compute a value for each non-leaf node. Squares represent max nodes and circles represent min nodes. Indicate which move the maximizing player should make. Edit game_trees.ppt via powerpoint or google docs and push the .ppt and .pdf versions of the result to your repo.

**1.2** Simulate the alpha-beta algorithm on the [second game tree on the HW3 page](https://www.csee.umbc.edu/courses/undergraduate/471/spring21/02/hw/HW3/mm1.png), crossing out the nodes that are pruned. For each non-leaf node that is not pruned, show the exact value (e.g., =3) or the last constraint (e.g., <= 2, >=8) that the alpha-beta algorithm determines. Edit game_trees.ppt via powerpoint or google docs and push the .ppt and .pdf versions of the result to your repo.


## 2. Game characteristics

For each of the following statements, say whether it is true or false and provide a short (e.g. one paragraph) justification for your answer.

**2.1** Given a two-player, turn-taking, zero-sum, fully observable game between two perfectly rational players, it does not help the first player's outcome to know what strategy the second player is using -- that is, what move the second player will make, given the first player's move.

It would be false, because strategy is very important in a game like this. Take chess for example. If you're making the first move in chess, you need to immediately start thinking about what the second player will do based on what piece you move first. So no, it is very important to know what strategy the second player is using, or at least try to figure out what the strategy is as soon as possible.

**2.2** Given a two-player, turn-taking, zero-sum, partially observable game between two perfectly rational players, it does not help the first player to know what move the second player will make, given the first player's move.

Although in this case the game is only partially observable, this is still false. There can still be some elements of strategy in a game that's partially observable, which means that knowing what the second player's would be is still important. The only time where it wouldn't be important to know what move the second player will make is if the game is randomized, which would make it really hard if not impossible to have a strategy.

**2.3** A perfectly rational backgammon-playing agent with unlimited resources never loses.

This is also false. Backgammon game is randomized, due to the game being played via dice rolls. Though if the resources the game are unlimited, the game would never end, as the pieces could keep going back and forth permanently and nothing would really happen. So you wouldn't lose, but you wouldn't win either. 


## 3. Answer the following questions for the game of NIM.

**3.1** For a NIM game with initial configuration [5,4,3], what is the shortest possible game in terms of plys?

If each person took everything from each heap, the shortest game would be three plays, as they would take everything from the first, then the second, and then the third. If this happens the winner will always be whoever makes the first move.

**3.2** For a Nim game with initial configuration [5,4,3], what is the longest possible game in terms of plys?

The longest game with this figuration would be 12 moves, and the second player would always win. This would happen if they took one at a time for each turn.

**3.3** For a Nim game with initial configuration [H1, H2, ... Hn] where the Hi values are all positive integers greater than 0 and n is greater than 0, what is the initial branching factor of the game tree, i.e., how many initial moves are there?

For initial moves there's n inital moves, because if there n heaps, theres a move for each heap.

**3.3** For a Nim game with initial configuration [H1, H2, ... Hn] where the Hi values are all positive integers greater than 0 and n is greater than 0, what is the shortest possible game in terms of plys?

Like the earlier answer, the shortest possible game would be if each heap was taken in its entiriety, since you can only take as much as is in a heap, and can't go to other ones. 

**3.4** For a Nim game with initial configuration [H1, H2, ... Hn] where the Hi values are all positive integers greater than 0 and n is greater than 0, what is the longest possible game in terms of plys?

For here, like a previous answer, the longest game would be if one coin or stick was taken each turn until the game ends, this means you're taking the minimum amount each time, which would result in the longest game.

## 4. Answer the following questions about your Nim program

**4.1** Describe the heuristic you used to compute a static evaluation of a non-terminal game node

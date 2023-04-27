# Tic-Tac-Toe Game Implementation using Multi Agents


![](https://mostafa-samir.github.io/assets/images/ai_tic_tac_toe_header.png)

# Introduction

Tic-tac-toe is a two-player game played on a 3x3 grid. One player plays as "X" and the other player plays as "O". Players take turns placing their symbol in an empty square of the grid. The objective of the game is to get three of your symbols in a row, either horizontally, vertically, or diagonally.
The first player to get three in a row wins the game. If all squares are filled and no player has three in a row, the game is a tie.

# Implementation
   
In this project, we are using a combination of algorithms such as Min-Max algorithm, Alpha-Beta pruning, and Q-learning. The Min-Max algorithm can be used to generate a decision tree that represents all possible moves and outcomes. Alpha-Beta pruning can then be applied to the decision tree to eliminate branches that are unlikely to lead to a winning move. Finally, Q-learning can be used to improve the performance of the AI agents by enabling them to learn from their past experiences.

![](https://courses.cognitiveclass.ai/asset-v1:IBM+GPXX0XENEN+v1+type@asset+block@course_card.png)

In this implementation, the AI agents would play against each other. One agent would use the Min-Max algorithm with Alpha-Beta pruning to make its moves. Another agent would use Q-learning to make its moves. The two agents would play multiple games, and the Q-learning agent would learn from its past experiences to improve its performance over time.

# Objectives

The objective of this project is to Design Adversarial Search Algorithm and Reinforcement Agents to solve Tic Tac Toe game and also to create an intelligent system that can play the game at a high level. The AI agents would learn from their past experiences and improve their performance over time, leading to a more challenging and engaging game.

Design of 3 Artificial Intelligence Agents:

 1.Q learning Technique
 
 2.Min-Max Algorithm
 
 3.Alpha-Beta Pruning

To Play Tic Tac Toe game multiple times among them to find the efficient Algorithm. Also, Comparing the efficiency of three algorithms by calculating the corresponding performance metrics and to find out which performs better either adversarial search or Reinforcement Learning.

Ultimately, the main idea of this project would be to create an intelligent system that can learn and adapt to new challenges, leading to more robust and capable AI systems in the future.

# Approaches
The first step is to implement Q-Learning from Reinforcement Learning. 

The next step is Adversarial Search using the below two algorithms.

           1.Min-Max Algorithm
           
           2.Alpha-Beta Pruning.
           
Technology Stack:
           1.Python

![](https://miro.medium.com/v2/resize:fit:1400/0*WC4l7u90TsKs_eXj.png)


# Brief Description of Agents

# Min-Max Algorithm

In Tic-Tac-Toe, the Min-Max algorithm works by generating a decision tree that represents all possible moves and outcomes, and then recursively evaluating each possible move to determine which one leads to the best outcome for the player.

At each level of the decision tree, the algorithm alternates between maximizing and minimizing the outcome of the game. For example, if the algorithm is trying to find the best move for the "X" player, it will maximize the outcome of the game at each level, assuming that the "O" player will make the best move possible.

The algorithm assigns a score to each outcome, with a higher score indicating a better outcome for the "X" player and a lower score indicating a better outcome for the "O" player. The algorithm then selects the move that leads to the highest score for the "X" player, or the lowest score for the "O" player.

In Tic-Tac-Toe, the algorithm can evaluate all possible moves on the 3x3 grid to determine the best move to make. However, as the game becomes more complex, the number of possible moves increases dramatically, making it difficult for the algorithm to evaluate all possible moves in a reasonable amount of time. That's where techniques like Alpha-Beta pruning and Q-learning come in, to help reduce the search space and make the algorithm more efficient.
  
  ![](https://alialaa.com/static/38d8b0523fa99f139df7564e6def9a61/c58a3/minimax.jpg)

            

# Alpha-Beta 

In Tic-Tac-Toe, Alpha-Beta pruning works by eliminating branches of the decision tree that are unlikely to lead to a better outcome.

During the Min-Max algorithm, Alpha-Beta pruning maintains two values, alpha and beta, which represent the best possible score that the maximizer (e.g. "X" player) can achieve and the best possible score that the minimizer (e.g. "O" player) can achieve, respectively. As the algorithm evaluates each node, it updates these values, and prunes any nodes that will not lead to a better outcome than the already evaluated nodes.

For example, suppose that the algorithm is evaluating a node where the maximizer (e.g. "X" player) has already found a move that leads to a score of 2, and is evaluating a child node that can only lead to a score of 1 or less. Since the minimizer (e.g. "O" player) will never choose a move that leads to a score of 1 or less, the algorithm can prune that branch of the decision tree, and move on to evaluate other nodes.

In Tic-Tac-Toe, Alpha-Beta pruning can significantly reduce the number of nodes that need to be evaluated, especially in situations where the outcome of the game is clear. By reducing the search space, the algorithm can make better use of its computational resources and find the best move more efficiently.

![](https://blog-c7ff.kxcdn.com/blog/wp-content/uploads/2017/03/ttt-minimax.jpg)

         

# Q-Learning   

Q-learning is a type of reinforcement learning algorithm that can be used to teach an AI agent how to play Tic-Tac-Toe. In Q-learning, the AI agent learns by playing multiple games and observing the outcomes of its actions. The agent then updates its "Q-table," which contains values that represent the expected reward for each action in each state of the game.

The Q-table is initially filled with random values, but as the agent plays more games, it updates the values in the table based on the rewards it receives. For example, if the agent makes a move that leads to a win, it will update the Q-table to increase the expected reward for that move in that state of the game. Conversely, if the agent makes a move that leads to a loss, it will decrease the expected reward for that move in that state of the game.

Over time, the AI agent learns which moves are more likely to lead to a win or a loss, and adjusts its behavior accordingly. By continuously updating the Q-table based on its experiences, the AI agent can improve its performance and become a more challenging opponent.

In Tic-Tac-Toe, the AI agent can use the Q-table to decide which move to make in each state of the game. The agent will choose the move that has the highest expected reward in that state, according to the Q-table. As the agent plays more games, the Q-table is updated with better estimates of the expected rewards, and the agent's performance improves.
       
   ![](https://nestedsoftware.com/assets/images/2019-07-25-tic-tac-toe-with-tabular-q-learning-1kdn.139811/4vzn7gq5mil1yerqmtlk.png)
  

 # Deliverables

  a.User Documentation model which gives details about the Tic Tac Toe game implementation using Min-Max, Alpha-Beta and Reinforcement Learning Agents.

  b.Algorithms developed for AI Agents using Python Programming Language(.py files)

  c.Github Repository link for Python code and related files.

  d.Youtube video Demonstrating the project and its implementation using slides 
        
 # Evaluation Methodolgy

When evaluating the performance of AI agents playing Tic-Tac-Toe, there are several metrics that can be used to measure their effectiveness.

Win rate: This measures the percentage of games that the AI agent wins against a specific opponent. The higher the win rate, the better the agent's performance.

Average number of moves per game: This measures the average number of moves that the AI agent takes to win or lose a game. A lower average number of moves indicates that the agent is making more efficient and strategic moves.

Training time: This measures the amount of time it takes for the AI agent to learn how to play Tic-Tac-Toe. A faster training time indicates that the agent is learning more quickly and efficiently.

Performance against different opponents: It is important to test the AI agent's performance against different opponents with varying skill levels. This helps to determine how well the agent can adapt to different playing styles and skill levels.

Human-like behavior: A good AI agent should not only be able to win games but also exhibit human-like behavior, such as making moves that are not just focused on winning but also aimed at blocking the opponent's moves.

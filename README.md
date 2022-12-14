# CSCI E-80 - Introduction to Artificial Intelligence with Python
## My solutions for CS50 Introduction to Artificial Intelligence with Python
<br/>
https://cs50.harvard.edu/extension/ai/2022/spring/
<br/>
I took this course from Harvard Extension School to pursue a graduate certificate in Bioinformatics.

## Course description
This course explores the concepts and algorithms at the foundation of modern artificial intelligence, diving into the ideas that give rise to technologies like game-playing engines, handwriting recognition, and machine translation. Through hands-on projects, students gain exposure to the theory behind graph search algorithms, classification, optimization, reinforcement learning, and other topics in artificial intelligence and machine learning as they incorporate them into their own Python programs. By course’s end, students emerge with experience in libraries for machine learning as well as knowledge of artificial intelligence principles that enable them to design intelligent systems of their own.  
<br/>
*Before viewing my files, I would highly recommend to read about [CS50's Academic Honesty rules](https://cs50.harvard.edu/college/2021/fall/syllabus/#academic-honesty)*.  

<br/>

### [Week 0: Search](https://github.com/julianajlee/cs50-ai/tree/main/week0)
#### Project 1: Degrees

Click [here](https://cdn.cs50.net/ai/2020/spring/projects/0/degrees.zip and unzip it) for the skeleton code.  
<br/>
The **goal** of this project is to find the shortest path between two nodes, by implementing Breadth-First Search (BFS) algorithm. I used a Queue-based frontier to manage the neighbouring nodes that share the same parameter. When you're done, the final result should look like this:  


      $ python degrees.py large
      Loading data...
      Data loaded.
      Name: Emma Watson
      Name: Jennifer Lawrence
      3 degrees of separation.
      1: Emma Watson and Daniel Radcliffe starred in Harry Potter and the Chamber of Secrets
      2: Daniel Radcliffe and James McAvoy starred in Victor Frankenstein
      3: James McAvoy and Jennifer Lawrence starred in Dark Phoenix
      

#### Project 2: Tic-tac-toe  

This one is pretty straight-forward. If you don't know what a tic-tac-toe is, it's a game where you (X or O) have to draw on a 3x3 grid. Whoever makes a drawing in a horizontal, vertical, or diagonal row wins the game.  
<br/>
Click [here](https://cdn.cs50.net/ai/2020/spring/projects/0/tictactoe.zip) for the skeleton code.  
<br/>
The **goal** of this project is to beat the AI and win!  

### [Week 1: Knowledge](/week1)
#### Project 1: Knights
Click [here](https://cdn.cs50.net/ai/2020/spring/projects/1/knights.zip) for the skeleton code.  
<br/>
The **goal** of this project is to solve puzzles using propositional logic (and (∧), or (∨), biconditional (↔)). The basic knowledge for solving this puzzle is that knaves only *lie* and knight only tell the *truth*.    

The end result should look like this:  


      $ python puzzle.py 
      Puzzle 0
          A is a Knave
      Puzzle 1
          A is a Knave
          B is a Knight
      Puzzle 2
          A is a Knave
          B is a Knight
      Puzzle 3
          A is a Knight
          B is a Knave
          C is a Knight


#### Project 2: Minesweeper
Click [here](https://cdn.cs50.net/ai/2020/spring/projects/1/minesweeper.zip) for the skeleton code.  
<br/>
The *goal* of this project is to write an AI that plays minesweeper using propositional logic and inference. In short, each piece of information is a sentence that has sets of cells and the number of mines each set contains. By inference, we can deduct potential cells with a mine by infering the number of shared mines between sets. Don't forget to update the knowledge everytime something new is found!  


### [Week 2: Uncertainty](/week2)
#### Project: Heredity
Click [here](https://cdn.cs50.net/ai/2020/spring/projects/2/heredity.zip) for the skeleton code.
<br/>
The *goal* of this project is to use a bayesian network to make a model that provides inferences on gene trait heredity in a given population. You provide information about people and their heritage, and then AI infers the probability of gene heredity for each person.  
The end result should look like this:  


      $ python heredity.py data/family2.csv 
      Arthur:
        Gene:
          2: 0.0147
          1: 0.0344
          0: 0.9509
        Trait:
          True: 0.0000
          False: 1.0000
      Hermione:
        Gene:
          2: 0.0608
          1: 0.1203
          0: 0.8189
        Trait:
          True: 0.0000
          False: 1.0000
      Molly:
        Gene:
          2: 0.0404
          1: 0.0744
          0: 0.8852
        Trait:
          True: 0.0768
          False: 0.9232
      Ron:
        Gene:
          2: 0.0043
          1: 0.2149
          0: 0.7808
        Trait:
          True: 0.0000
          False: 1.0000
      Rose:
        Gene:
          2: 0.0088
          1: 0.7022
          0: 0.2890
        Trait:
          True: 1.0000
          False: 0.0000



### [Week 3: Optimization](/week3)
#### Project: Crossword
Click [here](https://cdn.cs50.net/ai/2020/spring/projects/3/crossword.zip) for the skeleton code.  
<br/>
The **goal** of this project is to solve a crossword using backtracking search while incoporating and maintaining arc and node consistencies. The end result should look like this:  

      $ python generate.py data/structure1.txt data/words1.txt output.png
      ██████████████
      ███████M████R█
      █INTELLIGENCE█
      █N█████N████S█
      █F██LOGIC███O█
      █E█████M████L█
      █R███SEARCH█V█
      ███████X████E█
      ██████████████

Key is consistency! Make sure the assignment of words to grid variables are consisten in nodes and edges.  


### [Week 4: Learning](/week4)
#### Project 1: Shopping
Click [here](https://cdn.cs50.net/ai/2020/spring/projects/4/shopping.zip) for the skeleton code.
<br/>
THe **goal** of this project is to create an AI that predicts whether online shopping customers will complete their purchases. For this project, nearest-neighbour classifier is used train the AI with given datasets. The end result should look like this:  

      $ python shopping.py shopping.csv
      Correct: 4088
      Incorrect: 844
      True Positive Rate: 41.02%
      True Negative Rate: 90.55%

#### Project 2: Nim
Click [here](https://cdn.cs50.net/ai/2020/spring/projects/4/nim.zip) for the skeleton code.
<br/>
The **goal** of this project is to train a model using Reinforcement Learning. The AI will play against itself, and if it wins it will reward itself but if it loses, it will punish itself. How cruel!  
The key is to use Q-Learning where losing results in -1 and winning results in 1. Recall that Q-learning formula is: Q(s, a) <- old value estimate + alpha * (new value estimate - old value estimate).  The end result should look like this:

      

      $ python play.py
      Playing training game 1
      Playing training game 2
      Playing training game 3
      ...
      Playing training game 9999
      Playing training game 10000
      Done training
      
      Piles:
      Pile 0: 1
      Pile 1: 3
      Pile 2: 5
      Pile 3: 7
      
      Your Turn
      Choose Pile: 1
      Choose Count: 3
      
      Piles:
      Pile 0: 1
      Pile 1: 0
      Pile 2: 5
      Pile 3: 7
      
      AI's Turn
      AI chose to take 7 from pile 3.
      
      Piles:
      Pile 0: 1
      Pile 1: 0
      Pile 2: 5
      Pile 3: 0
      
      Your Turn
      Choose Pile: 2
      Choose Count: 5
      
      Piles:
      Pile 0: 1
      Pile 1: 0
      Pile 2: 0
      Pile 3: 0
      
      AI's Turn
      AI chose to take 1 from pile 0.
      
      GAME OVER
      Winner is Human
      # I actually won here, which never happened to me before
      # But it shows that reinforcement learning is not ideal
      # as the model could not train for ALL possible outcomes



### [Week 5: Neural networks](/week5)
Click [here](https://cdn.cs50.net/ai/2020/x/projects/5/traffic.zip) for the skeleton code.
<br/>
The **goal** of this project is to use provided images to train a neural network that classifies road signs. It mimics convolutional neural network and we build an efficient network using the concept of convolutional and pooling layers. It is recommended to experiment with:  
      - different numbers of convolutional and pooling layers
      - different numbers and sizes of filters for convolutional layers
      - different pool sizes for pooling layers
      - different numbers and sizes of hidden layers
      - dropout  
The final result should look like this:  


    
      $ python traffic.py gtsrb/
      Epoch 1/10
      497/497 [==============================] - 3s 7ms/step - loss: 2.8686 - accuracy: 0.3052 
      Epoch 2/10
      497/497 [==============================] - 4s 7ms/step - loss: 1.1733 - accuracy: 0.6533
      Epoch 3/10
      497/497 [==============================] - 4s 8ms/step - loss: 0.6370 - accuracy: 0.8115
      Epoch 4/10
      497/497 [==============================] - 4s 8ms/step - loss: 0.4136 - accuracy: 0.8793
      Epoch 5/10
      497/497 [==============================] - 4s 8ms/step - loss: 0.2983 - accuracy: 0.9171
      Epoch 6/10
      497/497 [==============================] - 4s 8ms/step - loss: 0.2715 - accuracy: 0.9251
      Epoch 7/10
      497/497 [==============================] - 4s 8ms/step - loss: 0.2239 - accuracy: 0.9393
      Epoch 8/10
      497/497 [==============================] - 4s 8ms/step - loss: 0.1857 - accuracy: 0.9497
      Epoch 9/10
      497/497 [==============================] - 4s 8ms/step - loss: 0.1619 - accuracy: 0.9581
      Epoch 10/10
      497/497 [==============================] - 4s 8ms/step - loss: 0.1507 - accuracy: 0.9604
      331/331 - 1s - loss: 0.1485 - accuracy: 0.9654




### [Week 6: Languages](/week6)
#### [Project 1: Parser](/week6/parser)
Click [here](https://cdn.cs50.net/ai/2020/spring/projects/6/parser.zip) for the skeleton code.  
<br/>
The **goal** of this project is to generate an AI that parses sentences and extract noun phrases. Tip is to deconstruct the sentences into a list of words. Then, build a set of rules that lets us to parse all sentences. The end result should look something like this:  
      
      
      
      $ python parser.py
      Sentence: Holmes sat.
              S
         _____|___
        NP        VP
        |         |
        N         V
        |         |
      holmes     sat

      Noun Phrase Chunks
      holmes


#### [Project 2: Questions](/week6/questions)
Click [here](https://cdn.cs50.net/ai/2020/spring/projects/6/questions.zip) for the skeleton code.
<br/>
The **goal** of this project... is to generate an AI that answers questions. Pretty straight forward, eh? With the given texts, the AI should answer questions based on the concept of Inverse Document Frequency. The end result should look something like this:
      $ python questions.py corpus
      Query: What are the types of supervised learning?
      Types of supervised learning algorithms include Active learning , classification and regression.
      
      $ python questions.py corpus
      Query: When was Python 3.0 released?
      Python 3.0 was released on 3 December 2008.
      
      $ python questions.py corpus
      Query: How do neurons connect in a neural network?
      Neurons of one layer connect only to neurons of the immediately preceding and immediately following layers.
      

<br/>
<br/>
**Good luck!!**

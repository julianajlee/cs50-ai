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

## Table of contents:
### [Week 0: Search](/week0)
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


### Week 4: Learning
### Week 5: Neural networks
### Week 6: Languages

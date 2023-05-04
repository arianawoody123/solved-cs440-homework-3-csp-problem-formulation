Download Link: https://assignmentchef.com/product/solved-cs440-homework-3-csp-problem-formulation
<br>
<strong>Problem 1 . </strong>Write down the CSP problem formulation for the map coloring example covered in class, for a general graph <em>G = (V, E) </em>where each edge ei,i E <em>E </em>is of the form (v<sub>i</sub>, v<sub>i</sub>) for some vi, vj E V with i <em>j. </em>Assume that there are <em>k </em>different colors Ici, … , ckl.

<strong>Problem 2  </strong>Consider the standard Sudoku game on a 9 x 9 grid (look up the game on the Internet if you are not already familiar with it). To fix a coordinate system, let the top-left cell be (i = 1, <em>j </em>= 1) and the bottom-right cell be (i = 9, <em>j </em>= 9), where i is the row number and <em>j </em>is the column number. In a given game instance, some of the numbers are already filled in. To represent this, we use variables vi,j such that vi,j = 0 if a number is not already given at coordinates

(i, <em>j). </em>Otherwise, vi,i is the actual number that is assigned to coordinates (i, <em>j) </em>at the beginning of the game. Translate the problem into a constraint satisfaction problem (CSP). For your solution, you need to provide your choice of variables, the associated domains for each variable, and the constraints. Please provide brief explanation of the meaning of your constraints.

<strong>Problem 3 [20 points]. </strong>Consider the game search tree given in the figure below. MAX

<em>rn             n op q r st u v w</em>

12 2125 2 26 11 144 10 8 9

<ol>

 <li>[8 points] Apply MinMax (minimax) algorithm to the game tree. Write down the intermediate values at the nodes. What is the best sequence of moves at the max node a (a path along the tree)? What is the utility?</li>

 <li>[12 points] Apply MinMax with alpha-beta pruning in left-to-right order. Write down all nodes that are visited in the order they are visited. Here, by “visited”, we mean the first time a node is seen by the algorithm. Whenever truncation is applied, i.e., when part of the tree is skipped, provide the node where this is happening and explain why the truncation is applied. In particular, write down the values of a and 0 at this point.</li>

</ol>

<strong>Problem 4 . </strong>Consider the two-player game described in Figure 1. For the given game, provide answers to the following questions.

<ol>

 <li>[5 points] Draw the complete game tree, using the following conventions:</li>

</ol>

<ul>

 <li>Write each state as <em>(sA, sB) </em>where sA and <em>sB </em>denote the token locations.</li>

 <li>Put each terminal state in a square box and write its game value in a circle.</li>

</ul>




Figure 1: The start position of a simple game. Player A moves first. The two players take turns moving, and each player must move his token to an open adjacent space in <em>either direction. </em>If the opponent occupies an adjacent space, than a player may jump over the opponent to the next open space if any. (For example, if A is on 3 and <strong>B </strong>is on 2, then A may move back to <strong>1.) </strong>The game ends when one player reaches the opposite end. If player A reaches space 4 first, then the value of the game to A is +1; if player B reaches space 1 first, then the value of the game to A is -1.

<ul>

 <li>Put <em>loop states </em>(states that already appear on the path to the root) in double square boxes. Since it is not clear how to assign values to loop states, annotate each with a “?” in a circle.</li>

</ul>

<ol>

 <li>[5 points] Now mark each node with its backed-up MinMax value (also in circle). Explain how you handled the “?” values and why.</li>

 <li>[5 points] Explain why the standard MinMax algorithm would fail on this game tree and briefly sketch how you might fix it, drawing on your answer to (b). Does your modified algorithm give optimal decisions for all games with loops?</li>

 <li>[5 points] This 4-square game can be generalized to n squares for any n &gt; 2. Prove that A wins if n is even and loses if n is odd.</li>

</ol>

<strong>Problem 5. </strong>Game in normal form. Consider the payoff matrix given in the figure. For each entry, the first number is P1’s payoff and the second number if P2’s payoff.

<em>P1</em>1          2         3




<table>

 <tbody>

  <tr>

   <td width="35">1,2</td>

   <td width="35">6,3</td>

   <td width="35">6,3</td>

  </tr>

  <tr>

   <td width="35">4,4</td>

   <td width="35">3,1</td>

   <td width="35">4,7</td>

  </tr>

 </tbody>

</table>




<ol>

 <li>[7 points] Is there a dominant strategy (from 1, 2, 3) for player 1? And player 2 (from a, <em>b)? </em>If the answer is yes for either player, provide the corresponding dominant strategy or strategies. Justify your answer.</li>

 <li>[8 points] Write down all Nash equilibrium(s), if any. Justify your answer.</li>

</ol>

<strong>Problem 6 . </strong>Consider the following sequence of statements, which describe the oper­ation of a security system.

<em>If the system is armed and motion is detected, then the alarm will sound. If the alarm sounds, then </em><em>the system has been armed or there has been a fire. Regardless of whether the system is armed, the </em><em>alarm should go off when there is a fire. Motion is constantly detected.</em>

<ol>

 <li>[6 points] Convert the above statements into a knowledge base using propositional logic.</li>

 <li>[9 points] Using the resolution rule and your knowledge base, derive the following theorem: <em>The </em><em>alarm will sound if and only if the system is armed or there is a fire.</em></li>

</ol>

<strong>Problem 7  </strong>Expectation. Consider tossing a fair coin continuously until you get two consecutive heads, e.g., <strong>HTTTHH. </strong>Let <em>X </em>be the RV representing the number of tosses. In this case <em>X = </em>6. Compute the expectation of <em>X .</em>
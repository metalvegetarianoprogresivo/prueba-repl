# prueba-repl

### Exercises:
* [Cycle Detection](#cycle-Detection)
* [Diagonal Sum](#diagonal-Sum)
* [Round Robin Tournament](#round-robin-tournament)
* [Le Sammy Sequence](#Le-Sammy-Sequence)
  
<br/>
<br/>
  
# Cycle Detection
A [linked list](https://en.wikipedia.org/wiki/Linked_list) is a linear collection of data elements, whose order is not given by their physical placement in memory. Instead, each element points to the next. It is a data structure consisting of a collection of _nodes_ which together represent a sequence. In its most basic form, each _node_ contains: data, and a reference (in other words, a _link_) to the next _node_ in the sequence. 

![linked list](https://user-images.githubusercontent.com/7025727/72859700-5b1cf800-3c8a-11ea-8dc8-3dca1a40a8b3.png)

A linked list is said to contain a cycle if any node is visited more than once while traversing the list.

<p align="center"> 
  <img alt="cycled linked list" src="https://user-images.githubusercontent.com/7025727/72859796-9b7c7600-3c8a-11ea-8576-d0ffab5e8c45.png" width="500px">
</p>

## What you need to do...
1. Create a data structure that will be used for your linked list.
1. Create function that will receive one parameter: 
    * `head` := A _node_ structure/object that is the _head_ of a linked list.
1. Your function must return a boolean denoting whether or not there is a cycle in the list. If there is a cycle, return true; otherwise, return false.

<br/>
<br/>
<br/>

# Diagonal Sum
Given a matrix _F_ of size _n_ by _m_ (where: _m_ >= _n_) filled with integer numbers you can calculate a diagonal sum by summing all of the numbers starting from one of the corners (_a, b, c, d_) in _F_ following a diagonal path until you reach the last number in the diagonal line.

<p align="center"> 
  <img alt="matrix corners" src="https://user-images.githubusercontent.com/7025727/72861516-c1f0e000-3c8f-11ea-94b6-a2e2423c203b.png" width="600px">
</p>

**Example:**
<p align="center"> 
  <img alt="diagonal sum 1" src="https://user-images.githubusercontent.com/7025727/72861810-98848400-3c90-11ea-813e-94678319b53b.png" width="600px">
</p>

In this case we start at corner _c_ of a matrix of size _n=3_ by _m=4_, which has the diagonal numbers: _[3, -7, -3]_. The sum of all these numbers is: _3 + (-7) + (-3) = -7_. 

Our diagonal sum result is **-7**.

**Another Example:**
<p align="center"> 
  <img alt="diagonal sum 2" src="https://user-images.githubusercontent.com/7025727/72862397-a0ddbe80-3c92-11ea-8ddb-f814bff40b60.png" width="600px">
</p>

In this case we start at corner _a_ of a matrix of size _n=3_ by _m=3_, which has the diagonal numbers: _[-4, 8, 7]_. The sum of all these numbers is: _-4 + 8 + 7 = 11_. 

Our diagonal sum result is **11**.

## What you need to do...
1. Create a function named `diagonalSum` that receives two arguments:
    1. `matrix`:= An _Array\[\]\[\]_ of size _n_ by _m_: **_Array\[n\]\[m\]_**.
    1. `corner` := A character that represents the corner (_a, b, c, d_).
1. The function `diagonalSum(matrix, corner)` must return an integer number, the diagonal sum result.

<br/>
<br/>
<br/>

# Round Robin Tournament
A [round-robin tournament](https://en.wikipedia.org/wiki/Round-robin_tournament) (or all-play-all tournament) is a competition in which each contestant meets all other contestants in turn. Also if there are several contestants is common to create groups that runs their own round robin tournament per group.


<p align="center">
  <img alt="Group A" src="https://user-images.githubusercontent.com/7025727/72864608-40527f80-3c9a-11ea-9027-d444a9fb9a37.png" width="600px">
</p>
<p align="center"><em>Example of a round robin tournament: Group A results.</em></p>

<br/>
<br/>

<p align="center">
  <img alt="Group B" src="https://user-images.githubusercontent.com/7025727/72864660-64ae5c00-3c9a-11ea-87eb-816ec91ec444.png" width="600px">
</p>
<p align="center"><em>Example of a round robin tournament: Group B results.</em></p>

A tournament can have _g_ number of groups and each group can have _c_ number of contestants. Not all of the groups will have the same number of contestants, for example _Group C_ (no picture for this group) will have _6_ contestants instead of _5_ which _Group A_ has.

The total number of matches that can happen in a given group is calculated by:

<p align="center">
  <img alt="matches formula" src="https://latex.codecogs.com/png.latex?\dpi{300}&space;\huge&space;\frac{c&space;(c-1)}{2}" width="150px">
</p>

Note that each match has a score, it's not just a win or a lose.

At the end of a round robin tournament (or a group tournament) the sum of all of the scores in which a contestant _T_ participated will be used to determine the final position of the contestant _T_. The contestant with the best score will be placed first, then the second best score and so on.

Example of results:

  <img alt="Group A" src="https://user-images.githubusercontent.com/7025727/72864608-40527f80-3c9a-11ea-9027-d444a9fb9a37.png" width="500px" align="right">
  
  <img alt="Group A positions" src="https://user-images.githubusercontent.com/7025727/72865982-662e5300-3c9f-11ea-9300-0d631b273a5e.png" width="300px">

The sum of the scores in which a particular contestant participated it's shown to the right of the row: 
  
  <img alt="scores" src="https://user-images.githubusercontent.com/7025727/72866392-b8bc3f00-3ca0-11ea-967e-abe14e9ebf05.png" width="200px">

Both numbers represent the score at the end of the tournament, the black number is a minified & rounded version and the grey one is the score without any modification. The grey score is the one that we want and we will call it _final score_.

The _final score_ can be calculated by getting the sum of all scores of the matches in which a contestant participated.

## What you need to do...
1. Design a data structure that can hold the results of all of the groups and matches with the score.
1. Create a function that allows to report a result of a match (score).
1. Create a function that given a contestant name, returns the position and the _final score_ of that contestant.

<br/>
<br/>
<br/>

# Le Sammy Sequence
A [linked list](https://en.wikipedia.org/wiki/Linked_list) is a linear collection of data elements, whose order is not given by their physical placement in memory. Instead, each element points to the next. It is a data structure consisting of a collection of _nodes_ which together represent a sequence. In its most basic form, each _node_ contains: data, and a reference (in other words, a _link_) to the next _node_ in the sequence. 

![linked list](https://user-images.githubusercontent.com/7025727/72859700-5b1cf800-3c8a-11ea-8dc8-3dca1a40a8b3.png)

Given a linked list, the sum of all consecutive nodes that results in a _0_ (zero) will be called _Le Sammy sequence_.

Example of _Le Sammy sequence_:
> 3 -> 4 -> -7 -> 5 -> -6 -> 6

In the above case you should first remove `3 -> 4 -> -7`, then `-6 -> 6`, leaving only `5`.

## What you need to do...
1. Create a function that given a linked list, removes the presence of all _Le Sammy sequence_ (basically removes all the consecutive nodes that sum zero).

<br/>
<br/>
<br/>

# Elo Rating Caculator

The Elo rating system is a method for calculating the relative skill levels of players in zero-sum games such as chess.
We want to create a simple calculation that obtain the new Elo Rating of two players. You should receive data like this:

* Elo Rating of Player A (Ra) = 1200
* Elo Rating of Player B (Rb) = 1000
* Player A Score (Sa) = 0
* Player B Score (Sb) = 1

## Formulas
The formula to obtain the new Elo Rating is:

<p align="center">
  <img alt="matches formula" src="https://latex.codecogs.com/gif.latex?%5Cdpi%7B100%7D%20%5Chuge%20R_%7BA%7D%5E%7B%5Cprime%20%7D%3DR_%7BA%7D&plus;K%28S_%7BA%7D-E_%7BA%7D%29" width="150px">
</p>

* Ra is the Elo Rating of Player A.
* Sa is the Score of player A.
* K is the K-factor.
* Ea is the Expected outcome of player A.

To obtain the value Ea, you should use the next formula:

<p align="center">
  <img alt="matches formula" src="https://latex.codecogs.com/png.latex?\dpi{300}&space;\huge&space;E_{A}={\frac{1}{1+10^{(R_{B}-R_{A})/400}}}" width="150px">
</p>

* Rb is the Elo Rating for Player B.
* Ra is the Elo Rating of Player A.

These formulas are calculated for player A, you should do the same for player B.

## K-factor
These are the values that should be used to calculate the K-factor on the formula based on the Elo Rating of the players.

* Players below 2100: K-factor of 32 used
* Players between 2100 and 2400: K-factor of 24 used
* Players above 2400: K-factor of 16 used.

## What you need to do...
Your implementation should be able to:
* Evaluate the score of player A and player B and which one is considered the winner of the match.
* Return the new Elo Rating of both players.
* Obtain the corresponding K factor.

<br>
<br>
<br>
<br>

# Thank you! 😊

  <img alt="scores" src="https://user-images.githubusercontent.com/7025727/72866668-c45c3580-3ca1-11ea-9e3f-b794fb8b0629.png" width="150px" align="right">

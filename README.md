# prueba-repl

- Index
  * [Cycle Detection](#cycle-Detection)
  * [Diagonal Sum](#diagonal-Sum)
  * [Round Robin Tournament](#round-robin-tournament)
  
<br/>
<br/>
  
# Cycle Detection
A linked list is a linear collection of data elements, whose order is not given by their physical placement in memory. Instead, each element points to the next. It is a data structure consisting of a collection of _nodes_ which together represent a sequence. In its most basic form, each _node_ contains: data, and a reference (in other words, a _link_) to the next _node_ in the sequence. 

![linked list](https://user-images.githubusercontent.com/7025727/72859700-5b1cf800-3c8a-11ea-8dc8-3dca1a40a8b3.png)

A linked list is said to contain a cycle if any node is visited more than once while traversing the list.

<p align="center"> 
  <img alt="cycled linked list" src="https://user-images.githubusercontent.com/7025727/72859796-9b7c7600-3c8a-11ea-8576-d0ffab5e8c45.png" width="500px">
</p>

## What you need to do...
1. Create a data structure that will be used for your linked list.
1. Create function that will receive one parameter: a pointer to a _node_ object named _head_ that points to the head of a linked list. Your function must return a boolean denoting whether or not there is a cycle in the list. If there is a cycle, return true; otherwise, return false.

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

In this case we start at corner _c_ of a matrix of size _n=3_ by _m=4_, which has the diagonal numbers: _[3, -7, -3]_. So we sum all the numbers: _3 + (-7) + (-3) = -7_. 

Our diagonal sum is **-7**.

**Another Example:**
<p align="center"> 
  <img alt="diagonal sum 2" src="https://user-images.githubusercontent.com/7025727/72862397-a0ddbe80-3c92-11ea-8ddb-f814bff40b60.png" width="600px">
</p>

In this case we start at corner _a_ of a matrix of size _n=3_ by _m=3_, which has the diagonal numbers: _[-4, 8, 7]_. So we sum all the numbers: _-4 + 8 + 7 = 11_. 

Our diagonal sum is **11**.

## What you need to do...
1. Create a function named `diagonalSum` that receives two arguments:
    1. `matrix`:= An _Array\[\]\[\]_ of size _n_ by _m_: **_Array\[n\]\[m\]_**.
    1. `corner` := A character that represents the corner (_a, b, c, d_).
1. The function `diagonalSum(matrix, corner)` must return an integer number of the diagonal sum represented by the arguments passed during the call of that function.

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

A tournament can have _g_ number of groups and each group can have _c_ number of contestants. Not all of the groups will have the same number of contestants, for example _Group C_ (no picture for this example) will have _6_ contestants instead of _5_ which _Group A_ has.

The total number of matches that can happen in a given group is calculated by:

<p align="center">
  <img alt="matches formula" src="http://www.sciweavers.org/tex2img.php?eq=%5Cfrac%7Bc%20%28c%20-%201%29%7D%7B2%7D%20&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0">
</p>

Note that each match has a score, it´s not just a win or a lose.

At the end of a round robin tournament (or a group torunament) the sum of all of the scores in which a contestant _T_ participated will be used determine a winner. The contestant with the best score will be placed first, then the second best score and so on.

Example of results:

  <img alt="Group A" src="https://user-images.githubusercontent.com/7025727/72864608-40527f80-3c9a-11ea-9027-d444a9fb9a37.png" width="500px" align="right">
  
  <img alt="Group A positions" src="https://user-images.githubusercontent.com/7025727/72865982-662e5300-3c9f-11ea-9300-0d631b273a5e.png" width="300px">

The results of a match appears on the right of the row: 
  
  <img alt="scores" src="https://user-images.githubusercontent.com/7025727/72866392-b8bc3f00-3ca0-11ea-967e-abe14e9ebf05.png" width="200px">

Both numbers represent the score at the end of the tournament, the black number is a minified & rounded version and the grey one is the score without any modification. The grey score is the one that we want and we will call it _final score_.

The _final score_ can be calculated by getting the sum of all of scores of the matches in which a contestants participated.

## What you need to do...
1. Design a data structure that can hold the results of all of the groups and matches with the score.
1. Create a function that allows to report a match score.
1. Create a function that given a contestant name it will give you the the position and the _final score_.

<br/>
<br/>
<br/>
<br/>

# Thank you! 😊

  <img alt="scores" src="https://user-images.githubusercontent.com/7025727/72866668-c45c3580-3ca1-11ea-9e3f-b794fb8b0629.png" width="150px" align="right">

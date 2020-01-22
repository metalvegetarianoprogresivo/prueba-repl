# prueba-repl

- Index
  1. [Cycle Detection](#cycle-Detection)
  1. [Diagonal Sum](#diagonal-Sum)
  1. 
  
  
# Cycle Detection
A linked list is a linear collection of data elements, whose order is not given by their physical placement in memory. Instead, each element points to the next. It is a data structure consisting of a collection of _nodes_ which together represent a sequence. In its most basic form, each _node_ contains: data, and a reference (in other words, a _link_) to the next _node_ in the sequence. 

![linked list](https://user-images.githubusercontent.com/7025727/72859700-5b1cf800-3c8a-11ea-8dc8-3dca1a40a8b3.png)

A linked list is said to contain a cycle if any node is visited more than once while traversing the list.

![cycled linked list](https://user-images.githubusercontent.com/7025727/72859796-9b7c7600-3c8a-11ea-8576-d0ffab5e8c45.png)

## What you need to do...
1. Create a data structure that will be used for your linked list.
1. Create function that will receive one parameter: a pointer to a _node_ object named _head_ that points to the head of a linked list. Your function must return a boolean denoting whether or not there is a cycle in the list. If there is a cycle, return true; otherwise, return false.

# Diagonal Sum
Given a matrix _F_ of size _n_ by _m_ (where: _m_ >= _n_) filled with integer numbers you can calculate a diagonal sum by summing all of the numbers starting from one of the corners (_a, b, c, d_) in _F_ following a diagonal path until you reach the last number in the diagonal line.

![matrix corners](https://user-images.githubusercontent.com/7025727/72861516-c1f0e000-3c8f-11ea-94b6-a2e2423c203b.png)

**Example:**
![diagonal sum 1](https://user-images.githubusercontent.com/7025727/72861810-98848400-3c90-11ea-813e-94678319b53b.png)

In this case we start at corner _c_ of a matrix of size _n=3_ by _m=4_, which has the diagonal numbers: _[3, -7, -3]_. So we sum all the numbers: _3 + (-7) + (-3) = -7_. 

Our diagonal sum is **-7**.

**Another Example:**
![diagonal sum 2](https://user-images.githubusercontent.com/7025727/72862397-a0ddbe80-3c92-11ea-8ddb-f814bff40b60.png)

In this case we start at corner _a_ of a matrix of size _n=3_ by _m=3_, which has the diagonal numbers: _[-4, 8, 7]_. So we sum all the numbers: _-4 + 8 + 7 = 11_. 

Our diagonal sum is **11**.

## What you need to do...
1. Create a function named `diagonalSum` that receives two arguments:
    1. `matrix`:= An _Array\[\]\[\]_ of size _n_ by _m_: **_Array\[n\]\[m\]_**
    1. `corner` := A character that represents the corner (_a, b, c, d_).
1. The function `diagonalSum(matrix, corner)` must return an integer number of the diagonal sum represented by the arguments passed during the call of that function.




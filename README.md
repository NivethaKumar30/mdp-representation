NAME : NIVETHA .K

REG NO: 212222230102

# MDP REPRESENTATION

## AIM:
To represent a Markov Decision Process(MDP) problem in the following ways:

Text representation

Graphical representation

Python - Dictonary representation

## PROBLEM STATEMENT:

A toddler is learning to walk. The toddler starts out by crawling, and then eventually learns to stand up and walk. The toddler must learn to balance itself and take steps, while also avoiding obstacles.

### Problem Description
The toddler has to reach the goal state(moving forward to target) by taking the correct step towards the goal without hitting any obstacles or losing balance. After reaching the goal the toddler will be rewarded if not then no reward will be provided.

State Space :

{S,B,G,O}->{0,1,2,3
```
0-> Starting point (S)
  
1-> Balanced walking (B)
  
2-> Targeted point (G)

3-> Dashed onto obstacle (O)
```
### Sample State

B-> 1-> Balanced walking

### Action Space

{W,C}->{1,2}

W-> Walking

C-> Crawling

### Sample Action

W-> 1-> Walking

C-> 2-> Crawling

### Reward Function
```
R =
{
    +1, if : the toddler comes to the targeted point
    0, else : no reward
}
```

### Graphical Representation
Write your answer here

## PYTHON REPRESENTATION:

```
Toddler =
{ 
    # Starting point state (S) -> 0
    # Action: Walking (W) -> 1, Crawling (C) -> 2

  0:
  {

     1:[(0.82 , 1 , 0,False),(0.18 , 0 , 0 , False)],
     2:[(0.88 , 0 , 0,False),(0.12 , 1 , 0 , False)]

  },

    # Balanced walking state (B) -> 1

  1:
  {
     1:[(0.91 , 2 , 0,False),(0.09 , 0 , 0 , False)],
     2:[(0.75 , 0 , 0,False),(0.25 , 2 , 0 , False)]

  },

    # Targeted point state (G) -> 2

  2:
  {

      1:[(0.92 , 3 , 1,True),(0.08 , 1 , 0 , False)],
      2:[(0.91 , 1 , 0,False),(0.09 , 3 , 1 , True)]

  },

    # Dashed onto obstacle state (O) -> 3

  3:
  {

      1:[(0.82, 3 , 0, True),(0.18 , 2 , 0 , False)],
      2:[(0.73, 2 , 0, False),(0.27 , 3 , 0 , True)]

  }

}

Toddler
```

## OUTPUT:

![image](https://github.com/NivethaKumar30/mdp-representation/assets/119559844/157c30a4-976b-4472-b016-45c7b941ebbf)


## RESULT:

Thus, to represent a Markov Decision Process (MDP) problem in the representation of text, graphical and also by python program by displaying an appropriate dictionary for the above mentioned problem is implemented and executed successfully.


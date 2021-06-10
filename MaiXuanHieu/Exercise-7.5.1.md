**a) We do not care which specific objects are in the queue. Consequently, there are really just four useful values for the variable elements. What are they?**

- [null, null]
- [object, null]
- [null, object]
- [object, object]

**b) How many states are there? **
```
Element*size*front*back = number of states.
=> Number of states = 4*3*2*2 = 48 states
```

**c) How many of these states are reachable ?**

The 4 element values is reachable => 4 states reachable.

**d) Show the reachable states in a drawing.**

**e) Add edges for the enQueue() and deQueue() methods. (For this assignment, ignore the exceptional returns, although you should observe that when exceptional returns are taken, none of the instance variables are modified.)**

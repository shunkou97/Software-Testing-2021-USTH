### *Question*
Graph defined by the following sets:
- N = {1, 2, 3, 4, 5, 6, 7}
- N0 = {1}
- Nf = {7}
- E = {(1, 2), (1, 7), (2, 3), (2, 4), (3, 2), (4, 5), (4, 6), (5, 6), (6, 1)}

Also consider the following (candidate) test paths:
- p1 = [1, 2, 4, 5, 6, 1, 7]
- p2 = [1, 2, 3, 2, 4, 6, 1, 7]
- p3 = [1, 2, 3, 2, 4, 5, 6, 1, 7]

### *Solution*
**a) Draw the graph**:

**b) List the test requirements for Edge-Pair Coverage**:
```
[1,2,4], [1,7], [2,4,6], [4,6,1], [6,1,7], [2,4,5]
[4,5,6], [5,6,1], [1,2,3], [2,3,2], [3,2,3], [3,2,4].
```
**c) Does the given set of test paths satisfy Edge-Pair Coverage? If not, state what is missing.**

No, the set doesn't satisfy Edge-Pair Coverage:
```
p1 miss (2,3,2) and (2,4,6).
p2 miss (2,4,5) and (4,5,6).
p3 miss (4,6,1) and (2,4,6).
```
**d) Consider the simple path [3, 2, 4, 5, 6] and test path [1, 2, 3, 2, 4, 6, 1, 2, 4, 5, 6, 1, 7]. Does the test path tour the simple path directly? With a sidetrip? If so, write down the sidetrip.**

Not directly but with a sidetrip [4, 6, 1, 2, 4].

**e) List the test requirements for Node Coverage, Edge Coverage, and Prime Path Coverage on the graph.**

*Node Coverage:*
```
{1,2,3,4,5,6,7}
```
*Edge Coverage:*
```
[1,2] [1,7] [2,3] [2,4] [3,2] [4,5] [4,6] [5,6] [6,1]
```
*Prime Path Coverage:*
```
[3, 2, 4, 5, 6, 1, 7], [4, 6, 1, 2, 4], [4, 5, 6, 1, 2, 4], [4, 6, 1, 2, 3]
[4, 5, 6, 1, 2, 3], [5, 6, 1, 2, 4, 5], [6, 1, 2, 4, 6], [1, 2, 4, 5, 6, 1]
[1, 2, 4, 6, 1], [2, 4, 6, 1, 2], [2, 4, 5, 6, 1, 2], [3, 2, 4, 6, 1, 7], [6, 1, 2, 4, 5, 6]
[3, 2, 3], [2, 3, 2]
```
**f) List test paths from the given set that achieve Node Coverage but not Edge Coverage on the graph.**
```
[1, 2, 3, 2, 4, 5, 6, 1, 7]
```
**g) List test paths from the given set that achieve Edge Coverage but not Prime Path Coverage on the graph.**
```
[1, 2, 3, 2, 4, 6, 1, 7], [1, 2, 4, 5, 6, 1, 7]
```

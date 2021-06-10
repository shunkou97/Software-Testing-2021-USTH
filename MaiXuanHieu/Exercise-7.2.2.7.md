### Question
The graph defined by the following sets:
```
N = {1, 2, 3}
N0 = {1}
Nf = {3}
E = {(1, 2), (1, 3), (2, 1), (2, 3), (3, 1)}
```
Also consider the following (candidate) paths:
```
p1 = [1, 2, 3, 1]
p2 = [1, 3, 1, 2, 3]
p3 = [1, 2, 3, 1, 2, 1, 3]
p4 = [2, 3, 1, 3]
p5 = [1, 2, 3, 2, 3]
```
### Solution

**a) Which of the listed paths are test paths? For any path that is not a test path, explain why not.**
```
p1 doesn't end at 3 => not test path.
p4 doesn't start at 1 => not test path.
p5 can't go to 2 from 3 directly => not test path.
```
*Conclusion: **p2 and p3 are test paths.***

**b) List the eight test requirements for Edge-Pair Coverage (only the length two subpaths).**
```
[1,2,1], [2,3,1], [2,1,3], [1,3,1]
[2,1,2], [3,1,3], [3,1,2], [1,2,3]
```
**c) Does the set of test paths from part (a) above satisfy Edge-Pair Coverage? If not, state what is missing.**

No, because p2 and p3 tour [2, 1, 2] or [3, 1, 3].

**d) Consider the prime path [3, 1, 3] and path p2. Does p2 tour the prime path directly? With a sidetrip?**

p3 doesn't tour [3, 1, 3] directly, but it does tour [3, 1, 3] with sidetrip [1, 2, 1].

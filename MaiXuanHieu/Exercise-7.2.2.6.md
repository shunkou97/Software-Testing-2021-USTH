**a) List the test requirements for Node Coverage, Edge Coverage, and Prime Path Coverage on the graph.**

*Node Coverage:*
```
{1, 2, 3, 4, 5, 6, 7, 8, 9, 10}
```
*Edge Coverage:*
```
[1,4], [1,5], [2,5], [2,6], [3,6], [3,7], [4,8], [5,8], [5,9], [6,9], [6,10], [7,10]
```
*Prime Path Coverage:*
```
[1, 4, 8], [1, 5, 8], [1, 5, 9, 6, 2], [1, 5, 9, 6, 10], [2, 5, 9, 6, 2], [2, 5, 9, 6, 10], [3, 6, 2, 5, 8]
[3, 6, 2, 5, 9], [3, 6, 10], [3, 7, 10], [5, 9, 6, 2, 5], [6, 2, 5, 9, 6], [9, 6, 2, 5, 8], [9, 6, 2, 5, 9]

```
**b) List test paths that achieve Node Coverage but not Edge Coverage on the graph.**
```
[1, 4, 8], [1, 5, 8], [2, 5, 9], [3, 6, 10], [3, 7, 10]
```
**c) List test paths that achieve Edge Coverage but not Prime Path Coverage on the graph.**
```
[2, 6, 9]
```

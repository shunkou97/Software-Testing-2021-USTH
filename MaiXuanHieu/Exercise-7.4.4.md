### Given two methods:
```js
 1 public void trash (int x) 
 2 {
 3  int m, n; 
 4 
 5    m = 0;
 6     if (x > 0)
 7     m = 4;
 8    if (x > 5)
 9          n = 3*m;
 10   else 
 11       n = 4*m; 
 12 int o = takeOut (m, n);
 13  System.out.println ("o is: " + o);
 14 }
 15 public int takeOut (int a, int b)
 16 {
 17 int d, e;
 18 
 19   d = 42*a;
 20   if(a > 0)
 21      e = 2*b+d;
 22  else
 23       e = b+d;
 24  return (e);
 25 }
 ```
 **a) Give all call sites using the line numbers given.**
 ```
 m : line 3, 5, 7, 9, 11, 12.
 n : line 3, 9, 11, 12.
 ```
 **b) Give all pairs of last-defs and first-uses.**
 
 *Last-def:*
 ```
 m: line 7
 n: line 11
 ```
 *First-use:*
 ```
 m: line 9
 n: line 21
 ```
 **c) Provide test inputs that satisfy all-coupling-uses (note that trash() only has one input).**
```
x = 0
x = 1
x = 6
```
 

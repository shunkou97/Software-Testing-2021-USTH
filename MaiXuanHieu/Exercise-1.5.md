Ex1.5

1) Find last index of element
	
a) The program will not check the first value in the array because the condition for loop is wrong.

Modification:

	for(int i = x.length-1; i >= 0; i--)
	
b) Test case:

	test : x = null, y = 2
	
Because x is null the program will execute NullPointerException right off the bat.

c) Test case:

	test : x = [2, 3, 5]; y = 3; Expected = 1
	
Not result in an error state because 3 is in index 1 of the array.

d) Test case:

	test : x = [2, 3, 5]; y = 4; Expected = -1
	
Result in an error, but not a failure because 4 is not in the array.

e) Test case:

	x = [2, 3, 5]; y = 2; Expected = 0 
	
Actual = -1

Complete state is after the execute of i-- but right before return -1;.

2) Find last index of zero

a) The intention is to return the last index of 0 in x, but the program will return the first 0 found.

Modification:

	for(int i = x.length-1; i >= 0; i--)
	
b) Test case:

	test : x = [0, 1, 2]; Expected = 0
	
c) Test case:

	test : x is empty
	
d) Test case:

	test : [0, 0, 0]; Expected = 0

3) Count positive element

a) According to the program, it will takes 0 as a positive value.

Modification:

	if(x[i] > 0)

b) Test case:

	test : x = null
	
c) Test case:

	test : x = [-4, 2, 2, 2]
	
e) Test case:

	x = [-4, 2, 0, 2]; Expected = 2
	
Actual = 3

Complete state is after execution of i++ but right before the count++.

4) Count odd or positive element:

a) According to the program, it will takes 0 as a positive value.

Modification: 

	if(x[i] > 0)
	{
  	 count++;
	}
	else
	{
  	if (x[i]%2 ==1 ) 
	 count++;
	}

b) Test case:

	test: x = null

c) Test case:

	test: x = [1, 2, 3, 4, 5]

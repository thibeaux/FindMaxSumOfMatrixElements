# FindMaxSumOfMatrixElements
This program takes a 6x6 matrix of numbers and finds and hourglasses or "I" shapes in the matrix and adds all of the elements contained in the "I" shape together. After going through all of the possible "I" shapes contained in the matrix, the program prints the max sum result. Disclaimer, this is a challenge I found on hackerrank, but I really enjoyed working this challenge out so I'd like to post my submission here.

# Example
```
Input:
1 1 1 0 0 0
0 1 0 0 0 0
1 1 1 0 0 0
0 0 2 4 4 0
0 0 0 2 0 0
0 0 1 2 4 0
```
```
output:
19
```

You can use the printHourGlass function to see the possible hourglasses contained in the matrix. It will look like this:
```
1 1 1
  1     = 1+1+1+1+1+1+1 = 7 
1 1 1
```
```
2 4 4
  2     = 2 + 4 + 4 + 2 + 1 +2 + 4 = 19 Here is your max
1 2 4
```

You can uncomment out the debugging lines to see what is going on internally. 

# What did I learn?
I learned alot from this challenge. I got to familiarize myself more with 2D arrays/vectors in c++ and I got to learn how to use the data in a matrix to form results and I got to learn how to form and recognize patterns within a matrix using 2D vectors. Up until now the only experience I had with programming with matrices was in matlabs. I can see how skills like this could be used to potentially find the determinant of a matrix or even the symmetry of a matrix or something similar to these pattern finding ideas.

# Challenges
The challenges I faced were trying to find a good and consistent way of of identifying the "I" shaped pattern. I was trying to not overload my functions with code, so I was trying different ways of tackling the problem. One was visualizing the I shape patterns first and then add them up after so I can confirm what was being done was correct. I also didn't want unexpected problems to arise later on in the challenge so I tried had to dial in the hourglass print function. Once that was working perfectly I created the FindMax function.

So in short I overcame the problem by implementing a two step strategy, 1.) identify and print the hourglasses contained in the matrix 2.) add the elements of each hourglass up and test if it is greater than the max varible. 

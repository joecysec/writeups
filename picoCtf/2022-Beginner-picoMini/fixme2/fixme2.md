<<<<<<< HEAD
## fixme2
25 points
## Category
General Skills
## Description
=======
## fixme2 (General Skills, 25 points)
>>>>>>> 06214870d66d238c22488aad8ee395cb58a6d9db
Fix the syntax error in the Python script to print the flag.

## Solution
In this challenge we are given a Python script, lets start by opening the script in an IDE.

![line22](https://i.imgur.com/DAkQTv1.png)

We are looking for a syntax error and on line 22 we find a syntax error. In this case, if flag = "": we can see that in an if statement equals is represented by == instead of the singular =. 

The solution is if flag == "":

Now all that is left to is run the script to capture the flag:
<<<<<<< HEAD
## Flag
=======
>>>>>>> 06214870d66d238c22488aad8ee395cb58a6d9db
```
picoCTF{3qu4l1ty_n0t_4551gnm3nt_b4d595d9}
```

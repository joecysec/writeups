## fixme2 (General Skills, 25 points)
### Description
Fix the syntax error in the Python script to print the flag.

In this challenge we are given a Python script, lets start by opening the script in an IDE.

![](https://imgur.com/a/CMxk1BP)

We are looking for a syntax error and on line 22 we find a syntax error. In this case, if flag = "": we can see that in an if statement equals is represented by == instead of the singular =. 

The solution is if flag == "":

Now all that is left to is run the script to capture the flag.
```
picoCTF{3qu4l1ty_n0t_4551gnm3nt_b4d595d9}
```

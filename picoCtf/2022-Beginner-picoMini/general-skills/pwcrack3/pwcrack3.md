## PW Crack 3
75 points
## Description
Can you crack the password to get the flag? <br/>
Download the password checker [here](https://artifacts.picoctf.net/c/28/level3.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/28/level3.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/28/level3.hash.bin) in the same directory too. <br/>
There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.
## Solution
Place the 3 files provided in an IDE in the same directory. Upon examing the script,
 we find that there are 7 passwords located on line 44: 
```
pos_pw_list = ["f7f3", "4aa2", "8e1d", "2266", "7243", "9f43", "f634"]
```
When we run the script, we are asked to enter the correct password for the flag. We need to brute force the passwords until
we enter in the right password (f634) to reveal the flag.
## Flag
```
picoCTF{m45h_fl1ng1ng_64840799}
```
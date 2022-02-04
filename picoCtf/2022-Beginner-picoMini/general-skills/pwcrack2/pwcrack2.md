## PW Crack 2
35 points
## Description
Can you crack the password to get the flag?
Download the password checker [here](https://artifacts.picoctf.net/c/19/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/19/level2.flag.txt.enc) in the same directory too.
## Solution
Download the password checker and the encrypted flag files. Place the files in an IDE in the same directory. Upon examining the level2.py file, we can see that on line 18 if the user password is equal to "chr(0x35) + chr(0x39) + chr(0x30) + chr(0x39)", then the flag will be decrypted. 

![line18](https://i.imgur.com/eUUMrgM.png)

The password is in ASCII format, convert it by printing the ASCII characters in a Python file and running it in the IDE. It should look like "print(chr(0x35) + chr(0x39) + chr(0x30) + chr(0x39))"
This outputs "5909". Now we need to run the password checker (level2.py) and entering "5909" as the input to get the flag.
## Flag
```
picoCTF{tr45h_51ng1ng_b0539d96}
```
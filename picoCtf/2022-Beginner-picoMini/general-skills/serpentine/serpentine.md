## Serpentine
50 points
## Description 
Find the flag in the Python script! <br/>
[Download Python script](https://artifacts.picoctf.net/c/97/serpentine.py)
## Solution
Open the Python script in an IDE and run the script. The script outputs three options, <br/>
<br/>
a) Print encouragement <br/>
b) Print flag <br/>
c) Quit <br/>
<br/>

The script asks to input a character a, b, or c. Upon inputting b, the script outputs:
 Oops! I must have misplaced the print_flag function! Check my source code!
 Upon examining the source code we find that the script did not call to the print_flag() method correctly on lines 68-69.
Simply replace 
```
print('\nOops! I must have misplaced the print_flag function! Check my source code!\n\n')
```
with
```
print_flag()
```
then run the script again and enter in b for the input to capture the flag.
## Flag
```
picoCTF{7h3_r04d_l355_7r4v3l3d_ae743140}
```
## Glitch Cat
30 points
## Description
Our flag printing service has started glitching!
$ nc saturn.picoctf.net 50562
## Solution
Enter the command $ nc saturn.picoctf.net 50562 into the picoCTF Webshell. Which yields:
'picoCTF{gl17ch_m3_n07_' + chr(0x38) + chr(0x39) + chr(0x38) + chr(0x61) + chr(0x33) + chr(0x66) + chr(0x61) + chr(0x36) + '}'
Create a new python file and create a print statement printing "chr(0x38) + chr(0x39)........... + chr(0x36)". It should look like this: 
print(chr(0x38) + chr(0x39) + chr(0x38) + chr(0x61) + chr(0x33) + chr(0x66) + chr(0x61) + chr(0x36)). Run the Python script which outputs: "898a3fa6".
Now add it back into the original flag before the printing glitch to get the completed flag.
## Flag
picoCTF{gl17ch_m3_n07_898a3fa6}

# basic-mod1
#### Description
We found this weird message being passed around on the servers, we think we have a working decryption scheme.
Download the message [here](https://artifacts.picoctf.net/c/395/message.txt)
Take each number mod 37 and map it to the following character set: 0-25 is the alphabet 
(uppercase), 26-35 are the decimal digits, and 36 is an underscore. 
Wrap your decrypted message in the picoCTF flag format (i.e. picoCTF{decrypted_message})
### hint
1. Do you know what mod 37 means?
2. mod 37 means modulo 37. It gives the remainder of a number after being divided by 37.
### Solution
As given in the hint all the numbers in the file is first made into a list.Then each number is moduled with 37 and appended to a list. Now each value in the list is run through a loop with different if condition according to the cases given in the description and is addeinto a new sting and the end result is enclosed in picoCTF{decrypted_message}
### Flag
the flag is: picoCTF{R0UND_N_R0UND_ADD17EC2}

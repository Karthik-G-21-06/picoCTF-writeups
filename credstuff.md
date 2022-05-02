# credstuff
### description
We found a leak of a blackmarket website's login credentials. Can you find the password of the user "cultiris" and successfully decrypt it?
dowload the leak [here](https://artifacts.picoctf.net/c/534/leak.tar)
The first user in usernames.txt corresponds to the first password in passwords.txt. The second user corresponds to the second password, and so on.
### hint
1. Maybe other passwords will have hints about the leak?
### solution
Firstly the zip file should be unzipped we will get two files usernames.txt and passwords.txt. Now using file manupulation,i.e., opening the file in read mode, in python traverse through the usernams.txt  using for loop to find "cultiris" and get the index. Since the password is in corresponding position as the username print the string in the index from the passwords.txt opened in read mode.
Now the output will be "cvpbPGS{P7e1S_54I35_71Z3}".If u check this output with the start of flag "picoCTF{" it is clearly understood that the output is encrypted.The difference in the correspondint letters ascii value is 13. Now decrypt by adding shifting the ascii value by 13 forward if it is furthur than 13th position or backword fi it is behind 13th position
### flag
the flag is : picoCTF{C7r1F_54V35_71M3}

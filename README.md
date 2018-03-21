---------------------------------------------------      Welcome to Md5 Hash Cracker     ---------------------------------------------------

You can crack the 32 char md5 hashes with this program. Please follow the instructions to use the program.

--------------------------------------------------------------------------------------------------------------------------------------------------

1) .\md5HashCracker.ps1 -help h

User can use this command to get informations about how to use. This command will show you parameters and some
usage examples.

--------------------------------------------------------------------------------------------------------------------------------------------------

2) .\md5HashCracker.ps1 -crackType single -Wordlist <path of wordlist file> -inputArgument <hash>

User should use this command if he/she has just 1 hash to crack.

-crackType argument will be 'single'
-Wordlist argument will be the path of wordlist.txt that contains words.
-inputArgument argument will be that hash.

You can download and use inputWordList.txt for demo .

--------------------------------------------------------------------------------------------------------------------------------------------------

3) .\md5HashCracker.ps1 -crackType plural -Wordlist <path of wordlist file> -inputArgument <path of hashlist>

User should use this command if he/she has more than 1 hashes  to crack.

-crackType argument will be 'plural'
-Wordlist argument will be the path of wordlist.txt that contains words.
-inputArgument argument will be the path of hashlist.txt that contains hashes that he/she wants to crack.

You can download and use inputWordList.txt and inputHashList.txt for demo.

--------------------------------------------------------------------------------------------------------------------------------------------------


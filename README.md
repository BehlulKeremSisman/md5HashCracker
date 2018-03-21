                                           Welcome to Md5 Hash Cracker 
                                          
----------------------------------------------------------------------------------------------------------------------

You can crack the 32 char md5 hashes with this program. Please follow the instructions to use the program.

Program will produce you a 'Report.txt' report file. And you will see the results from powershell terminal too.

**How it works ? (Algorithm):** Input hash will be compared to each word's md5 hash. If they matches the word will
be the answer for crack. If not that means crack could not be done. Input md5 hash should be 32 characters. So there is
a control about length of it.

----------------------------------------------------------------------------------------------------------------------

**1) ./md5HashCracker.ps1 -help h**

User can use this command to get informations about how to use. This command will show you parameters and some
usage examples.

**Example Usage --> ./md5HashCracker.ps1 -help h**

Demo screenshot: ![alt text](https://github.com/BehlulKeremSisman/md5HashCracker/blob/master/help.png)


----------------------------------------------------------------------------------------------------------------------

**2) ./md5HashCracker.ps1 -crackType single -Wordlist <path of wordlist file> -inputArgument <hash>**

User should use this command if he/she has just 1 hash to crack.

[-crackType] argument will be 'single'

[-Wordlist] argument will be the path of wordlist.txt that contains words.

[-inputArgument] argument will be that hash.

You can download and use inputWordList.txt for demo.

**Example Usage --> ./md5HashCracker.ps1 -crackType single -Wordlist C:\Users\decoder\Desktop\inputWordList.txt -inputArgument 900150983cd24fb0d6963f7d28e17f72**

Demo screenshot: ![alt text](https://github.com/BehlulKeremSisman/md5HashCracker/blob/master/single.png)

----------------------------------------------------------------------------------------------------------------------

**3) ./md5HashCracker.ps1 -crackType plural -Wordlist <path of wordlist file> -inputArgument <path of hashlist>**

User should use this command if he/she has more than 1 hashes  to crack.

[-crackType] argument will be 'plural'

[-Wordlist] argument will be the path of wordlist.txt that contains words.

[-inputArgument] argument will be the path of hashlist.txt that contains hashes that he/she wants to crack.

You can download and use inputWordList.txt and inputHashList.txt for demo.

**Example Usage --> ./md5HashCracker.ps1 -crackType plural -Wordlist C:\Users\decoder\Desktop\inputWordList.txt -inputArgument C:\Users\decoder\Desktop\inputHashList.txt**

Demo screenshot: ![alt text](https://github.com/BehlulKeremSisman/md5HashCracker/blob/master/plural.png)

----------------------------------------------------------------------------------------------------------------------



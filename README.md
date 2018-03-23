                                           Welcome to Md5 Hash Cracker 
                                          
----------------------------------------------------------------------------------------------------------------------

You can crack the 32 char md5 hashes with this program. Please follow the instructions to use the program and see the details.

**How it works ? (Algorithm):** Input hash -you can give as an argument or make read from file- will be compared to each word's md5 hash. These words are in the inputWordList.txt file. You can extend or edit this file as you want. I only put 10 words on it for demo. I also added crackstation-human-only.txt file. You can use this file for wordlist file. This file's crack rate will be about %99.9 but it contains all human passwords, so your program execution time can takes like 1 hour for it. It's size about 700 MB. Or you can just use inputWordList.txt file for quick demo. If input hash and word's hash matches the word will be the answer for crack. If not that means crack could not be done. Input md5 hash should be 32 characters. So there is a control about length of it. 

All the informations and errors are given as a output. Also the program's execution time is produced as a duration time at the end of the output. 

You can download crackstation-human-only.txt that contains nearly all words from this link --> https://drive.google.com/open?id=10nF6ua7A1OKyRLWdD4UWIzt2br_wRrKs

Program will produce you a 'Report.txt' report file and you will see the results from powershell terminal too.

You can test these 10 hashes for demo --> 900150983cd24fb0d6963f7d28e17f72
                                          4c36fa32c9d93a002c3e14ce038aa709
                                          e2fc714c4727ee9395f324cd2e7f331f
                                          e10adc3949ba59abbe56e057f20f883e
                                          e99a18c428cb38d5f260853678922e03
                                          0659c7992e268962384eb17fafe88364
                                          7bc6c31880aeda581aa34e218af25753
                                          3c086f596b4aee58e1d71b3626fefc87
                                          e86fdc2283aff4717103f2d44d0610f7
                                          200820e3227815ed1756a6b531e7e0d2

There are 3 types of usage. You can check them below:

----------------------------------------------------------------------------------------------------------------------

**1) ./md5HashCracker.ps1 -help h**

User can use this command to get informations about how to use. This command will show you parameters and some
usage examples.

**Example Usage --> ./md5HashCracker.ps1 -help h**

Demo screenshot: ![alt text](https://github.com/BehlulKeremSisman/md5HashCracker/blob/master/demoScreenShots/help.png)


----------------------------------------------------------------------------------------------------------------------

**2) ./md5HashCracker.ps1 -crackType single -Wordlist <path of wordlist file> -inputArgument <hash>**

User should use this command if he/she has just 1 hash to crack.

[-crackType] argument will be 'single'

[-Wordlist] argument will be the path of wordlist.txt that contains words.

[-inputArgument] argument will be that hash.

You can download and use inputWordList.txt for demo.

**Example Usage --> ./md5HashCracker.ps1 -crackType single -Wordlist C:\Users\decoder\Desktop\inputWordList.txt -inputArgument 900150983cd24fb0d6963f7d28e17f72**

Demo screenshot: ![alt text](https://github.com/BehlulKeremSisman/md5HashCracker/blob/master/demoScreenShots/single.png)

----------------------------------------------------------------------------------------------------------------------

**3) ./md5HashCracker.ps1 -crackType plural -Wordlist <path of wordlist file> -inputArgument <path of hashlist>**

User should use this command if he/she has more than 1 hashes  to crack.

[-crackType] argument will be 'plural'

[-Wordlist] argument will be the path of wordlist.txt that contains words.

[-inputArgument] argument will be the path of hashlist.txt that contains hashes that he/she wants to crack.

You can download and use inputWordList.txt and inputHashList.txt for demo.

**Example Usage --> ./md5HashCracker.ps1 -crackType plural -Wordlist C:\Users\decoder\Desktop\inputWordList.txt -inputArgument C:\Users\decoder\Desktop\inputHashList.txt**

Demo screenshot: ![alt text](https://github.com/BehlulKeremSisman/md5HashCracker/blob/master/demoScreenShots/plural.png)

----------------------------------------------------------------------------------------------------------------------



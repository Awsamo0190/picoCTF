# picoCTF

# Description: Can you crack the password to get the flag?Download the password checker here and you'll need the encrypted flag in the same directory too.  

# Hints:
1. Does that encoding look familiar?  
2. The str_xor function does not need to be reverse engineered for this challenge.  

# Solving Steps:
1. Used wget to download level2.py and level2.flag.txt.enc
2. Ran level2.py 

      2.1 ![image](https://user-images.githubusercontent.com/99389724/154407523-444aa851-600b-4766-a208-d22d69743023.png)

        
3. Used cat to view level2.py 

      3.1 ![image](https://user-images.githubusercontent.com/99389724/154407671-581f22b8-1a04-4f58-8ee0-ceb07fe692e9.png)


4. Used my Convert_ASCII.py to translate the [ chr(0x63) + chr(0x30) + chr(0x30) + chr(0x30) ]
 
      4.1 ![image](https://user-images.githubusercontent.com/99389724/154407760-370f3417-dd8d-4ab7-944a-455f45f9cb36.png)
    

5. Entered Translated characters [ c000 ] as password when prompted.

      5.1 Got the Flag!!! ![image](https://user-images.githubusercontent.com/99389724/154407803-3841c331-37fb-4c8c-b9db-81a5be498ab2.png)

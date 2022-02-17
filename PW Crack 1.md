# picoCTF

# Description:  Can you crack the password to get the flag? Download the password checker here and you'll need the encrypted flag in the same directory too.  

# Hints:
1. To view the file in the webshell, do: $ nano level1.py  
2. To exit nano, press Ctrl and x and follow the on-screen prompts.  
3. The str_xor function does not need to be reverse engineered for this challenge.  

Solving Steps:
1. Used wget to level1.py and level1.flag.txt.enc
2. Ran cat on the level1.py file 

      2.1 Found the password? ![image](https://user-images.githubusercontent.com/99389724/154408159-95b686d9-c8b9-4d60-aac7-7256116be467.png)

3. Ran level1.py with python3 and entered e9e8

      3.1 Got the flag ![image](https://user-images.githubusercontent.com/99389724/154408259-1de24279-743b-46d3-8bf7-9c0584ba2929.png)
 

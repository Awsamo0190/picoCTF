# picoCTF

# Catagory: General Skills

# Name: PW Crack 2

Description: Can you crack the password to get the flag?Download the password checker here and you'll need the encrypted flag in the same directory too.    

Hints: 

1. Does that encoding look familiar?  
2. The str_xor function does not need to be reverse engineered for this challenge.  

Solving Steps: 
1. Used wget to download level2.py and level2.flag.txt.enc
2. Ran level2.py 

        2.1 ![image](https://user-images.githubusercontent.com/99389724/154405125-76bfef2f-ef65-4a25-922b-a31a5c50c2d2.png)

3. Used cat to view level2.py 

        3.1 ![image](https://user-images.githubusercontent.com/99389724/154405226-7a3d86bf-ddc2-4c13-a7b5-2d2543e5bf30.png)

4. Used my Convert_ASCII.py to translate the [ chr(0x63) + chr(0x30) + chr(0x30) + chr(0x30) ]
        
        4.1 ![image](https://user-images.githubusercontent.com/99389724/154405383-8ca989f2-fc2e-4274-96a5-c0bd23b33406.png)

5. Entered Translated characters [ c000 ] as password when prompted. 
       
       5.1 ![image](https://user-images.githubusercontent.com/99389724/154405504-3bb93731-ef7d-466d-9d9b-243dbb21300d.png)

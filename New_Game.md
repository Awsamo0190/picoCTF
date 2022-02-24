# picoCTF 

# Category: General Skills password_cracking hashing

# Name: PW Crack 3 

# Description: 

Can you crack the password to get the flag?
Download the password checker here and you'll need the encrypted flag and the hash in the same directory too.
There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.


# Hints: 
 
 1. To view the level3.hash.bin file in the webshell, do: $ bvi level3.hash.bin
 2. To exit bvi type :q and press enter.
 3. The str_xor function does not need to be reverse engineered for this challenge.

# Solving Steps 

1. Used wget to download all mentioned files 
2. Ran cat to look at the level3.py file 

    2.1 
    
    ![image](https://user-images.githubusercontent.com/99389724/155468899-2e33325d-977b-4f32-a09e-9dbcb8c59491.png)
 
 3. Noticed the list at the bottom script. 
    
    3.1 Tried each entry in the list till one worked

![image](https://user-images.githubusercontent.com/99389724/155469179-ede93e02-0b35-4c57-ab91-9d29a9c4b2a7.png)

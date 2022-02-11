# picoCTF Game Log

# Catagory: General Skills

# Name: FixMe1.py

Description: Fix the syntax error in this Python script to print the flag.Download Python script  

Hints: 
1. Indentation is very meaningful in Python  
2. To view the file in the webshell, do: $ nano fixme1.py
3. To exit nano, press Ctrl and x and follow the on-screen prompts.
4. The str_xor function does not need to be reverse engineered for this challenge.

Solving Steps: 
1. Used wget to download fixme1.py
2. Used python to run script and got error below
 2.1 

![image](https://user-images.githubusercontent.com/99389724/153542232-83e11722-8684-4b97-aee1-1115797b9a00.png)
 
3. Removed the spacing infront of the word "print" and saved changes  
4. Ran script again
 4.1 
 
 ![image](https://user-images.githubusercontent.com/99389724/153542271-50a6c0db-fb38-4739-970a-70f0942fd5b3.png)
 
5.Got the Flag!!

Broken Code:

![image](https://user-images.githubusercontent.com/99389724/153542532-0f67f619-8e4d-43a4-b97f-61befabf5543.png)


Fixed Code:

![image](https://user-images.githubusercontent.com/99389724/153542555-3f92c3a7-d50e-42d6-8fd6-04e5a63d9470.png)


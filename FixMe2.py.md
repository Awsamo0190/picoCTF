# picoCTF

# Game: FixMe2.PY

# Description:

Fix the syntax error in the Python script to print the flag.Download Python script  

# Hints: 

1. Indentation is very meaningful in Python  
2. To view the file in the webshell, do: $ nano fixme1.py
3. To exit nano, press Ctrl and x and follow the on-screen prompts.
4. The str_xor function does not need to be reverse engineered for this challenge.

# Solving Steps:

1. Used wget to download fixme2.py
2. ran fixme2.py

![image](https://user-images.githubusercontent.com/99389724/153553762-6ddcb6cb-282e-4052-b095-21c364628b5a.png)

3. Searched Google for and answers to syntax erros 

    3.1 Found this page: https://discover.cs.ucsb.edu/commonerrors/error/1009.xml

4. Added a equal sign to the one mentioned

    4.1 This made the code understand flag equaled (==) black or empty ("")
  
    4.2 You could also swap the "if" and "else" statements... while still adding the second "=" sign
  
    4.3 Flag was defined in the code
  
5. Ran the script and got the FLAG!!!!!

![image](https://user-images.githubusercontent.com/99389724/153553912-63c962a9-41a2-46f0-b0a2-40df691c7a14.png)

# Broken Code

![image](https://user-images.githubusercontent.com/99389724/153553994-b6b34b1a-afce-4ef3-a835-ef358b49c7b0.png)

# Fixed Code 1

![image](https://user-images.githubusercontent.com/99389724/153554127-64dcd104-f57f-4379-a09c-992acc26c48e.png)

# Real Fix?

![image](https://user-images.githubusercontent.com/99389724/153555516-b7793bab-7537-4ebd-ad5d-082b9faf1a84.png)





# picoCTF 

# Category:Cryptography

# Name: credstuff

# Description: 

We found a leak of a blackmarket website's login credentials. Can you find the password of the user cultiris and successfully decrypt it?

Download the leak here.
The first user in usernames.txt corresponds to the first password in passwords.txt. The second user corresponds to the second password, and so on.

# Hints: 
 
1. Maybe other passwords will have hints about the leak?

# Solving Steps 

1. Used wget  to download the .tar file 

    1.1 ![image](https://user-images.githubusercontent.com/99389724/162604443-4c1803f7-9b69-41dd-b987-f818d106e103.png)

2. Used the tar -xvf  to extrac the the contents of the .tar file 

    2.1 It seems to be a directory with two files in it

    2.2 ![image](https://user-images.githubusercontent.com/99389724/162604460-7b687ce0-ed55-474a-9b83-87ed970c629d.png)

3. Moved to the new "leak" directory using the cd command 
 
    3.1  ![image](https://user-images.githubusercontent.com/99389724/162604473-b1869f22-ed37-41b0-a9d9-783fce967016.png)

4. Used  cat with grep  to find the mentioned username and line number 

    4.1  ![image](https://user-images.githubusercontent.com/99389724/162604516-1c76d5bd-6dce-40b6-afb8-81bea29e94cf.png)

5. Used sed to view the password stored on line 378 

    5.1 ![image](https://user-images.githubusercontent.com/99389724/162604533-428cc54b-2f5d-42e0-a5ba-71874a465176.png)
  
6. Used Google to Search the string to see if recognized the string for any patterns

    6.1 Turns out it is rot13

7.  Used rot13.com from previous challenges to convert this string to clear text 

    7.1  ![image](https://user-images.githubusercontent.com/99389724/162604572-00f511ae-5006-4349-a377-146d08321cc2.png)
  
8. This brought me to write a script for converting rot13 cipher to plain text
  
    8.1 The Script ![image](https://user-images.githubusercontent.com/99389724/162604589-b0ec6c7a-2e7d-4465-bc58-8399d797a8ad.png)

    8.2 Proof of Concept for the script ![image](https://user-images.githubusercontent.com/99389724/162604622-7da0e63b-32dd-4190-ad93-8c46ee4e1799.png)

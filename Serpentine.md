# picoCTF 

# Category: General Skills

# Name: Serpentine

# Description: 

Find the flag in the Python script! Download Python script

# Hints: 

1. Try running the script and see what happens  
2. In the webshell, try examining the script with a text editor like nano  
3. To exit nano, press Ctrl and x and follow the on-screen prompts  
4. The str_xor function does not need to be reverse engineered for this challenge.  

# Solving Steps 

1. Used wget to download python script.
2. Used cat to view the script 
 
      2.1 Part 1 
     
      ![image](https://user-images.githubusercontent.com/99389724/154830624-b58d38e6-ca01-4e7a-846c-42c62de962f6.png)
      
      2.2 Part 2

      ![image](https://user-images.githubusercontent.com/99389724/154830651-b4b13eb1-40cf-4e24-a805-990e3ad56fda.png)

3. Ran the script knowing it would fail. Just wanted to see it happen 

      3.1
     
     ![image](https://user-images.githubusercontent.com/99389724/154830708-33a0f92c-d59a-4de2-ac27-5777c4c19546.png)
     
4. Ran nano to edit script
 
      4.1 Noticed the "b" option was not using the defined function for "print_flag" which was set. But that option "a" was using the defined function for          
      "print_encouragement" 
          
      ![image](https://user-images.githubusercontent.com/99389724/154830797-1859ba55-5914-4838-a2c1-b8a6d3dd7199.png)
      
      4.2 Here are the functions I am mentioning above 

      ![image](https://user-images.githubusercontent.com/99389724/154830859-fa5c9013-4625-481c-bb3b-3221bc9a178a.png)


5. Changed the "b" option to print_flag()

      5.1 
 
      ![image](https://user-images.githubusercontent.com/99389724/154830879-307a3c02-f080-4f6e-b9a6-ef83e981da1a.png)

6. Ran the script again and chose the "b" option 

      6.1 Got the Flag!!!! 
      
      ![image](https://user-images.githubusercontent.com/99389724/154830917-e0c1439f-0e6e-486f-abfd-a3364871edb7.png)



   
          

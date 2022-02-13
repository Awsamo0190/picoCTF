# picoCTF

# Category: General Skills

# Name: Glitch Cat

Description: Our flag printing service has started glitching!$ nc saturn.picoctf.net 52680  

Hints: 
1. ASCII is one of the most common encodings used in programming  
2. We know that the glitch output is valid Python, somehow!  
3. Press Ctrl and c on your keyboard to close your connection and return to the command prompt.  

Solving Steps:

1. Attempted to connect to site with url listed

    1.1 Got "Page isn't working" message with "HTTP:"
    1.2 Got "Page cannot provide a secure connection." with "HTTPS:"

2. Checked what "nc" is 
 
   2.1 Stands for "netcat" which is a utility for connecting and listening over UDP and TCP connections

3. Used "man nc" to get more information on the utility 
4. Used the below commands and got different output 

   4.1  ![image](https://user-images.githubusercontent.com/99389724/153706754-9379c286-8302-41d5-93d7-6caab5e8bdab.png)

   4.2 This created a file named flag.txt   ![image](https://user-images.githubusercontent.com/99389724/153706795-9a5cbe3f-fa55-4573-844a-29837d17f395.png)
  
   4.3  ![image](https://user-images.githubusercontent.com/99389724/153706838-56806fc9-cd93-488b-b8ed-4192eebad0e5.png)

5. Found Port Scanning Option from man page 

   5.1 The site is listening on port 52680 on tcp  ![image](https://user-images.githubusercontent.com/99389724/153706877-d2805810-8749-4e2e-874a-6f82b58feaf9.png)

6. Discovered the "chr(0x62)" and alike are ASCII Code
7. Leanred Python can convert ASCII code 
 
  7.1 Ran Python through terminal, copied the ASCII value out of the flag and pasted it into the Python prompt
 
 ![image](https://user-images.githubusercontent.com/99389724/153707030-dd467336-085b-439d-ba72-b69f94f34bc5.png)

8. Used "cat" to print the flag.txt information and appended the characters obtained from Python to the end.
9. Pasted new "Flag" into flag box on PICO 
  
   9.1  ![image](https://user-images.githubusercontent.com/99389724/153707142-abcf6a89-8ac2-41d0-b6e0-046d492caa3a.png)

10. It was correct

# picoCTF 

# Category: Web Exploit

# Name: Power Cookie

# Description: 

Can you get the flag? Go to this website and see what you can discover.


# Hints: 
 
 1. Do you know how to modify cookies?

# Solving Steps 

1. Went Website Provided

    1.1 ![image](https://user-images.githubusercontent.com/99389724/162605136-8cefec3f-a8a9-4ac8-8041-1ca466359546.png)

2. Clicked Continue as Guest

    2.1 ![image](https://user-images.githubusercontent.com/99389724/162605177-ee8ee01b-f1aa-4ed3-9ae6-4efcb7996c50.png)

3.  Checked Web Developer Tools 

    3.1 Saw this error ![image](https://user-images.githubusercontent.com/99389724/162605211-53a3eae8-99d5-4690-90f2-836eb947c6df.png)

4. Checked Cookies as mentioned above (And by the name of the game)

    4.1 Found "isAdmin" ![image](https://user-images.githubusercontent.com/99389724/162605234-b45888a0-287b-4bcb-9cf4-2964e5458eb3.png)

5. Googled how to modify Cookies. 

    5.1 Changed Value of "isAdmin" from 0 to 1 From inital page where you can click "continue as guest"
 
    5.2 Got the same error but noticed the Cookie error message was still poping up

    5.3 ![image](https://user-images.githubusercontent.com/99389724/162605262-0ee8f9cd-57fe-4c6c-8df6-4419184974f6.png)

6. I checked the Cookies again and found "isAdmin" back to 0. So I changed it from 0 to 1 again on the Page Shown above "We appologize,"
 
 6.1 Then I refreshed the page ![image](https://user-images.githubusercontent.com/99389724/162605388-18cc168e-0d0e-425a-9921-8faff8ef8a21.png)

7. The Flag was obtained and the Value for the Cookie "isAdmin" maintained 1 instead of reverting to 0 

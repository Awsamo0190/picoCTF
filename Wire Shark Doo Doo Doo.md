# picoCTF 

# Category: Forensics

# Name: Wire Shark Doo Doooo Do

# Description: Can you find the flag? shark1.pcapng.

# Hints: 

None

# Solving Steps 

1. Downloaded Wire Shark and the Capture File.

2. Watched Video on wireshark from youtube
        
      2.1 https://www.youtube.com/watch?v=TkCSr30UojM

3. Opened Wire Shark and the Capture File

4. Most of the file was just chatter between two different IP Addresses 

      4.1 192.168.38.103 <> 192.168.38.104
    
      ![image](https://user-images.githubusercontent.com/99389724/154807378-d2a57ab4-2182-42bc-b11a-e8fcf6087627.png)
    
5. Found a Section where a new IP Address started communicating 
        
      5.1 192.168.38.105
      
      ![image](https://user-images.githubusercontent.com/99389724/154807443-622806c9-4c8a-4ec3-bed5-3bb1010f8749.png)

6. From seeing the red reset "RST" packet it seems that the device at X.X.38.104 does not want to continue communicating with X.X.38.105
        
      6.1 The conversation between them seems to stop 

7. Shortly after the conversation is killed X.X.38.105 starts communicating again 
        
      7.1 But this time the traffic seems to change 

      ![image](https://user-images.githubusercontent.com/99389724/154807562-a3d6227e-cda4-47ab-8c7f-c4747025a153.png)

      7.2 There is a ARP request from a seemingliny new IP Address (18.222.37.134) that seems to have requested and received some HTML TXT file 
      
      ![image](https://user-images.githubusercontent.com/99389724/154807725-95ad9d83-731b-4201-aaba-d90fc585ff31.png)      
      
8. Started Inspecting the Packet with the HTM TXT file in it 

      8.1 Found the file in the Packet 

      ![image](https://user-images.githubusercontent.com/99389724/154807620-67187f7b-f6ae-4898-8cdf-b976594d7a61.png)

9. Searched Google using the text 
 
      9.1 Brought me to ROT13 translator

      9.2 Used translarot to translate the text 

      ![image](https://user-images.githubusercontent.com/99389724/154807662-d04595c1-fe6c-4581-834d-c594d063aef8.png)


10. Got the Flag!!!!


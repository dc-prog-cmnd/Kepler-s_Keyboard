Title: "Kepler's Keyboard"
Author: dc-prog-cmnd (me obv)
Description: A custom 75% keyboard with a rotary encoder
created_at: "2026-10-14"
---------
# October 14: Brainstorming the Design and getting the Matrix Down 
Spent a bit of time just browsing keyboards to see what I want to design and how I want the layout to be, and then created a matrix for the keys. 
<img width="1069" height="430" alt="image" src="https://github.com/user-attachments/assets/b074f14a-9f82-4a92-864a-9a5afab4112e" />
(Time Spent: 1 hour 15 minutes)

# October 15: Microcontroller Layout
I decided that I'd attempt to make a wireless keyboard. This came with a set of problems: the main one being about the battery. Also, because I have never designed a full sized keyboard I have never used a daughterboard. Overall, I'm pretty confused, but I mapped the matrix onto the microcontroller. (Oh yea I chose the nRF52840) 
<img width="1158" height="758" alt="image" src="https://github.com/user-attachments/assets/1feba451-d74b-4779-bb88-ee74e920fe59" />
(Time Spent: 2 hours 5 minutes)

# October 16: Switching EVERYTHING...
So... I might have messed up. Somehow I didn't notice how gargantuan the base nRF52840 is. So, I made the move of switching over to the nice!nano, which is a smaller dev board of the nRF52840. That came with its own set of problems but also solutions. The dev board handles a good amount of the struggles with Bluetooth and the battery that I would have had. However, it wasn't all sunshine and rainbows. I had to redo the matrix because of the lack of GPIO pins on the nice!nano. Honestly, the matrix I first made was terrible anyways, not to say the current one doesn't need improvement. Long story short, the schematic is finished. 
<img width="1031" height="739" alt="image" src="https://github.com/user-attachments/assets/b3d49120-aaa9-41db-a26d-4f00f69a9d63" />
(Time Spent: 1 hour 30 minutes)

# October 17: PCB Editing (sorta)
The keyboard plugin isn't working for some reason, and my keys are all misaligned on the PCB editor. Also, I didn't think about this earlier, but my matrix doesn't match my actual key layout, so I have to do everything weirdly on the PCB editor. I wasted an hour trying to figure that out. I also switched my keys to 45-degree symbols just cuz. That was the only real progress made today. I also downloaded a library for stabilizers.  This has been the longest I have spent on the project so far, and yet it is the least amount of work that has been accomplished. >:C
<img width="906" height="604" alt="image" src="https://github.com/user-attachments/assets/8e22d2e8-cd5b-4dd2-8730-bbd026c6e92b" />
     (Time Spent: 2 hours 15 minutes)
     
# October 18: The day of reckoning...
So I made negative progress today. Yes I went backwards. So I got to the PCB routing part, and I was doing pretty well. Actually, no I wasn't; it took me way too long to get the connections to work. And I finally had everything ready and almost complete. Until I realized I didn't have space for the connections to the GPIO pins. 
<img width="1277" height="532" alt="keyboardproto" src="https://github.com/user-attachments/assets/eeef0b47-72e2-4ef9-ad43-34bac2895696" />
So, instead of doing the normal thing, like switching to the back (which I forgot I could do) or just having the connections go outward more. I decided to redo my matrix. Honestly, I don't know why I chose a square matrix; I should have just matched the keyboard layout.  
<img width="1245" height="617" alt="newmatrix" src="https://github.com/user-attachments/assets/d5eb7708-0d62-4a5b-8830-ce670ff2b07b" />
So I did that, but  when I did it ended up not working when I tried to use the Keyboard Placer plugin. I then scoured the internet for a fix, to no luck. So, I decided to switch back to the square matrix. In total I have wasted countless hours of my time, and I just ended up farther back than when I started. 
(Time Spent: 4 hours 10 minutes) 

# October 19 - 23: Routing the PCB
I stuck with the square matrix. Routing was the worst thing I did. I started over like 2 times when I realized that I made mistakes with the patterns I wanted to do. I spent forever getting the wires to work, and near the end I thought I would have to start over because I forgot to finish one of the wire patterns from the earlier steps. Luckily, I managed to figure it out after a whole lot of trial and error. This was probably the most mind-numbing part of this whole project. It took me forever because of little mistakes I made from trying to rush it. The main  takeaway I learned is that you shouldn't use auto-route too often and should leave space properly; otherwise, you're cooked. 
<img width="1253" height="491" alt="image" src="https://github.com/user-attachments/assets/8887fbbc-2fb4-45c6-be16-dae556d508a3" />
(Time Spent: 5 hours 30 minutes)


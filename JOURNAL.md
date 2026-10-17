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
So... I might have messed up. Somehow I didn't notice how gargantuan the base nRF52840 is. So, I made the move of switching over to the nice!nano, which is a smaller dev board of the nRF52840. That came with it's own set of problems but also solutions. The dev board handles a good amount of the struggles with Bluetooth and the battery that I would have had. However, it wasn't all sunshine and rainbows. I had to redo the matrix because of the lack of GPIO pins on the nice!nano. Honestly, the matrix I first made was terrible anyways, not to say the current one doesn't need improvement. Long story short, the schematic is finished. 
<img width="1031" height="739" alt="image" src="https://github.com/user-attachments/assets/b3d49120-aaa9-41db-a26d-4f00f69a9d63" />
(Time Spent: 1 hour 30 minutes)

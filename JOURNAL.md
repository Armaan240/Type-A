# JOURNAL

| Title | TYPE-A |
|-------|---------------------|
| Author | ARMAAN SONI  |
| Slack Id | U091M21518T (@AMU)|
| Created  | 2026-07-2 |
| Last Updated  | 2026-07-2 |
| Total Time Till date| 3 Hours|
| Project Type | A custom split keeb !! |

# 2 JULY 2026 2:30 pm - 5:30 pm 

## Keys Matrix
ok so yah after lot of procastination i finaly started to make a keeb i so now it was time to decide to make which type a normal , or a split umm spilt keeb is the option for which i went cuz i feel using a spilt keeb could help make my posture correct , umm i love rgb leds so i had decided to to make it a backlit using SK6812 mini - E , these leds are pretty easy and doable with handsoldering , and sets perfect under keys for proper backlit effect , i want it make it compact and sleek so using a whole big pico for 3X6 and two extra keys wouldnt be feasible , so i decided to go with seed studio RP2040 and code with KMK , it have 11 pins which are sufficient for my thingi , 10 pins for keys and one pin for DIN , so yah i started making the schematic i would be design it in hirearchy so that it would be easy to handle (not too easy tbh !!) 
so i created left and right sheets under one root sheet AMUS idk i why i kep the name AMUS may be cuz i am amu :P , anyways i started with lfet hand idk why i could start with right but i started with left , so yah so i made a basic 3X6 martx cuz i love maths :D , and then extended the matrix to 4X6 for two keys and then added diodes to bottom for avoiding ghosting ! , and labeled the rows and coulumns 

<img width="960" height="540" alt="Screenshot (289)" src="https://github.com/user-attachments/assets/02a1f413-41a0-4913-9f3a-feb0a50c94d7" />
<img width="960" height="540" alt="Screenshot (290)" src="https://github.com/user-attachments/assets/c1925386-8362-434c-988d-365ece6423b8" />
<img width="960" height="540" alt="Screenshot (291)" src="https://github.com/user-attachments/assets/efce05a6-426c-4f48-8f13-c74ad06f12b6" />

## Leds and MCU 
yup so it was time to add my fav neo pixels yes thos sk6812 mini e blah blah leds , they a re pretty easy to wire what you have to do is connect vdd with 5v and vcc with gnd and dout to din of other and fisrt din to xiao , like you can do this with lables and wires upto you i did both and the wire one was looksing a mess yah a complete mess ! , idk i really fast with kicad now after all i have made cool things except a keeb lol , yah now i download the sym file of xiao fo kicad from internet and the footprint and then connected the net labes , and one more important thing!! , never ever forget caps , yes caps not the keycaps but the 0.1uf or 100nf caps near leds these capcictors are really need to manage the current and have a stable effect and also to keep the rgb safe from a bust of current !! , after that i used the last pin on xiao yah last pin lol , i cant add a oled but anyways the rgb is cool alone !! organised the caps and then every thing under text boxes to have clean thingi after that it was time to assign foot prints i yah my luck is soo good that the xia foot print was :) after that i assigned foot prints i am so dumb that i misunderstood diodes and leds since thwy had D symbol as of them it took me time to relise and assigne othere footprints but yah it was eays epeasy , and so i did a big disaster i forgot about the TRS jack need to make both keeb connect to each other for which i need a one GPIO pin free , so it need me to make the matrix 4X5 which will not look good but i will keep the pcb 3X6 but yah it work  it needed me to move the every switch one by one with the diode "|-|"  :( :(  
<img width="1920" height="1080" alt="Screenshot (293)" src="https://github.com/user-attachments/assets/2a1ae13f-569f-4bd7-b4ff-770a949927dd" />
<img width="1920" height="1080" alt="Screenshot (292)" src="https://github.com/user-attachments/assets/53676d2c-4792-478f-a6fb-ea012f0d7ac8" />


## Started with PCB 
yah the schematic thingi litt time taking but now it was time to make the pcb for the keeb , i had tow make it look good and sleek so i went for a 3X6 matrix and it took me a lot of time for the left hand keys to postion since the grid line are just awe full , after all i managed to make them in the place i liked :) , and then i traced out edge cuts around the pcb didnt took me much time but actually moretime was spent on making those edges cute and rounder :P , like i had to keep the pcb ouline lesser so i had to do the fillets at bottle neck and it need me to adjust the lines alot and finnaly aftert setting up thing for first i started doing placemnet for the right hand idk is there any tool or somthing to get rid o fthis hassle to keep things alligned and mirrror the left but anyways i first alligend the switch from right to left and moved them to the postition in right and dudring this i was having a wiered problem with one key in which it was not alligned idk if that will cause a problem since i going to have the switches of the plate and then pcb so yah after doing the placement i selected the layout and then grouped it and then duplicated and then fliped so after doing some tweaks and postioning i feel it looks good now !! , i placed both the xiao and then place mouse bites of 3mm , made the arcs and deleted the edgecut after that joined to it so that everyhting becomes under single thingi so yah it lloks cool and will the the routing and other things !

<img width="1920" height="1080" alt="Screenshot (294)" src="https://github.com/user-attachments/assets/80dba122-e8f6-4587-abb5-640ee8ec2066" />
<img width="1920" height="1080" alt="Screenshot (295)" src="https://github.com/user-attachments/assets/7d0d2027-ba3d-4936-bd93-66840747f165" />
<img width="1920" height="1080" alt="Screenshot (296)" src="https://github.com/user-attachments/assets/471ef407-52c5-4995-8b29-80bd9f7c2002" />
<img width="1920" height="1080" alt="Screenshot (297)" src="https://github.com/user-attachments/assets/77ca020d-b527-47e4-89b2-d6fd4b378de4" />
<img width="1920" height="1080" alt="Screenshot (298)" src="https://github.com/user-attachments/assets/e12e3404-82b1-4577-ba56-c35f503f89bc" />
<img width="1920" height="1080" alt="Screenshot (299)" src="https://github.com/user-attachments/assets/d86873c8-ea7a-48f4-b666-cff0256a1bea" />
<img width="1920" height="1080" alt="Screenshot (300)" src="https://github.com/user-attachments/assets/8d686f32-dbfd-4f21-855d-ff5bf53a80b9" />
<img width="1920" height="1080" alt="Screenshot (301)" src="https://github.com/user-attachments/assets/2dad1cb3-6431-4ec6-a5d6-db8a9c67fc09" />
<img width="1920" height="1080" alt="Screenshot (302)" src="https://github.com/user-attachments/assets/1edd02ce-4dce-41f3-8b1d-33c29f05069e" />
<img width="1920" height="1080" alt="Screenshot (303)" src="https://github.com/user-attachments/assets/83e1c5e2-ca36-4d70-9b86-c88d13a03756" />


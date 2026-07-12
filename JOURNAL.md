# JOURNAL

| Title | TYPE-A |
|-------|---------------------|
| Author | ARMAAN SONI  |
| Slack Id | U091M21518T (@AMU)|
| Created  | 2026-07-2 |
| Last Updated  | 2026-07-9 |
| Total Time Till date| 6 Hours 30 min|
| Project Type | A custom split keeb !! |



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

# 3 JULY 2026 7:00 pm - 8:00 pm 
So yah all this took me hour cuz i had to arrange 40 rgb leds by flipping and rotaing them , 40 capcitors and 40 diodes , so first i started with placing diodes i am going to solder at the back and and completed the left side of the pcb , and then placed the leds backmounted , i have kept the diode for the switch at a odd postion but it works , after all these i plced capcitors and left side was complted , the move to right side i did the same i lol i forgot to flip them so it need me the flip again some of them like 5-6 were of them which got left out so after diodes , i placed the capictors and leds , all these were easy but timke taking to place one by one , and yah i using smd capcitors which would be quite easy to solder by hand too! i have kep the pos of rgb at a aprox where the switch sets so yah it would look amazing when it will glow !! 
<img width="1920" height="1080" alt="Screenshot (313)" src="https://github.com/user-attachments/assets/797049f5-8b7c-41ed-8d5b-849b76cd3995" />
<img width="1920" height="1080" alt="Screenshot (314)" src="https://github.com/user-attachments/assets/3dc28394-16ec-4ad4-a93a-806c451c6e0d" />
<img width="1920" height="1080" alt="Screenshot (315)" src="https://github.com/user-attachments/assets/392648ca-d11b-4146-937f-dce322d422ec" />
<img width="1920" height="1080" alt="Screenshot (317)" src="https://github.com/user-attachments/assets/4233732e-2447-4a01-a548-553a256c1761" />

# 3 JULY 2026 9:00 pm - 9:30 pm (I DID THIS ON 3 JULY BUT WRITING UP ON 9 :P )
Oki it was time to route the pcb , i started with colums or ig rows i am really bad at identifing rown and columns lol , anyways i routed the switchs and diodes to the xiao it was easy peasy (it was not tbh! ) cuz like i messed with positions so it made it harder to route things , i fear what i would do while routing 5v and gnd and rgbs like it gonna make the task 10x  but nvm i  gonna handle it ! btw i have kep the traces 0.4 cuz like thats a safe zone since my switches are far way so it would cause less resistence ! 
<img width="1920" height="1080" alt="Screenshot (319)" src="https://github.com/user-attachments/assets/318ae4be-7570-4857-a136-907388f81b21" />
<img width="1920" height="1080" alt="Screenshot (320)" src="https://github.com/user-attachments/assets/9260b3f7-7a37-4731-a17c-7b4e4a7681e8" />
<img width="1920" height="1080" alt="Screenshot (321)" src="https://github.com/user-attachments/assets/561d0727-d876-4a62-b756-e0cd43eeb5f9" />
<img width="1920" height="1080" alt="Screenshot (322)" src="https://github.com/user-attachments/assets/0b0be09f-7c80-4f0a-b239-6e0fff0d6634" />

# 7 JULY 2026 10:30 pm - 12:20 am (I DID THIS ON 7 JULY BUT WRITING UP ON 9 :P )
oki so yah it was time to do 5v and gnd to those tiny leds and caps (capcitors) not head caps or keycaps , anyways i already knew that i gonna had a lot of vias so kept the trace 0.5 mm thick , so i started the 5v routing with back copper cuz the leds and caps are on the back so it would be easy to do so , from the first switch rgb i finally complted the last to the last rgb , i have intenitly made it rounder and messy like had some gap so that i could easily delete some of the trace while routing gnd and reconnect it , an yup i did the same and dtarted with routing gnd it was time taking but i manged to do so ! now it was time to do routing for leds first i thought it would be easy but no i relealised that could cuz bad led rgb effect and to prevent i get every led out of the board and then placed by order to the places and then routed the din and dout for diff leds like there were 20 ! of them 😭 now its time to route and the right side and yay then we move to cad ! 
<img width="1920" height="1080" alt="Screenshot (337)" src="https://github.com/user-attachments/assets/825fb50d-c0e8-4a88-ac88-f1f851501a6f" />
<img width="1920" height="1080" alt="Screenshot (338)" src="https://github.com/user-attachments/assets/00dc426b-2db2-48df-a3eb-003043dbdbd9" />
<img width="1920" height="1080" alt="Screenshot (339)" src="https://github.com/user-attachments/assets/5917258f-f729-4539-9093-276715e8b29a" />
<img width="1920" height="1080" alt="Screenshot (341)" src="https://github.com/user-attachments/assets/f629eec5-e409-420d-bc58-bf35d400a3df" />
<img width="1920" height="1080" alt="Screenshot (331)" src="https://github.com/user-attachments/assets/de1efada-e479-4624-9df5-6b4a4cedeb05" />
<img width="1920" height="1080" alt="Screenshot (332)" src="https://github.com/user-attachments/assets/fe1d8c24-4970-41b5-9eb7-dbef758d71c0" />
<img width="1920" height="1080" alt="Screenshot (333)" src="https://github.com/user-attachments/assets/fc5ee015-52a9-409f-8deb-ca1a03f8f956" />
<img width="1920" height="1080" alt="Screenshot (334)" src="https://github.com/user-attachments/assets/ca3483ae-b596-4d48-b7f7-3eac06eacd66" />
<img width="1920" height="1080" alt="Screenshot (335)" src="https://github.com/user-attachments/assets/da5ebdc3-52ae-44e1-a072-44441f46a5b1" />
<img width="1920" height="1080" alt="Screenshot (336)" src="https://github.com/user-attachments/assets/1405209e-316c-4d2e-b13c-b8ecc0398310" />

# 11 JULY 2026 12:00 pm - 1:40 (I DID THIS ON 11 JULY BUT WRITING UP ON 12 :P )
yah i was really tired yesterday after all the work i did because of my low end potato pc it took me a loot of time to do things anyways today it was time to do do routing for the right hand side and i knewed before that i not gonna repeat the same mistake again of having everything at 4 km apart :P , and i did different thing this time , i routed rows on the back copper and the colums on the front copper so that it would help me routing 5 v and gnd and DIN of leds , yup do the routing of rowns and colums took me 30 min and then it was time to route the din in which i made a blunder of not keeping the led colser at the end so it needed me to go back and the route from the next line , anyways i did that too and then on 0.5 mm thickness i routed the 5v and gnd i starded from teh top and routed it in a stright line rathar than making a spider net , this doesnt effect anything since i have a thicker trace so power ralis would be okay if i have vias on it and thrn i poured the gnd on both side for thermal relif <img width="1920" height="1080" alt="Screenshot (12)" src="https://github.com/user-attachments/assets/2140b6a0-29d2-4a33-8aba-5905b1ccba1c" />
<img width="1920" height="1080" alt="Screenshot (11)" src="https://github.com/user-attachments/assets/5992a759-4ab4-4eff-b950-c8030327384e" />
<img width="1920" height="1080" alt="Screenshot (10)" src="https://github.com/user-attachments/assets/1cd34f98-d9e6-49f9-8c1c-1bceb643ebdd" />
<img width="1920" height="1080" alt="Screenshot (9)" src="https://github.com/user-attachments/assets/4ebec203-2248-414f-b922-f5cd41a4af63" />
<img width="1920" height="1080" alt="Screenshot (8)" src="https://github.com/user-attachments/assets/cb34f637-95fd-4975-92a9-7d486794c983" />



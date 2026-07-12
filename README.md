# Type-A
so yah this is my split mechanical keyboard build i went with a split cuz i feel it could help make my posture correct , its a 3X6 layout with two extra thumb keys per side (so 4X5 matrix internally to keep one GPIO free for the TRS jack). i wanted it compact and sleek so no big old pico here , went with the seeed studio XIAO RP2040 running KMK firmware , it has 11 pins which is just enough for my thingi (10 for keys , 1 for DIN).
its fully backlit with SK6812 mini-e leds under the keys for that proper glow effect , 20 leds per side (40 total) , and each led has its own 0.1uF (100nf) decoupling cap right next to it to keep the current stable and the rgb safe from a burst of current !! diodes on every switch to avoid ghosting. two halves connect over a TRS jack. case is a minimal integrated mount design with m2 screws and fillets for a softer look

## Where i can find Assembly ?
yup since theres no f3z file in the repo (curruntly have the derived case from assembly in the form of stl and step ), cuz of the size limit so you can find all the files like f3z , step , stl , assembly in the following link 
https://a360.co/3RwVUDl
https://a360.co/4eYcRzC

# Renders
<img width="900" height="277" alt="Screenshot__32_-removebg-preview" src="https://github.com/user-attachments/assets/981acb7c-5eb9-4727-aa26-78d498405ceb" />
<img width="900" height="277" alt="Screenshot (31)" src="https://github.com/user-attachments/assets/c70afcc8-3c71-4fc4-b059-19280c59d673" />
<img width="900" height="350" alt="Screenshot__40_-removebg-preview" src="https://github.com/user-attachments/assets/75e2b1f9-6a4a-4589-aa12-43702387a705" />

# Cad
<img width="900" height="277" alt="Screenshot (33)" src="https://github.com/user-attachments/assets/a2991c26-f509-457e-bca8-2813076d0d27" />
<img width="1079" height="405" alt="Screenshot (42)" src="https://github.com/user-attachments/assets/bec289de-d49f-48bd-ba4e-7b37b18f29f5" />


 ## BOM

| Qty | Component | Notes |Price|Buy Link|
|-----|-----------|-------|-----|--------|
| 2 | Seeed Studio XIAO RP2040 | one per half, runs KMK |$11.6|https://thinkrobotics.com/products/seeed-studio-xiao-rp2040?variant=47933480173885&country=IN&currency=INR|
| 40 | Mechanical switches | 3X6 + 2 thumb keys per side |$5|https://www.amazon.in/Keyboard-Switches-Dust-Proof-Keycap-Puller/dp/B0GZVJZP6V/ref=pd_rhf_se_s_pd_sbs_rvi_d_sccl_2_4/523-8533341-7350922?psc=1|
| 40 | Keycaps | one per switch |-|3d Printed|
| 40 | 1N4148 diodes | one per switch, anti-ghosting, back mounted |$0.55|https://robu.in/product/1n4148-1w-zener-diode-pack-of-50/|
| 40 | SK6812 mini-e RGB leds | 20 per side, back mounted under keys for backlight |$33|https://www.amazon.in/gp/product/B0D5LGQ629/ref=ox_sc_act_title_2?smid=A473XUTYXHG1Q&psc=1|
| 40 | 0.1uF (100nF) SMD capacitors | decoupling, one per led |Already Have|-|
| 2 | TRS jack (PJ-320A style) | connects the two halves |Locally Sourced|-|
| 1 | TRS cable | to link both halves |-|-|
| ~8 | M2 screws | integrated mount case |-|-|
| 2 | Custom PCB | 3X6 layout, mouse bites 3mm |$15|Jlc PCB|
| 2 | Custom case (3D printed) | minimal integrated mount, 4mm walls, fillets |-|3D printed|

## TOTAL ~ $50 
(i didnt included the cost of PCB , because i will handwiring it , if needed i can afford it :P )

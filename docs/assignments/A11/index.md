# A11 – Motor Selection

## Objective
The objective of the assignment is to select a motor that is appropriate for our purposes. The motor needs to help deliver up to 2kN or 450lbf on a piece of material to be stretched to failure. Within this selection, it was important to consider the aforementioned parametes and other related specifications within a safety factor of 4 (already included in the diameter selection of the screw, affecting all related measurements).

## Motor Selection (Milena)

Based on the calculations from the last assignment, the required torque is 19.62 lb-in and the speed range is 0.3937-19.685RPM. 19.62lb-in is 313.92in-oz (Calculation: 19.62lb-in*16oz/lb).

Inspecting the stepper motors on McMaster-Carr, the strongest only goes up to 175.6in-oz.

<img width="1072" height="443" alt="image" src="https://github.com/user-attachments/assets/2dd4c407-a4b5-423f-8e48-c568644b06b7" />

The DC gearmotors have a much higher maximum torque:

<img width="1009" height="542" alt="image" src="https://github.com/user-attachments/assets/57d25450-151e-4915-bc1c-cf131d595134" />

However, after closer inspection, these motors only supplied a continuous operating torque at a certain speed. We need a speed range.
Going over to the compact DC motors, torque-speed charts are provided. Selecting the weakest motor:

<img width="383" height="292" alt="image" src="https://github.com/user-attachments/assets/f5f28200-e626-4b3b-883e-3f9cff68420d" />

This motor is NOT appropriate. It cannot reach the required ~20RPM with a ~20lbf-in or ~315RPM. We need less torque and higher RPM.

<img width="1028" height="339" alt="image" src="https://github.com/user-attachments/assets/6f8295f2-1e04-412d-91ad-7b280a03c60d" />

This motor is the first out of the list that goes above 20RPM. So it fulfills that requirement. We now inspect the speed-torque curve.

<img width="374" height="287" alt="image" src="https://github.com/user-attachments/assets/cb4d3078-c1ee-4bbd-9019-0ea044364fe0" />

Inspecting the possible ranges, this motor fulfills the required range and load based on torque.

Just to make sure, inspecting the previous motor in the list, it is observable that this motor cannot reach the ~315in-oz at an RPM of 20. 

<img width="377" height="290" alt="image" src="https://github.com/user-attachments/assets/16562909-8c2b-49c4-824b-8315692de7b1" />

Considering that the previous motor that has the correct range is around $73, which is affordable compared to higher-end options, we shall select that motor:

<img width="1439" height="680" alt="image" src="https://github.com/user-attachments/assets/4fc24422-8e27-4193-b623-a29b49886887" />

Which has the following torque-speed chart:

<img width="765" height="585" alt="image" src="https://github.com/user-attachments/assets/f670b268-19a8-4163-bfb1-91977dacc257" />

Link to Part: https://www.mcmaster.com/6409K17/



## Motor Mount Bracket Housing Design (Milena)

To analyze the geometry of the required bracket, I inserted one of the motors and made it cocentric with one of the lead screws:

<img width="674" height="453" alt="image" src="https://github.com/user-attachments/assets/fa5016ba-d31c-46f0-820c-1b51054d7828" />
<img width="599" height="274" alt="image" src="https://github.com/user-attachments/assets/1bafd899-8524-4443-8992-c3914f9c453b" />

It is noticeable that the motor itself already has bolt screw connections. It seems like it isn't possible to remove them. So I decided to design a bracket that would use nuts that screw onto the threads and with that onto the frame.

I chose to go with hex nuts.

<img width="1210" height="264" alt="image" src="https://github.com/user-attachments/assets/3a0c03e0-b457-45ab-9d7a-ceaf93b498df" />

<img width="1918" height="790" alt="image" src="https://github.com/user-attachments/assets/5e76e142-526d-4f40-860f-92be6dd0a998" />

I chose this one because it comes in a pack of 5. I can buy 2 packs and have two backup nuts.

Calculations-wise, I found the following:

<img width="876" height="681" alt="image" src="https://github.com/user-attachments/assets/10577186-d48a-4090-8c21-4594da853c62" />

The nut is taking too much thickness away from the plate. We need a thinner fastener. Since the main forces will be horizontally and the vertical forces will be pulling the motor downwards, the nut just needs to hold the motor in place enough not to come off easily.

I choose this narrow nut.

<img width="1916" height="736" alt="image" src="https://github.com/user-attachments/assets/9cc17951-1e59-422c-821b-6345ceb1dc0c" />

Link: https://www.mcmaster.com/90760A150/

<img width="876" height="490" alt="image" src="https://github.com/user-attachments/assets/198e4cfb-a8ba-437e-aed3-84261daba4b0" />

Upond second viewing, I did find another fastener, however I realized that my assumption of 450lbf was most likely off. We use the torque. I drew the distances of the bolts to the motor in SolidWorks:

<img width="867" height="718" alt="image" src="https://github.com/user-attachments/assets/693492a1-d174-485b-8b74-9be8ae1b9077" />

Since it is a spinning motion, we assume that the force works perpendicular to each line.

To confirm the chosen thickness, we use the longest distance:

<img width="883" height="408" alt="image" src="https://github.com/user-attachments/assets/540ca804-44c9-404f-b235-5a7ee1beeafd" />

<img width="828" height="475" alt="image" src="https://github.com/user-attachments/assets/d211a363-938b-4cce-9c26-2255c1554879" />

Based on the calculations, the minimum thickness is 0.00612in. We choose to go with a thickness of 0.186in.

I started making the bottom plate:

<img width="1296" height="903" alt="image" src="https://github.com/user-attachments/assets/cd3fa3d0-a13e-429c-bd61-8f583a31d767" />

I had to edit it.

<img width="751" height="562" alt="image" src="https://github.com/user-attachments/assets/f750e733-9952-43f1-91f9-e4ff65260932" />

I realized again that I had to edit it because it would not line up properly.

<img width="1060" height="721" alt="image" src="https://github.com/user-attachments/assets/9db53ab8-31ef-4605-bf42-cf7ec5eabce4" />

I continue to edit the dimensions.

<img width="1302" height="913" alt="image" src="https://github.com/user-attachments/assets/9ebf067f-4d1c-4b23-a880-6fe07749ae4b" />

I insert the edited parts.

<img width="1282" height="682" alt="image" src="https://github.com/user-attachments/assets/10b3fbc5-4d70-4193-bff0-0cc1f27388d5" />

These holes wouldn't line up.

<img width="1072" height="645" alt="image" src="https://github.com/user-attachments/assets/badc636e-e9ea-4a20-b264-7ef578d3ae7f" />

I fixed it.

<img width="1137" height="592" alt="image" src="https://github.com/user-attachments/assets/553008f7-26e9-4d4f-87cd-25fa3a5d1448" />

An attempt was made to make further holes.

<img width="1122" height="778" alt="image" src="https://github.com/user-attachments/assets/13747902-5859-479a-8762-e4e7c15a63c5" />

The attempt was successful.

<img width="1203" height="760" alt="image" src="https://github.com/user-attachments/assets/c4c970d2-c960-4526-a700-26c6e40f893b" />

The final brackets accomodate for the studs from the motor as well have holes for bolts and nuts combos to fasten everything. The same part can be used for the top and bottom. The final configuration looks like:

<img width="1374" height="909" alt="image" src="https://github.com/user-attachments/assets/c4ac0a4e-a6a3-436e-be2c-240d638391c0" />


## Coupler Design (Milena)
We calculate the dimensions of the coupler.

<img width="1450" height="538" alt="image" src="https://github.com/user-attachments/assets/580265f8-33df-45bb-b6ce-a4fb6039012a" />

<img width="1449" height="591" alt="image" src="https://github.com/user-attachments/assets/bf2d4b93-6e47-4aec-a3e3-da0986632674" />

<img width="1277" height="534" alt="image" src="https://github.com/user-attachments/assets/9b795eb7-98dd-4079-97ce-9135e5f868ec" />

<img width="1284" height="277" alt="image" src="https://github.com/user-attachments/assets/c0ec431d-d37e-443f-b6cf-4018469f3b9f" />

The mininum thickness with the chosen material is 0.0016in.

We choose the following values:

<img width="1328" height="406" alt="image" src="https://github.com/user-attachments/assets/35b05b14-9892-4191-a95b-65b368dec69a" />

The motor side dimensions are also calculated.

<img width="1353" height="763" alt="image" src="https://github.com/user-attachments/assets/bb8b4e97-fcd5-45c5-b3b7-ec6b9c9ea5e3" />

<img width="1455" height="573" alt="image" src="https://github.com/user-attachments/assets/3e634bec-e01e-4b25-90cf-3aafe4d3a72a" />

<img width="1451" height="732" alt="image" src="https://github.com/user-attachments/assets/abb4f8de-a41d-40d3-8c26-6b7819532e60" />

We now have all of the dimensions we need
Finally, the coupler is designed.

<img width="1308" height="946" alt="image" src="https://github.com/user-attachments/assets/e1e017c2-cb42-4902-b9c1-d39b4fee85c8" />

After making the cylindrical features, I make the holes for the sides that will house the screws holding on to the shafts. I choose screws that are of appropriate length. Since the wall thickness is 0.2244in and 0.3179in, it is necessary to select screws that are appropriate. A screw of 0.375in of thread should suffice:

<img width="953" height="373" alt="image" src="https://github.com/user-attachments/assets/127b8a29-4bcb-4206-91b7-5d528ede539c" />

The diameter is 0.164in. I adjust it in my drawing.

<img width="1315" height="909" alt="image" src="https://github.com/user-attachments/assets/8967de27-68f2-4c78-b0b3-b95b5fc3aa84" />

I added in threads.

<img width="1593" height="963" alt="image" src="https://github.com/user-attachments/assets/29cca27e-ab8c-4390-9a9d-813adb4ab144" />

The coupler is finished.

<img width="825" height="787" alt="image" src="https://github.com/user-attachments/assets/633ff138-4f1c-468e-812f-5b83a9197335" />


## Analyze and Design a Frame (Yazahira)

The Frame 

Before working on the FEA i had to analyze the twist caused by the motors and find the forces required to stabilize the top of the frame. 

After analyzing the twist caused by the motor on the frame I confirmed that the frame would be able to handle the stressed caused by the motors. I also found the force on each side of the frame where the motors would be. 


<img width="557" height="280" alt="Screenshot 2026-11-18 103852" src="https://github.com/user-attachments/assets/66d535a8-a9ba-41aa-8975-eb14cdf4e4c6" />



 Based on the information I have I decided on this frame connector. 


<img width="921" height="398" alt="Screenshot 2026-11-18 200101" src="https://github.com/user-attachments/assets/b7521f91-0250-49a9-82ab-082e823d62a0" />


 The FEA

Top frame

The first FEA I will run will be on the Top frame. I began by adding the torque and the fixed geometry on the top frame before starting the analysis. I ran an analysis with a medium coarse mesh and followed by a fine mesh in order to test for convergence.




<img width="960" height="540" alt="Screenshot 2026-11-18 222817" src="https://github.com/user-attachments/assets/1a3ada13-27fa-4cb4-9c26-c66e4f8d88dc" />


<img width="649" height="224" alt="Screenshot 2026-11-18 222838" src="https://github.com/user-attachments/assets/4aa3dc56-2a6b-4002-abd3-ffb396b9cc27" />

From both I got Von Misses stress and deflection graphs.

<img width="775" height="344" alt="Screenshot 2026-11-18 230416" src="https://github.com/user-attachments/assets/93442718-5005-4dc1-bc31-62a507ea0b5f" />

<img width="755" height="349" alt="Screenshot 2026-11-18 230539" src="https://github.com/user-attachments/assets/39eac69a-7fc0-4684-9224-a32e87fcdfd7" />

These are the results with the fine mesh analysis. 



<img width="758" height="353" alt="Screenshot 2026-11-18 233055" src="https://github.com/user-attachments/assets/186ee8a6-7683-4013-bf45-7f2f7671e236" />


<img width="743" height="350" alt="Screenshot 2026-11-18 233149" src="https://github.com/user-attachments/assets/4d85d0d9-46bc-49b6-be2d-e5c524d0d60b" />

After finishing both analysis i tested for convergence.



|   | SF    | Stress    |Deflection|
|---|-----|--------------|-----------
|1  |35.52| 1.126x10^2 psi |8.653x10^-4 mm|
|2  |27.91|1.433x10^2 psi|8.668x10^-4  mm|
|Convergence| 0.24%|  0.24%| 0%|


There was convergence however our frame failed the analysis. The frames twist is too large and wouldn't be able to handle a big load. A way to fix this could be changing the material of the frame into something stronger that can handle more load. Making the frame thicker i think would also help prevent this much twist on it. 

Vertical Components

Now that I've run the FEA on the top frame I will run an FEA on a side frame. The frame material will remain the same. As the top frame. I added the axial and transverse load to the frame as well as the fixed geometry. 


<img width="951" height="500" alt="Screenshot 2026-11-18 142458" src="https://github.com/user-attachments/assets/5fafa718-421e-439e-92a6-a6f4137edf81" />


<img width="535" height="320" alt="Screenshot 2026-11-18 142707" src="https://github.com/user-attachments/assets/4838094b-dba5-4be7-9f8d-d590c5283598" />


I ran the first simulation with a medium coarse mesh. These were the resulting graphs for Von Misses Stress and deflection. The graphs also graph where the maximum stress and deflection points are and their value. 


<img width="551" height="343" alt="Screenshot 2026-11-18 143758" src="https://github.com/user-attachments/assets/f6c6e5c2-80ab-4c61-b543-7b9decc85a4d" />


<img width="578" height="328" alt="Screenshot 2026-11-18 143914" src="https://github.com/user-attachments/assets/7e547545-b346-45ce-939f-774a22a36fcd" />


I then ran another simulation everything staying the same but this time with a fine mesh. 


<img width="767" height="365" alt="Screenshot 2026-11-18 150100" src="https://github.com/user-attachments/assets/58d19e3b-3950-4170-ac63-28206c509265" />



<img width="497" height="326" alt="Screenshot 2026-11-18 145933" src="https://github.com/user-attachments/assets/20f2b80b-71fa-40f7-906e-fe3ac50bb426" />

After finishing up both simulations I checked for convergence and these were my values. All the values did converge on the after the first two simulations with different sized mesh. However the safety factor is too low.


|   | SF    | Stress    |Deflection|
|---|-----|--------------|-----------
|1  |0.27| 1.496x10^4 psi |6.912 mm|
|2  |0.25|1.584x10^4 psi|  6.913 mm|
|Convergence| 0.1%|  0.1%| 0%|


Since the safety factor is way to low that being below 1. This would main our frame would most likely fail. A change that we propose could help the frame from failing would be a changing the material. A material with a higher yield strength would help the frame hold despite the forces acting on it currently. The locations of the maximum stress and deflection didn't change and the values didn't change much either. I believe changing the material would lead to better results. 

## Bearing Mount Design (Yazahira)


<img width="444" height="352" alt="Screenshot 2026-11-18 213641" src="https://github.com/user-attachments/assets/b95717c4-ca6b-4feb-8a28-c2757e89ac91" />
<img width="466" height="280" alt="Screenshot 2026-11-18 213543" src="https://github.com/user-attachments/assets/842c5811-ea4f-4665-aaa1-3f3f975416cc" />


This is what my design for the bearing mount looks like.I made the mount 3x3 because the width of the frame we used is 3 in. I made the middle hole where the screw would go .5 in diameter since that is the diameter of the lead screw. According to the Machinery Handbook the clearance for this hole for an RC3 fir is +.6 - 0. I decided to use  1/4 in bolts that are 2 in apart for his mount. Based on the book i made the holes for the bolts 0.266 in in diameter. 



<img width="683" height="346" alt="Screenshot 2026-11-18 205308" src="https://github.com/user-attachments/assets/c45c3c5c-d76a-43a1-b1d4-62a61652dfe5" />


<img width="443" height="248" alt="Screenshot 2026-11-18 215037" src="https://github.com/user-attachments/assets/34eabbbc-9b6b-4644-883a-3da8b9822307" />


## Costs (Milena)

Bill of Material
---------------------------------------------------------------------------------------------------------------------------------------------------
| Item Number | Quantity           | Name               | Cost/Item          | Cost               | Purchase Link      |
|--------------------|--------------------|--------------------|--------------------|--------------------|--------------------|
|98935A911 |2 |Carbon Steel Acme Steel Screw| $6.95 |$13.90 |https://www.mcmaster.com/98935A911/ |
|97790A110 |2 |932 Bearing Bronze- Flange Nut |$170.60 |$341.2 |https://www.mcmaster.com/97790A110/
|804T38 |1 |T-Slot Framing System |$202.12 |$202.12 |https://www.grainger.com/product/80-20-T-Slot-Framing-System-15-Series-804T38 
|LC103B-200 |1 |Load Cell| $349.56| $349.56| https://www.digikey.com/en/products/detail/omega/LC103B-200/25641942?gclsrc=aw.ds&gad_source=1&gad_campaignid=20243136172&gbraid=0AAAAADrbLlgO0kpqYMPhThlLdTwOcFLcR&gclid=Cj0KCQiAnsvXBhCqARIsAHKgGNbBoN82Wys6nRpzejUwxvXapOkhnu5bYxU6HeHkMHgI7gQFWMUO5JcaAgmxEALw_wcB 
|90760A150|1|Steel Narrow-Profile Hex Nuts|$6.73|$6.73|https://www.mcmaster.com/90760A150/|
|92200A192|1|Mil. Spec. 18-8 Stainless Steel Socket Head Screw|$4.46 |$4.46 |https://www.mcmaster.com/92200A192/|
||||Total Cost|$917.97

Design Cost
---------------------------------------------------------------------------------------------------------------------------------------------------
| Person | Hours Worked           | Cost/Hour              | Cost         | 
|--------------------|--------------------|--------------------|--------------------|
|Yazahira |9 |$35| $315.00 |
|Milena |9 |$35|$315.00|
||||Total Cost|$630.00


## Lessons Learned (Yazahira) (Milena)

Yazahira:
With this assignment we learned more about motors. We learned how to correctly read a motor graph and choose a motor based on that graph that would correctly fit our needed torque and rpm. With this assignment I struggled a lot with the FEA and adding the correct loads to the frames. Our safety factor for the frames were both terribly low. The top frame completely twists. Im not sure if its the way i added the torque on the frame or the material. The material could be changed into something stronger like i mentioned before which i believe could help. Ultimately I learned I  need more practice running FEAs to correctly add all the parts and have then run how they should. Both our vertical and top frame failed but i learned more about running FEAs.

Milena:
Building on the aforementioned lessons, for this assignment, we expanded our knowledge on how to select component dimensions based on stress and shear stress analysis. We further learned about including labor cost in our financial break-down, and had more freedom to choose additional components for our design parts, so we became more experienced with part selection on McMaster-Carr.

## Drawings (Milena)

This part is completed in our portfolios. Due to time restraints, in the pdf, it may not be complete yet. Please view the portfolios for the complete list.

Crosshead:

<img width="875" height="678" alt="image" src="https://github.com/user-attachments/assets/fc7e80aa-7d57-4900-8b69-d101d2a03639" />

Bracket:

<img width="1015" height="793" alt="image" src="https://github.com/user-attachments/assets/b0bd3fa7-574f-4a7d-a3ee-aad7872bddb5" />

Coupler:

<img width="943" height="729" alt="image" src="https://github.com/user-attachments/assets/ffc54f47-b4ab-4768-be02-6e45021ed579" />

Bearing Mount:
<img width="961" height="750" alt="image" src="https://github.com/user-attachments/assets/0d123b4b-f115-466c-9ea4-4a6fc59f8bce" />


Assembly:

<img width="1101" height="855" alt="image" src="https://github.com/user-attachments/assets/4b07ba98-f2e7-4f11-a3da-25ba185e256a" />






Links/ Files

Assembly:
https://drive.google.com/file/d/1jvs3zJaRhWwpZOseqy1sttTnRuknASGv/view?usp=sharing

Bearing Mount:
[Bearing Mount.zip](https://github.com/user-attachments/files/35063638/Bearing.Mount.zip)

Crosshead: 
https://github.com/user-attachments/files/34715581/A10-Crosshead.zip

Coupler: 
https://drive.google.com/file/d/1GuYkOA52rBS0G1NjtK-RXSCid_3poeph/view?usp=sharing

Bracket: 
https://drive.google.com/file/d/1Zvus47xIyk_wDwblzxl0XrPstExCGH9W/view?usp=sharing

Frame connectors-
https://www.grainger.com/product/80-20-Inside-Corner-Bracket-Inside-2RCW7

Drawings
Assembly: https://drive.google.com/file/d/1uv5e6CHI4BamPSoJpvlyusi8F6wJ0cF1/view?usp=sharing
Bearing Mount: https://drive.google.com/file/d/1BaNCaJZN-w9a922esPNYgBY0_WvW0srY/view?usp=sharing
Crosshead: https://drive.google.com/file/d/1pujiDOheSiMVagM07jkx1YiQIuYr1rcw/view?usp=sharing
Coupler: https://drive.google.com/file/d/15NqupJznTeGRP_lSAphICiyA7gY0lpIo/view?usp=sharing
Bracket: https://drive.google.com/file/d/16rjLPQL1Cs2SYSnDRxgf8m4yrTM6NGv1/view?usp=sharing


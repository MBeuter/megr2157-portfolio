# A11 – Motor Selection

## Objective
The objective of the assignment is to select a motor that is appropriate for our purposes. The motor needs to help deliver up to 2kN or 450lbf on a piece of material to be stretched to failure. Within this selection, it was important to consider the aforementioned parametes and other related specifications within a safety factor of 4 (already included in the diameter selection of the screw, affecting all related measurements).

## Motor Selection

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


## Motor Mount Bracket Housing Design

To analyze the geometry of the required bracket, I inserted one of the motors and made it cocentric with one of the lead screws:

<img width="674" height="453" alt="image" src="https://github.com/user-attachments/assets/fa5016ba-d31c-46f0-820c-1b51054d7828" />
<img width="599" height="274" alt="image" src="https://github.com/user-attachments/assets/1bafd899-8524-4443-8992-c3914f9c453b" />

It is noticeable that the motor itself already has bolt screw connections. It seems like it isn't possible to remove them. So I decided to design a bracket that would use nuts that screw onto the threads and with that onto the frame.

I chose to go with hex nuts.

<img width="1210" height="264" alt="image" src="https://github.com/user-attachments/assets/3a0c03e0-b457-45ab-9d7a-ceaf93b498df" />

<img width="1918" height="790" alt="image" src="https://github.com/user-attachments/assets/5e76e142-526d-4f40-860f-92be6dd0a998" />

I chose this one because it comes in a pack of 5. I can buy 2 packs and have two backup nuts.

Calculations-wise, I found the following:

The nut is taking too much thickness away from the plate. We need a thinner fastener. Since the main forces will be horizontally and the vertical forces will be pulling the motor downwards, the nut just needs to hold the motor in place enough not to come off easily.
Upond second viewing, I did find another fastener, however I realized that my assumption of 450lbf was most likely off. WE use the torque. I drew the distances of the bolts to the motor in SolidWorks:

<img width="867" height="718" alt="image" src="https://github.com/user-attachments/assets/693492a1-d174-485b-8b74-9be8ae1b9077" />

Since it is a spinning motion, we assume that the force works perpendicular to each line.

To confirm the chosen thickness, we use the longest distance:

I made the bottom plate:

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

The final brackets accomodate for the studs from the motor as well have holes for bolts and nuts combos to fasten everything.

## Coupler

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



## Frame 

## FEA

## Bearing Mount Design

## Costs

## Lessons Learned

## Drawing

# A3 – [Topic]

## Objective

<img width="906" height="199" alt="image" src="https://github.com/user-attachments/assets/615283ad-6a08-415d-a5b3-2887189e2f7d" />

The objective of the assignment is to deisgn a bar with circulart cross-section including its corresponding parameters.

The bar is to have an applied direct load between 300 lbf < F < 500 lbf. The max axial deflection of the bar is .009 inches. The bar is to be designed from Aluminum with a range of Young’s Modulus from (8.5 - 11.5) x 106 psi. 

I choose 300lbf for the force.

6061-T4 Alloy (Aluminum) is chosen with a Young Modulus of around 10MPSI.


## Calculations
To determine the radius of the bar, we must calculate the max elongation allowed at 0.009in first. First, I made the mistake of mixing up some values, not knowing I get to choose my diameter and area myself, so I "calcualted" the necessary diameter.

<img width="648" height="556" alt="image" src="https://github.com/user-attachments/assets/f71c9b32-1dd0-4206-a060-bee1016ca3a3" />

Then I realized my mistake, and I chose values, as I was supposed to.

<img width="579" height="267" alt="image" src="https://github.com/user-attachments/assets/94675540-5354-4b44-a765-cd80ee95f29a" />

The material closest to my chosen values was Alloy 6061-T4:

<img width="714" height="757" alt="image" src="https://github.com/user-attachments/assets/cd0b6120-7b64-4e2d-b34a-399e23ab8dee" />

# Simulation
During my first simulation attempt, the elongation change ended up being 0.009072in. This is above the specification, most likely due to me using a different Young Modulus (a smaller one) than the material being used. I recalculated with this in mind.

<img width="523" height="141" alt="image" src="https://github.com/user-attachments/assets/3f239ebe-d1d4-489a-a61b-7b0d11595723" />

This was the result:

<img width="1443" height="967" alt="image" src="https://github.com/user-attachments/assets/2411250a-c0e3-4ce3-b094-9307886309d4" />

The new resulting displacement was 0.009073in. I managed to make it a little bit worse. I decided it be best if we round it up to 0.009 and call it a day.

## Von Mises Map

<img width="1477" height="855" alt="image" src="https://github.com/user-attachments/assets/381b0083-6374-4c4b-9957-06dcc95a28cc" />

The greatest stress is lower than the 40 ksi max for aluminum with 227500000Nm^2 of stress, or 32.996085334 ksi. The safety factor is 1.21.

<img width="678" height="490" alt="image" src="https://github.com/user-attachments/assets/a492c81d-778e-4de3-9ab4-af22b58a9272" />

<img width="1477" height="813" alt="image" src="https://github.com/user-attachments/assets/b9b18862-43c2-470f-807c-2822875cc6b0" />


## Results
The overall axial deflection ended up being 0.009073in, which is a little off from the 0.009in given for the problem. At first I thought it was due to the different Young Moduli used, so I modified it. However, that did not help. The assignment did not take long to complete, around 1.5h, however it was my first  time using the simulation function and it is possible I made mistakes along the way I was too novice to catch, resulting in a slightly off deflection.
The result I would trust more is the simulations. It is good to trust the results that would create a slightly larger deflection to be able to have a more generous trajectory of the final results in mind and design around those.
The stress concentration factor (Kt) for a hole in a flat bar in tension is 3.0. This would make for a stress of 32.996 times 3.0, meaning the final stress is 98.99 ksi, which would not pass the safety factor at all. It would actually fail over two times over.

# For 2157 Students

I already changed the length of my bar during the investigation. My prediction was that an increase in deflection would be caused by a shortening of the length. The length actually became longer.


# A9 – Pulley System Design

## Objective
The purpose of the assignment is to be familiarized with friction, static analysis and dynamic analysis. The following conditions are listed, alongside chosen variables within the constraints of the problem set:
- Pulley Diameter: 3in
- Center Distance between Pulleys: 5in
- RPM: 1000Rev/min
- Belt Tension F: 5lbf
- Pulley Material: Aluminum
- Safety Factor: 3
- Belt Material: polyurethane rubber (Sy=471psi at 20% strain)

The following image taken from the assignment statement shows the pulley conditions:

<img width="745" height="238" alt="image" src="https://github.com/user-attachments/assets/2c909c6c-1ecf-4c39-a3ce-3cff61b42443" />



## Component Designs
## Belt Design

I want to use the exact kinetic coefficient of friction for polyurethane rubber, so I found an article on scientific.net: https://www.scientific.net/AMM.26-28.320

 Despite finding this article, it was inaccessible to me. Although UNCC had a logon for students, trying to use my credentials brought up issues. I tried at least 3 times through these 2 UNCC pages and a third one I found:
 
<img width="1824" height="876" alt="image" src="https://github.com/user-attachments/assets/68ef7b44-a6bc-490b-9a41-b32d5f4d7559" />
 
<img width="1831" height="880" alt="image" src="https://github.com/user-attachments/assets/ced58f4b-90f1-420e-8af7-2d529e610525" />

I decided to be happy with finding the coefficient of friction between regular rubber and aluminum.

I was able to find a table by the Slovak University of Technology in Bratislava: https://atc.sjf.stuba.sk/files/mechanika_vms_ADAMS/Contact_Table.pdf

<img width="1186" height="94" alt="image" src="https://github.com/user-attachments/assets/fbc78f78-e81f-4094-9e4b-270866cfe1c0" />

<img width="1192" height="60" alt="image" src="https://github.com/user-attachments/assets/0bbc04e0-149d-4c14-8948-17b005474607" />

Here, MuStatic=0.8. We are picking the 


## Shaft's Diameter Design

## Journal Bearing Design

## Design of Frame

## Lessons Learned


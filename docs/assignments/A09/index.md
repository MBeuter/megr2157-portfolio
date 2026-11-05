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

Here, MuStatic=0.8. We are picking the static coefficient of friction because we do not want the belt to slip against the circumferal surfaces of the pulley. Otherwise, the pulled pulley would not be put into motion.

With this in mind, we can now move on to figuring out the forces throught the belt

This belt is chosen as it fulfills the requirements for a minimum belt diameter of 0.274" and can have a possible belt circumference of 25.43":

<img width="1267" height="370" alt="image" src="https://github.com/user-attachments/assets/6482a9d2-a513-4458-b7d4-ed076ea2f4aa" />


## Shaft's Diameter Design

<img width="699" height="88" alt="image" src="https://github.com/user-attachments/assets/41fa006c-e0b7-4ae7-8c9c-e11470ccae68" />


## Journal Bearing Design

## Design of Frame

Based on this graphic, found that a o.5" thick pulley can support a 5/16" belt:

<img width="1366" height="639" alt="image" src="https://github.com/user-attachments/assets/ad94afb2-06fe-424e-9c8e-37f28081aea7" />

During the upcoming calculations, it shall be assumed that the pulley is a plate of thickness t. For simplicity, the groove around the circumference shall not be subtracted from the overall volume. This will not affect our choice in frame material negatively. Quite the opposite. It will make it safer thanks to a slight overstimation in mass of the pulleys.

I used the following source to obtain the density of the aluminum: https://www.azom.com/article.aspx?ArticleID=6636

<img width="1093" height="547" alt="image" src="https://github.com/user-attachments/assets/48b6caed-d3aa-43de-8530-6b4653a1c4a3" />


I used the following source to obstain the density of the 1060 hardened steel: https://www.azom.com/article.aspx?ArticleID=6542

<img width="1111" height="586" alt="image" src="https://github.com/user-attachments/assets/50c8d905-b4bd-4a5e-a62f-1db9245ed472" />

I used the following website to obtain the density of teflon for the bearings: https://laminatedplastics.com/teflon.pdf

<img width="433" height="73" alt="image" src="https://github.com/user-attachments/assets/b2433bb3-a15a-4ef9-a2a6-29ab73f1bf8f" />

The link to the data sheet for the Al-1060-O information to gain the bearing yield strength is here: https://www.scribd.com/document/559748450/Aluminum-1060-data-sheet

<img width="543" height="49" alt="image" src="https://github.com/user-attachments/assets/5140c23d-6bf1-40f4-b9bf-35e0ffa3e27c" />


## Lessons Learned


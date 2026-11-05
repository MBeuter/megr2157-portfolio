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

Starting with the belt design, it is important to understand the parameters required to make a choice on https://www.google.com/url?q=https://www.mcmaster.com/products/round-belts/round-belts-8/&sa=D&source=editors&ust=1793859999195149&usg=AOvVaw3hLMaxaDO5wEofOq5mYEw7 .

Listing all important variables:

<img width="921" height="379" alt="image" src="https://github.com/user-attachments/assets/7cdf2a7e-280c-4285-befc-794a78ea54f7" />

Providing the FDB:

<img width="967" height="634" alt="image" src="https://github.com/user-attachments/assets/f7234a31-7a16-4654-8b1b-67bde1e54538" />

I attempted to calculate the two pulley forces (FH and FL) by using the power formula. Until I realized that we do not have the power...

<img width="993" height="379" alt="image" src="https://github.com/user-attachments/assets/52994128-800c-4066-a782-e296a02eee7d" />

Instead I used the belt friction formula:

<img width="630" height="276" alt="image" src="https://github.com/user-attachments/assets/1f7835e1-8e7d-4368-93f7-dcaeaefe9b26" />

I wanted to use the exact kinetic coefficient of friction for polyurethane rubber, so I found an article on scientific.net: https://www.scientific.net/AMM.26-28.320

Despite finding this article, it was inaccessible to me. Although UNCC had a log-on for students, trying to use my credentials brought up issues. I tried at least 3 times through these 2 UNCC pages and a third one I found:
 
<img width="1824" height="876" alt="image" src="https://github.com/user-attachments/assets/68ef7b44-a6bc-490b-9a41-b32d5f4d7559" />
 
<img width="1831" height="880" alt="image" src="https://github.com/user-attachments/assets/ced58f4b-90f1-420e-8af7-2d529e610525" />

I decided to be happy with finding the coefficient of friction between regular rubber and aluminum.

I was able to find a table by the Slovak University of Technology in Bratislava: https://atc.sjf.stuba.sk/files/mechanika_vms_ADAMS/Contact_Table.pdf

<img width="1186" height="94" alt="image" src="https://github.com/user-attachments/assets/fbc78f78-e81f-4094-9e4b-270866cfe1c0" />

<img width="1192" height="60" alt="image" src="https://github.com/user-attachments/assets/0bbc04e0-149d-4c14-8948-17b005474607" />

Here, MuStatic=0.8. We are picking the static coefficient of friction because we do not want the belt to slip against the circumferal surfaces of the pulley. Otherwise, the pulled pulley would not be put into motion.

<img width="441" height="208" alt="image" src="https://github.com/user-attachments/assets/8653bb61-b4d9-4938-aa04-2ad86c4c011f" />

With this in mind, we can now move on to figuring out the forces throught the belt.

<img width="1060" height="775" alt="image" src="https://github.com/user-attachments/assets/4275f5f4-5b01-42bc-99ec-06d32f9bf865" />

<img width="730" height="117" alt="image" src="https://github.com/user-attachments/assets/5b46c7a1-ba95-44b7-9dd2-72468957692b" />

Next, it was necessary to figure out which belt would be used. I calculated the required area and diameter.

<img width="1176" height="771" alt="image" src="https://github.com/user-attachments/assets/3445ec68-90b2-4d7b-8bef-60712435f85f" />

Then I chose a diameter that would fulfill these minimum requirements on the website provided:

<img width="762" height="741" alt="image" src="https://github.com/user-attachments/assets/5d510340-e920-4b08-aafe-534f9688bc2e" />

Then I calculated the required circumferal length of the belt:

<img width="1125" height="525" alt="image" src="https://github.com/user-attachments/assets/4425a8a3-8ce2-45c7-92ff-eb98d6833d70" />

This belt is chosen as it fulfills the requirements for a minimum belt diameter of 0.274" and can have a possible belt circumference of 25.43":

<img width="1267" height="370" alt="image" src="https://github.com/user-attachments/assets/6482a9d2-a513-4458-b7d4-ed076ea2f4aa" />


## Shaft's Diameter Design
First we determine the required variables and provided numbers:

<img width="793" height="363" alt="image" src="https://github.com/user-attachments/assets/795813fa-62d9-4356-b9e8-18dd94c76e8a" />

<img width="915" height="433" alt="image" src="https://github.com/user-attachments/assets/99d88abe-4bce-4c64-a652-8b97353e8a17" />

Here is the FDB. A single plane shear force will decide the required minimum diameter of the shaft:

<img width="1099" height="354" alt="image" src="https://github.com/user-attachments/assets/cc59e3f8-48aa-4dec-bd27-4ec00e2cade7" />

I obtained the shear stress value:

<img width="699" height="88" alt="image" src="https://github.com/user-attachments/assets/41fa006c-e0b7-4ae7-8c9c-e11470ccae68" />

Source: https://www.fabdigit.com/materials/steel-1060/

Finally, we calculate:

<img width="723" height="295" alt="image" src="https://github.com/user-attachments/assets/e2f6a787-24ea-4957-b937-80a73d04d1c0" />



## Journal Bearing Design

We begin with what is provided and what is sought, and create a sketch to guide the process:

<img width="1158" height="616" alt="image" src="https://github.com/user-attachments/assets/11628e69-0716-4c94-b8b2-89ea8347e846" />

Next, we calculate the required clearances and diameters to be able to use them for our calculations. For this, we go based on a graphic in the book on page 2412. It is also possible to verify the calculated clearances with those of a sliding fit on page 654:

<img width="942" height="823" alt="image" src="https://github.com/user-attachments/assets/8ff2bc5e-376a-4540-b7cd-44ad14c8e2d0" />

We use the information on page 2412 to also determine which length we would like our bearings to have. In this, we assume that the bearing is for generators or motor with a L/d ratio of 1.2 to 2.5. This assumption in the context makes sense considering that many pulleys in the real world that work beside each other will most likely have a driving pulley that has a motor. We choose 2:

<img width="936" height="285" alt="image" src="https://github.com/user-attachments/assets/bdef8ecf-f172-48a3-bbf4-6a709f9281fc" />

We calculate P, V and PV:

<img width="934" height="403" alt="image" src="https://github.com/user-attachments/assets/9d5a0e17-86b0-47e6-ab20-346938a0a7a9" />

Through these calculations, we choose the table on page 2442 to decide on a material for our bearings:

<img width="922" height="676" alt="image" src="https://github.com/user-attachments/assets/d0cc14c0-04f6-4f0b-9b03-7b2d934c8ddb" />

Reinforced teflon checks all of the boxes so we choose that for our bearing material.

## Design of Frame
We were tasked to design a frame for the above set-up. A sketch illustrates a potential design:

<img width="826" height="289" alt="image" src="https://github.com/user-attachments/assets/a9e8eb97-b2d7-4985-ab17-067a35097b35" />

I calculated and choose the clearances around the holes based on page 655 in the course materials book:

<img width="729" height="634" alt="image" src="https://github.com/user-attachments/assets/a369b226-839b-49ef-bbc7-89d07e5df9ac" />

<img width="865" height="156" alt="image" src="https://github.com/user-attachments/assets/4ea8d34e-e6ef-495a-a6ab-e066a0115866" />

Next we calculate the weight of the individual materials that will be weighing down on the frame to be able to determine the minimum thickness required to support everything:

<img width="819" height="268" alt="image" src="https://github.com/user-attachments/assets/115a422a-2a40-496d-a210-174aa38bb77a" />

Before I can calculate the weight of a pulley, I need its thickness.
Based on this graphic, I found that a o.5" thick pulley can support a 5/16" belt:

<img width="1366" height="639" alt="image" src="https://github.com/user-attachments/assets/ad94afb2-06fe-424e-9c8e-37f28081aea7" />

During the upcoming calculations, it shall be assumed that the pulley is a plate of thickness t. For simplicity, the groove around the circumference shall not be subtracted from the overall volume. This will not affect our choice in frame material negatively. Quite the opposite. It will make it safer thanks to a slight overstimation in mass of the pulleys.

I used the following source to obtain the density of the aluminum: https://www.azom.com/article.aspx?ArticleID=6636

<img width="1093" height="547" alt="image" src="https://github.com/user-attachments/assets/48b6caed-d3aa-43de-8530-6b4653a1c4a3" />

<img width="897" height="682" alt="image" src="https://github.com/user-attachments/assets/c5b44216-ed87-47a7-b1e7-0ef5273ee3f5" />


I used the following source to obstain the density of the 1060 hardened steel: https://www.azom.com/article.aspx?ArticleID=6542

<img width="1111" height="586" alt="image" src="https://github.com/user-attachments/assets/50c8d905-b4bd-4a5e-a62f-1db9245ed472" />

I used the following website to obtain the density of teflon for the bearings: https://laminatedplastics.com/teflon.pdf

<img width="433" height="73" alt="image" src="https://github.com/user-attachments/assets/b2433bb3-a15a-4ef9-a2a6-29ab73f1bf8f" />

Then I calculated the weight of one bearing  in its minimal length:
<img width="925" height="397" alt="image" src="https://github.com/user-attachments/assets/e6834cca-848f-4c36-971d-bbc9efe50026" />

The link to the data sheet for the Al-1060-O information to gain the bearing yield strength is here: https://www.scribd.com/document/559748450/Aluminum-1060-data-sheet

<img width="543" height="49" alt="image" src="https://github.com/user-attachments/assets/5140c23d-6bf1-40f4-b9bf-35e0ffa3e27c" />



## Lessons Learned


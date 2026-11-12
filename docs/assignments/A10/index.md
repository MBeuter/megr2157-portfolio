# A10 – Lead Screw Translating System

## Objective

The task was to assemble a tensile tester by designing a screw-drive crosshead and selecting the required components. The assignment puts stress on selecting components based on the required force applied, stresses caused and geometries affecting the overall behavior of the materials. We had to evaluate the cost of the parts selected as well.


## Lead Screw - Yazahira

1) In order to select my leadscrew I first have to find the minimum diameter needed for the leadscrew. I used the axial stress analysis equations to find the minimum diameter needed. We did end up choosing steel as the material and used the yield strength and friction factor for this material in order to solve for the values. 


   <img width="871" height="606" alt="image" src="https://github.com/user-attachments/assets/a5b5b9e6-8b75-49af-995c-00d7af011560" />


The determined minimum diameter is 0.1380in.


2) After finding the diameter I needed I followed by calculating the range of the rotational speed my leadscrew would have. I used the linear speed provided in order to find my range. 

   
<img width="814" height="517" alt="image" src="https://github.com/user-attachments/assets/ec102cf6-cb0e-4864-91c8-70d2c4ff7649" />


The determined range of rotational speed for the screw is 0.3937-19.685RPM.


3) Now i need to follow up by calculating the torque that would provide the load needed of 2kN. This would help me select my leadscrew. 

   
<img width="885" height="532" alt="image" src="https://github.com/user-attachments/assets/6391fbc2-7cf6-4d1b-9ba1-a35db46b18a6" />


The determine torque at this speed


4) After finishing  up all my calculations and finding all my missing values I was able to select my screw. Based on the minimum required height of 18 in. and my minimum diameter I decided to choose the acme leadscrew below made of carbon steel. I thought it'd be the best fit for the assignment. 


<img width="960" height="436" alt="Screenshot 2026-11-11 171830" src="https://github.com/user-attachments/assets/fcc72e62-cb8e-440b-bcde-d1204f3debd5" />


## Nut and Flange - Yazahira

In order to select the Nut/Flange for this assignment I had to find the minimum amount of threads that'd be able to support the load required of 2kN. After finishing the calculations I choose the Nut Flange that I thought would be the best fit. 


<img width="472" height="323" alt="Screenshot 2026-11-11 173143" src="https://github.com/user-attachments/assets/de87cc28-de04-40b1-a928-5d1618dfb1f4" />


<img width="958" height="437" alt="Screenshot 2026-11-11 172810" src="https://github.com/user-attachments/assets/1cbe162d-16ba-4353-a196-08e982eb0aeb" />



## Crosshead - Milena
1+2) Size + Material: Simple Beam Stress and Deflection Analysis

In order to design the crosshead, it was important to determine the stresses acting on its geometry. To verify the appropriate chosen dimensions, we had to do a deflection analysis. This ensures that the deflection of the crosshead, which we treated as a beam with both ends fixed, would support its load within the required specifications.


The known dimensions and wanted variables have been listed.


<img width="924" height="576" alt="image" src="https://github.com/user-attachments/assets/ea335f0a-8823-4542-b697-ed6ba436345a" />


The calculated axial stress under the given conditions is 12.5 psi. The yield strength of carbon steel is 60200 psi. Considering the safety factor of 4, this means that the allowed axial stress is 60200psi / 4 = 15050 psi. The calculated 12.5 psi is way below the allowed stress. We considered changing the material, however considering that it is a machine that is designed to stretch apart metals, we decided to keep the carbon steel material for the crossbeam. The lack of stress relative to its allowed maximum prevents excessive fatigue from repeated use over time.


Next, I calculated the maximum deflection under the given conditions. 


<img width="837" height="222" alt="image" src="https://github.com/user-attachments/assets/6dfea0ee-4ee5-41db-b68a-daa504e68a92" />


I correct that the maximum deflection in the last line is actually 3.94x10^(-3), not 39.4x10^(-3).


With a maximum deflection of 0.000559in, and a maximum allowed deflection of around 0.00394in, the results are within the allowable range. We are only at 14% of the allowed deflection. One may argue that we could change the material to reduce the overall productionb price of the crossbeam. However, in this exercise, we were not asked to consider price specifically as one of the deciding factors in our design. The benefits of a sturdy material, disregarding pricing, outweigh the chance of creating a critical component that will fail early on due to excessive repeative stress in exchange for lesser cost.


3) Multiview Paper Sketch


The multiview paper sketch showcases the crosshead from a front view, a top view and a side view. The material is Carbon Steel.


<img width="455" height="201" alt="Screenshot 2026-11-11 180225" src="https://github.com/user-attachments/assets/8a92cbe6-8947-4cf8-aec4-0bbf0e5db1fd" />


## Costs - Milena
Table

---------------------------------------------------------------------------------------------------------------------------------------------------
| Item Number | Quantity           | Name               | Cost/Item          | Cost               | Purchase Link      |
|--------------------|--------------------|--------------------|--------------------|--------------------|--------------------|
|98935A911 |2 |Carbon Steel Acme Steel Screw| $6.95 |$13.90 |https://www.mcmaster.com/98935A911/ |
|97790A110 |2 |932 Bearing Bronze- Flange Nut |$170.60 |$341.2 |https://www.mcmaster.com/97790A110/
|804T38 |1 |T-Slot Framing System |$202.12 |$202.12 |https://www.grainger.com/product/80-20-T-Slot-Framing-System-15-Series-804T38 
|LC103B-200 |1 |Load Cell| $349.56| $349.56| https://www.digikey.com/en/products/detail/omega/LC103B-200/25641942?gclsrc=aw.ds&gad_source=1&gad_campaignid=20243136172&gbraid=0AAAAADrbLlgO0kpqYMPhThlLdTwOcFLcR&gclid=Cj0KCQiAnsvXBhCqARIsAHKgGNbBoN82Wys6nRpzejUwxvXapOkhnu5bYxU6HeHkMHgI7gQFWMUO5JcaAgmxEALw_wcB 
||||Total Cost|$906.78
---------------------------------------------------------------------------------------------------------------------------------



## CAD Model - Milena
During the CAD model design process, I reduced the scale of the T-Slot framing system in order to make the length correspond to our needs.

I imported the T-slot:

<img width="1096" height="235" alt="image" src="https://github.com/user-attachments/assets/3e2a6c89-7b5a-435c-b5d5-fe99277b51f7" />

I reduced the sizing with the Insert > Features > Scale function.

<img width="936" height="199" alt="image" src="https://github.com/user-attachments/assets/e7d22159-8d1f-4ca0-8d8c-745684821a99" />

Next, I imported all components into an assembly. I copy and pasted any parts corresponding to their required amounts.

<img width="1645" height="943" alt="image" src="https://github.com/user-attachments/assets/bf47e2a9-b15c-4d75-a7a7-807e2ad5e8a6" />

Then, I edited the parts' relations to one another. I matched the surfaces with mating features in order to make a sturdy geometry.

<img width="1300" height="772" alt="image" src="https://github.com/user-attachments/assets/a7452e51-484f-4eb3-8844-1122e59998be" />

This is what the final assembly with all the parts provided and the crosshead looks like.

From the front:

<img width="950" height="485" alt="Screenshot 2026-11-11 130505" src="https://github.com/user-attachments/assets/7d4f72a9-30fe-416c-ad41-3107aa0e6c7f" />

In isometric view:

<img width="950" height="485" alt="Screenshot 2026-11-11 130516" src="https://github.com/user-attachments/assets/8ddd9f37-246a-4b86-8029-5efd373c2274" />


## MEGR 2157

## FEA - Yazahira

For the FEA I  took the crosshead that was designed by Milena and added the load and proper fixed features on it. 


<img width="960" height="504" alt="Screenshot 2026-11-11 164231" src="https://github.com/user-attachments/assets/1ffe74d8-705d-430e-9c20-d945e19b3ea0" />



I created a medium coarse mesh to run the first FEA on this part. 



<img width="960" height="504" alt="Screenshot 2026-11-11 164442" src="https://github.com/user-attachments/assets/7f4d2d1f-4801-4610-b4a1-4d5549ba0494" />

After running my simulation these where the graphs provided for Von Misses stress and Deflection. Based on the the values derived the safety factor is 9.5.


<img width="960" height="504" alt="Screenshot 2026-11-11 164650" src="https://github.com/user-attachments/assets/6c58754a-7cc9-404c-b7f8-1d52104c1710" />


<img width="960" height="504" alt="Screenshot 2026-11-11 164719" src="https://github.com/user-attachments/assets/fa2b748e-f2bc-47a0-869d-e7fe6e23e9ab" />



I followed by running a second study this time with a finer mesh. Below are the graphs provided after running the study. The safety factor after this study is 2.4. 



<img width="960" height="504" alt="Screenshot 2026-11-11 165452" src="https://github.com/user-attachments/assets/b2a8a476-55bf-4b79-a0d8-6f02c0c7ac5f" />


<img width="960" height="504" alt="Screenshot 2026-11-11 165530" src="https://github.com/user-attachments/assets/4f2e74dc-fb38-4ec8-a931-ff0e8c8024e9" />


<img width="960" height="504" alt="Screenshot 2026-11-11 165538" src="https://github.com/user-attachments/assets/ffaea6bc-7d7b-421d-9d97-aaef74507d33" />


After calculating the values for convergence 

Stress = 1.18%

Displacement = 0.12%

SF = 1.19%

They are all below 7% which means they converged. 


Even though there was convergence I decided to make the piece thicker, from 1 in to 1.5 inches. I though this would help decrease the max stress in the middle of the part. I did make sure that after this change the part still met the constrains required. 


I created a fine mesh to begin the simulation.


<img width="960" height="504" alt="Screenshot 2026-11-11 170017" src="https://github.com/user-attachments/assets/64299d17-402d-4053-887a-6270ba12ffce" />



After running the simulation these were my final graphs for stress and displacement. 



<img width="960" height="504" alt="Screenshot 2026-11-11 170053" src="https://github.com/user-attachments/assets/92ef460c-d7a3-4e23-9af7-292e2c6e7df2" />


<img width="960" height="504" alt="Screenshot 2026-11-11 170100" src="https://github.com/user-attachments/assets/e7abbeac-5795-4895-bc67-f9269ad3829d" />


## Crosshead Drawing - Milena

I designed the crosshead drawing according to ASME Y14.5 standards. The link to the file is at the end of the document.

<img width="1048" height="816" alt="image" src="https://github.com/user-attachments/assets/1292226f-22f6-480b-b5b5-e737db9412bd" />


## Lessons Learned - Yazahira

We learned a lot of important lessons with this assigment. The most important lesson we learned was how to properly distrubute the work load and work as a team to assemble everything. We learned how to use axial stress analysis to find the diameter of our leadscrew and choose one that would align with our design. We learned how to use thread bending stress analysis to choose a nut that would fit our lead screw properly. Learning how to properly assemble all of these parts and make them work together in SolidWorks was also a big skill that we got to practice since we havent done many assembly assignments. We spent a lot of time selecting a proper material for the crosshead and we learned how many aspects go into that selction such as loading force, longevity and availability. Finally we spent approximatly 15 hrs on this assigment as a whole. 



## Links to Assembly and Components

Crosshead-

[A10-Crosshead.zip](https://github.com/user-attachments/files/34715581/A10-Crosshead.zip)

Modified T-Slot Frame-

https://drive.google.com/file/d/17JVSgx9yDsT-I6QQELfhOLy1jh88mmQO/view?usp=sharing

Assembly- 

[A10_Assembly.zip](https://github.com/user-attachments/files/34715612/A10_Assembly.zip)

Crosshead Drawing-

https://drive.google.com/file/d/1nJXs743CZaL6XLMNCWTA-TmUF-NGBPkc/view?usp=sharing


# A6 – Bracket Drawing

## Objective

The goal of this assignment is to create a bracket that will hang on a T beam in Solidworks. We are supposed to use calculations from the last assignment. 

<img width="702" height="397" alt="image" src="https://github.com/user-attachments/assets/e09f4f91-21bb-4527-af43-860a4516d587" />

<img width="569" height="474" alt="image" src="https://github.com/user-attachments/assets/91ceea82-648d-481d-8ecb-b9e83b2d9912" />

It is also expected to make a Link that will fit this bracket:

<img width="453" height="492" alt="image" src="https://github.com/user-attachments/assets/6eaf1daf-9a02-45ae-860c-f97add6efc91" />

## Preliminary Calculations
Due to incompleteness of the previous assignment from my part, I decided to redo the strength calculations for the individual features on the bracket.

<img width="558" height="409" alt="image" src="https://github.com/user-attachments/assets/32a901af-de45-41d4-9f36-0122038b52a7" />

<img width="505" height="551" alt="image" src="https://github.com/user-attachments/assets/34e3d226-a952-48b6-a861-1849de6975c1" />

<img width="541" height="749" alt="image" src="https://github.com/user-attachments/assets/96a6ed46-14e6-4932-bbb6-c3e6684295b4" />

<img width="570" height="441" alt="image" src="https://github.com/user-attachments/assets/d2c5caff-6a9f-405f-9a61-50623535053a" />

<img width="831" height="535" alt="image" src="https://github.com/user-attachments/assets/be0a0d88-4c1d-457e-9aa3-ad666165180e" />


## PARAMETRIC DESIGN
In the following pictures, I designed my bracket and overcame... situations.

<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/09d62103-0aae-424b-ba00-63cb72413b8d" />

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/86e92ee4-cee3-43f3-a096-0b67d23a33bf" />

As I went through, I chose to change my value for f. I had already increased it in my calclations since it was thin and may look unstable, even if the calculations imply that it isn't.

<img width="533" height="187" alt="image" src="https://github.com/user-attachments/assets/893dcc4a-9b7e-44f0-998d-177ad164beb7" />

I also realized that my decimals weren't exact enough.

<img width="1023" height="778" alt="image" src="https://github.com/user-attachments/assets/731cbb4e-682f-48ce-a70e-541de8cbff1a" />

I double checked that my dimensions made sense and moved on to the extrusional features.

The program then crashed on me and erased all of my progress while I was adding the extrusions... What I came back to:

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/0814f827-e147-4833-9424-885ec0167f16" />

I redid everything and realized that to calculate the width of feature B, I accidentally used r instead of 2r. I fixed that dimension and adjusted the widths.
Here are all of the improveddimensions.

<img width="838" height="806" alt="image" src="https://github.com/user-attachments/assets/e64a5e1d-3809-4285-8c6c-1ce91e2a5139" />

<img width="1453" height="938" alt="image" src="https://github.com/user-attachments/assets/ef4166fb-d6aa-4b58-a8e6-8ba1aa4a743b" />

Feature B looked a little thin. I made it 4 times as thick. This is to increase the safety factor in the area.

<img width="931" height="804" alt="image" src="https://github.com/user-attachments/assets/e7908957-98c6-4395-96d0-9e68eb3c2e81" />

I was satisfied with the way it looks. I moved on.

<img width="951" height="298" alt="image" src="https://github.com/user-attachments/assets/d20b25d5-2cf5-48a0-8673-414852ae34d0" />

I configured the material to the T6 aluminum alloy:

<img width="848" height="754" alt="image" src="https://github.com/user-attachments/assets/4106a615-a1a8-4a62-9e4f-91193008bd1e" />

## DRAWING

The drawing process was fairly uneventful. I did not have the templates available at first, but I copy and pasted the path to them into SolidWorks and then I managed to get my hands on some.

<img width="894" height="703" alt="image" src="https://github.com/user-attachments/assets/57ff0ec7-131f-4fbc-a818-8bdbf26bd349" />

This is the finished view of my design drawing. I decided to change the scale from 1:5 to 1:3 to make it easier to look at.

## REFLECTIONS

A) I used the cantilever beam equation Sigma=Force/Area in order to calculate the needed dimensions of feature B. The controlled variable here is the thickness of the feature. There are some equations involved in other parts, such as the sectional part along feature C, having a width 2r+2f where r is the radius of the circle below and f is the thickness of the top-most corners. I actually did mess up the calculation for b at first because I inserted r instead of 2r. I caught myself and was able to change the calculation. It did not affect other calculations however. I did need to manually rework some of the document, so I updated some of the equations spread throughout to match what it needed to be.

B) There is a very tight tolerance at gap a of -0.0005, and a lesser tolerance at the radius of the part of 0.01. The tight tolerance at a is reasonable due to the fact that it is the main surface that will prevent yaw movement of the part. The lower one for the radius makes sense because it is not a geometric value that is essential to the stability of the product in terms of fixation to a surface.
I do have some parts with higher tolerance due to their relationship to gap a. When there are too many low tolerances, engineering production price sky-rockets and the project may not be approved for production until further revision.





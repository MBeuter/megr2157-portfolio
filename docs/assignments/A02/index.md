# A2 – Truss Stress Analysis

## Objective
A light weight planar truss is designed and roughly created in CAD for this assignment. Failure modes for the individual truss members is also discussed.

<img width="555" height="370" alt="image" src="https://github.com/user-attachments/assets/991fb548-33cc-49f2-9e59-e4dfc25c29dd" />

The truss will be based off of this image provided, where A is a pin and B is a roller.

Further:
- The truss members are made of A500 Structural Steel.
- The pins are made of hardened tool steel.

## Analysis
## Truss geometry
In designing the final truss, it took several steps. At times, the forces could not cancel and I was forced to add a member, lest the structure turn dynamic. The following 3 images show the design process, with the third one being the final implemented design.
<img width="631" height="280" alt="image" src="https://github.com/user-attachments/assets/1120487c-fd05-4d43-ba14-2c19f32116f5" />
<img width="525" height="256" alt="image" src="https://github.com/user-attachments/assets/13e1b65f-9cce-4aad-bc59-bb01de6e8845" />
<img width="637" height="400" alt="image" src="https://github.com/user-attachments/assets/b159049e-a12d-4648-b6c3-bd68625b1dfa" />

The corresponding FDBs look as following:

<img width="502" height="420" alt="image" src="https://github.com/user-attachments/assets/1bdf3ef6-8095-4b32-8ee0-5ae56babf254" />

By setting up linear systems, it is possible to calculate most unknown values:

<img width="643" height="712" alt="image" src="https://github.com/user-attachments/assets/4903291d-1644-4d9f-86b0-7ab941756d70" />

The following calculations organize the known and unknown variables for a better overview. This is all symbolically:

<img width="640" height="594" alt="image" src="https://github.com/user-attachments/assets/b13df59c-6773-4d02-a8b8-c544c73a64b5" />

Numerically, we can use the values given for this assignment, where P=30kN, a=0.4m and b=0.3m, to determine some of the values.

<img width="622" height="475" alt="image" src="https://github.com/user-attachments/assets/a7cc45f6-e376-4ee6-b706-488fa1d38de1" />

The image shows the known variables (top) and the unknown variables (bottom). If two of the unknown variables are chosen, we can determine the rest. We choose not to go above the maximum determined (2/3)P value for the following problems.

## Safe Cross-sectional Area of the Members
We calculated the required cross-sectional area of a member to support the maximum internal force of (2/3)P. We used a safety factor of 3.5. The yield strength is researched to be 532MPa for A500 Steel. This is shown symbolically.

<img width="670" height="144" alt="image" src="https://github.com/user-attachments/assets/18719bbb-1f8e-49bd-8581-b4aa184a48e6" />

Numerically, we receive these values:

<img width="672" height="268" alt="image" src="https://github.com/user-attachments/assets/56d7e8e4-a410-43a1-b574-2b7c9d926cf4" />

If we want to approximate the weight of an individual member, utilizing a density of 7850kg/m^3:

<img width="606" height="286" alt="image" src="https://github.com/user-attachments/assets/00e9e6fb-493e-4ec6-bbfb-25d1fe5c0e8e" />

## Pins and Safe Cross-sectional Area of the Pins
With a yield shear strength of 170 ksi and a density of 0.278 lb/in3 and the assumption that elements that are in compression won’t fail in buckling, we determine the cross-sectional area required by the pins. The safety factor is 4.

Here are the knowns and unknown qualities with a sketch:

<img width="199" height="235" alt="image" src="https://github.com/user-attachments/assets/2e67663f-1fd9-4d93-b97a-0a734332a13a" />

The following shows the joint in sketch form.

<img width="373" height="219" alt="image" src="https://github.com/user-attachments/assets/54486648-9348-40cb-a1c2-13d19a4394e8" />

An FBD can be made from this sketch:

<img width="315" height="196" alt="image" src="https://github.com/user-attachments/assets/8b9a080d-b065-4e50-b859-a9d5fbb06ad6" />

With this, the minimum cross-sectional area of a single pin can be calculated. It is 0.02645in^2.

<img width="793" height="211" alt="image" src="https://github.com/user-attachments/assets/9e5658e0-5f5f-4d84-a20a-a0309078591e" />

The minimum thickness can be calculated as well. It is 0.0165cm or 0.006506in.The corresponding diameter of the pins is 1.294cm or 0.5094inch.

<img width="369" height="345" alt="image" src="https://github.com/user-attachments/assets/4dfb85a7-46ea-46e8-91d0-0c26ac9e38d3" />

All pins together will have a weight, as following:

<img width="757" height="159" alt="image" src="https://github.com/user-attachments/assets/3f676579-7d08-48a4-a42c-897dd2f6884a" />

In the following, CAD software was used to create a planar truss.

<img width="1918" height="1078" alt="image" src="https://github.com/user-attachments/assets/d1998c73-27e4-467a-a146-5a3aab4ce3fc" />

A sketch is made, as seen above. The measurements are based off the calculations made prior. 

The preliminary sketch is made:

<img width="1309" height="732" alt="image" src="https://github.com/user-attachments/assets/0f80ce62-d585-4875-a59f-e2389866b00e" />

Edits are made to the overall truss. The members are lengthened and thickened, the joints are made thick enough, the angles are changed, and the correct thickness double-checked to ensure a proper cross-sectional area.

<img width="1105" height="703" alt="image" src="https://github.com/user-attachments/assets/918aa3df-6427-4fda-9a90-593bc0aba123" />

Assuming the same height as width, the minimum thickness of the truss members should be sqrt(1.316cm^2<)=1.147(2.54)inch=2.914inch, so that is their thickness.

The final result looks like:

<img width="1333" height="693" alt="image" src="https://github.com/user-attachments/assets/d190bb5d-358a-478a-b84a-82427898614a" />

AISI 1015 Steel is used for the model, since it is closest to the A500 steel properties, ensuring that the previous calculations are not too far off for the required metrics.

## Reflection
I learned how to design a truss from scratch and which constraints can affect the choice in individual member directions. I also learned that the material of the truss is important, considering that it can limit the forces that can act on the material and decide its sizing. This means that certain materials can make the overall geometry smaller or thinner with less material overall, saving resources, while maintaining the required standards and restraints. Overall, I learned about the different basics steps that may go into designing a part; initial geometry and expected forces, material choice and structural rigity, safety factors and lastly actual implementation of the design in a CAD software.        

## Additional Work For MEGR 2157:
## Failure Modes of Truss Members and Pins
   
## Truss Members
There are 7 members in the truss. Each of them is either under tension, compression or may fail due to the applied load.

<img width="910" height="514" alt="image" src="https://github.com/user-attachments/assets/6ee4683e-f2df-4c0d-9e1b-d9105385bbd3" />

All of the members have been numbered for simple reference. We will list a) the expected mode of failure, b) whether the material is ductile or brittle, and c) suggest potential improvements for each member.

1) This member is under 

    Identify the expected failure mode (yielding, fracture, or buckling).
    State whether the material is ductile or brittle.
    Support your choice using stress comparisons and simple reasoning.
    Propose a design modification that could reduce the likelihood of this failure.

    Part 2 – Pin Connections

    Identify the expected failure mode of the pin.
    Support your answer with data from credible, known sources.
    Propose a design modification to reduce the likelihood of this failure

From start to finish this assignment took about 8 hours total, which can be divided into 3h of designing and calculations, 2h of creating the piece and editing it, and 3h to take pictures, document, double check, edit and upload the assignment,

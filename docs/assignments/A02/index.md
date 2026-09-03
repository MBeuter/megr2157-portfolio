# A2 – Truss Stress Analysis

## Objective
A light weight planar truss is designed and roughly created in CAD for this assignment. Failure modes for the individual truss members is also discussed.
<img width="555" height="370" alt="image" src="https://github.com/user-attachments/assets/991fb548-33cc-49f2-9e59-e4dfc25c29dd" />
The truss will be based off of this image provided, where A is a pin and B is a roller.

Further:
- The truss members are made of A500 Structural Steel.
- The pins are made of hardened tool steel.

## Analyze
    Truss geometry
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

Numerically, we can use the values given for this assignment, where P=30kN, a=0.4m and b=0.3m.



    Sketch a truss structure by generating the lengths of each element based to support the loads at point C and D.
    Sketch and label a FBD of each joint on the truss.
    Symbolically solve for all internal forces.
    Numerically solve for all internal forces.

    (25pt) Use the largest internal force to calculate the required cross-sectional area of the elements using a safety factor of 3.5, and the yield strength. 

    (2pt) List all the knowns and unknowns.
    (18pt) Symbolically solve for minimum cross-sectional area (without numbers).
    (3pt) Numerically solve for the cross-sectional area.        
    (2pt)Determine the approximate weight of the truss.

        20pt) Determine the cross-sectional area of the connecting pins which are made of hardened tool steel with a yield shear strength of 170 ksi and a density of 0.278 lb/in3. Assume that elements that are in compression won’t fail in buckling.

    Calculate the required cross-sectional area of the pins to withstand the expected shear forces. Design a single shear connection. Use a safety factor of 4.

    (1pt) list all the knowns and quantities and unknowns.
    (2pt) Generate a FBD of the pin with the largest reaction load.
    (14pt) Symbolically solve for minimum cross-sectional area.
    (2pt) Numerically solve for the cross-sectional area        
    (1pt) Determine the approximate combined weight of the pins. 

    (20pt) Utilize CAD software to generate a 3D model of the truss. Model the pins as cylinders with the appropriate cross-sectional areas and lengths.

    Represent the truss minus the pins as one part in CAD.
    Maintain the cross-sectional area of each element at the intersection of the pin joint.
    Ensure that the truss design satisfies the safety factor, weight optimization goal, and geometric constraints while maintaining structural integrity and stability.
    Implement mass properties in the CAD model and determine the predicted weight, accordingly.      
        pt) Detail engineering lesson learned and be specific. Eliminate words like good and bad from this section. Be more articulate. 

    For example, I learned how to design a truss using the yield strength of the material by comparing it with the external stress of the load.

    Instructions:
Research the likelihood of different failure modes in the components of a truss. Cite all sources used. If you use AI, include the exact prompts and responses, and make sure AI is used only as a tool to support—not replace—your own critical thinking.

(10pt) Part 1 – Truss Members
Each truss member is under either tension or compression and may fail due to the applied loading. For each member:

    Identify the expected failure mode (yielding, fracture, or buckling).
    State whether the material is ductile or brittle.
    Support your choice using stress comparisons and simple reasoning.
    Propose a design modification that could reduce the likelihood of this failure.

    Part 2 – Pin Connections

    Identify the expected failure mode of the pin.
    Support your answer with data from credible, known sources.
    Propose a design modification to reduce the likelihood of this failure

## Decide
_Which geometry did you select, and why? This is your first open design choice in the course — defend it._

## Communicate


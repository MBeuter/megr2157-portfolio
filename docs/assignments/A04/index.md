# A4 – Motor Mount Design

## Objective
The objective of this assignment is to design a motor mount using the (Brushed 24V DC Gear Motor 3.6Kg.cm/46RPM w/ 99.5:1 Planetary Gearbox) HERE which attaches to the rigid wall.

<img width="826" height="633" alt="image" src="https://github.com/user-attachments/assets/c85a35aa-0c62-430a-b8fd-b1e9e892cf0f" />

I chose PLA as a motor mount material.
Cantilever beam formulas shall be used alongside a safety factor of 3. The maximum deflection may be 0.3mm. P is 300N.


## Feature 1 & Feature 2
First I made a sketch of the problem.

<img width="160" height="87" alt="image" src="https://github.com/user-attachments/assets/1b6add6b-f4a1-4d67-af88-1d9877e2d2fc" />

Then I calculated the max numbers with variables.

<img width="646" height="346" alt="image" src="https://github.com/user-attachments/assets/55a1c64c-55b0-42af-b4c1-07f669453f30" />

Based on the technical document featuring the motor, I made desugn choices for the lengths and used the previously derived formulae. The E for PLA is around 3,500GPa. The cross section of the beam is 144mm^2.

<img width="541" height="255" alt="image" src="https://github.com/user-attachments/assets/29935b8f-9527-4b9a-9ebf-937e96173296" />

<img width="744" height="304" alt="image" src="https://github.com/user-attachments/assets/b8dc297c-b4a2-47a4-8868-8dc46927d253" />

It was determined that the calculated deflection was too high, so measurements need to be changed.

I calculated for the required b, then changed my values.

<img width="423" height="475" alt="image" src="https://github.com/user-attachments/assets/235ea84f-4019-4752-8848-b99424f6a49e" />

My maximum deflection is now 0.272mm, which is within the required 0.3mm range.

# Sketch
A sketch was made with the measurements calculated in the previous section:

<img width="502" height="468" alt="image" src="https://github.com/user-attachments/assets/d76dc41e-c539-4598-ac86-4ce3e66cdd85" />

# CAD Model
I converted everything into inches and made a representation of the motor mount on Solidworks.

<img width="1248" height="843" alt="image" src="https://github.com/user-attachments/assets/bb5197e0-81e0-4e31-87e8-57a59a75597e" />



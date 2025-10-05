# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean function minimization is the process of simplifying Boolean algebraic expressions to reduce the number of logic gates and complexity in a digital circuit, leading to more efficient, faster, and less costly hardware

For minimizing Boolean expressions,we can use a set of rules and laws (like distributive, associative, and complement laws) to simplify Boolean expressions. This method focuses on applying algebraic manipulations to reduce the complexity of the expression by eliminating redundant terms.


Identity Law	A ⋅ 1 = A, A + 0 = A

Null Law	A ⋅ 0 = 0, A + 1 = 1

Idempotent Law	A ⋅ A = A, A + A = A

Complement Law	A ⋅ A′ = 0, A + A' = 1

Distributive Law	A ⋅ (B + C) = A ⋅ B + A ⋅ C

De Morgan’s Law	(A ⋅ B)′ = A′ + B', (A + B)′ = A′ ⋅ B′

Absorption Law	A ⋅ (A + B) = A, A + (A ⋅ B) = A

Associative Law A + (B + C) = (A + B) + C, A.(B.C) = (A.B).C

Commutative law A B = B A,A + B = B + A


**Logic Diagram**

Identity Law


<img width="773" height="404" alt="image" src="https://github.com/user-attachments/assets/ee03b072-d12d-4316-bccb-25f30d794241" />


Idempotent Law


<img width="189" height="135" alt="image" src="https://github.com/user-attachments/assets/9583b752-472d-4695-b4bc-cdf91ff5e373" />


Complement Law


<img width="206" height="130" alt="image" src="https://github.com/user-attachments/assets/f496bf36-4a72-4b1e-8069-0fed06ea2866" />


Distributive Law	


<img width="527" height="140" alt="image" src="https://github.com/user-attachments/assets/a575682e-5533-4511-b359-7044bda2ed85" />


De Morgan’s Law


<img width="700" height="270" alt="image" src="https://github.com/user-attachments/assets/a83e7a79-8da7-4b8c-ac39-19b3315e39cc" />


<img width="700" height="270" alt="image" src="https://github.com/user-attachments/assets/feea9c93-2a80-4de0-bdc2-44993e071e8c" />


Absorption Law	


<img width="365" height="79" alt="image" src="https://github.com/user-attachments/assets/98601cb8-d805-438b-a684-970277dc076b" />


Associative Law 


<img width="295" height="301" alt="image" src="https://github.com/user-attachments/assets/a413bfed-04c2-4d97-a431-6a1e81a4bf40" />


Commutative law 


<img width="270" height="277" alt="image" src="https://github.com/user-attachments/assets/6dd84e0f-d5de-4ef3-8957-b5f6177e21ee" />


Null law


<img width="537" height="261" alt="image" src="https://github.com/user-attachments/assets/a0d2df72-4e06-408e-b09c-711b04792a5c" />











**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

i)

module funct1(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule


ii)

module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule

**RTL realization**

**Output:**
i)

<img width="1880" height="1006" alt="Screenshot 2025-10-05 193245" src="https://github.com/user-attachments/assets/15a4a9f6-2d39-4752-aa0f-cf46bd8bdffa" />

ii)

<img width="1920" height="1018" alt="Screenshot 2025-10-05 194036" src="https://github.com/user-attachments/assets/33153ffe-9b82-460d-888d-0d4f8ea0395e" />

**RTL**

**Timing Diagram**
i)

<img width="1918" height="1014" alt="Screenshot 2025-10-05 193224" src="https://github.com/user-attachments/assets/2c6cdfac-9e26-4016-855e-fc093da18c58" />

ii)

<img width="1920" height="1018" alt="Screenshot 2025-10-05 194003" src="https://github.com/user-attachments/assets/61d67c2e-c936-4705-9a10-1c7d2ee89a40" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


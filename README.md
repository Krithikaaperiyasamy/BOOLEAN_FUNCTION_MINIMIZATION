# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

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


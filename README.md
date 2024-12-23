# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Theory**

Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions
**MINIMIZATION**
![WhatsApp Image 2024-12-21 at 08 55 30_08931644](https://github.com/user-attachments/assets/64027da4-d07a-40aa-92a8-71ca8cd7858d)
![WhatsApp Image 2024-12-21 at 08 55 43_e806439e](https://github.com/user-attachments/assets/c9d9a616-3261-41bf-a6ef-604533f793bd)

**TRUTH TABLE**
TRUTH TABLE:
i)	F1
A	B	C	D	F1
0	0	0	0	1
0	0	0	1	0
0	0	1	0	1
0	0	1	1	0
0	1	0	0	0
0	1	0	1	1
0	1	1	0	0
0	1	1	1	1
1	0	0	0	1
1	0	0	1	0
1	0	1	0	1
1	0	1	1	0
1	1	0	0	1
1	1	0	1	1
1	1	1	0	0
1	1	1	1	0

ii)	F2
W	X	Y	Z	F2
0	0	0	0	0
0	0	0	1	1
0	0	1	0	0
0	0	1	1	0
0	1	0	0	0
0	1	0	1	1
0	1	1	0	1
0	1	1	1	1
1	0	0	0	0
1	0	0	1	1
1	0	1	0	1
1	0	1	1	1
1	1	0	0	0
1	1	0	1	1
1	1	1	0	1
1	1	1	1	1


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Developed by: b r Swetha Nivasini
RegisterNumber:24900367
i)f1
'''
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
'''

ii)f2
'''
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
'''

**RTL**

*f1*

![Screenshot (46)](https://github.com/user-attachments/assets/806ff78a-c3a8-4290-9ce1-16a83ef14486)

*f2*

![Screenshot (48)](https://github.com/user-attachments/assets/81cae870-e3a4-42e7-9b31-8b9da925da36)


  
**Output:**
*f1*

![Screenshot (47)](https://github.com/user-attachments/assets/4bd03106-aa51-43c1-b014-d1a24e2e3806)

*f2*
![Screenshot (49)](https://github.com/user-attachments/assets/3193f834-7ce4-48a8-a691-01d1f7d31079)




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


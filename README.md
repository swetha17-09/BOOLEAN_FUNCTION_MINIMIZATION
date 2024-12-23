# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II, USB flasher

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
'''
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule '''


**output**
![Screenshot (47)](https://github.com/user-attachments/assets/b253c963-a1c6-48c7-bea6-049c884b7c5c)

**RTL**
![Screenshot (46)](https://github.com/user-attachments/assets/cb93c950-2438-48d9-a3e7-aee98502c7a4)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


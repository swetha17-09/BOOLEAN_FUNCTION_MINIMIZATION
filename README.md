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
Developed by: RegisterNumber:24900367

'''module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule '''

ii)
''' module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule '''


**RTL realization**
![Screenshot (46)](https://github.com/user-attachments/assets/a7bf0260-9a48-4555-81ff-4600ca3b0ce9)
![Screenshot (48)](https://github.com/user-attachments/assets/504b5a2b-3172-4454-a33c-d5b823e11d0b)


**Output:**

![Screenshot (47)](https://github.com/user-attachments/assets/a308438d-e2b3-4268-828f-83b04ecc0461)
![Screenshot (49)](https://github.com/user-attachments/assets/cf86305a-40ab-48bc-a877-0db57a966d92)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


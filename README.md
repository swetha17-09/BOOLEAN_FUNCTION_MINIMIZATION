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
'''module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule '''

''' module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule   '''




**RTL realization**
![Screenshot (48)](https://github.com/user-attachments/assets/f2dcbc26-efee-4043-af74-6197503d59a5)
![Screenshot (46)](https://github.com/user-attachments/assets/8ba63397-b652-4302-ba6f-a319d92ddbab)


**Output:**
![Screenshot (49)](https://github.com/user-attachments/assets/fe9fd726-14c8-4d0e-b616-400cfdde8c97)
![Screenshot (47)](https://github.com/user-attachments/assets/a821f274-9e3c-4bca-9804-bf3b9fc38b9f)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


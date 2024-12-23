# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions
**minimisation**
F1

![WhatsApp Image 2024-12-21 at 08 55 31_fcac11b5](https://github.com/user-attachments/assets/dd620181-e169-4ab9-b441-e7467c4c32b6)

F2

![WhatsApp Image 2024-12-21 at 08 55 44_d57584cd](https://github.com/user-attachments/assets/3f30937c-4f03-4076-904b-ee11257b403d)


**Logic Diagram**
![TRUTH TABLE (1)](https://github.com/user-attachments/assets/30f4e2ff-a85f-40af-ae9e-7506b1af19ea)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**


Developed by:SWETHA NIVASINI
RegisterNumber:24900367
F1

```
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```


F2

```
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```




**RTL realization**
  F1 
  
  ![Screenshot (46)](https://github.com/user-attachments/assets/31f5f1d5-f8c4-4b01-9097-720045a19511)

  F2

  ![Screenshot (48)](https://github.com/user-attachments/assets/a0844ec9-54dc-4c19-bc92-16f782e11a45)


  
**Output:**

F1
![Screenshot (47)](https://github.com/user-attachments/assets/3c33645a-0a1e-47ad-9251-55e8413117e9)

F2

![Screenshot (49)](https://github.com/user-attachments/assets/8aaaf821-ab17-4350-bf06-01d6cc81e4e2)





**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II, USB flasher

**Software – Quartus prime**

**Theory**

Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions

**Logic Diagram**

![TRUTH TABLE (1)](https://github.com/user-attachments/assets/15f999b3-a0e8-4513-a7fb-387751e5da60)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
developed by: B R SWETHA NIVASINI 
Registration number: 24900367

F1 



``` module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule ```


F2


```module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule  ```



**RTL**
F1

![Screenshot (46)](https://github.com/user-attachments/assets/b1fd313a-5dc5-429b-8b0a-8025d47e04e3)


F2

![Screenshot (48)](https://github.com/user-attachments/assets/849890f0-8858-4668-b6d1-6a0e792222c9)




**output**


F1 


![Screenshot (47)](https://github.com/user-attachments/assets/b253c963-a1c6-48c7-bea6-049c884b7c5c)

F2 

![Screenshot (49)](https://github.com/user-attachments/assets/8e313aba-277d-4ecc-90de-d9236911965d)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


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
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:VEMBARASI.A.R
RegisterNumber:24900729 */
```
```
module EP21(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```
```
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```

**RTL realization**

**Output:**
![Screenshot (80)](https://github.com/user-attachments/assets/65349cd9-f767-455f-96d7-9943f9a69d32)
![Screenshot (82)](https://github.com/user-attachments/assets/b1526d40-1ba4-47fd-95bd-1bd0329a3be5)



**RTL**
![Screenshot (81)](https://github.com/user-attachments/assets/287a5a56-de40-46dc-92d5-3a26bae4b890)
![Screenshot (85)](https://github.com/user-attachments/assets/360518d6-1051-4c17-a3a8-f2783fa4170d)



**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


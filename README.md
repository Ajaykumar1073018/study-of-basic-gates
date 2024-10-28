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

## Developed by: THRIKESWAR P
# RegisterNumber:212222230162
```
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule
```
**Logic Symbol And Truth Table**
![367221898-1448d3a9-cbf9-4c27-b6d5-4fa7c42418fd](https://github.com/user-attachments/assets/0a156975-83c2-4d7a-9833-565119211470)
![367221944-79d67801-6b59-449c-8346-4ecc8b05bca4](https://github.com/user-attachments/assets/4da30fc9-2ba2-4706-bb9c-c7a3d06b5b3a)

**RTL realization**

**Output:**

**RTL**

![image](https://github.com/user-attachments/assets/506314e6-2903-4419-a030-ac10c8f07f58)

**Timing Diagram**

![image](https://github.com/user-attachments/assets/721ee628-65b4-4296-a929-f130162f58aa)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


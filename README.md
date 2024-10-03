# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram and Truth Table**

![image](https://github.com/user-attachments/assets/a24e4f59-f846-44f2-a4d9-856a1fdd5a66)
![image](https://github.com/user-attachments/assets/14a6a432-5360-4988-899b-2a9df028945b)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**


#### Developed by:
S.Sajetha

#### RegisterNumber:
212223100049



```
module Verilog1(A,B,C,D,W,X,Y,Z,F1,F2);
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


![Screenshot (159)](https://github.com/user-attachments/assets/3cc2293e-4599-4c96-950d-059c92ebe6a5)

**Output:**

**RTL**

![image](https://github.com/user-attachments/assets/0c838c25-d477-4097-bba3-8457eebf1daa)

**Timing Diagram**

![Screenshot (160)](https://github.com/user-attachments/assets/989ac378-03d4-45b7-8f67-662cda4d9842)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


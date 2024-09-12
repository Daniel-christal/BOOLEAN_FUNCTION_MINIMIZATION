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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Daniel C 

RegisterNumber: 212223240023
```
module expno2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(~A)&(~C)&(~D);
assign x3=(~B)&(~C)&(~D);
assign x4=(~A)&(~B)&(~C)&(~D);
assign x5=(~B)&(~C)&(~D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```


**RTL realization**

![image](https://github.com/user-attachments/assets/628e7d16-e6cd-4b6b-b3d8-68d33e2df1a4)


**Truthtable**
![image](https://github.com/user-attachments/assets/0d1d0fe6-8e3c-4de0-9000-3eb4a21b8b98)

**Timing Diagram**
![image](https://github.com/user-attachments/assets/84ca0cdf-2b54-4100-a2e6-d973acd39f39)

**Result:**
Thus, the given logic functions are implemented using and their operations are verified using Verilog programming.


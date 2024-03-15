# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: ALAN ZION H
RegisterNumber:212223240004
/*
```
module (A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```

**Output**

![image](https://github.com/ALANZION/BOOLEAN_FUNCTION_MINIMIZATION/assets/145743064/04f3f92f-e2ba-4b8f-a9f6-84d33a7e12fc)

**Waveform**

![image](https://github.com/ALANZION/BOOLEAN_FUNCTION_MINIMIZATION/assets/145743064/1898920b-e32e-44a1-8d01-0dc528cbe4c3)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


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

To implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: P.Rithish

RegisterNumber: 212223230173
```
 module fff(a,b,c,d,w,x,y,z,F1,F2);
input a,b,c,d,w,x,y,z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~a)&(~b)&(~c)&(~d);
assign x2=(a)&(~c)&(~d);
assign x3=(~b)&(c)&(~d);
assign x4=(~a)&(b)&(c)&(d);
assign x5=(b)&(~c)&(d);
assign x6=(x)&(~y)&(z);
assign x7=(~x)&(~y)&(z);
assign x8=(~w)&(x)&(y);
assign x9=(w)&(~x)&(y);
assign x10=(w)&(x)&(y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule


```

**Output:**


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7294b873-be89-4955-8aa6-b64b2a6b9d80" />

 

**Truth table**

 
 <img width="622" height="677" alt="image" src="https://github.com/user-attachments/assets/f6fb4f93-1dcb-4847-9fed-53fb8e6885f3" />


**RTL**

 <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/3fc668e7-015f-47c5-8aee-f82de3c7e1eb" />



**Result:**



Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

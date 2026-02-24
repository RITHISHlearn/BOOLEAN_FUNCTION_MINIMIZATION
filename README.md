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
module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = (~a & ~b & ~c & ~d) |
            (a & ~c & ~d) |
            (~b & c & ~d) |
            (~a & b & c & d) |
            (b & ~c & d);
assign f2 = (x & ~y & z) |
            (~x & ~y & z) |
            (~w & x & y) |
            (w & ~x & y) |
            (w & x & y);
endmodule

```

**Output:**
 <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e00894fd-e93e-45a4-8708-683c61e6cccd" />


**Truth table**

 
<img width="483" height="292" alt="image" src="https://github.com/user-attachments/assets/a642052d-f9bb-4fd0-9e1b-68cef421a9c1" />


**RTL**

 <img width="1915" height="1079" alt="image" src="https://github.com/user-attachments/assets/5c63d105-de35-450d-9688-211f892e563b" />





**Result:**



Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

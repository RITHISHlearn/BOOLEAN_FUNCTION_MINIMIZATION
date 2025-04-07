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

Developed by: A.Pugazh sozhan

RegisterNumber: 212224240121

2a:
~~~

module ex2a(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~a&b&d)|(~b&~d)|(a&b&~c));
endmodule

~~~

2b:

~~~

module ex2b(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y&z)|(x&y)|(w&y));
endmodule

~~~


**Output:**
2a

![WhatsApp Image 2025-04-07 at 13 47 53_3d14af62](https://github.com/user-attachments/assets/15e2961a-41c4-4d22-a43d-d2a3f304a2e5)
2b

![WhatsApp Image 2025-04-07 at 13 47 53_a7550fea](https://github.com/user-attachments/assets/b1b7670f-d398-4a7e-bff4-ed97c84adae3)



**RTL realization**

 2a

 ![image](https://github.com/user-attachments/assets/dddb8603-3dea-4f5e-8c6a-8683bb223f10)

 2b

 ![image](https://github.com/user-attachments/assets/4341ab35-ca6d-4325-b080-91ff78e6ce47)





**RTL**

2a

![image](https://github.com/user-attachments/assets/e823398d-3411-4f2b-988b-1032760bd901)

2b

![image](https://github.com/user-attachments/assets/7b665ec5-cd5b-4181-a623-96d5fdaa0f2b)





**Result:**



Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


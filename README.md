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

Developed by: RegisterNumber:*/
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule


**RTL realization**
<img width="1920" height="1080" alt="Screenshot (74)" src="https://github.com/user-attachments/assets/f06768f8-6811-440f-9f54-bb411699826d" />
<img width="1920" height="1080" alt="Screenshot (79)" src="https://github.com/user-attachments/assets/ea5fcd8e-e1ce-4f15-9386-af844f91c14a" />



**Output:**


**RTL**
<img width="1920" height="1080" alt="Screenshot (75)" src="https://github.com/user-attachments/assets/0c39e5bf-ef93-43cc-8595-46db73aa1862" />
<img width="1920" height="1080" alt="Screenshot (80)" src="https://github.com/user-attachments/assets/9bb04206-0cbb-4c43-bd7a-74fc3015549d" />



**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


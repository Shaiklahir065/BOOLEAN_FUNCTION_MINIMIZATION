# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:shaiklahir RegisterNumber:24005737
        
        i)
        module funct1(a,b,c,d,f1);
        input a,b,c,d;
        output f1;
        assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
        endmodule
        
        ii)
        module funct2(w,x,y,z,f2);
        input w,x,y,z;
        output f2;
        assign f2=((~y & z)|( w & y )|(x & y));
        endmodule


**RTL realization**
![min_fun2](https://github.com/user-attachments/assets/bd01644a-847b-4838-820f-f2c20da19697)


**Timing Diagram**
![Screenshot (11)](https://github.com/user-attachments/assets/8f2b9c82-90ce-4e93-a567-4e42219dbd35)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


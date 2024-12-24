# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**
**Theory**
Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions
**Boolean expression**
i)F1
![WhatsApp Image 2024-12-21 at 11 58 24_3be891b8](https://github.com/user-attachments/assets/54c70d85-ce42-4f68-b23b-8ce391dab067)
ii)F2
![WhatsApp Image 2024-12-21 at 11 58 43_1396de8e](https://github.com/user-attachments/assets/bd3e52e6-aa5e-424d-b373-edd650f99e34)
**Truth Table**
i)F1
![Screenshot 2024-12-24 112344](https://github.com/user-attachments/assets/0ad9c687-f8e7-45f6-b0a3-eb0d7cd72675)
ii)F2
![Screenshot 2024-12-24 112353](https://github.com/user-attachments/assets/02176ea0-62b6-4c7a-a00a-af18fa1cc6bb)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:shaiklahir 
RegisterNumber:24005737
        
        i) F1
        module funct1(a,b,c,d,f1);
        input a,b,c,d;
        output f1;
        assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
        endmodule
        
        ii) F2
        module funct2(w,x,y,z,f2);
        input w,x,y,z;
        output f2;
        assign f2=((~y & z)|( w & y )|(x & y));
        endmodule


**RTL realization**
i)F1
![Screenshot 2024-12-24 112838](https://github.com/user-attachments/assets/0f7b5558-515b-4b74-adbf-d965adb12e33)

ii)F2
![min_fun2](https://github.com/user-attachments/assets/bd01644a-847b-4838-820f-f2c20da19697)


**Timing Diagram**
i)F1
![Screenshot 2024-12-24 113016](https://github.com/user-attachments/assets/0459f26a-c585-4628-a721-0776cc0fa2cd)

ii)F2
![Screenshot (11)](https://github.com/user-attachments/assets/8f2b9c82-90ce-4e93-a567-4e42219dbd35)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


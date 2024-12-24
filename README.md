# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions

**Boolean expression**

i)F1
![WhatsApp Image 2024-12-21 at 11 58 24_eb956024](https://github.com/user-attachments/assets/93ad4242-a4bc-4a01-b255-721ea3b81263)
ii)F2
![WhatsApp Image 2024-12-21 at 11 58 43_37781517](https://github.com/user-attachments/assets/2de52889-36ba-4a8d-b43a-8f311eb0123d)

**Truth Table**


![Screenshot 2024-12-24 112344](https://github.com/user-attachments/assets/1392c3e8-a2d2-4445-9fd6-6eed208a8546)

![Screenshot 2024-12-24 112353](https://github.com/user-attachments/assets/4de1f505-3ff8-4960-8281-0973055d30a6)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:shaiklahir RegisterNumber:24005737
        
        i)F1
        module funct1(a,b,c,d,f1);
        input a,b,c,d;
        output f1;
        assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
        endmodule
        
        ii)F2
        module funct2(w,x,y,z,f2);
        input w,x,y,z;
        output f2;
        assign f2=((~y & z)|( w & y )|(x & y));
        endmodule


**RTL realization**


i)F1

![Screenshot 2024-12-24 112838](https://github.com/user-attachments/assets/d2757c58-a18a-46e3-8923-c5384912bc3a)

ii)F2

![min_fun2](https://github.com/user-attachments/assets/bd01644a-847b-4838-820f-f2c20da19697)


**Timing Diagram**


i)F1

![Screenshot 2024-12-24 113016](https://github.com/user-attachments/assets/8780f45a-4257-465a-a6e2-ccbf3eae0120)

ii)F2

![Screenshot (11)](https://github.com/user-attachments/assets/8f2b9c82-90ce-4e93-a567-4e42219dbd35)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


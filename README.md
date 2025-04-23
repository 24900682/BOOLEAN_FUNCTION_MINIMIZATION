# NAME: ASWIN
# REG NO: 212224230028

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
```
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
```


**Truth Table**

![Screenshot 2025-04-22 191756](https://github.com/user-attachments/assets/b81f5732-e0db-4fde-9759-93feaaaa811e)


![Screenshot 2025-04-22 191817](https://github.com/user-attachments/assets/959a8be7-1d30-4c9f-bb8b-cd169e10899e)


**Output:**

**RTL**

![Screenshot 2025-04-22 191912](https://github.com/user-attachments/assets/8c8c6d77-d5fd-477b-8126-2974288840a9)

![Screenshot 2025-04-22 191949](https://github.com/user-attachments/assets/28a7c741-a7f8-438e-aaef-73b1cf7a1408)


**Timing Diagram**

![Screenshot 2025-04-22 192002](https://github.com/user-attachments/assets/af94d592-89d3-4506-a9bf-6d0253088143)


![Screenshot 2025-04-22 192023](https://github.com/user-attachments/assets/3fd9ed5d-bd01-49fb-a62c-c940aa69d4fe)

**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


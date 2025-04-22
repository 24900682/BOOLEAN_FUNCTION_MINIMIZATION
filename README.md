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
![Screenshot 2025-04-22 191756](https://github.com/user-attachments/assets/4291397a-5330-41fa-968d-81a8358bcd66)
![Screenshot 2025-04-22 191817](https://github.com/user-attachments/assets/9e32002c-e5d3-4f22-9087-66719e4ccf85)

**Output:**
**RTL**
![Screenshot 2025-04-22 191912](https://github.com/user-attachments/assets/7fdf5944-4c50-4a89-9b5a-a20bf0a4355d)
![Screenshot 2025-04-22 191949](https://github.com/user-attachments/assets/21b79ed8-e925-4126-8347-c1da34cabd58)

**Timing Diagram**
![Screenshot 2025-04-22 192002](https://github.com/user-attachments/assets/8b449439-faba-4326-b54d-c4a612944869)
![Screenshot 2025-04-22 192023](https://github.com/user-attachments/assets/99c64f5b-61c2-4bc0-ab39-2f9da3410861)


**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


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

~~~
**Program:**
i)
module DE2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

ii)
module DE2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Punniyakotti.M 
RegisterNumber:24006503
~~~

**RTL realization**
![de ex 2 rtl](https://github.com/user-attachments/assets/30553ce4-9f1b-4db9-b78e-db72781429a0)
![de ex 2 rtl2](https://github.com/user-attachments/assets/0ac425df-5c1f-4b44-a274-c267228ec907)
**WAVEFORM**
![ex 2 waveform 2](https://github.com/user-attachments/assets/c99f596d-37eb-4851-863d-5e31debfac9a)
![ex 2 waveform](https://github.com/user-attachments/assets/0713224a-aed0-4050-81cf-55cd49b8c7eb)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


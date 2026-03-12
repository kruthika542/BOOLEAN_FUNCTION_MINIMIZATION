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


````
Developed by:KRUTHIKA R
RegisterNumber:212225240075
```

```
module EX2(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)| (~a&b&d)| (a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
```
**RTL realization**
<img width="852" height="477" alt="image" src="https://github.com/user-attachments/assets/7835b94e-2833-40be-95d5-4d8b47303d46" />

**RTL**
<img width="1050" height="558" alt="image" src="https://github.com/user-attachments/assets/ce76e8c2-a8b5-475e-9c83-dbe9e20ef3ab" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


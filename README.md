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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

## Developed by: Jaiyantan S
## RegisterNumber: 212224100021


```python
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule

```



**Output:**
![434138303-e84a837f-65e0-4837-ae7f-7e058b5bd6e7](https://github.com/user-attachments/assets/e51427d0-c5c2-4487-9851-c5caed6c9ec5)
![434138350-ea96cd46-b063-4cd3-a460-8015ebe62033](https://github.com/user-attachments/assets/887567ad-1fc2-49a1-8838-c462038b6a9e)

**RTL**

![434138460-e421164b-8abc-4f36-8f83-2a3e9ef35532](https://github.com/user-attachments/assets/1d823175-0c69-4206-9649-a6eb6020a7f3)

**Waveform**
![434138863-ac2a1b7e-06d0-4f7f-bb80-b40f5403899f](https://github.com/user-attachments/assets/e887bd4b-f2ea-4473-a979-cf5538126389)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


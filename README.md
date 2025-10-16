### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.
<img width="368" height="337" alt="image" src="https://github.com/user-attachments/assets/827da65d-7439-467a-8a77-c96676c99b29" />


Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**
<img width="519" height="400" alt="image" src="https://github.com/user-attachments/assets/c0ab08eb-e5a8-4411-b06b-eb2faa03bb31" />


The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below
<img width="857" height="421" alt="image" src="https://github.com/user-attachments/assets/93bd4dc5-d6ca-452e-ab9e-2d873eb54d8a" />


Figure 02  Encoder 8 * 3

**Procedure**
 1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram

**PROGRAM**
 module encoder(a0,a1,a2,d0,d1,d2,d3,d4,d5,d6,d7);
input d0,d1,d2,d3,d4,d5,d6,d7;
output a0,a1,a2;
assign a0=d1|d3|d5|d7;
assign a1=d2|d3|d6|d7;
assign a2=d4|d5|d6|d7;
endmodule

/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by:kavya p
RegisterNumber:25008896*/

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**
<img width="900" height="723" alt="image" src="https://github.com/user-attachments/assets/67cd270b-dd1f-481e-9807-16a71737744f" />


**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
<img width="1358" height="438" alt="image" src="https://github.com/user-attachments/assets/577e136c-6201-4f9f-9aaf-d6abc9736a23" />


**RESULT**

Therefore the code has been successfully executed.




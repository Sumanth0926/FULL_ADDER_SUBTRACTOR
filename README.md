# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

**Procedure**

Write the detailed procedure here

**Program:**

 Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
 Developed by: POTHU SUMANTH
 RegisterNumber:24000831
 
      i)HALF ADDER
      
      module ha(a,b,sum,carry);
      input a,b;
      output sum,carry;
      assign sum= (a ^ b);
      assign carry= ( a & b);
      endmodule

      ii)HALF SUBTRACTOR
      
      module hs(a,b,difference,borrow);
      input a,b;
      output difference,borrow;
      assign difference= (a ^ b);
      assign borrow= ( ~a & b);
      endmodule



**RTL Schematic**
![Screenshot 2024-11-15 135808](https://github.com/user-attachments/assets/14c0b377-5b66-4f34-b7e2-21b3f7a5092e)
![Screenshot 2024-11-15 140712](https://github.com/user-attachments/assets/9bf1c529-04ab-4e86-a869-552fd2dd0a7b)

**Timing Waveform**
![Screenshot 2024-11-15 135909](https://github.com/user-attachments/assets/5990c7a7-c3ae-4109-acc1-839221720e36)
![min_fa](https://github.com/user-attachments/assets/10280c6e-0ff7-419a-a6d6-b4fd4023eadd)

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.




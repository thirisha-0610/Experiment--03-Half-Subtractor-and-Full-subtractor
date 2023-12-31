# Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

## Half Subtractor Full Subtractor
## Half Subtractor
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![half-subtractor9](https://user-images.githubusercontent.com/36288975/166112538-58c3bc7c-ee5d-4e6a-ac8d-8e8328efe27a.png)


Sum = X'Y+XY' = X ⊕ Y
Carry=X'Y

## Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![full-subtractor6](https://user-images.githubusercontent.com/36288975/166112541-24c68359-3de8-4674-ae22-8272ffc385ed.png)


Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

## Procedure
STEP 1: Use module project name(input,output) to start the Verilog programming.

STEP 2: Assign inputs and outputs using the word input and output respectively.

STEP 3: Use defined keyword like wire,assign and required logic gates to represent the boolean expression.

STEP 4: Use each output to represent one for difference and other for borrow.

STEP 5: End the verilog program using keyword endmodule.
## Program:
/*
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.

Developed by: THIRISHA A

RegisterNumber:  23005642*/
Half subtractor:
![image](https://github.com/thirisha-0610/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149347494/953fb981-dee8-40b4-bc96-79bd441bb699)
Full Subtractor:
![image](https://github.com/thirisha-0610/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149347494/688d6a3a-d94f-4dea-8906-188145140c9f)


## Output:
Half subtractor:
![image](https://github.com/thirisha-0610/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149347494/8e87a4f5-4afc-4a5c-b3d7-22b8e8927e85)
Full subtractor:
![image](https://github.com/thirisha-0610/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149347494/6a16c2f8-e68d-4420-b436-4b1ac63683e8)

## Truthtable
Half subtractor:
![image](https://github.com/thirisha-0610/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149347494/56363377-b43d-4608-9c08-84d0e6c473b8)

Full subtractor:
![image](https://github.com/thirisha-0610/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149347494/f651e235-6d13-4b1a-993c-52c9a17c24b4)

##  RTL realization
Half subtractor:
![image](https://github.com/thirisha-0610/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149347494/fef4fdde-90e9-40f8-9005-a54fe80a11da)
Full subtractor:
![image](https://github.com/thirisha-0610/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149347494/8ebd1c52-2ed9-41a3-9eb5-e06635fc0b80)

## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.

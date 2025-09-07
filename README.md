# EXPERIMENT--01-ALP-FOR-8086
Name : S.D. Surendar
Roll no : 212224110052
Date of experiment :29.8.2025





## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition  of 8 bit ALP 

MOV CL,00

MOV AX,[3001H] 

MOV BX,[3003H] 

ADD AX,BX 

JNC Loop

INC CL

Loop:

MOV [3005H],AX 

MOV [3007H],CL 

HLT 

## Output  

<img width="1919" height="1137" alt="addition pmc" src="https://github.com/user-attachments/assets/504a6c1e-5928-40f0-8ad6-7207d27aac2c" />

 
## Subtraction   of 8 bit numbers  ALP 
MOV CL,00

MOV AX,[3001H] 

MOV BX,[3003H] 

SUB AX,BX 

JNC Loop 

INC CL 

NOT AX 

INC AX 

Loop:

MOV [3005H],AX 

MOV [3007H],CL

HLT 
 
## Output  
<img width="1144" height="448" alt="image" src="https://github.com/user-attachments/assets/234a85b5-4cda-4d26-abe7-c12de428b96d" />

## Multiplication alp 
MOV CL,00 

MOV AX,[3001H] 

MOV BX,[3003H]

MUL BX 

MOV [3005H],AX

MOV [3007H],DX

HLT

 ## Output  
<img width="1191" height="594" alt="image" src="https://github.com/user-attachments/assets/f1d29be2-d1e8-41d8-b314-7fefd79634ea" />


## Division alp 
MOV CL,00 

MOV AX,[3001H]

MOV BX,[3003H] 

DIV BX 

MOV [3005H],AX

MOV [3007H],DX 

HLT

## Output  
<img width="1207" height="568" alt="image" src="https://github.com/user-attachments/assets/d3d26f92-f16a-43c5-81c8-db975ff56558" />

Truth table for logic gate:

<img width="702" height="706" alt="logic_gates_truth_table" src="https://github.com/user-attachments/assets/ada4fc7d-c363-47f6-b737-ef16beba9539" />

AND

MOV AX,[3001H] 

MOV BX,[3003H]

AND AX,BX

MOV [3005H],AX

HLT

OUTPUT:
<img width="705" height="429" alt="image" src="https://github.com/user-attachments/assets/65a8f950-873a-4c56-8876-d44f44b1501f" />

OR:

MOV AX,[3001H]

MOV BX,[3003H] 

OR AX,BX 

MOV [3005H],AX 

HLT

OUTPUT:

<img width="623" height="383" alt="image" src="https://github.com/user-attachments/assets/5810564c-19dc-4ee2-887a-33d9660c1c18" />

NOR:
MOV AX,[3001H]

MOV BX,[3003H]

OR AX,BX 

NOT AX 

MOV [3005H],AX 

HLT

OUTPUT:
<img width="1028" height="639" alt="image" src="https://github.com/user-attachments/assets/0e222306-7525-47ba-91fe-bc4a10fc3b1d" />

NOT:

MOV AX,[3001H]

NOT AX 

MOV [3003H],AX 

HLT

OUTPUT:
<img width="1041" height="464" alt="image" src="https://github.com/user-attachments/assets/e85f74a0-a0a8-471b-a0b9-04eb5f805b0e" />

XOR:
MOV AX,[3001H]

MOV BX,[3003H]

XOR AX,BX

MOV [3005H],AX

HLT 

OUTPUT:
<img width="1026" height="638" alt="image" src="https://github.com/user-attachments/assets/c6b712d2-ef2e-4cb0-ae87-30088cbff68c" />

XNOR:

MOV AX,[3001H] 

MOV BX,[3003H] 

XOR AX,BX

NOT AX

MOV [3005H],AX 

HLT

OUTPUT:

<img width="1028" height="639" alt="image" src="https://github.com/user-attachments/assets/bd89384b-d42a-4393-98ed-6c7db8596684" />

NAND:

MOV AX,[3001H] 

MOV BX,[3003H]

AND AX,BX 

NOT AX

MOV [3005H],AX 

HLT

OUTPUT:
<img width="1022" height="598" alt="image" src="https://github.com/user-attachments/assets/9308ed5c-fa1d-4f40-9146-86b1d4c46b63" />




## Result :
 
 Thus the given arithmetic and logical operations have been successfully executed.









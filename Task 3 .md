## task 3 

Step 1: Understand RISC-V Instruction Types
RISC-V instructions are categorized into six primary formats, each serving specific purposes:
R-type: Register-to-register operations (e.g., add, sub, and)
I-type: Immediate operations and loads (e.g., addi, lw, jalr)
S-type: Store operations (e.g., sw, sb)
B-type: Conditional branches (e.g., beq, bne)
U-type: Upper immediate operations (e.g., lui, auipc)
J-type: Unconditional jumps (e.g., jal)

# 1. Initialize a git repository (if not done yet)
git init

# 2. Create a README file (optional but useful)
echo "# RISC-V Disassembly Task 3" > README.md
git add README.md

# 3. Add your disassembly output text file
git add disassembly.txt

# 4. Commit the added files
git commit -m "Added disassembly output for RISC-V Task 3"

# 5. Push to GitHub
git branch -M main
git push -u origin main
##Identify 15 Unique RISC-V Instructions
![task 3(1)](https://github.com/user-attachments/assets/a35172f3-4261-4797-a9cf-cb018e0921cf)
![task 3(2)](https://github.com/user-attachments/assets/d8a5b79d-95ab-4610-9a9b-62f9d5032f5d)
![task 3(3)](https://github.com/user-attachments/assets/e90cbcf8-e7b5-47f2-a045-01f9b9362b82)
![task 3(4)](https://github.com/user-attachments/assets/72f2a2f3-edf9-4654-a97c-e17efa0d63ed)

15 Unique RISC-V Instructions and Their 32-bit Format Decoding
-> R-Type Instructions
1. Instruction: add x5, x6, x7
Type: R-Type
Hex: 00b303b3
Binary: 0000000 00111 00110 000 00101 0110011
Breakdown:

funct7 = 0000000

rs2 = x7

rs1 = x6

funct3 = 000

rd = x5

opcode = 0110011

2. Instruction: sub x5, x6, x7
Type: R-Type
Hex: 40b303b3
Binary: 0100000 00111 00110 000 00101 0110011
Breakdown:

funct7 = 0100000

rs2 = x7

rs1 = x6

funct3 = 000

rd = x5

opcode = 0110011

3. Instruction: and x5, x6, x7
Type: R-Type
Hex: 00f303b3
Binary: 0000000 00111 00110 111 00101 0110011
Breakdown:

funct7 = 0000000

rs2 = x7

rs1 = x6

funct3 = 111

rd = x5

opcode = 0110011

4. Instruction: or x5, x6, x7
Type: R-Type
Hex: 00e303b3
Binary: 0000000 00111 00110 110 00101 0110011
Breakdown:

funct7 = 0000000

rs2 = x7

rs1 = x6

funct3 = 110

rd = x5

opcode = 0110011

5. Instruction: sll x5, x6, x7
Type: R-Type
Hex: 007313b3
Binary: 0000000 00111 00110 001 00101 0110011
Breakdown:

funct7 = 0000000

rs2 = x7

rs1 = x6

funct3 = 001

rd = x5

opcode = 0110011

->I-Type Instructions
6. Instruction: addi x5, x6, 10
Type: I-Type
Hex: 00a30313
Binary: 000000001010 00110 000 00101 0010011
Breakdown:

imm = 000000001010

rs1 = x6

funct3 = 000

rd = x5

opcode = 0010011

7. Instruction: andi x5, x6, 10
Type: I-Type
Hex: 00a31313
Binary: 000000001010 00110 111 00101 0010011
Breakdown:

imm = 000000001010

rs1 = x6

funct3 = 111

rd = x5

opcode = 0010011

8. Instruction: lw x5, 0(x6)
Type: I-Type
Hex: 00032303
Binary: 000000000000 00110 010 00101 0000011
Breakdown:

imm = 000000000000

rs1 = x6

funct3 = 010

rd = x5

opcode = 0000011

🧾 S-Type Instruction
9. Instruction: sw x5, 0(x6)
Type: S-Type
Hex: 00532023
Binary: 0000000 00101 00110 010 00000 0100011
Breakdown:

imm[11:5] = 0000000

rs2 = x5

rs1 = x6

funct3 = 010

imm[4:0] = 00000

opcode = 0100011

-> B-Type Instructions
10. Instruction: beq x5, x6, label
Type: B-Type
Hex: 00530663
Binary: 0000000 00110 00101 000 00010 1100011
Breakdown:

imm[12|10:5|4:1|11] = 000000000010

rs1 = x5

rs2 = x6

funct3 = 000

opcode = 1100011

11. Instruction: bne x5, x6, label
Type: B-Type
Hex: 00531663
Binary: 0000000 00110 00101 001 00010 1100011
Breakdown:

funct3 = 001

Same imm field encoding

rs1 = x5, rs2 = x6, opcode = 1100011

🏗️ U-Type Instructions
12. Instruction: lui x5, 0x10000
Type: U-Type
Hex: 00010537
Binary: 00000000000100000000 00101 0110111
Breakdown:

imm = 00000000000100000000

rd = x5

opcode = 0110111

13. Instruction: auipc x5, 0x10000
Type: U-Type
Hex: 00010517
Binary: 00000000000100000000 00101 0010111
Breakdown:

imm = 00000000000100000000

rd = x5

opcode = 0010111

-> J-Type Instructions
14. Instruction: jal x5, label
Type: J-Type
Hex: 000000ef
Binary: 00000000000000000000 00101 1101111
Breakdown:

imm = [20|10:1|11|19:12]

rd = x5

opcode = 1101111

15. Instruction: jalr x5, 0(x6)
Type: I-Type
Hex: 00030367
Binary: 000000000000 00110 000 00101 1100111
Breakdown:

imm = 000000000000

rs1 = x6

funct3 = 000

rd = x5

opcode = 1100111

![task 3(1)](https://github.com/user-attachments/assets/43b14883-4ad8-43c9-b673-2d84bcf1dc04)
![task 3(2)](https://github.com/user-attachments/assets/6392415d-fd51-471e-82ee-661fb2841f06)
![task 3(3)](https://github.com/user-attachments/assets/9da94a39-2c51-479d-8d12-892a0a02a4a3)
![task 3(4)](https://github.com/user-attachments/assets/8e397410-fd57-4ec8-a566-378495519858)

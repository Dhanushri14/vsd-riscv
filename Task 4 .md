##Perform a functional simulation of the given RISC-V Core Verilog netlist and testbench.

# 1. Go to your project folder
cd ~/riscv_simulation
![task 4(1)](https://github.com/user-attachments/assets/acf9dc61-02f0-46d6-ab1e-413cd84d0150)


# 2. Initialize Git repo
git init

# 3. Add all files
git add .

# 4. Commit the files
git commit -m "Initial commit - Added core.v and core_tb.v"

![task 4(2)](https://github.com/user-attachments/assets/e0d03b0f-3107-446a-acbd-4dd8df97ef8c)
![task 4(3)](https://github.com/user-attachments/assets/8c4975a3-b7c1-4cd4-8f55-0815e51cf1fe)

1. Move the images to your repository folder
-> mv ~/Downloads/task\ 4* ~/Desktop/rv32i/
  ![task 4(4)](https://github.com/user-attachments/assets/03db55b5-bc63-4f4a-9e6d-13a9c226e0ed)
3. Navigate to your Git repository
->cd ~/Desktop/rv32i
![task 4(5)](https://github.com/user-attachments/assets/28f90de8-8db8-4260-afd3-ae6898784f49)
5. Add the images to Git
 ->git add task\ 4* task4\(6\).png
   ![task4(6)](https://github.com/user-attachments/assets/d678e7a6-1703-43b6-b0d7-6bbf56b2c027)
7. Commit the images with a message
 ->git commit -m "Added GTKWave simulation screenshots for Task 4"
   ![task 4(7)](https://github.com/user-attachments/assets/b4cc91a3-6bb6-4c5e-aa7d-e017b846d7e2)
9. Push to GitHub
   git push origin main
   
10. Instruction observed: SUB
Operands: A = 2, B = 3
Result: A - B = -1 (0xFFFFFFFF)
Signal in GTKWave: SUB = 1, output is -1
Added waveform verification for SUB instruction: SUB(2, 3) = -1
![task4(8)](https://github.com/user-attachments/assets/6dd0d34a-2137-4f0d-bb16-66f2ea6dd742)

11.Instruction observed: AND
Operands: A = 0x2, B = 0x5
Result: A & B = 0x1
Signal in GTKWave: AND = 2, result in EX_MEM_ALUOUT = 1
Verified AND instruction: AND(0x2, 0x5) = 0x1
![task4(9)](https://github.com/user-attachments/assets/d34cce98-3460-4eb7-bee8-7142a0c8cf5e)

12.Instruction observed: OR
Operands: A = 0x2, B = 0x5
Result: A | B = 0x7
Signal in GTKWave: OR = 3, output EX_MEM_ALUOUT = 0x7
Verified OR instruction: OR(0x2, 0x5) = 0x7
![task4(10)](https://github.com/user-attachments/assets/3744c3d0-a967-45da-bacc-37ab99069cdf)

13.Verified OR instruction: OR(0x2, 0x5) = 0x7
Operands: A = 0x2, B = 0x5
Result: A ^ B = 0x7
Signal in GTKWave: XOR = 4, output shows 0x7
Verified XOR instruction: XOR(0x2, 0x5) = 0x7
![task 4(11)](https://github.com/user-attachments/assets/088b843d-f96e-4ec5-96ae-53f6519831cd)

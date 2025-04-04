# VSD RISC-V TASK 2
This repository documents the steps to compile and run a RISC-V program using the RISC-V GCC toolchain and the Spike simulator.

## Steps
### 1. Navigate to the Working Directory
cd ~
![riscv task 2](https://github.com/user-attachments/assets/b3ad7a15-df6b-4370-b424-40ea6d29a37a)
2. Compile the C Program for RISC-V
riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
![riscv task 2](https://github.com/user-attachments/assets/92ca9cce-b524-40f7-89af-7c63eece2155)
3. Execute the Compiled Program
./a.out
4. Run the Program using Spike Emulator
spike pk sum1ton.o
![task 2(3)](https://github.com/user-attachments/assets/a9e75926-1d60-49b6-9a2f-935e51415c90)
5. Run in Debug Mode with Spike
spike -d pk sum1ton.o
![task 2(4)](https://github.com/user-attachments/assets/7765d908-ad08-41da-b545-305fa42745e5)


![riscv task 2](https://github.com/user-attachments/assets/cccaa816-9d2b-4d84-aef7-5c476474f519)
![task 2](https://github.com/user-attachments/assets/9e2712dd-527a-4f1c-8670-1a80afcad813)
![task 2(3)](https://github.com/user-attachments/assets/88319b47-ebb3-4d87-bd4f-76125511245f)
![task 2(4)](https://github.com/user-attachments/assets/d2534d4f-3dd7-42a8-a325-9646d0329609)

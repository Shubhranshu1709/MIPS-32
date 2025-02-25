# MIPS-32
The MIPS 32-bit 5-stage pipeline is a classic RISC processor design that divides instruction execution into five distinct stages to improve performance through instruction-level parallelism. The five stages are:

1. Instruction Fetch (IF)
The instruction is fetched from memory using the Program Counter (PC).
The PC is incremented to point to the next instruction.
This stage interacts with the instruction memory.
2. Instruction Decode (ID)
The instruction is decoded to identify the operation.
Registers are read from the Register File (for register operands).
Control signals are generated for the execution stage.
3. Execute (EX)
The Arithmetic Logic Unit (ALU) performs computations such as addition, subtraction, or logical operations.
Branch conditions are evaluated (for branch/jump instructions).
Shift operations are executed here.
4. Memory Access (MEM)
If the instruction is a load (LW) or store (SW), memory is accessed.
If not a memory-related instruction, this stage is bypassed.
5. Write Back (WB)
The result from the ALU or memory is written back into the register file.
Only instructions that modify registers (e.g., ALU ops, loads) perform this step

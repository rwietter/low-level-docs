# RISC (Reduced Instruction Set Computer)

RISC is a type of microprocessor architecture that uses a small, highly-optimized set of instructions, rather than a more specialized set of instructions often found in other types of architectures.

RISC instructions are allocated in memory and executed by the processor. The instructions are executed in one clock cycle, which is the time it takes for the processor to execute a single instruction. This is in contrast to CISC (Complex Instruction Set Computer) architectures, which use a more complex set of instructions that take longer to execute.

RISC architectures are designed to be simple and efficient, and are often used in embedded systems and mobile devices. They are also used in supercomputers, where they are often combined with other architectures to create a hybrid system.

Most RISC instructions involve register addressing without memory access. This means that the instructions are executed directly from the processor's registers, rather than from memory. This allows the processor to execute instructions more quickly, since it does not have to access memory to retrieve the instructions.

LOAD and STORE instructions are used to move data between memory and registers. These instructions are used to load data from memory into a register, and to store data from a register into memory. As LOAD/STORE act between the registers and the memory, the speed is discrepant, as the memory is much slower than the registers, which is where Pipelining comes in.

In each cycle of the processor, the instruction is fetched from memory, decoded, and executed. The pipeline allow to fetch next instruction while the current instruction is being executed. It means that the processor act in parallel.

The instructions have same length of the UCP Architecture e.g. 32 bits. The instructions are divided in 3 parts: opcode, source register and destination register. The opcode is the instruction itself, the source register is the register that will be used to execute the instruction and the destination register is the register that will receive the result of the instruction.

Example of RISC Architecture:

- ARM (embedded systems and mobile devices)
- Intel i860 and i960
- MIPS (game consoles, routers, etc.)
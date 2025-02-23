# PIPELINED-PROCESSOR

COMPANY NAME:CODE TECH IT SOLUTIONS PVT.LTD

NAME:GudipalliMounika

INTERN ID:CT12GUG

DOMAIN:VLSI

BATCH DURATION:January 20th,2025 to March 20th,2025

MENTOR NAME: NEELA SANTHOSH

DESCRIPTION:Verilog module implements a basic pipelined processor with a 5-stage pipeline:

Instruction Fetch (IF)
Instruction Decode (ID)
Execute (EX)
Memory Access (MEM)
Write Back (WB)
Registers and Memory

Instruction Memory (instruction_memory): Stores machine instructions.
Data Memory (data_memory): Stores data used during execution.
Registers (registers): Holds temporary values used in operations.
Pipeline Registers (IF_ID_instr, ID_EX_instr, EX_MEM_result, MEM_WB_result): Hold intermediate values at each pipeline stage.

Instruction Fetch (IF)
Fetches the instruction from instruction_memory.
Stores it in IF_ID_instr for the next stage.

 Instruction Decode (ID)
Reads the fetched instruction (IF_ID_instr) and moves it to ID_EX_instr.

 Execute (EX)
Decodes the instruction and performs the corresponding operation.
Stores the result in EX_MEM_result.

 Memory Access (MEM)
Moves the execution result to MEM_WB_result.

 Write Back (WB)
Writes the result back into register 2.

Instruction Memory is loaded with:
00000001 (ADD)
00000010 (SUB)
00000011 (LOAD)
00000000 (NOP)

Data Memory is initialized with values 0-15.
Registers are initialized with values 0-3.
Simulation and Output
After 10 time units (#10), the final value in register 2 is displayed.


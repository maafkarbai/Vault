## **1. Overview of the Cycle**

The CPU executes programs by repeatedly performing these four steps for each instruction:

1. **Fetch**: Retrieve the instruction from memory.
2. **Decode**: Understand what the instruction means and determine required actions.
3. **Execute**: Carry out the specified operation.
4. **Store**: Save the result of the operation to memory or registers.

The cycle is controlled by the **Control Unit** and involves several CPU components, including registers, the Arithmetic Logic Unit (ALU), and memory.

---

## **2. The Detailed Stages**

### **Stage 1: Fetch**

- **Goal**: Retrieve the next instruction from memory.
    
- **Process**:
    
    - The **Program Counter (PC)** holds the memory address of the next instruction.
    - The CPU sends this address to the **Memory Address Register (MAR)**.
    - The CPU issues a memory read request, fetching the instruction from memory into the **Memory Data Register (MDR)**.
    - The instruction is then transferred to the **Instruction Register (IR)** for processing.
    - The **PC is incremented** to point to the address of the next instruction.
- **Key Components**:
    
    - **Program Counter (PC)**: Tracks the next instruction.
    - **Memory Address Register (MAR)**: Holds the address of the instruction to be fetched.
    - **Memory Data Register (MDR)**: Temporarily stores the fetched data (instruction).
- **Example**: Fetch the instruction `ADD R1, R2` from memory address `0x1000`.
    

---

### **Stage 2: Decode**

- **Goal**: Interpret the fetched instruction.
    
- **Process**:
    
    - The fetched instruction in the **Instruction Register (IR)** is analyzed by the **Control Unit (CU)**.
    - The Control Unit decodes the operation code (**opcode**) to determine the type of operation (e.g., arithmetic, logic, data movement).
    - It identifies the operands (data) required for the operation:
        - Where the data is located (memory, registers, or immediate values).
        - How many operands are needed.
    - Signals are generated to prepare the CPU for execution (e.g., activate the ALU or load data into registers).
- **Key Components**:
    
    - **Instruction Register (IR)**: Holds the fetched instruction.
    - **Control Unit (CU)**: Decodes the instruction and prepares control signals.
- **Example**: Decode `ADD R1, R2`:
    
    - Opcode: `ADD` (Addition operation).
    - Operands: `R1` and `R2` (values in registers).

---

### **Stage 3: Execute**

- **Goal**: Perform the operation specified by the instruction.
    
- **Process**:
    
    - The decoded operation is carried out by the CPU.
    - If it’s an arithmetic or logical operation:
        - The **Arithmetic Logic Unit (ALU)** performs the computation.
    - If it’s a data movement operation:
        - Data is transferred between memory and registers.
    - If it’s a control instruction:
        - The PC may be updated (e.g., for jumps or branches).
- **Key Components**:
    
    - **Arithmetic Logic Unit (ALU)**: Performs mathematical and logical operations.
    - **Registers**: Provide fast access to operands and intermediate results.
- **Example**: Execute `ADD R1, R2`:
    
    - Add the values in `R1` and `R2`.
    - Store the result temporarily in a register or in the ALU output.

---

### **Stage 4: Store**

- **Goal**: Save the result of the executed instruction.
    
- **Process**:
    
    - The result of the operation is written back to:
        - A **register**, for quick access in subsequent operations.
        - A **memory location**, if required.
    - This step ensures the result is available for further processing or program output.
- **Key Components**:
    
    - **General Purpose Registers (GPRs)**: Temporarily hold data or results.
    - **Memory**: Stores data persistently.
- **Example**: Store the result of `ADD R1, R2`:
    
    - Write the sum back to `R1` or another specified register.

---

## **3. Supporting CPU Components**

### **Control Unit (CU)**

The "brain" that orchestrates the cycle:

- Directs the fetching and decoding of instructions.
- Generates signals to control data flow within the CPU and between the CPU and memory.

### **Registers**

- **Program Counter (PC)**: Tracks the address of the next instruction.
- **Instruction Register (IR)**: Holds the current instruction.
- **General Purpose Registers (e.g., R1, R2)**: Temporarily store data for operations.

### **Arithmetic Logic Unit (ALU)**

- Executes mathematical and logical operations during the Execute stage.

### **Memory**

- Stores instructions and data for the program being executed.

---

## **4. Full Cycle Example**

Suppose the program includes the instruction `ADD R1, R2`. Here’s how it works:

1. **Fetch**:
    
    - The PC points to address `0x1000`, where the instruction `ADD R1, R2` is stored.
    - The CPU fetches this instruction from memory into the IR.
    - The PC is incremented to `0x1004` (assuming 4 bytes per instruction).
2. **Decode**:
    
    - The Control Unit decodes the instruction:
        - Opcode: `ADD`.
        - Operands: `R1` (destination register) and `R2` (source register).
3. **Execute**:
    
    - The ALU performs the addition of the values in `R1` and `R2`.
4. **Store**:
    
    - The result of the addition is written back to `R1`.
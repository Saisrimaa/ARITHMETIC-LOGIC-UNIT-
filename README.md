# ARITHMETIC-LOGIC-UNIT-

**COMPANY** :CODTECH IT SOLUTIONS

**NAME** :B.SAISRIMA

**INTERN ID** :CT04DM37

**DOMAIN** : VLSI

**DURATION** : 4 WEEKS

**MENTOR** : NEELA SANTHOSH

#DESCRIPTION :

### **Design and Implementation of a Basic ALU**

The goal of this project was to design and simulate a basic Arithmetic Logic Unit (ALU) capable of performing fundamental arithmetic and logical operations: **addition**, **subtraction**, **bitwise AND**, **bitwise OR**, and **bitwise NOT**. The ALU is a critical component of any processor, serving as the computational engine for executing instructions. This ALU design forms a foundational block for more complex CPU architectures and was implemented with clarity and simplicity to demonstrate key digital logic concepts.

The design process began with identifying the operations the ALU needed to support. These included:

* **Addition**: Computes the sum of two 8-bit inputs.
* **Subtraction**: Computes the difference between two 8-bit inputs.
* **AND**: Performs a bitwise AND operation on two inputs.
* **OR**: Performs a bitwise OR operation on two inputs.
* **NOT**: Performs a bitwise NOT operation on one input.

The ALU accepts two 8-bit inputs (A and B) and a 3-bit **operation select code**. The select code determines which operation the ALU will execute. For example:

* `000`: ADD
* `001`: SUB
* `010`: AND
* `011`: OR
* `100`: NOT A

A **case-based approach** was used to evaluate the opcode and determine the result. In hardware design languages like Verilog or VHDL, this would be implemented using a `case` or `if-else` statement in an `always` block. For simulation and prototyping purposes, the ALU was modeled in Python to allow easy visualization and debugging.

Here's a high-level overview of the implementation steps:

1. **Input Declaration**: Two 8-bit binary values are defined as inputs to the ALU. A 3-bit opcode input is used to control the operation mode.
2. **Operation Logic**: Depending on the opcode, the corresponding operation is performed:

   * Addition and subtraction are implemented using Python’s arithmetic operators.
   * Bitwise operations are done using `&`, `|`, and `~` operators.
3. **Output Assignment**: The result of the selected operation is stored in an output variable, and optionally, status flags such as `zero`, `carry`, or `negative` could be added for enhanced functionality.
4. **Testing**: A simple simulation loop was written to test all operations with example input values. This helped verify correctness and ensured all outputs behaved as expected.

The simulation results confirmed that the ALU correctly computed each operation. For instance, given A = 15 and B = 10:

* ADD produced 25
* SUB produced 5
* AND produced 10
* OR produced 15
* NOT A produced the bitwise complement of 15

This project emphasized modularity, clarity, and extensibility. The ALU is easily extendable to include more operations like XOR, NOR, shifts, or multiplication. It can also be synthesized in an HDL for FPGA or ASIC design.

**OUTPUT** :

![Image](https://github.com/user-attachments/assets/681c4148-a49e-4de6-87f6-0765b89250f7)

Overall, designing this ALU helped reinforce the principles of combinational logic, binary arithmetic, and the structure of computational units in modern processors.

**OUTPUT** :



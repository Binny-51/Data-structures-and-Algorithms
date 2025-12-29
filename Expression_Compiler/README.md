## 🧮 Expression Compiler (E++ Compiler)

**Description:**  
Implemented a compiler for a custom expression language **E++**, supporting variable assignments, arithmetic expressions, and control statements such as **delete** and **return**. The compiler parses tokenized expressions into **expression trees**, maintains a balanced **AVL-tree–based symbol table**, and generates executable code for a **stack-based target machine (Targ)**.

**Key Features:**
- Parsing of tokenized E++ expressions into structured **expression trees**
- Support for:
  - Variable assignment
  - `delete` statements for symbol removal
  - `return` statements to terminate execution and return computed values
- **AVL Tree–based Symbol Table** for efficient variable lookup, insertion, deletion (`O(log n)`)
- Dynamic memory address allocation and deallocation during compilation
- Recursive code generation for a **stack machine–based target language**
- Optional optimization using a **min-heap** to assign the least available memory index

**Core Data Structures Used:**
- AVL Trees (Symbol Table)
- Expression Trees
- Heaps (for optimized memory allocation)
- Stacks (Target Machine Model)

**Technologies:**
- C++
- Tree Rotations (LL, RR, LR, RL)
- Compiler Design Principles
- Stack-based Code Generation


# cflat-compiler

This is a course project in CS536

The compiler translates cflat lanaguage (a c-like language) into MIPS assembly code.  

&nbsp;

To compile this project: `make`  
&nbsp;  
To test: `make test`, test.cflat file will be compiled into test.s file, which you can run on any MIPS simulator 

&nbsp;

This project was developed in 5 stages:

&nbsp;

**Stage1: Jlex scanner and regex**  
Use regex to build a scanner that scans the input file into tokens

**Stage2: JCup and parser, Context free grammar**  
Build a parser using pre defined context free grammar, takes tokens into AST

**Stage3: Name Analysis**  
Traverse the AST to build a symbol table. Check if any identifier is declared before use

**Stage4: Type Check**  
Check type of each assignment and operation, make sure no type mismatch

**Stage5: Code generation**  
After passing static analysis, generate the actual assembly code.


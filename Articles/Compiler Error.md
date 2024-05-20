Compiler [[Errors and Exceptions|errors]] are mistakes in a program's source code that prevent it from being successfully [[Compiler|compiled]] into an executable program. When a programmer writes code, they usually write it in a high-level [[programming language]] like [[Python]], Java, or C++. A [[Compiler|compiler]] is a tool that translates this high-level code into [[machine code]] that a [[Computers and Computing|computer]] can understand. If there are errors in the code, the compiler will generate error messages and stop the translation process.

---
#### Types of Compiler Errors

 * **Syntax Errors**: These occur when the code violates the rules of the programming language. For example, if you forget a semicolon at the end of a statement in C++ or misspell a [[keyword]], you'll get a syntax error. Syntax errors are often the easiest to fix because the compiler usually provides specific details about what and where the problem is.
 
 * **Semantic Errors**: These happen when the code is syntactically correct but makes no sense logically. For instance, if you try to perform an operation on incompatible data types (like adding a number to a [[string]] in a language that doesn't allow it), you'll encounter a semantic error. These errors are harder to spot because the code looks correct but doesn't behave as expected.
 
 * **Linker Errors**: These errors occur during the linking stage, which is after the compilation of the code. Linker errors happen when the compiler cannot find the correct references to functions or variables defined in other files or [[libraries]]. This might happen if you forget to include a necessary library or if there is a mismatch in [[Functions|function]] declarations.


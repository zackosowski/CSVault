#article 

**Debugging** is the process of identifying, analyzing, and fixing bugs or [[Errors|errors]] in software. Bugs are flaws or issues in a [[Computers and Computing|computer]] program that cause it to produce incorrect or unexpected results or to behave in unintended ways. Debugging is a critical skill for programmers, as it ensures that software functions correctly and efficiently.

---
#### History and Origin

The term "debugging" dates back to the early days of computing. One famous anecdote involves computer scientist Grace Hopper finding a moth causing issues in the Mark II computer in 1947, which she referred to as a "bug." Removing the moth was called "debugging," and the term has been used ever since.

![[bug1.jpg]]

---
#### Debugging Process

1. **Reproduce the Bug**: The first step in debugging is to reproduce the problem. This means running the program in a way that consistently causes the bug to appear.
2. **Diagnose the Problem**: Next, the programmer needs to understand why the bug occurs. This often involves reading through the error messages, checking for logical errors in the code, and using debugging tools.
3. **Fix the Bug**: Once the cause of the bug is identified, the programmer makes changes to the code to correct the issue.
4. **Test the Solution**: After making a fix, it is crucial to test the program to ensure that the bug is resolved and that no new bugs have been introduced.

---
#### Tools and Techniques

Programmers use various tools and techniques to debug their code:

- **Print Statements**: Adding [[Print Functions|print]] statements in the code to display [[Data|values]] of [[Variables]] and the flow of execution. This is a simple but effective way to understand what the program is doing.
- **Debuggers**: Special software tools, such as gdb (GNU Debugger) for C/C++ or the integrated debugger in [[IDE (Integrated Development Environment)|IDEs]]. These tools allow programmers to step through code line by line, inspect variables, and control the execution flow.
- **Unit Testing**: Writing tests for individual parts of the code (units) to ensure they work correctly. Automated testing frameworks like JUnit for Java or PyTest for [[Python]] are commonly used.
- **Rubber Duck Debugging**: Explaining the code and the problem to a rubber duck (or any inanimate object) as a way to clarify the programmer's thinking and often reveal the bug's source.

---
#### Debugging Golden Question

Sometimes, finding the error in your code can be a confusing and frustrating process. When in doubt, ask yourself the "debugging golden question":

*"What changed since it worked last?"*

---
#### Debugging Tool in VS Code

The debugging tool in [[Visual Studio Code]] can be very powerful in revealing problems with your code. It allows you to "step through" the program line by line so you can see what each line is doing at a human speed, rather than computer speed.

To use the built-in debugger, click the icon on the action bar that looks like a bug with a play button. Alternatively, you can use the shortcut `Ctrl + Shift + D`.

1. Click `Run and Debug`
2. On the dropdown that opens, click `Python Debugger`
3. On the next dropdown, click python current file

###### Breakpoints

Breakpoints pause the code on a specific line, allowing you to "step through" each individual line after that. You can set breakpoints by clicking in the gutter next to the line number, or by pressing `F9` on the desired line. Once the program pauses, you have these options:

- **Continue (F5)**: Resumes program execution until the next breakpoint is encountered or the program ends.
- **Step Over (F10)**: Executes the current line of code and moves to the next line, without entering any called functions.
- **Step Into (F11)**: Steps into the function call on the current line, allowing you to debug inside the called function.
- **Step Out (Shift+F11)**: Completes execution of the current function and returns to the calling function, pausing at the next line of code after the call.
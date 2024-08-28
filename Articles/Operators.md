#article 

In computer science, an operator is a symbol or [[Functions|function]] that tells the [[compiler]] or interpreter to perform a specific mathematical, logical, or relational operation on one or more [[Operators#Operands|operands]]. Operators are essential building blocks of programming languages and enable developers to perform various tasks such as math calculations, comparisons, and [[data]] manipulation. Here are the main types of operators commonly used in programming:

---
#### Arithmetic Operators

An arithmetic operator is a symbol used to perform basic mathematical operations on numerical values.

   - **Addition (+)**: Adds two operands. For example, `5 + 3` results in `8`.
   - **Subtraction (-)**: Subtracts the second operand from the first. For example, `5 - 3` results in `2`.
   - **Multiplication (*)**: Multiplies two operands. For example, `5 * 3` results in `15`.
   - **Division (/)**: Divides the first operand by the second. For example, `5 / 3` results in approximately `1.67`.
   - **Modulus (%)**: Returns the remainder of the division of two operands. For example, `5 % 3` results in `2`.
   - **Exponentiation (∗∗)**: Raises the first value to the power of the second. For instance, `10 ** 2` equals 100.
   - **Floor Division (//)**: Divides and rounds down to the nearest integer. For example, `10 // 3` gives 3.

---
#### Comparison Operators

A comparison operator is a symbol used to compare two values (no way), returning a [[Boolean Expression (Condition)|Boolean]] result (`True` or `False`) based on whether the specified condition is met.

   - **Equal to (==)**: Checks if two operands are equal. For example, `5 == 3` results in `false`.
   - **Greater than (>)**: Checks if the first operand is greater than the second. For example, `5 > 3` results in `true`.
   - **Less than (<)**: Checks if the first operand is less than the second. For example, `5 < 3` results in `false`.
   - **Greater than or equal to (>=)**: Checks if the first operand is greater than or equal to the second. For example, `5 >= 3` results in `true`.
   - **Less than or equal to (<=)**: Checks if the first operand is less than or equal to the second. For example, `5 <= 3` results in `false`.

---
#### Logical Operators

A logical operator is a symbol or [[keyword]] used to **COMBINE** or **INVERT** [[Boolean Expression (Condition)|Boolean expressions]], returning a Boolean result (`True` or `False`) based on the logical relationship between the expressions.

   - **AND (&&)**: Returns true if both operands are true. For example, `true && false` results in `false`.
   - **OR (||)**: Returns true if at least one of the operands is true. For example, `true || false` results in `true`.
   - **NOT (!) **: Reverses the logical state of its operand. For example, `!true` results in `false`.

<span style="position: relative; font-weight: 700;background-color: #C80000; border-bottom: 2px solid #C80000;padding-top:1px; padding-bottom:1px;  padding-left: 11px; padding-right: 7px;border-top: 2px solid #C80000; border-radius:10px 0px 0px 10px;">!</span><span style= "background-color: #520000; margin-left:-14px;padding:3px;padding-left:14px; padding-right:10px;border-right:3px solid #C80000"> Example: "4 > 3 and 2" is an error. Use "4 > 3 and 4 > 2" instead.</span>

---
#### Bitwise Operators

A bitwise operator is a symbol used to perform operations directly on the individual [[Binary#Units of Memory|bits]] of [[binary]] numbers, manipulating data at the binary level.

   - **AND (&)**: Performs a bitwise AND operation. For example, `5 & 3` results in `1`.
   - **OR (|)**: Performs a bitwise OR operation. For example, `5 | 3` results in `7`.
   - **XOR (^)**: Performs a bitwise XOR operation. For example, `5 ^ 3` results in `6`.
   - **NOT (~)**: Inverts all the bits of its operand. For example, `~5` results in `-6` (in a 32-bit system).
   - **Left Shift (<<)**: Shifts bits to the left. For example, `5 << 1` results in `10`.
   - **Right Shift (>>)**: Shifts bits to the right. For example, `5 >> 1` results in `2`.

---
#### Assignment Operators

An assignment operator is a symbol used to assign a value to a [[Variables|variable]], with the most common operator being `=`, and other variations for performing arithmetic operations while assigning a result at the same time. These are great shorthand ways to do math on a variable.

   - **Assignment (=)**: Assigns the value of the right operand to the left operand. For example, `x = 5`.
   - **Add and assign (+=)**: Adds the right operand to the left operand and assigns the result to the left operand. For example, `x += 5` is equivalent to `x = x + 5`.
   - **Subtract and assign (-=)**: Subtracts the right operand from the left operand and assigns the result to the left operand. For example, `x -= 5` is equivalent to `x = x - 5`.
   - **Multiply and assign (*=)**: Multiplies the left operand by the right operand and assigns the result to the left operand. For example, `x *= 5` is equivalent to `x = x * 5`.
   - **Divide and assign (/=)**: Divides the left operand by the right operand and assigns the result to the left operand. For example, `x /= 5` is equivalent to `x = x / 5`.
   - **Modulus and assign (%=)**: Takes the modulus using two operands and assigns the result to the left operand. For example, `x %= 5` is equivalent to `x = x % 5`.

---
#### Other Operators

   - **Concatenation (in some languages, e.g., `+` for strings)**: Concatenates two strings. For example, `"Hello " + "World"` results in `"Hello World"`.
   - **Increment (++)**: Increases an integer value by one. For example, `x++` is equivalent to `x = x + 1`.
   - **Decrement (--)**: Decreases an integer value by one. For example, `x--` is equivalent to `x = x - 1`.

---
#### Operands

An operand is a value or [[data]] that an operator acts upon. Operands can be constants, [[Variables]], or expressions, and they provide the necessary inputs for operators to perform operations. Here are examples to illustrate different types of operands in various contexts:

1. **Arithmetic Operations**:
    - **Addition**: In `sum = a + b`, `a` and `b` are operands of the addition operator `+`.
    - **Subtraction**: In `difference = a - b`, `a` and `b` are operands of the subtraction operator `-`.

2. **Logical Operations**:
    - **AND**: In `result = x && y`, `x` and `y` are operands of the logical AND operator `&&`.
    - **OR**: In `result = x || y`, `x` and `y` are operands of the logical OR operator `||`.

3. **Comparison Operations**:
    - **Greater than**: In `isGreater = a > b`, `a` and `b` are operands of the greater-than operator `>`.
    - **Equal to**: In `isEqual = a == b`, `a` and `b` are operands of the equality operator `==`.

4. **Bitwise Operations**:
    - **Bitwise AND**: In `result = a & b`, `a` and `b` are operands of the bitwise AND operator `&`.
    - **Bitwise OR**: In `result = a | b`, `a` and `b` are operands of the bitwise OR operator `|`.

5. **Assignment Operations**:
    - **Simple Assignment**: In `x = y`, `x` is the operand on the left-hand side of the assignment operator `=`, and `y` is the operand on the right-hand side.
    - **Add and Assign**: In `x += y`, `x` is the left-hand operand, and `y` is the right-hand operand of the add and assign operator `+=`.

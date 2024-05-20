In computer science, an operator is a symbol or [[Functions|function]] that tells the [[compiler]] or interpreter to perform a specific mathematical, logical, or relational operation on one or more [[Operators#Operands|operands]]. Operators are essential building blocks of programming languages and enable developers to perform various tasks such as math calculations, comparisons, and [[data]] manipulation. Here are the main types of operators commonly used in programming:

---
#### Arithmetic Operators

   - **Addition (+)**: Adds two operands. For example, `5 + 3` results in `8`.
   - **Subtraction (-)**: Subtracts the second operand from the first. For example, `5 - 3` results in `2`.
   - **Multiplication (*)**: Multiplies two operands. For example, `5 * 3` results in `15`.
   - **Division (/)**: Divides the first operand by the second. For example, `5 / 3` results in approximately `1.67`.
   - **Modulus (%)**: Returns the remainder of the division of two operands. For example, `5 % 3` results in `2`.

---
#### Relational Operators

   - **Equal to (==)**: Checks if two operands are equal. For example, `5 == 3` results in `false`.==
   - **Not equal to (!=)**: Checks if two operands are not equal. For example, `5 != 3` results in `true`.
   - **Greater than (>)**: Checks if the first operand is greater than the second. For example, `5 > 3` results in `true`.
   - **Less than (<)**: Checks if the first operand is less than the second. For example, `5 < 3` results in `false`.
   - **Greater than or equal to (>=)**: Checks if the first operand is greater than or equal to the second. For example, `5 >= 3` results in `true`.
   - **Less than or equal to (<=)**: Checks if the first operand is less than or equal to the second. For example, `5 <= 3` results in `false`.

---
#### Logical Operators

   - **AND (&&)**: Returns true if both operands are true. For example, `true && false` results in `false`.
   - **OR (||)**: Returns true if at least one of the operands is true. For example, `true || false` results in `true`.
   - **NOT (!) **: Reverses the logical state of its operand. For example, `!true` results in `false`.

---
#### Bitwise Operators

   - **AND (&)**: Performs a bitwise AND operation. For example, `5 & 3` results in `1`.
   - **OR (|)**: Performs a bitwise OR operation. For example, `5 | 3` results in `7`.
   - **XOR (^)**: Performs a bitwise XOR operation. For example, `5 ^ 3` results in `6`.
   - **NOT (~)**: Inverts all the bits of its operand. For example, `~5` results in `-6` (in a 32-bit system).
   - **Left Shift (<<)**: Shifts bits to the left. For example, `5 << 1` results in `10`.
   - **Right Shift (>>)**: Shifts bits to the right. For example, `5 >> 1` results in `2`.

---
#### Assignment Operators

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

An operand is a value or [[data]] that an operator acts upon. Operands can be constants, [[variables]], or expressions, and they provide the necessary inputs for operators to perform operations. Here are examples to illustrate different types of operands in various contexts:

1. **Arithmetic Operations**:
    - **Addition**: In `sum = a + b`, `a` and `b` are operands of the addition operator `+`.
    - **Subtraction**: In `difference = a - b`, `a` and `b` are operands of the subtraction operator `-`.

2. **Logical Operations**:
    - **AND**: In `result = x && y`, `x` and `y` are operands of the logical AND operator `&&`.
    - **OR**: In `result = x || y`, `x` and `y` are operands of the logical OR operator `||`.

3. **Relational Operations**:
    - **Greater than**: In `isGreater = a > b`, `a` and `b` are operands of the greater-than operator `>`.
    - **Equal to**: In `isEqual = a == b`, `a` and `b` are operands of the equality operator `==`.

4. **Bitwise Operations**:
    - **Bitwise AND**: In `result = a & b`, `a` and `b` are operands of the bitwise AND operator `&`.
    - **Bitwise OR**: In `result = a | b`, `a` and `b` are operands of the bitwise OR operator `|`.

5. **Assignment Operations**:
    - **Simple Assignment**: In `x = y`, `x` is the operand on the left-hand side of the assignment operator `=`, and `y` is the operand on the right-hand side.
    - **Add and Assign**: In `x += y`, `x` is the left-hand operand, and `y` is the right-hand operand of the add and assign operator `+=`.

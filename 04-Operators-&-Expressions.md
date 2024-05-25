## 🔣 Operators, Operators Types & Expressions

Operators are symbols that perform operations on one or more operands.

In C#, operators are classified into different types based on their functionality.

Classification, based on their type:
- Arithmetic Operators;
- Assignment Operators;
- Comparison Operators;
- Logical Operators;
- Bitwise Operators;
- String Concatenation Operator.

Classification, based on the number of operands:
- Unary Operators;
- Binary Operators;
- Ternary Operators.

Classification, based on where the operator stands:
- Prefix Operator;
- Infix Operator;
- Postfix Operator.

An expression is a combination of operators, operands, and variables that results in a single value. They are the building blocks of your code, allowing you to perform computations, make decisions, and create dynamic behavior.

An expression consists of:
- Operators: Symbols that perform operations;
- Operands: Values or variables the operators act upon;
- Literals: Hard-coded constant values.

The data type of the calculated result is determined based on the data types of the operands and the operation.

### Unary Operators

Unary operators are operators that perform operations on a single operand, which means they work with only one value or variable. Here are some common unary operators:

1. **Unary Plus (+)**: It simply represents the identity of a numeric expression. For example, `+5` remains `5`, but it's useful for clarity or when converting a string to a number.

2. **Unary Minus (-)**: It negates a numeric expression. For example, `-5` turns `5` into `-5`.

3. **Increment (++)**: It increases the value of a variable by one. It can be used as a prefix (++x) or postfix (x++). For example, if `x` is `5`, `++x` would make it `6`, and `x++` would also make it `6` but then return the original value of `5`.

4. **Decrement (--)**: It decreases the value of a variable by one. Like increment, it can be used as a prefix (--x) or postfix (x--). For example, if `x` is `5`, `--x` would make it `4`, and `x--` would also make it `4` but then return the original value of `5`.

5. **Logical NOT (!)**: It reverses the logical state of its operand. If the operand is true, it returns false; if the operand is false, it returns true.

6. **Bitwise NOT (~)**: It flips all the bits of its operand, converting 0s to 1s and 1s to 0s. For example, `~5` in binary would be `11111111111111111111111111111010`, assuming 32-bit representation.

Unary operators are essential for performing various operations and transformations on single values in programming.

### Binary Operators

Binary operators are operators that operate on two operands or values. They perform various operations like arithmetic operations, logical operations, bitwise operations, and more. Here are some common binary operators:

1. **Arithmetic Operators**:
   - Addition (+): Adds two operands.
   - Subtraction (-): Subtracts the second operand from the first.
   - Multiplication (*): Multiplies two operands.
   - Division (/): Divides the first operand by the second.
   - Modulus (%): Computes the remainder of dividing the first operand by the second.

2. **Assignment Operators**:
   - Assigns a value to a variable. For example, `=` assigns the value on the right to the variable on the left.
   - Also, compound assignment operators like `+=`, `-=`, `*=`, `/=`, etc., combine an arithmetic operation with assignment.

3. **Comparison Operators**:
   - Equal to (==): Checks if two operands are equal.
   - Not equal to (!=): Checks if two operands are not equal.
   - Greater than (>), Less than (<), Greater than or equal to (>=), Less than or equal to (<=): Compare two operands based on their values.

4. **Logical Operators**:
   - AND (&&): Returns true if both operands are true.
   - OR (||): Returns true if at least one of the operands is true.
   - NOT (!): Reverses the logical state of its operand.

5. **Bitwise Operators**:
   - AND (&), OR (|), XOR (^), NOT (~): Perform bitwise operations on the binary representations of the operands.
   - Left Shift (<<), Right Shift (>>): Shift bits to the left or right by a specified number of positions.

Binary operators are fundamental in programming and are used extensively for various computations, comparisons, and logical operations.

### Ternary Operators

In C#, the ternary operator functions similarly to other languages, providing a compact way to express conditional operations. Its syntax is:

```
condition ? expression1 : expression2
```

Here's a usage example in C#:

```csharp
int x = 10;
string result = (x > 5) ? "x is greater than 5" : "x is not greater than 5";
```

In this code:

- If the condition `(x > 5)` is true, the value of `result` will be `"x is greater than 5"`.
- If the condition is false, the value of `result` will be `"x is not greater than 5"`.

C# allows for concise and readable code with the ternary operator, particularly for simple conditional assignments or expressions.

### Prefix Operator

In C#, prefix operators are unary operators that are placed before their operand. They perform an operation on the operand before using its value. Here are the common prefix operators in C#:

1. **Increment (++):** This operator increases the value of its operand by 1. It can be used both as a prefix (++variable) and as a postfix (variable++). However, in the prefix form, the value is increased before any other operation is performed.

    ```csharp
    int x = 5;
    int y = ++x; // y will be 6, x will be 6
    ```

2. **Decrement (--):** This operator decreases the value of its operand by 1. Similar to the increment operator, it can be used as both a prefix and a postfix. In the prefix form, the value is decreased before any other operation is performed.

    ```csharp
    int x = 5;
    int y = --x; // y will be 4, x will be 4
    ```

Prefix operators are commonly used for incrementing or decrementing variables in C# before using their updated values in expressions or assignments.

### Infix Operator

In C# and many other programming languages, infix operators are binary operators that are placed between their operands. They perform an operation involving two operands. 

Common infix operators in C# include arithmetic operators like addition (+), subtraction (-), multiplication (*), and division (/), as well as comparison operators like equality (==), inequality (!=), greater than (>), less than (<), greater than or equal to (>=), and less than or equal to (<=).

Here are some examples of infix operators in C#:

```csharp
int result = 5 + 3;   // addition operator
bool isEqual = 5 == 3;  // equality operator
int product = 5 * 3;   // multiplication operator
bool isGreater = 5 > 3; // greater than operator
```

In each case, the infix operator operates on the two operands that surround it. The infix notation is the typical way operators are used in expressions within programming languages.

### Postfix Operator

In C#, postfix operators are unary operators that are placed after their operand. They perform an operation on the operand after using its value. Here's the common postfix operator in C#:

1. **Increment (++)**: This operator increases the value of its operand by 1. It can be used both as a prefix (++variable) and as a postfix (variable++). However, in the postfix form, the value is increased after any other operation is performed.

   ```csharp
   int x = 5;
   int y = x++; // y will be 5, x will be 6
   ```

2. **Decrement (--)**: This operator decreases the value of its operand by 1. Similar to the increment operator, it can be used as both a prefix and a postfix. In the postfix form, the value is decreased after any other operation is performed.

   ```csharp
   int x = 5;
   int y = x--; // y will be 5, x will be 4
   ```

Postfix operators are commonly used when you need to perform an operation after using the current value of a variable in an expression or assignment.

### Associativity

Associativity in C# refers to the order in which operators of the same precedence are evaluated in an expression. In C#, operators can be left-associative or right-associative.

Let's break it down:

1. **Precedence Level**: Operators in programming languages have different levels of precedence, which determine the order in which they are evaluated within an expression. Operators with higher precedence are evaluated before operators with lower precedence.
    
2. **Associativity**: When multiple operators of the same precedence level appear in an expression, associativity determines the order in which they are evaluated. There are two types of associativity:
    
    - **Left Associativity**: Operators with left associativity are evaluated from left to right. This means that if you have multiple operators of the same precedence level in an expression, they are evaluated in a left-to-right order.
        
    - **Right Associativity**: Operators with right associativity are evaluated from right to left. This means that if you have multiple operators of the same precedence level in an expression, they are evaluated in a right-to-left order.
        
Associativity is essential for understanding how expressions are evaluated in programming languages. It helps determine the outcome of complex expressions and ensures that the result is consistent and predictable.

In C#, most operators follow left-to-right associativity, which means they are evaluated from left to right. For example, in the expression a + b + c, the addition operator (+) has left-to-right associativity. This means that a + b is evaluated first, and then the result is added to c.

However, there are a few operators that have right-to-left associativity. One common example is the assignment operator (=). In the expression a = b = c, the assignment operator has right-to-left associativity. This means that b = c is evaluated first, and then the result is assigned to a.

- **Left-associative**: Operators are evaluated from left to right.
- **Right-associative**: Operators are evaluated from right to left.

The associativity of an operator determines how expressions are grouped and evaluated when multiple operators of the same precedence appear in the same expression.

For example, the addition (`+`) and subtraction (`-`) operators are left-associative, meaning they are evaluated from left to right. So, in the expression `a + b - c`, the addition `+` is evaluated first, followed by the subtraction `-`.

On the other hand, the assignment operator (`=`) is right-associative, meaning it is evaluated from right to left. So, in the expression `a = b = c`, the assignment starts from the rightmost `c`, then assigns the value to `b`, and finally assigns the value to `a`.

Here are examples illustrating associativity in C#:

```csharp
class Program
{
    static void Main(string[] args)
    {
        // Left-associative operators
        int result1 = 10 + 5 - 3; // result1 = (10 + 5) - 3 = 12
        Console.WriteLine("Result 1: " + result1);

        // Right-associative operators
        int a = 10;
        int b = 5;
        int c = 3;
        int result2 = a = b = c; // result2 = (a = (b = c)) = 3
        Console.WriteLine("Result 2: " + result2); // Output: Result 2: 3
        Console.WriteLine("Value of a: " + a);    // Output: Value of a: 3
        Console.WriteLine("Value of b: " + b);    // Output: Value of b: 3
        Console.WriteLine("Value of c: " + c);    // Output: Value of c: 3
    }
}
```

In the above examples, the associativity of operators determines the order of evaluation and assignment, leading to different results.

## 🔢 Arithmetic Operators

Arithmetic operators are symbols used in math to perform basic calculations like addition, subtraction, multiplication, and division. 

Here are the common ones:

1. **Addition (+)**: It combines numbers together. For example, 2 + 3 = 5.

2. **Subtraction (-)**: It finds the difference between numbers. For example, 5 - 3 = 2.

3. **Multiplication (\*)**: It's like repeated addition. For example, 2 * 3 means 2 added to itself 3 times, which equals 6.

4. **Division (/)**: It splits numbers into equal parts. For example, 6 / 3 means dividing 6 into 3 equal parts, which equals 2.

5. **Modulo (%)**: It gives you the remainder of a division. For example, 7 % 3 equals 1 because 7 divided by 3 is 2 with a remainder of 1.

These symbols help us do math easily in programming and everyday life!

Arithmetic operators perform basic mathematical operations. Arithmetic operators include:
- Addition: `+`;
- Subtraction: `-`;
- Multiplication: `*`;
- Division: `/`;
- Modulus (remainder): `%`.

```csharp
var x = 10;
var y = 5;

Console.WriteLine(x + y); // 👈 Prints "15"
Console.WriteLine(x - y); // 👈 Prints "5"
Console.WriteLine(x * y); // 👈 Prints "50"
Console.WriteLine(x / y); // 👈 Prints "2"
Console.WriteLine(x % y); // 👈 Prints "0"
```

The Modulus operator, symbolized by `%`, returns the remainder of the division of the left operand by the right operand.

In C#, the modulus operator works the same way as in other programming languages. It's represented by the percent sign (%) and returns the remainder of dividing one number by another. Here's how you use it in C#:

```csharp
int result = 5 % 2;  // result will be 1
int anotherResult = 10 % 3;  // result will be 1
int yetAnotherResult = 8 % 4;  // result will be 0
```

In each case, the modulus operator (`%`) calculates the remainder of the division and returns the result. This operator is particularly handy when you need to check for divisibility, create patterns, or perform cyclic operations in your C# code.

```csharp
Console.WriteLine(12 % 3); // 👈 Prints "0", 3 * 4 + 0 = 12
Console.WriteLine(13 % 3); // 👈 Prints "1", 3 * 4 + 1 = 13
```

The Increment (`++`) and Decrement (`--`) operators are specialized arithmetic operators that increase or decrease the value of a variable by `1`. They can be written either as a prefix or as a postfix operator.

```csharp
int counter = 5;

counter++; // Written as a postfix we use the value and then the counter is set to 6

++counter; // Written as a prefix we increment the value and then use it

counter--;

--counter;
```

## 🏗️ Assignment Operators

Assignment operators are used in programming to assign values to variables. They're pretty straightforward! Here are the common ones:

1. **Equal (=)**: This is the basic assignment operator. It assigns the value on the right to the variable on the left. For example, `x = 5` assigns the value 5 to the variable `x`.

2. **Addition and Assignment (+=)**: It adds the value on the right to the variable on the left and assigns the result to the variable. For example, `x += 3` is the same as `x = x + 3`.

3. **Subtraction and Assignment (-=)**: It subtracts the value on the right from the variable on the left and assigns the result to the variable. For example, `x -= 3` is the same as `x = x - 3`.

4. **Multiplication and Assignment (\*=)**: It multiplies the variable on the left by the value on the right and assigns the result to the variable. For example, `x *= 3` is the same as `x = x * 3`.

5. **Division and Assignment (/=)**: It divides the variable on the left by the value on the right and assigns the result to the variable. For example, `x /= 3` is the same as `x = x / 3`.

6. **Modulo and Assignment (%=)**: It takes the modulo of the variable on the left by the value on the right and assigns the result to the variable. For example, `x %= 3` is the same as `x = x % 3`.

These operators are handy shortcuts for updating variables in programming!

Assignment operators allow us to assign and modify the values stored in variables.

The most basic assignment operator (`=`) assigns the value on the right to the variable on the left.

```csharp
int x = 10; // Assigns the value 10 to the variable x
```

```csharp
int count = 5;
int total = count; // Assigns the value of count to the variable total

Console.WriteLine(count); // 👈 Prints "5"
Console.WriteLine(total); // 👈 Prints "5"
```

Compound assignment operators (`+=`, `-=`, `*=`, `/=`, etc.) combine the assignment with another operation.

```csharp
int number = 5;

number += 3; // 👈 Equivalent to: number = number + 3;

Console.WriteLine(number); // 👈 Prints "8"
```

The difference between `number + 3` and `number += 3` is that in the second scenario the value of number is updated.

```csharp
int x = 5;

x += 3; // x = 5 + 3 = 8

x -= 2; // x = 8 - 2 = 6

x *= 4; // x = 6 * 4 = 24

x /= 6; // x = 24 / 6 = 4

Console.WriteLine(x); // 👈 Prints "4"
```

We can also chain assignment operators.

```csharp
int a, b;
a = b = 7; // Both a and b are assigned the value 7.

Console.WriteLine(a); // 👈 Prints "7"
Console.WriteLine(b); // 👈 Prints "7"

int x, y, z;
x = y = z = 10;
Console.WriteLine(x); // 👈 Prints "10"
Console.WriteLine(y); // 👈 Prints "10"
Console.WriteLine(z); // 👈 Prints "10"
```

## 🎯 Comparison Operators

Comparison operators are used in programming to compare values. They help determine the relationship between two values and produce a result based on whether the comparison is true or false. Here are the common ones:

1. **Equal to (==)**: Checks if two values are equal. Returns true if they are, false otherwise. For example, `5 == 5` would be true, while `5 == 3` would be false.

2. **Not equal to (!=)**: Checks if two values are not equal. Returns true if they are different, false if they are the same. For example, `5 != 3` would be true, while `5 != 5` would be false.

3. **Greater than (>)**: Checks if the left value is greater than the right value. Returns true if it is, false otherwise. For example, `5 > 3` would be true, while `3 > 5` would be false.

4. **Less than (<)**: Checks if the left value is less than the right value. Returns true if it is, false otherwise. For example, `3 < 5` would be true, while `5 < 3` would be false.

5. **Greater than or equal to (>=)**: Checks if the left value is greater than or equal to the right value. Returns true if it is, false otherwise. For example, `5 >= 5` would be true, while `3 >= 5` would be false.

6. **Less than or equal to (<=)**: Checks if the left value is less than or equal to the right value. Returns true if it is, false otherwise. For example, `3 <= 5` would be true, while `5 <= 3` would be false.

These operators are essential for making decisions in programming, like determining when to execute certain parts of code or controlling loops.

Comparison operators compare values and return a result of type `bool`. Comparison operators include:
- Equal to: `==`;
- Not equal to: `!=`;
- Greater than: `>`;
- Less than: `<`;
- Greater than or equal to: `>=`;
- Less than or equal to: `<=`.

```csharp
var x = 5;
var y = 6;

Console.WriteLine(x == y); // 👈 Prints "False"
Console.WriteLine(x != y); // 👈 Prints "True"

Console.WriteLine(x > y); // 👈 Prints "False"
Console.WriteLine(x < y); // 👈 Prints "True"

Console.WriteLine(x >= x); // 👈 Prints "True"
Console.WriteLine(x <= x); // 👈 Prints "True"
```

Characters can be compared using the same comparison operators. The comparison is based on the Unicode values of the characters.

## 🧠 Logical Operators

Logical operators are used in programming to combine multiple conditions or expressions. They help you make decisions based on more than one condition. Here are the common ones:

1. **AND (&&)**: This operator returns true if both conditions on its left and right sides are true. If any one of them is false, it returns false. For example, `A && B` is true only if both A and B are true.

2. **OR (||)**: This operator returns true if at least one of the conditions on its left and right sides is true. It returns false only if both conditions are false. For example, `A || B` is true if either A or B or both are true.

3. **NOT (!)**: This operator is used to reverse the logical state of its operand. If the operand is true, it returns false, and if the operand is false, it returns true. For example, `!A` is true if A is false, and false if A is true.

These operators allow you to create more complex conditions and control the flow of your program based on different scenarios.

Logical operators allow us to create conditions that involve multiple values of type `bool`. Logical operators include:
- Logical `AND`: `&&`;
- Logical `OR`: `||`;
- Logical `NOT`: `!`.

The logical `AND` operator returns `true` when both operands are evaluated to `true`.

|A|B|A && B|
|-|-|-|
|true|true|true|
|true|false|false|
|false|true|false|
|false|false|false|

The logical `AND` operator returns `true` when both operands are evaluated to `true`.

```csharp
var hasLicense = true;
var hasCar = true;

var canDrive = hasLicense && hasCar;
Console.WriteLine(canDrive); // 👈 Prints "True"
```

The logical `OR` operator returns `true` when at least one operand is evaluated to `true`.

|A|B|A \|\| B|
|-|-|-|
|true|true|true|
|true|false|true|
|false|true|true|
|false|false|false|

```csharp
var isSunny = true;
var isWarm = false;

var goOutside = isSunny || isWarm;
Console.WriteLine(goOutside); // 👈 Prints "True"
```

The logical `NOT` operator flips the value of type `bool`.

|A|!A|
|-|-|
|true|false|
|false|true|

```csharp
var isRaining = false;

Console.WriteLine(!isRaining); // 👈 Prints "True"
```

## 🔬 Bitwise Operators

Bitwise operators are used in programming to manipulate individual bits of data. They perform operations at the binary level, which means they work on the binary representation of numbers. Here are the common bitwise operators:

1. **AND (&)**: Performs a bitwise AND operation between the corresponding bits of two operands. If both bits are 1, the resulting bit is 1; otherwise, it's 0.

2. **OR (|)**: Performs a bitwise OR operation between the corresponding bits of two operands. If at least one bit is 1, the resulting bit is 1; otherwise, it's 0.

3. **XOR (^)**: Performs a bitwise XOR (exclusive OR) operation between the corresponding bits of two operands. The result is 1 if the bits are different, and 0 if they are the same.

4. **NOT (~)**: Performs a bitwise NOT operation on a single operand. It inverts each bit; 1 becomes 0, and 0 becomes 1.

5. **Left Shift (<<)**: Shifts the bits of the left operand to the left by a specified number of positions. Zeros are shifted in from the right.

6. **Right Shift (>>)**: Shifts the bits of the left operand to the right by a specified number of positions. For unsigned numbers, zeros are shifted in from the left. For signed numbers, the sign bit (the leftmost bit) is shifted in from the left, which means the result depends on the implementation.

These operators are useful in low-level programming, such as working with device drivers, network protocols, or when optimizing code for performance.


Bitwise operators provide a way to perform operations at the bit level. They work directly with the binary representation of numbers. Bitwise operators include:
- Bitwise `AND`: `&`;
- Bitwise `OR`: `|`;
- Bitwise `XOR`: `^`;
- Bitwise `NOT`: `~`;
- Bitwise Left Shift: `<<`;
- Bitwise Right Shift: `>>`.

The bitwise `AND` operator (`&`) performs a bitwise `AND` operation between the corresponding bits of two integers.

```csharp
int a = 5; // Binary: 0101
int b = 3; // Binary: 0011

Console.WriteLine(a & b); // Prints "1" (Binary: 0001)
// 0 & 0 = 0
// 1 & 0 = 0
// 0 & 1 = 0
// 1 & 1 = 1
```

The bitwise `OR` operator (`|`) performs a bitwise `OR` operation between the corresponding bits of two integers.

```csharp
int x = 9; // Binary: 1001
int y = 6; // Binary: 0110

Console.WriteLine(x | y); // Prints "15" (Binary: 1111)
// 1 | 0 = 1
// 0 | 1 = 1
// 0 | 1 = 1
// 1 | 0 = 1
```

The `XOR` operator (`^`) performs a bitwise exclusive `OR` operation. It sets a bit to 1 if the corresponding bits are different.

```csharp
int m = 12; // Binary: 1100
int n = 7; // Binary: 0111

Console.WriteLine(m ^ n); // Prints "11" (Binary: 1011)
// 1 ^ 0 = 1
// 1 ^ 1 = 0
// 0 ^ 1 = 1
// 0 ^ 1 = 1
```

The `NOT` operator (`~`) is a unary operator that performs a bitwise `NOT` operation. It flips the bits, turning zeroes into ones and vice versa.

```csharp
int p = 10; // Binary: 1010

Console.WriteLine(~p); // Prints: "-11" (Binary: 0101)
```

Keep in mind that the NOT operator also flips the sign.

The Left Shift (`<<`) and Right Shift (`>>`) Operators shift the bits of a number to the left or right by a specified number of positions.

```csharp
int number = 5; // Binary: 0101

Console.WriteLine(number << 2); // 20 (Binary: 101000)
Console.WriteLine(number >> 1); // 2 (Binary: 0010)
```

## 🔗 String Concatenation Operator

In C#, the string concatenation operator is also the plus sign (+). It's used to concatenate or join strings together. Here's how you use it in C#:

```csharp
string str1 = "Hello";
string str2 = "world";
string result = str1 + " " + str2; // result will be "Hello world"
```

You can use the plus sign to combine strings with other strings, variables, or even other data types. C# is smart enough to convert non-string values to strings when they're used with the plus operator in a string concatenation operation.

String concatenation is the process of combining strings to create a new string. In C#, the string concatenation operator is represented by the `+` symbol.

```csharp
var firstName = "Peter";
var lastName = "Smith";

var fullName = firstName + " " + lastName;
Console.WriteLine(fullName); // 👈 Prints "Peter Smith"
```

We can combine strings and variables.

```csharp
var fullName = "Peter Smith";
var greeting = "Hello, " + fullName + "!";
Console.WriteLine(greeting); // 👈 Prints "Hello, Peter Smith!"
```

Greeting Message:
   ```csharp
   string firstName = "John";
   string lastName = "Doe";
   string greeting = "Hello, " + firstName + " " + lastName + "!";
   Console.WriteLine(greeting);
   // Output: Hello, John Doe!
   ```

Building a Sentence:
   ```csharp
   string subject = "C#";
   string action = "learn";
   string sentence = "I want to " + action + " " + subject + ".";
   Console.WriteLine(sentence);
   // Output: I want to learn C#.
   ```

Displaying User Input:
   ```csharp
   Console.WriteLine("Enter your name:");
   string name = Console.ReadLine();
   string message = "Hello, " + name + "! Welcome to C#!";
   Console.WriteLine(message);
   // Output (if user inputs "Alice"): Hello, Alice! Welcome to C#!"
   ```

Building a Story:
   ```csharp
   string character = "Tom";
   string place = "park";
   string action = "ran";
   string story = character + " " + action + " in the " + place + ".";
   Console.WriteLine(story);
   // Output: Tom ran in the park.
   ```

Concatenating Numbers:
   ```csharp
   int num1 = 5;
   int num2 = 3;
   string result = "The sum of " + num1 + " and " + num2 + " is " + (num1 + num2) + ".";
   Console.WriteLine(result);
   // Output: The sum of 5 and 3 is 8.
   ```

## 🎩 Operators Precedence

Basic arithmetic operators follow the standard rules. Multiplication and division take precedence over addition and subtraction.

Operators precedence is the set of rules that dictate the order in which operators are evaluated in an expression. Just like in a mathematical equation, certain operators take precedence over others.

```csharp
int x = 8;
int y = 5;
int z = 10;

Console.WriteLine(x > y && x < z); // Evaluates as true && true => true, because the comparison operators have higher precedence than the logical AND operator.
```


In programming, operators are symbols that perform operations on variables or values. When multiple operators are used in an expression, the order in which they are evaluated can impact the result. This order of evaluation is determined by the precedence of operators.

**Understanding Precedence:**

Operator precedence determines the order in which operators are evaluated in an expression. Operators with higher precedence are evaluated before those with lower precedence. If operators have the same precedence, their evaluation order depends on their associativity, which can be left-to-right or right-to-left.

**Common Operators and Their Precedence:**

Here's a table illustrating the precedence of some common operators in programming languages:

| Operator     | Description                      | Associativity |
|--------------|----------------------------------|---------------|
| ()           | Parentheses (grouping)           | Left-to-right |
| !            | Logical NOT                      | Right-to-left |
| * / %        | Multiplication, Division, Modulo | Left-to-right |
| + -          | Addition, Subtraction            | Left-to-right |
| < <= > >=    | Comparison Operators             | Left-to-right |
| == !=        | Equality Operators               | Left-to-right |
| &&           | Logical AND                      | Left-to-right |
| \|\|         | Logical OR                       | Left-to-right |
| =            | Assignment                       | Right-to-left |



| Operator     | Description                      | Associativity | Example                    |
|--------------|----------------------------------|---------------|----------------------------|
| ()           | Parentheses (grouping)           | Left-to-right | (true && false)            |
| !            | Logical NOT                      | Right-to-left | !true                      |
| * / %        | Multiplication, Division, Modulo | Left-to-right | 10 * 2 / 5                 |
| + -          | Addition, Subtraction            | Left-to-right | 5 + 3 - 2                  |
| < <= > >=    | Comparison Operators             | Left-to-right | 10 > 5                     |
| == !=        | Equality Operators               | Left-to-right | 5 == 5                     |
| &&           | Logical AND                      | Left-to-right | true && false              |
| \|\|         | Logical OR                       | Left-to-right | true \|\| false            |
| =            | Assignment                       | Right-to-left | x = 10                     |



**Example:**

Consider the expression `a * b + c`. The `*` operator has higher precedence than `+`, so `a * b` is evaluated first, then `c` is added to the result.

**Tips for Clarity:**

1. Use parentheses to explicitly specify the order of evaluation, especially when dealing with complex expressions.
2. Follow the precedence rules of the programming language you're using to avoid unexpected results.

Understanding operator precedence is crucial for writing correct and efficient code. By knowing which operators are evaluated first, you can ensure that your expressions produce the desired results.

## ⚙️ Parentheses Operator

One primary function of the parentheses is to group expressions, altering the order of evaluation. They allow us to explicitly define the order in which operations are evaluated.

```csharp
int x = 4;
int y = 2;
int z = 3;

Console.WriteLine(x + y * z); // Prints: "10"

// The addition inside the parentheses takes precedence
Console.WriteLine((x + y) * z); // Prints: "18"
```

Understanding precedence ensures that our code behaves as intended.

Parentheses are symbols used in programming to group expressions and control the order of operations. They are represented by `(` and `)`. Understanding how to use parentheses can help clarify and control the evaluation of expressions.

**Purpose of Parentheses:**

The main purpose of parentheses is to specify the order of operations in an expression. When parentheses are used, the operations inside them are performed first, overriding the default precedence rules of the language.

**Using Parentheses:**

Here's a simple table illustrating the use of parentheses in programming:

| Example                  | Description                            |
|--------------------------|----------------------------------------|
| (5 + 3) * 2              | Addition inside parentheses evaluated first, then multiplied by 2. Result: 16 |
| (10 - 4) / (3 + 2)       | Subtraction inside parentheses evaluated first, then divided by addition result. Result: 1.2 |
| (true && false) || true  | Logical AND expression evaluated first, then its result ORed with true. Result: true |

**Benefits of Using Parentheses:**

1. **Clarity:** Parentheses make expressions easier to read and understand, especially in complex expressions where the order of operations might not be immediately obvious.

2. **Control:** By using parentheses, programmers can explicitly specify the order of operations, ensuring that expressions are evaluated as intended.

**Example:**

Consider the expression `(5 + 3) * 2`. Here, the addition inside the parentheses `(5 + 3)` is evaluated first, resulting in `8`. Then, `8` is multiplied by `2`, resulting in `16`.

**Tips for Using Parentheses:**

1. **Balance:** Ensure that every opening parenthesis `(` has a corresponding closing parenthesis `)`. Unbalanced parentheses can lead to syntax errors.

2. **Nested Parentheses:** You can use multiple levels of parentheses to further control the order of operations in complex expressions.

Understanding how to use parentheses effectively can improve the readability and correctness of your code, especially when dealing with expressions involving multiple operations.

## 📜 Guides

1. **Understand Operator Precedence:** In C#, operators have predefined precedence levels. Familiarize yourself with these levels to understand the order of operations in expressions. Parentheses can be used to explicitly specify the evaluation order.

2. **Keep Expressions Simple and Readable:** Complex expressions can be challenging to understand and maintain. Break down complex expressions into smaller, more manageable parts. Use meaningful variable names to enhance readability.

3. **Avoid Excessive Nesting:** Excessive nesting of expressions can make code harder to follow. Simplify expressions where possible and consider splitting them into multiple statements for clarity.

4. **Consider Efficiency:** Certain operations may be more efficient than others in terms of performance. Understand the performance implications of different operations, especially in performance-critical applications.

5. **Use Comments for Explanation:** If an expression is particularly complex or non-intuitive, consider adding comments to explain its purpose and how it's evaluated.

**Guide and Best Practices for Using Bitwise Operators with Unsigned Data Types:**

1. **Know Your Data Types:** Understand the characteristics and limitations of unsigned data types in C#, such as `uint` and `ulong`. Unsigned data types only represent non-negative numbers and are commonly used with bitwise operations.

2. **Avoid Signed-to-Unsigned Conversions:** Be cautious when mixing signed and unsigned data types, as it can lead to unexpected behavior. Perform proper type casting or ensure consistency in data types throughout your code.

3. **Understand Bitwise Operators:** Familiarize yourself with bitwise operators such as `&` (AND), `|` (OR), `^` (XOR), `<<` (left shift), and `>>` (right shift). These operators manipulate individual bits within binary representations of numbers.

4. **Use Bitwise Operators for Flags and Masks:** Bitwise operators are frequently used to manipulate individual bits within bit fields, such as setting, clearing, or toggling specific flags or masks.

5. **Watch Out for Bitwise Overflow:** Be mindful of potential overflow issues when using bitwise operators with unsigned data types. Overflow occurs when the result of an operation exceeds the maximum value representable by the data type.

**Examples:**

**Operators & Expressions:**
```csharp
// Example of understanding operator precedence
int result = 5 + 3 * 2;  // Multiplication (*) has higher precedence than addition (+)
Console.WriteLine(result);  // Output: 11

// Example of keeping expressions simple and readable
int width = 10;
int height = 5;
int area = width * height;
Console.WriteLine(area);  // Output: 50

// Example of avoiding excessive nesting
// Instead of: int result = (((5 + 3) * 2) / 2) - 1;
// Prefer:
int tempResult = 5 + 3;
tempResult *= 2;
tempResult /= 2;
int result = tempResult - 1;
Console.WriteLine(result);  // Output: 7
```

**Using Bitwise Operators with Unsigned Data Types:**
```csharp
// Example of using bitwise AND (&) for masking
uint flags = 0b1010;  // Binary representation: 1010
uint mask = 0b0100;   // Binary representation: 0100
uint result = flags & mask;
Console.WriteLine(Convert.ToString(result, 2));  // Output: 1000

// Example of using bitwise OR (|) for setting flags
flags = 0b1010;  // Binary representation: 1010
mask = 0b0100;   // Binary representation: 0100
result = flags | mask;
Console.WriteLine(Convert.ToString(result, 2));  // Output: 1110

// Example of using bitwise XOR (^) for toggling flags
flags = 0b1010;  // Binary representation: 1010
mask = 0b0100;   // Binary representation: 0100
result = flags ^ mask;
Console.WriteLine(Convert.ToString(result, 2));  // Output: 1110
```

**Bitwise Left Shift (`<<`) and Right Shift (`>>`):**
   ```csharp
   // Example of bitwise left shift (<<)
   int num = 5;  // Binary representation: 0000 0101
   int shiftedNum = num << 2;  // Shift left by 2 bits
   Console.WriteLine(shiftedNum);  // Output: 20 (Binary representation: 0001 0100)

   // Example of bitwise right shift (>>)
   int num = 20;  // Binary representation: 0001 0100
   int shiftedNum = num >> 2;  // Shift right by 2 bits
   Console.WriteLine(shiftedNum);  // Output: 5 (Binary representation: 0000 0101)
   ```

**Bitwise NOT (`~`):**
   ```csharp
   // Example of bitwise NOT (~)
   uint num = 10;  // Binary representation: 0000 0000 0000 0000 0000 0000 0000 1010
   uint complement = ~num;
   Console.WriteLine(Convert.ToString(complement, 2));  // Output: 1111 1111 1111 1111 1111 1111 1111 0101
   ```

**Checking Even or Odd Numbers using Bitwise AND (`&`):**
   ```csharp
   int num = 7;  // Check if this number is even or odd
   if ((num & 1) == 0)
   {
       Console.WriteLine("Even");
   }
   else
   {
       Console.WriteLine("Odd");
   }
   ```


Understanding and applying these guides and best practices will help you write cleaner, more efficient, and more maintainable code when working with operators, expressions, and bitwise operations with unsigned data types in C#.



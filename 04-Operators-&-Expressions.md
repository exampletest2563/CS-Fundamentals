# 🔣 Operators & Expressions

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

// TODO: Associativity
Associativity in C# refers to the order in which operators of the same precedence are evaluated in an expression. In C#, operators can be left-associative or right-associative.

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

## 🎩 Operators Precedence

Basic arithmetic operators follow the standard rules. Multiplication and division take precedence over addition and subtraction.

Operators precedence is the set of rules that dictate the order in which operators are evaluated in an expression. Just like in a mathematical equation, certain operators take precedence over others.

```csharp
int x = 8;
int y = 5;
int z = 10;

Console.WriteLine(x > y && x < z); // Evaluates as true && true => true, because the comparison operators have higher precedence than the logical AND operator.
```

// TODO: Add table.
Apologies for misunderstanding your request. Let me provide you with a Markdown table specifically focused on operator precedence in C#:

```markdown
| Expression                   | Evaluation Result | Expected Result |
|------------------------------|-------------------|-----------------|
| `2 + 3 * 4`                  | `14`              | `14`            |
| `(2 + 3) * 4`                | `20`              | `20`            |
| `10 / 2 - 1`                 | `4`               | `4`             |
| `10 / (2 - 1)`               | `10`              | `10`            |
| `5 * 3 % 2`                  | `1`               | `1`             |
| `(5 * 3) % 2`                | `1`               | `1`             |
| `2 + 2 == 4 && 3 + 3 == 6`   | `True`            | `True`          |
| `2 + 2 == 4 || 3 + 3 == 6`   | `True`            | `True`          |
| `2 + 2 == 4 && 3 + 3 == 5`   | `False`           | `False`         |
| `2 + 2 == 3 || 3 + 3 == 5`   | `False`           | `False`         |
| `2 > 1 && 3 < 2`             | `False`           | `False`         |
| `2 > 1 || 3 < 2`             | `True`            | `True`          |
```

This table showcases various expressions along with their evaluation results to illustrate the operator precedence rules in C#.

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

## 📜 Guides

Use Bitwise Operators with unsigned data types.
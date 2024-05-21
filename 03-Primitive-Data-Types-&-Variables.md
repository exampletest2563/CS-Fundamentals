# 🌱 Primitive Data Types & Variables

## Computer Memory (Computer Science)

## Data Types (Computer Science)

## Variables Introduction

Variables are containers for storing and managing data. They allow us to name and manipulate values.

```csharp
//          👇 Value
int number = 5;
//   👆 Variable name

Console.WriteLine(number); // 👈 Prints "5"
```

```csharp
//                   👇 Value
string firstName = "John";
//        👆 Variable name

Console.WriteLine(firstName); // 👈 Prints "John"
```

Variables declared with the `int` keyword store integers.

Variables declared with the `string` keyword store text values or "strings".

Imagine building a shopping cart. Variables would hold information like item names, quantities, and prices.

## Literals

Literals are the raw, straightforward values that we use directly.

Numeric literals are straightforward values like integers that we explicitly write in our code.

```csharp
5
3.14
```

Character literals represent a single character, while string literals represent sequences of characters.

```csharp
'a'
'$'
"Some text"
```

Boolean literals represent the truth values - `true` or `false`.

```csharp
true // Type: Boolean
false

"true" // Type: String
```

C# supports binary and hexadecimal literals.

// TODO: Add examples.
```csharp
// Binary Literal Example
int binaryNumber = 0b101010; // Represents the binary number 101010 (42 in decimal)

// Hexadecimal Literal Example
int hexadecimalNumber = 0x2A; // Represents the hexadecimal number 2A (42 in decimal)
```

In the first example, `0b101010` represents the binary number 101010, which equals 42 in decimal. The `0b` prefix indicates that the number is in binary format.

In the second example, `0x2A` represents the hexadecimal number 2A, which also equals 42 in decimal. The `0x` prefix denotes that the number is in hexadecimal format.

C# allows us to make numeric literals more readable by using underscores for separation.

// TODO: Add examples.
```csharp
// Example with decimal literals
int largeNumber = 1_000_000; // Represents one million
int creditCardNumber = 1234_5678_9012_3456; // Represents a 16-digit credit card number

// Example with binary literals
int binaryNumber = 0b1010_1010_1010; // Represents the binary number 101010101010 (2730 in decimal)

// Example with hexadecimal literals
int hexadecimalNumber = 0xAB_CD_EF; // Represents the hexadecimal number ABCDEF (11259375 in decimal)

// Example with floating-point literals
double largeDouble = 1_000_000.123_456; // Represents one million and 123.456
```

In these examples, the underscores make it easier to read and understand large numeric values by visually separating groups of digits, similar to how commas or spaces are used in written numbers. The underscores do not affect the actual value of the literals.

This feature enhances code readability, especially for large numeric values.

// TODO: All data types have a default value - 0 / false, 0L, 0UL, etc.
In C#, all data types have default values that are assigned when variables are declared but not initialized.

### Default Values:

- **Numeric Types:** Default to `0`.
  - `int`, `float`, `double`, `byte`, `short`, `long`, `decimal`, `sbyte`, `ushort`, `uint`, `ulong`
  - Example: `int myInt; // Default value is 0`

- **Boolean Type:** Defaults to `false`.
  - `bool`
  - Example: `bool myBool; // Default value is false`

- **Character Type:** Defaults to the null character `'\0'`.
  - `char`
  - Example: `char myChar; // Default value is '\0'`

- **Reference Types:** Default to `null`.
  - `string`, arrays, classes, interfaces, delegates
  - Example: `string myString; // Default value is null`

### Examples:

```csharp
int myInt;            // Default value is 0
bool myBool;          // Default value is false
char myChar;          // Default value is '\0'
long myLong;          // Default value is 0L
ulong myULong;        // Default value is 0UL
string myString;      // Default value is null
```

These default values ensure that all variables have a defined state even if not explicitly initialized by the programmer.


OR

**Default Values of Data Types**

In C#, all data types have default values that are assigned when variables are declared but not initialized. Understanding these defaults is crucial for avoiding unintended behavior in your programs.

### Default Values and Explanations:

- **Numeric Types:**
  - **int, float, double, byte, short, long, decimal, sbyte, ushort, uint, ulong:** All numeric types default to `0`.
    - **Example:**
      ```csharp
      int myInt; // Default value is 0
      float myFloat; // Default value is 0.0f
      double myDouble; // Default value is 0.0
      long myLong; // Default value is 0L
      ulong myULong; // Default value is 0UL
      ```
    - **Explanation:** Numeric types default to zero because this is a neutral value that represents the absence of a meaningful number.

- **Boolean Type:**
  - **bool:** The boolean type defaults to `false`.
    - **Example:**
      ```csharp
      bool myBool; // Default value is false
      ```
    - **Explanation:** Booleans default to false to indicate the absence of a true condition.

- **Character Type:**
  - **char:** The character type defaults to the null character `'\0'`.
    - **Example:**
      ```csharp
      char myChar; // Default value is '\0'
      ```
    - **Explanation:** The null character `'\0'` is used as a default to represent an uninitialized character.

- **Reference Types:**
  - **string, arrays, classes, interfaces, delegates:** All reference types default to `null`.
    - **Example:**
      ```csharp
      string myString; // Default value is null
      int[] myArray; // Default value is null
      MyClass myClassInstance; // Default value is null
      ```
    - **Explanation:** Reference types default to null to indicate that they do not reference any object in memory.

## Integer Data Types

Integers represent whole numbers without any decimal places.

C# provides several basic integer data types, including `byte`, `short`, `int`, and `long`. Each has its own range, allowing you to choose the right type based on the magnitude of the numbers you need to work with.

|Data Type|Bits|Byte(s)|Minimum Value|Maximum Value|
|-|-|-|-|-|
|sbyte|8|1|-128|127|
|byte|8|1|0|255|
|short|16|2|-32768|32767|
|ushort|16|2|0|65535|
|int|32|4|-2147483648|2147483647|
|uint|32|4|0|4294967295|
|long|64|8|-9223372036854775808|9223372036854775807|
|ulong|64|8|0|18446744073709551615|

Choosing the right integer type is about finding a balance between saving memory and accommodating the range of values our program needs.

The `byte` data type is the smallest integer type in C#. It can store values from `0` to `255`. Perfect for situations where memory is a precious resource!

The `short` data type provides a bit more range, accommodating values from `-32,768` to `32,767`. Useful when you need a bigger range than a byte but want to save memory compared to an int.

The `int` data type is our go-to for most integer needs. It can handle values from about `-2 billion` to `2 billion`.

When we arere dealing with astronomical numbers, we could use the `long` data type. It can hold values ranging from approximately `-9 quintillion` to `9 quintillion`.

## 🚢 Floating-Point Data Types

C# provides two basic floating-point data types - `float` and `double`.

Sometimes numbers get so large or small that scientific notation is more convenient. In C#, you can express floating-point literals using scientific notation, like `1.5e3` for 1500.

// TODO: Positive Infinity, Negative Infinity, NaN
**Positive Infinity, Negative Infinity, NaN**

In C#, certain floating-point operations can result in special values: Positive Infinity, Negative Infinity, and NaN (Not a Number). These values are used to represent results that exceed the limits of what can be represented in a floating-point type, as well as undefined or unrepresentable results.

### Positive Infinity:

- **Representation:** `Double.PositiveInfinity`, `Single.PositiveInfinity`
- **Meaning:** Represents a value greater than any other number.
- **Example:**
  ```csharp
  double positiveInf = Double.PositiveInfinity;
  double result = 1.0 / 0.0; // result is PositiveInfinity
  ```
- **Usage:** Occurs in operations where the result exceeds the maximum representable value, such as dividing a positive number by zero or an overflow in arithmetic operations.

### Negative Infinity:

- **Representation:** `Double.NegativeInfinity`, `Single.NegativeInfinity`
- **Meaning:** Represents a value less than any other number.
- **Example:**
  ```csharp
  double negativeInf = Double.NegativeInfinity;
  double result = -1.0 / 0.0; // result is NegativeInfinity
  ```
- **Usage:** Occurs in operations where the result is less than the minimum representable value, such as dividing a negative number by zero or an underflow in arithmetic operations.

### NaN (Not a Number):

- **Representation:** `Double.NaN`, `Single.NaN`
- **Meaning:** Represents an undefined or unrepresentable value.
- **Example:**
  ```csharp
  double nanValue = Double.NaN;
  double result = 0.0 / 0.0; // result is NaN
  ```
- **Usage:** Occurs in operations that do not yield a defined numeric result, such as dividing zero by zero, taking the square root of a negative number, or invalid arithmetic operations.

### Example Code:

```csharp
using System;

class Program
{
    static void Main()
    {
        // Positive Infinity
        double positiveInf = 1.0 / 0.0;
        Console.WriteLine(positiveInf); // Output: Infinity
        
        // Negative Infinity
        double negativeInf = -1.0 / 0.0;
        Console.WriteLine(negativeInf); // Output: -Infinity
        
        // NaN (Not a Number)
        double nanValue = 0.0 / 0.0;
        Console.WriteLine(nanValue); // Output: NaN
        
        // Checking for Infinity and NaN
        Console.WriteLine(Double.IsInfinity(positiveInf)); // Output: True
        Console.WriteLine(Double.IsPositiveInfinity(positiveInf)); // Output: True
        Console.WriteLine(Double.IsNegativeInfinity(negativeInf)); // Output: True
        Console.WriteLine(Double.IsNaN(nanValue)); // Output: True
    }
}
```

### Summary:

- **Positive Infinity:** Indicates a value greater than any other number.
- **Negative Infinity:** Indicates a value less than any other number.
- **NaN (Not a Number):** Indicates an undefined or unrepresentable value.

These special values help handle exceptional cases in floating-point arithmetic and ensure that operations return predictable results even when they encounter limits or undefined conditions.

## 🤔 Precision, Accuracy & Computer Memory

Precision refers to how finely a value can be expressed, while accuracy relates to how closely the represented value matches the true value.

Floating-point numbers, like `float` and `double`, offer precision but with limitations. Due to binary representation, not all decimal fractions can be precisely represented. This can lead to rounding errors, impacting accuracy.

// TODO: 0.3 = 0.1 + 0.2
```csharp
double result = 0.1 + 0.2;

if (result == 0.3)
{
    Console.WriteLine("The result is exactly 0.3");
}
else
{
    Console.WriteLine("The result is not exactly 0.3");
}
```

```csharp
double result = 0.1 + 0.2;

Console.WriteLine(result == 0.3 ? "The result is exactly 0.3" : "");
```


// TODO: 99999999999999999999999 * 2
```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        // Example 1: Multiplying a large number by 2 using float
        float result1_float = 99999999999999999999999f * 2;
        Console.WriteLine("Result of multiplying a large number by 2 using float: " + result1_float);
        // Expected result: 2.0E+23

        // Example 1: Multiplying a large number by 2 using double
        double result1_double = 99999999999999999999999d * 2;
        Console.WriteLine("Result of multiplying a large number by 2 using double: " + result1_double);
        // Expected result: 2.0E+23
    }
}
```

// TODO: 10000000000000000000000000 + 1
```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        // Example 2: Adding 1 to a very large number using float
        float result2_float = 10000000000000000000000000f + 1;
        Console.WriteLine("Result of adding 1 to a very large number using float: " + result2_float);
        // Expected result: 1.0E+25

        // Example 2: Adding 1 to a very large number using double
        double result2_double = 10000000000000000000000000d + 1;
        Console.WriteLine("Result of adding 1 to a very large number using double: " + result2_double);
        // Expected result: 1.0E+25
    }
}
```

In this code, `f` is appended to the end of the floating-point literal to indicate that it's a `float`, and `d` is appended to indicate that it's a `double`. The results may not match the expected mathematical results due to limitations in floating-point precision.
## 🚀 Decimal Precision Data Type

Unlike `float` and `double`, `decimal` is designed to represent decimal fractions with high precision.

Memory is a precious resource, and choosing the right data type involves trade-offs. While `float` and `double` are more memory-efficient, they sacrifice some precision. On the other hand, `decimal` provides precision but at the cost of increased memory usage.

In financial calculations, where precision is crucial, using the `decimal` type ensures accurate representation of monetary values, avoiding potential rounding discrepancies.

## 🌓 Boolean Data Type

Booleans represent `true` or `false` values.

```csharp
bool isWarm; // 👈 Default value: false
isWarm = true;

bool isSunny = true;
bool isRaining = false;
```

When a boolean variable is declared but not explicitly initialized, it defaults to `false`.

An expression that could be evaluated to `true` or `false` is called a `boolean` expression.

Imagine a smart home system. Using `boolean` values, we can represent whether lights are on or off, doors are locked or unlocked, and create smart rules based on these conditions.

Functions can return boolean values, indicating the success or failure of an operation. For example, a function to check if a user is authenticated might return `true` if authentication is successful.

## 🔣 Character Data Type

Characters represent individual symbols, letters, or digits.

```csharp
char symbol;
symbol = '$';

char letter = 'A';
char emoji = '😊';
```

Behind the scenes, characters in C# are represented using Unicode. Unicode allows the representation of a vast array of characters, including international symbols, emojis, and special characters.

## String Data Type

// TODO: Strings are not a primitive data type.
In C# language, strings are not considered primitive data types. Unlike primitive data types, such as integers or floats, which store single values, strings are sequences of characters. They are represented by the `string` keyword in C#. Strings can store textual data, such as words or sentences, and are treated as objects with built-in methods for manipulation rather than simple data types like integers or floats. For example:

```csharp
string myString = "Hello, world!";
Console.WriteLine(myString.ToUpper()); // Output: "HELLO, WORLD!"
```

In this example, `myString` is a string object, and the `ToUpper()` method is used to convert the string to uppercase. This distinction is essential because strings often require special handling and operations compared to primitive data types.

```csharp
string firstName = "John";
string lastName = "Smith";

Console.Write(firstName);
Console.Write(" "); // 👈 Represents a space (1 symbol)
Console.Write(lastName);
```

```csharp
string emptyString = ""; // 👈 0 symbols
Console.WriteLine(emptyString); // 👈 Prints ""
```

```csharp
string emptyString = string.Empty; // 👈 Special value
Console.WriteLine(emptyString); // 👈 Prints ""
```

## Variables Characteristics

// TODO: Name
In C# programming, a variable's name serves as its identifier and is used to reference the stored data. A variable name must adhere to certain rules:

1. **Validity**: It must be a valid identifier according to the C# language's rules.
2. **Descriptive**: It should reflect the purpose or meaning of the stored data.
3. **Readable**: It should be easily understandable by other developers.
4. **Consistency**: It should follow a consistent naming convention within the codebase.
5. **Case sensitivity**: Variable names in C# are case-sensitive.

For example:

```csharp
// Valid variable names
int age = 25;
string firstName = "John";
bool isStudent = true;

// Invalid variable names
int 2ndName = 30;  // starts with a digit
string last name = "Doe";  // contains space
```

Here, `age`, `firstName`, and `isStudent` are valid variable names because they adhere to the rules, while `2ndName` and `last name` are invalid due to starting with a digit and containing a space, respectively.

// TODO: Type
In C# programming, variables have a type associated with them, which defines the kind of data they can store. The type of a variable determines the size of memory it occupies and the operations that can be performed on it. 

- **Primitive Types**: Basic data types built into the language, such as integers, floating-point numbers, characters, and Booleans.
- **Reference Types**: Types that are defined by classes and require memory allocation. These include objects, arrays, and strings.

For example:

```csharp
// Primitive types
int age = 25;
double salary = 1000.50;
char grade = 'A';
bool isStudent = true;

// Reference types
string name = "John";
object obj = new object();
int[] numbers = { 1, 2, 3, 4, 5 };
```

In this example, `age`, `salary`, `grade`, and `isStudent` are variables of primitive types (`int`, `double`, `char`, and `bool`, respectively), while `name` is a variable of reference type (`string`), and `obj` is a variable of type `object`, which is the base class for all types in C#. `numbers` is an array, which is also a reference type. Each type defines the range of values it can hold and the operations that can be performed on it.

// TODO: Value
In C# programming, the value of a variable refers to the data it currently holds. Variables can store various types of data, including numbers, characters, strings, and objects. The value of a variable can change during the execution of a program.

```csharp
int age = 25;         // age variable holds the value 25
double salary = 1000.50;  // salary variable holds the value 1000.50
char grade = 'A';      // grade variable holds the value 'A'
bool isStudent = true; // isStudent variable holds the value true

string name = "John";  // name variable holds the value "John"
object obj = new object();  // obj variable holds a reference to a new object instance

int[] numbers = { 1, 2, 3, 4, 5 };  // numbers variable holds a reference to an array of integers
```

In this example, each variable is assigned a specific value based on its type. These values can be manipulated, reassigned, or used in calculations as needed during the execution of the program.

## Variables Declaration & Initialization

Declaring a variable is like claiming a piece of memory and giving it a name.

```csharp
int age; // 👈 Variable Declaration
```

```csharp
age = 25; // 👈 Variable Initialization
```

```csharp
int age = 25; // 👈 Variable Declaration & Initialization
```

`Pseudocode`

```
<data_type> <variable_name> = <value>;
```

We can declare several variables in a single statement.

```csharp
int a, b, c, d, e;
```

// TODO: If we do not specify the value of a variable they default to their default values.
In C#, when a variable is declared but not initialized with a value explicitly, it will be assigned a default value based on its type. This ensures that variables always have a predictable starting value, even if one is not explicitly provided by the programmer. These default values are determined by the data type of the variable.

Here are the default values for some common data types in C#:

- **Numeric types (such as `int`, `double`, `float`, etc.)**: Default to 0.
- **Boolean type (`bool`)**: Defaults to `false`.
- **Character type (`char`)**: Defaults to the Unicode character with the value `\0` (null character).
- **Reference types (such as `string`, `object`, arrays, etc.)**: Defaults to `null`.

Here are examples demonstrating how variables default to their default values in C#:

```csharp
class Program
{
    static void Main(string[] args)
    {
        // Default values for numeric types
        int num;            // num defaults to 0
        double salary;      // salary defaults to 0.0
        float pi;           // pi defaults to 0.0f
        decimal amount;     // amount defaults to 0.0m

        // Default value for boolean type
        bool isStudent;     // isStudent defaults to false

        // Default value for character type
        char grade;         // grade defaults to '\0'

        // Default value for reference type (string)
        string name;        // name defaults to null

        // Default value for reference type (object)
        object obj;         // obj defaults to null

        // Default value for reference type (array)
        int[] numbers;      // numbers defaults to null
    }
}
```

In the above examples, variables are declared but not initialized with any specific values. As a result, they default to their respective default values based on their data types.

// TODO: Cascade assignment.
Cascade assignment in C# refers to the practice of assigning the same value to multiple variables in a single statement. This can help improve code readability and reduce redundancy by eliminating the need to repeat the same assignment expression multiple times.

Here's an example to illustrate cascade assignment:

```csharp
class Program
{
    static void Main(string[] args)
    {
        int x, y, z;

        // Cascade assignment
        x = y = z = 10;

        Console.WriteLine("x = " + x); // Output: x = 10
        Console.WriteLine("y = " + y); // Output: y = 10
        Console.WriteLine("z = " + z); // Output: z = 10
    }
}
```

In the example above, the value `10` is assigned to variables `x`, `y`, and `z` using cascade assignment. This single line of code is equivalent to the following three lines:

```csharp
z = 10;
y = z;
x = y;
```

Cascade assignment can also be combined with other operations, such as arithmetic or function calls:

```csharp
int a, b, c;

// Cascade assignment with arithmetic operations
a = b = c = 5;
a += 2;
b *= 3;
c -= 1;

Console.WriteLine("a = " + a); // Output: a = 7
Console.WriteLine("b = " + b); // Output: b = 15
Console.WriteLine("c = " + c); // Output: c = 4
```

In this example, the value `5` is assigned to variables `a`, `b`, and `c` using cascade assignment. Then, each variable undergoes a different arithmetic operation.

```csharp
int x, y;

x = y = 4;
```

## 🏷️ Naming Variables

In C#, camelCase is the norm for naming variables. This means the first word is in lowercase, and subsequent words start with an uppercase letter. For instance, `totalAmount`, not `totalamount` or `TotalAmount`.

When naming variables, choose names that reflect the purpose or content of the data they hold. For example, instead of `x` or `y`, use names like `width` and `height` to convey the meaning of the variables.

|Data Type(s)|👌|👎|
|-|-|-|
|`byte`, `short`, `int`, `long`|`employeesCount`, `discountPercent`|`a`, `number`, `value`, `variable`|
|`float`, `double`, `decimal`|`productDiscount`||
|`boolean`|`isAuthenticated`, `isVisible`, `gameOver`||
|`char`|||
|`string`|`queryString`, `firstName`, `lastName`|`str`, `theStringThatHoldsFirstName`|

|Incorrect Variable Names|Reason|
|-|-|
|`a`, `i`, `x`|Too short|
|`iAmAVeryVeryVeryLongName`|Too long|
|`first_name`|Contains `_` (Snake case)|
|`2pac`|Starts with a number|
|`FIRSTNAME`|Uppercase|
|`FirstName`|Starts with a capital letter (Pascal case)|

Variables follow the Single Responsibility Principle. Each variable should have a clear and single responsibility. For instance, a variable named `userName` should store the user's name and nothing else.

// TODO: Keywords use "@".
In C#, the `@` symbol can be used as a prefix to indicate that a word is a keyword or reserved word, allowing it to be used as an identifier (such as a variable or method name) without conflict. This is particularly useful when you need to use a keyword as an identifier, which would normally cause a syntax error.

Here's how you can use the `@` symbol to use keywords as identifiers:

```csharp
class @class // Using keyword "class" as an identifier
{
    public int @int; // Using keyword "int" as an identifier
    public string @string; // Using keyword "string" as an identifier
    public void @void() // Using keyword "void" as an identifier
    {
        // Method implementation
    }
}
```

In the above example:

- `@class` is a class identifier, using the keyword `class`.
- `@int` is a variable identifier, using the keyword `int`.
- `@string` is a variable identifier, using the keyword `string`.
- `@void` is a method identifier, using the keyword `void`.

By prefixing these identifiers with the `@` symbol, you can use C# keywords without causing compilation errors. However, it's generally recommended to avoid using keywords as identifiers whenever possible to maintain code readability and avoid confusion.

// TODO: Many examples online include the words "foo" and "bar". These words...
In programming, particularly in tutorials, examples, and documentation, you often encounter the words "foo" and "bar". These are placeholder names used to represent generic variables, functions, or values. They are not reserved keywords or predefined identifiers in programming languages; rather, they are used to illustrate concepts without introducing unnecessary complexity.

The usage of "foo" and "bar" is a convention that dates back to early computer science and programming literature. These words are chosen because they are short, easy to remember, and unlikely to be confused with actual programming constructs. They serve as placeholders that can be easily replaced with meaningful names when writing actual code.

Here's an example demonstrating the usage of "foo" and "bar" in C#:

```csharp
class Program
{
    static void Main(string[] args)
    {
        // Using "foo" and "bar" as generic variable names
        int foo = 10;
        int bar = 20;
        int result = foo + bar;

        Console.WriteLine("The result of adding foo and bar is: " + result);
    }
}
```

In this example, "foo" and "bar" are used as generic variable names representing integer values. While these names do not convey specific meaning in the context of the code snippet, they help illustrate the concept of variable assignment and arithmetic operations. In real-world scenarios, you would use more descriptive variable names to improve code readability and maintainability.

## .NET Common Type System

|.NET Type|Alias|
|-|-|
|System.SByte|sbyte|
|System.Byte|byte|
|System.Int16|short|
|System.UInt16|ushort|
|System.Int32|int|
|System.UInt32|uint|
|System.Int64|long|
|System.UInt64|ulong|
|System.Single|float|
|System.Double|double|
|System.Decimal|decimal|
|System.Boolean|bool|
|System.Char|char|
|System.String|string|

## 📜 Guides

Aim for clarity and avoid using abbreviations or acronyms that may be unclear to others (or even yourself in the future!). Choose names that make your intentions obvious, promoting easy understanding.

It's okay to revisit and refine names as your code evolves. If you discover a more fitting name or if the purpose of a variable changes, take the time to refactor and keep your codebase tidy.

Follow a consistent naming style throughout your codebase. Consistency simplifies reading and understanding.

Sometimes we can use short names for our variables testing purposes - whether the solution will work or not. Once we find a suitable solution we can refactor the code.

Avoid using magic values (hard-coded values) without context. Instead, use named variables to give these values meaning.

Use `decimal` when handling monetary values, scientific measurements, or any scenario where exact representation of decimal fractions is essential.

Do not declare more than one variable per statement. Try to initialize the variable if that is possible.

Avoid cascade assignments. We can assign the values to the variables using as many statements as needed.

```csharp
int x, y;

x = 4;
y = 4;
```
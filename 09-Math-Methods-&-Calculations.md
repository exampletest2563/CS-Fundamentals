# 📐 Math Methods & Calculations

## 🔢 The "Math" Class

The `Math` class provides constants and methods for trigonometric, logarithmic, and other common mathematical functions.

Some of the functions offered by the `Math` class include:
- `Math.Abs(x)`: Returns the absolute value of `x`;
- `Math.Sqrt(x)`: Returns the square root of `x`;
- `Math.Pow(x, y)`: Returns `x` raised to the power of `y`;
- `Math.Round(x)`: Rounds `x` to the nearest integer.

The `Math` class also provides useful constants:
- `Math.PI`: The mathematical constant `π`;
- `Math.E`: The mathematical constant `e`.

In programming, the "Math" class serves as a toolbox packed with tools to facilitate various mathematical operations. It's a predefined collection of functions and constants that programmers can utilize to simplify calculations within their code.

**Overview:**
The "Math" class in programming languages such as Java and C# provides a plethora of mathematical functions and constants, ranging from basic arithmetic operations to trigonometric functions and rounding methods. This chapter explores the capabilities of the "Math" class, demonstrating how it can be used to perform diverse mathematical tasks efficiently.

**Contents:**
1. **Basic Arithmetic Operations:** Addition, subtraction, multiplication, and division operations can be performed using the "Math" class, making it easier to manipulate numerical values within the code.
   
2. **Exponents and Roots:** The "Math" class enables programmers to calculate exponents (raising a number to a power) and find square roots effortlessly.
   
3. **Trigonometric Functions:** Trigonometric functions such as sine, cosine, and tangent are available in the "Math" class, allowing for the calculation of trigonometric values with ease.
   
4. **Constants:** The "Math" class includes essential mathematical constants like Pi (π), which can be utilized in calculations without needing to define them separately.
   
5. **Random Numbers:** Programmers can generate random numbers using the "Math" class, useful for simulations, games, and other applications requiring randomization.
   
6. **Rounding:** The "Math" class provides methods for rounding numerical values to the nearest integer or specified decimal places, simplifying the rounding process.
   
7. **Absolute Value:** Finding the absolute value of a number, regardless of its sign, can be achieved using the "Math" class, ensuring accurate calculations in various scenarios.

**Example in C#:**
```csharp
// Calculate the square root of a number
double root = Math.Sqrt(25); // Returns 5.0

// Find the sine of an angle in radians
double sinValue = Math.Sin(Math.PI / 6); // Returns 0.5 (sin of 30 degrees)

// Generate a random number between 0 and 1
double randomNumber = new Random().NextDouble(); 

// Round a decimal value to the nearest integer
int roundedValue = (int)Math.Round(5.7); // Returns 6
```

In conclusion, the "Math" class is a valuable resource for programmers, offering a wide range of mathematical functions and constants to streamline mathematical operations in code.

## 📈 The "Max" Method

The `Math.Max` method returns the larger of two given numbers.

```csharp
var firstNumber = int.Parse(Console.ReadLine());
var secondNumber = int.Parse(Console.ReadLine());

//                   👇 Evaluated at runtime
var maxNumber = Math.Max(firstNumber, secondNumber);
Console.WriteLine(maxNumber);
```

```csharp
var firstNumber = int.Parse(Console.ReadLine());
var secondNumber = int.Parse(Console.ReadLine());

var maxNumber = 0;

//             👇 We could use ">" too
if (firstNumber >= secondNumber)
{
	maxNumber = firstNumber;
}
else
{
	maxNumber = secondNumber;
}

Console.WriteLine(maxNumber);
```

```csharp
var firstNumber = int.Parse(Console.ReadLine());
var secondNumber = int.Parse(Console.ReadLine());

//                         👇 We could use ">" too
var maxNumber = firstNumber >= secondNumber ? firstNumber : secondNumber;
Console.WriteLine(maxNumber);
```

The "Max" method is a handy tool in programming languages like Java and C# that allows you to find the maximum value among two or more numbers. It's part of the standard libraries and simplifies the process of comparing values and determining the largest one.

**Overview:**
The "Max" method is used to determine the maximum value among a set of numbers. It takes two or more parameters as input and returns the largest value among them. This chapter explores the usage of the "Max" method, demonstrating how it can be applied in various scenarios to find the maximum value efficiently.

**Contents:**
1. **Basic Usage:** The "Max" method compares two numbers and returns the larger one.
   
2. **Comparing Multiple Numbers:** You can use the "Max" method to compare more than two numbers and find the maximum among them.
   
3. **Applicability:** The "Max" method is useful in scenarios where you need to determine the largest value among a collection of numbers, such as finding the highest score in a game or identifying the peak temperature in a set of data.

**Example in Java:**
```java
// Find the maximum of two numbers
int maxNum = Math.max(10, 20); // Returns 20

// Find the maximum of multiple numbers
int maxNum = Math.max(10, Math.max(30, 15)); // Returns 30
```

**Example in C#:**
```csharp
// Find the maximum of two numbers
int maxNum = Math.Max(10, 20); // Returns 20

// Find the maximum of multiple numbers
int maxNum = Math.Max(10, Math.Max(30, 15)); // Returns 30
```

In conclusion, the "Max" method is a simple yet powerful tool for finding the maximum value among a set of numbers. It provides a convenient way to perform comparisons and determine the largest value, making it a valuable asset in various programming tasks.

## 📉 The "Min" Method

The `Math.Min` method returns the smaller of two given numbers.

```csharp
var firstNumber = int.Parse(Console.ReadLine());
var secondNumber = int.Parse(Console.ReadLine());

//                   👇 Evaluated at runtime
var minNumber = Math.Min(firstNumber, secondNumber);
Console.WriteLine(minNumber);
```

```csharp
var firstNumber = int.Parse(Console.ReadLine());
var secondNumber = int.Parse(Console.ReadLine());

var minNumber = 0;

//             👇 We could use "<" too
if (firstNumber <= secondNumber)
{
	minNumber = firstNumber;
}
else
{
	minNumber = secondNumber;
}

Console.WriteLine(minNumber);
```

```csharp
var firstNumber = int.Parse(Console.ReadLine());
var secondNumber = int.Parse(Console.ReadLine());

//                         👇 We could use "<" too
var minNumber = firstNumber <= secondNumber ? firstNumber : secondNumber;
Console.WriteLine(minNumber);
```

The "Min" method is a useful function in programming languages like Java and C# that allows you to find the minimum value among two or more numbers. It's part of the standard libraries and simplifies the process of comparing values and determining the smallest one.

**Overview:**
The "Min" method is employed to identify the minimum value among a set of numbers. It takes two or more parameters as input and returns the smallest value among them. This chapter delves into the application of the "Min" method, illustrating how it can be utilized in various scenarios to efficiently find the minimum value.

**Contents:**
1. **Basic Usage:** The "Min" method compares two numbers and returns the smaller one.
   
2. **Comparing Multiple Numbers:** You can utilize the "Min" method to compare more than two numbers and find the minimum among them.
   
3. **Applicability:** The "Min" method proves beneficial in situations where you need to determine the smallest value among a collection of numbers, such as identifying the lowest temperature in a dataset or finding the minimum price among a list of products.

**Example in Java:**
```java
// Find the minimum of two numbers
int minNum = Math.min(10, 20); // Returns 10

// Find the minimum of multiple numbers
int minNum = Math.min(10, Math.min(30, 15)); // Returns 10
```

**Example in C#:**
```csharp
// Find the minimum of two numbers
int minNum = Math.Min(10, 20); // Returns 10

// Find the minimum of multiple numbers
int minNum = Math.Min(10, Math.Min(30, 15)); // Returns 10
```

In conclusion, the "Min" method provides a straightforward approach to finding the minimum value among a set of numbers. Its inclusion in standard libraries aids in simplifying comparisons and determining the smallest value, making it a valuable asset in programming tasks that involve identifying minimum values.

## 📏 Absolute Value

In mathematics, the absolute value or modulus of a real number is the non-negative value of the number without regard to its sign.

It is denoted by `|x|`, where `x` is a real number.

The `Math.Abs` method returns the non-negative value of `x`.

```csharp
var x = int.Parse(Console.ReadLine());

var absoluteValue = Math.Abs(x);
Console.WriteLine(absoluteValue);
```

The absolute value of a number measures the distance of the number from zero along the real number line, regardless of its direction, and is always a positive value.

Normally, we would use such functions when working with the value itself, regardless of its sign.

```csharp
var x = int.Parse(Console.ReadLine()); // Example: "-5"

//                               👇 -(-5) = 5
var absoluteValue = x >= 0 ? x : -x;
Console.WriteLine(absoluteValue); // 👈 Prints "5"

```

Understanding absolute value is crucial in programming, especially when dealing with numerical data. The absolute value of a number represents its distance from zero on the number line, regardless of its sign. In programming languages like Java and C#, the "Math" class provides a method to easily calculate the absolute value of a number.

**Overview:**
The absolute value of a number is its distance from zero on the number line, always resulting in a non-negative value. The "Math" class in programming languages like Java and C# offers a function to compute the absolute value of a given number, simplifying the process of determining its magnitude without considering its sign.

**Contents:**
1. **Definition:** The absolute value of a number is the value without regard to its sign. It represents the distance between the number and zero on the number line.
   
2. **Mathematical Representation:** The absolute value of a number 'x' is denoted as |x|.
   
3. **Usage:** In programming, the "Math" class provides a method to compute the absolute value of a number, irrespective of its sign.
   
4. **Application:** Absolute value finds application in various programming scenarios, such as calculating differences, distances, or ensuring positive values in calculations.

**Example in Java:**
```java
// Calculate the absolute value of a number
int absoluteValue = Math.abs(-10); // Returns 10
```

**Example in C#:**
```csharp
// Calculate the absolute value of a number
int absoluteValue = Math.Abs(-10); // Returns 10
```

In conclusion, understanding and utilizing the absolute value function provided by the "Math" class in programming languages like Java and C# is essential for tasks involving numerical computations. Whether it's determining distances, ensuring positive values, or handling differences, the absolute value function simplifies the process of working with numerical data.

## ✨ Exponentiation

In mathematics, exponentiation is the process of raising a number to a specific power.

The `Math.Pow` method returns a specified number raised to the specified power.

```csharp
var baseNumber = int.Parse(Console.ReadLine()); // Example: "2"
var exponent = int.Parse(Console.ReadLine()); // Example: "5"

var result = Math.Pow(baseNumber, exponent);
Console.WriteLine(result); // 👈 Prints "32"
```

```csharp
var number = int.Parse(Console.ReadLine()); // Example: "2"
var power = int.Parse(Console.ReadLine()); // Example: "5"
var result = 1;

for (int counter = 1; counter <= power; counter++)
{
	result *= number;
}

Console.WriteLine(result); // 👈 Prints "32"
```

The `Math.Pow` method can handle negative exponents, resulting in fractions or decimals.

Exponentiation is a fundamental mathematical operation that involves raising a number to a certain power. In programming, exponentiation is commonly used to perform calculations involving repeated multiplication. Languages like Java and C# provide built-in functions or operators to handle exponentiation efficiently.

**Overview:**
Exponentiation refers to the process of raising a base number to an exponent, which represents the number of times the base is multiplied by itself. It is denoted using the "^" symbol or specific functions in programming languages like Java and C#.

**Contents:**
1. **Basic Definition:** Exponentiation involves raising a base number to a specified exponent, resulting in the base number multiplied by itself a certain number of times.
   
2. **Mathematical Representation:** Exponentiation is typically represented as "base^exponent" or "base raised to the power of exponent."
   
3. **Usage in Programming:** Programming languages provide built-in functions or operators to perform exponentiation efficiently.
   
4. **Operator vs. Function:** Some languages, like C#, offer the "**" operator for exponentiation, while others, like Java, provide a dedicated function such as Math.pow().
   
5. **Application:** Exponentiation is widely used in various computational tasks, including scientific calculations, financial modeling, and data analysis.

**Example in Java:**
```java
// Using Math.pow() function to perform exponentiation
double result = Math.pow(2, 3); // Returns 8.0 (2 raised to the power of 3)
```

**Example in C#:**
```csharp
// Using the exponentiation operator "**"
double result = 2 ** 3; // Returns 8.0 (2 raised to the power of 3)
```

In conclusion, understanding exponentiation and how to perform it efficiently using built-in functions or operators provided by programming languages is essential for various computational tasks. Whether it's calculating compound interest, modeling exponential growth, or solving mathematical equations, exponentiation plays a crucial role in many programming scenarios.

## 🌱 Square Root

In mathematics, the square root of a number is a value that, when multiplied by itself, gives the original number.

The `Math.Sqrt` method returns the square root of a specified number.

```csharp
var number = int.Parse(Console.ReadLine()); // Example: "9"

var squareRoot = Math.Sqrt(number);
Console.WriteLine(squareRoot); // 👈 Prints "3"
```

While square roots of negative numbers are not real in the realm of real numbers, C# handles them using the `NaN` (Not a Number) value.

```csharp
var number = -4;

var squareRoot = Math.Sqrt(number);
Console.WriteLine(squareRoot); // 👈 Prints "NaN"
```

The square root is a mathematical operation that determines a value which, when multiplied by itself, equals a given number. In programming, finding the square root of a number is a common task, especially in applications involving geometry, physics, or numerical analysis. Languages like Java and C# provide built-in functions to calculate square roots efficiently.

**Overview:**
The square root of a number is a value that, when multiplied by itself, yields the original number. It's denoted using the radical symbol (√) or specific functions in programming languages like Java and C#.

**Contents:**
1. **Basic Definition:** The square root of a number 'x' is another number 'y' such that y * y = x.
   
2. **Mathematical Representation:** The square root of a number 'x' is represented as √x.
   
3. **Usage in Programming:** Programming languages offer built-in functions to compute square roots efficiently.
   
4. **Function or Operator:** Some languages, like Java, provide a dedicated function such as Math.sqrt(), while others, like C#, offer the Math.Sqrt() function.
   
5. **Application:** Square roots are used in various fields of science, engineering, and mathematics, including geometry, physics, and statistics.

**Example in Java:**
```java
// Using Math.sqrt() function to find the square root
double root = Math.sqrt(25); // Returns 5.0 (square root of 25)
```

**Example in C#:**
```csharp
// Using Math.Sqrt() function to find the square root
double root = Math.Sqrt(25); // Returns 5.0 (square root of 25)
```

In conclusion, understanding how to calculate square roots efficiently using built-in functions provided by programming languages is essential for various computational tasks. Whether it's determining distances in geometric problems, calculating velocities in physics, or performing statistical analysis, square roots play a vital role in many programming applications.

## 🎯 Rounding Numbers

Rounding could be used to present numbers in a more manageable form, especially when dealing with real-world scenarios that require precision.

The `Math.Floor` method returns the largest integral value less than or equal to the specified number.

```csharp
var realNumber = double.Parse(Console.ReadLine()); // Example: "7.64"

var roundedValue = Math.Floor(realNumber);
Console.WriteLine(roundedValue); // 👈 Prints "7"
```

The `Math.Ceiling` method returns the smallest integral value that is greater than or equal to the specified number.

```csharp
var realNumber = double.Parse(Console.ReadLine()); // Example: "7.24

var roundedValue = Math.Ceiling(realNumber);
Console.WriteLine(roundedValue); // 👈 Prints "8"
```

The `Math.Round` method rounds a decimal value to a specified number of fractional digits using the specified rounding convention.

```csharp
var realNumber = double.Parse(Console.ReadLine());

// 2 👈 Number of fractional digits
// MidpointRounding.AwayFromZero 👈 Rounding convention
var roundedNumber = Math.Round(realNumber, 2, MidpointRounding.AwayFromZero);

Console.WriteLine(roundedNumber);
```

The `Math.Round` method supports two rounding conventions for handling midpoint values:
- Rounding away from zero: This form of rounding is represented by `MidpointRounding.AwayFromZero`;
- Rounding to nearest even, or banker's rounding: This form of rounding is represented by `MidpointRounding.ToEven`.

The `Math.Truncate` method returns the number that remains after any fractional digits have been discarded.

```csharp
var realNumber = double.Parse(Console.ReadLine()); // Example: "6.8"

var doubleNumber = Math.Truncate(realNumber); // 👈 Data Type: System.Double
Console.WriteLine(doubleNumber); // 👈 Prints "6"
```

```csharp
var realNumber = double.Parse(Console.ReadLine()); // Example: "6.8"

var integerNumber = (int)(realNumber); // 👈 Data Type: System.Int32
Console.WriteLine(integerNumber); // 👈 Prints "6"
```

Rounding numbers is a common mathematical operation used to simplify values to a specific precision or to make them easier to work with. In programming, rounding numbers is crucial for tasks like formatting output, simplifying calculations, and improving readability. Both Java and C# offer built-in functions to round numbers efficiently.

**Overview:**
Rounding numbers involves adjusting numerical values to a certain level of precision by replacing them with nearby integers or multiples of powers of 10. It's denoted using specific functions or methods provided by programming languages like Java and C#.

**Contents:**
1. **Basic Definition:** Rounding a number involves approximating it to a specified level of precision, typically to a certain number of decimal places or to the nearest integer.
   
2. **Mathematical Concepts:** Rounding can be performed using various methods such as rounding up, rounding down, or rounding to the nearest integer.
   
3. **Usage in Programming:** Programming languages offer built-in functions or methods to perform rounding operations efficiently.
   
4. **Function or Method:** Languages like Java provide methods such as Math.round(), while C# offers functions like Math.Round().
   
5. **Rounding Modes:** Some rounding functions allow you to specify rounding modes such as rounding towards positive infinity, rounding towards negative infinity, or rounding towards zero.
   
6. **Application:** Rounding numbers is essential in various programming tasks, including financial calculations, statistical analysis, and data visualization.

**Example in Java:**
```java
// Using Math.round() function to round a decimal value to the nearest integer
int roundedValue = Math.round(5.7); // Returns 6

// Using Math.round() function to round a decimal value to two decimal places
double roundedDecimal = Math.round(3.14159 * 100) / 100.0; // Returns 3.14
```

**Example in C#:**
```csharp
// Using Math.Round() function to round a decimal value to the nearest integer
int roundedValue = (int)Math.Round(5.7); // Returns 6

// Using Math.Round() function to round a decimal value to two decimal places
double roundedDecimal = Math.Round(3.14159, 2); // Returns 3.14
```

In conclusion, understanding how to round numbers efficiently using built-in functions or methods provided by programming languages is crucial for various computational tasks. Whether it's formatting output for display, simplifying calculations, or ensuring accuracy in mathematical operations, rounding numbers plays a vital role in programming.
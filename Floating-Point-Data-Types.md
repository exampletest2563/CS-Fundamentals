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

In C#, both `float` and `double` are used to represent floating-point numbers, which are numbers that have a decimal point. However, they differ in terms of precision and size:

1. **float**:
   - `float` is a single-precision floating-point type.
   - It occupies 4 bytes (32 bits) of memory.
   - It can represent numbers with up to 7 significant digits.
   - Example:
     ```csharp
     float floatValue = 3.14f;
     ```

2. **double**:
   - `double` is a double-precision floating-point type.
   - It occupies 8 bytes (64 bits) of memory.
   - It can represent numbers with up to 15-16 significant digits.
   - Example:
     ```csharp
     double doubleValue = 3.14;
     ```

The 'f' and 'd' at the end of a numeric literal indicate the type of the literal:

- **'f' suffix**: It indicates that the literal is of type `float`. If you don't include the 'f' suffix, the compiler treats the literal as a `double` by default.
  Example:
  ```csharp
  float floatValue = 3.14f; // 'f' suffix indicates float
  ```

- **'d' suffix (optional)**: It indicates that the literal is of type `double`. However, it's optional because floating-point literals without any suffix are automatically treated as `double` by the compiler.
  Example:
  ```csharp
  double doubleValue = 3.14; // 'd' suffix (optional) indicates double
  ```

If you don't include the 'f' or 'd' suffix, the compiler determines the type of the literal based on its value and context. However, it's good practice to explicitly specify the suffix to avoid any confusion and to ensure that the literal is interpreted correctly.

Sure, let's explore some engaging examples of using floating-point data types in C# with creative variable names and interesting scenarios.

### Floating-Point Data Types in C#:
1. **`float`**: Single-precision floating-point type (suffix: `f`).
2. **`double`**: Double-precision floating-point type (no suffix).
3. **`decimal`**: Decimal floating-point type (suffix: `m`).

### Engaging Examples:

#### 1. Exploring Planetary Distances 🪐
```csharp
double distanceToSunInKm = 149_600_000; // Distance from Earth to Sun
double distanceToNeptuneInAU = 30.07;    // Distance from Earth to Neptune in Astronomical Units
```

#### 2. Calculating Wealth 🤑
```csharp
decimal billionaireNetWorthInUSD = 112_000_000_000.50m; // Jeff Bezos' net worth
```

#### 3. Mixing Colors in Design 🎨
```csharp
float redIntensity = 0.8f;    // Intensity of red in RGB color model
double greenSaturation = 0.55; // Saturation of green
```

#### 4. Measuring Cosmic Time 🕰️
```csharp
double ageOfUniverseInYears = 13.8e9;  // Approximate age of the universe in years
```

#### 5. Simulating Ocean Depths 🌊
```csharp
float depthOfMarianaTrenchInKm = 10.994f; // Maximum depth of the Mariana Trench in kilometers
```

#### 6. Tracking Temperature Changes 🌡️
```csharp
double temperatureOnVenusInCelsius = 462.0; // Surface temperature on Venus in Celsius
```

#### 7. Exploring Mathematical Constants 🧮
```csharp
double pi = 3.141592653589793238; // Approximate value of Pi
float goldenRatio = 1.6180339887498948482f; // Golden ratio
```

### Special Values:

#### Infinity and Not-a-Number (NaN):
```csharp
double infinity = double.PositiveInfinity; // Represents positive infinity
double negativeInfinity = double.NegativeInfinity; // Represents negative infinity
double notANumber = double.NaN; // Represents a value that is not a number
```

### Summary:
Floating-point data types in C# allow us to work with real numbers, making them essential for various applications, from scientific calculations to financial analysis and game development. By using creative variable names and engaging scenarios, we can explore the vast possibilities of working with floating-point numbers in C#. Remember to handle special values like infinity and NaN appropriately in your code for robustness and correctness.
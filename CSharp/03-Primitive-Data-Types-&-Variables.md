## 💾 Computer Memory

### 🧠 Computer Memory & Human Brain

Computers use two main storage components:

- **RAM** (Random Access Memory)
- **HDD** (Hard Disk Drive) or **SSD** (Solid State Drive)

Both components are physical components used for data storage.

The main difference between **RAM** and **HDD** is the type of storage.

**HDD** stores data permanently. It is responsible for storing all data no matter if the machine is turned on or off.

**RAM** stores data temporarily. It is responsible for all applications that run on the computer.

In terms of storing data, there are some rough similarities between computer memory and the human memory.

**RAM** in a computer serves as temporary storage for data that the computer is actively using. Similarly, the human brain's short-term memory functions as a temporary storage system for information that is currently being processed or manipulated.

**RAM** allows for fast access to stored data, with data retrieval times measured in nanoseconds. Similarly, short-term memory in the brain enables quick access to recently encountered information.

**RAM** has a limited capacity compared to other forms of storage in a computer, and its contents are typically erased when the computer is powered off. Similarly, short-term memory in the brain has a limited capacity and is susceptible to interference, with its contents often fading over time or being displaced by new information.

**HDD** in a computer serves as long-term storage for data that is not actively being used. Similarly, the human brain's long-term memory stores a vast amount of information accumulated over a lifetime, including facts, experiences, and skills.

Accessing data from an **HDD** is slower compared to **RAM**, with retrieval times measured in milliseconds. Similarly, accessing information from long-term memory in the brain may take longer compared to short-term memory.

**HDD** typically have a higher storage capacity compared to **RAM**, allowing it to store large amounts of data persistently. Similarly, long-term memory in the brain has a vast capacity, enabling individuals to retain a lifetime of experiences and knowledge.

### Memory Sizes

Understanding memory sizes is important because of their impact on data structures and efficient data handling.

A **bit** is the smallest unit of memory, capable of storing a single binary digit (`0` or `1`). It represents the basic building block of digital information in computers. For example, a bit can represent the state of an electrical signal in a computer circuit, where `0` might represent no voltage and `1` might represent a high voltage.

```
_
__
___
____
```

A **byte** consists of a group of 8 bits. Bytes are used to represent larger units of data, such as characters, numbers, or instructions. Bytes are used to represent larger units of data, such as characters, numbers, or instructions.

```
________
```

A **kilobyte** is equal to 1,024 bytes. It's commonly used to measure the size of small files, documents, or images.

A **megabyte** is equal to 1,024 kilobytes, or approximately 1 million bytes. It's used to measure the size of larger files, such as music files or high-resolution images.

A **gigabyte** is equal to 1,024 megabytes, or approximately 1 billion bytes. It's commonly used to measure the size of storage devices, such as hard drives or flash drives.

A **terabyte** is equal to 1,024 gigabytes, or approximately 1 trillion bytes. It's used to measure the size of large datasets, such as databases or video libraries.

## 🔣 Data Types (Computer Science)

### Introduction to Data Types

In computer science, data types serve as categories that inform the computer how to understand, interpret and handle different kinds of data and information.

Computers use a specific amount of memory to store each type of data.

Here's a simple breakdown of how much memory some common data types typically use:

- **1 byte:** This is like the smallest unit of storage in a computer. It can store a small number or a single character.
- **4 bytes:** This is a bit larger and can store bigger numbers or longer strings.
- **8 bytes:** Even larger, used for really big numbers or complex data.

When a program runs, it reserves memory space for each data type it needs. So, if you have an integer value, the computer will set aside enough memory to hold an integer value. This way, the computer knows how much space to allocate for each piece of data, making it easier and faster to work with.

By understanding the number of bits used to represent a data type and whether it is signed or unsigned, you can calculate the range of possible values that can be stored in variables of that data type.

To calculate the possible values for a data type, you need to consider the size (in bits) of the data type and whether it is signed (can represent positive and negative numbers) or unsigned (only represents positive numbers).

For example:

- Data type: `int`
- Signed: `true`
- Memory Usage: `32 bits` / `4 bytes`
- Possible Values Total: `2^32`, where `32` is the number of bits
- Possible Negative Numbers: `2^31`
- Possible Positive Numbers: `2^31 - 1` (includes `0`)

Primitive data types are data types that are built-in into the programming language.

### Data Types Characteristics

The characteristics of data types in programming include:

1. **Size**: Data types have a specific size, measured in bits or bytes, which determines the range of values they can represent. For example, an 8-bit integer can represent values from 0 to 255, while a 32-bit integer can represent values from -2,147,483,648 to 2,147,483,647.
2. **Range of Values**: Each data type has a range of values it can represent, which is determined by its size and whether it is signed (can represent positive and negative numbers) or unsigned (only represents positive numbers). For example, a 16-bit signed integer can represent values from -32,768 to 32,767, while an unsigned 16-bit integer can represent values from 0 to 65,535.
3. **Precision**: Precision refers to the level of detail or accuracy with which a data type can represent values. For example, floating-point data types provide greater precision for representing fractional numbers compared to integer data types.
4. **Default Values**: Data types may have default values assigned to variables of that type when they are declared but not explicitly initialized. For example, integer variables may default to 0, and boolean variables may default to false.
5. **Storage Format**: Different data types are stored in memory using different formats. For example, integers are typically stored using a fixed number of bits, while floating-point numbers use a format that includes a sign bit, exponent, and mantissa.
6. **Operations**: Data types support specific operations or behaviors, such as arithmetic operations (e.g., addition, subtraction), comparison operations (e.g., equality, inequality), and logical operations (e.g., AND, OR).
7. **Memory Allocation**: Each variable of a data type requires a certain amount of memory to store its value. The memory allocation for variables of different data types depends on their size and the underlying architecture of the computer system.

Understanding these characteristics is essential for selecting the appropriate data type. This way developers ensure ensuring that the program can store the necessary values accurately and efficiently.

## 📦 Variables Introduction

Variables are **containers** for storing and managing data. They allow us to **name** and **manipulate** values. Think of them as **labeled boxes** where we can put different things, like numbers, words, or other pieces of information.

```csharp
//          👇 Value
int number = 5;
//   👆 Variable name

Console.WriteLine(number); // 👈 Prints: "5"
```

Variables declared with the `int` keyword store integers.

```csharp
//                   👇 Value
string firstName = "John";
//        👆 Variable name

Console.WriteLine(firstName); // 👈 Prints: "John"
```

Variables declared with the `string` keyword store text values or "strings".

Variables need to be **declared** first. This way we are telling the computer to set aside some memory to store the data.

```
dataType variableName; // 👈 Pseudocode that declares a variable
```

The `dataType` defines the type of data the variable can hold, such as `numbers` (integers or decimals), `characters`, or `boolean` values.

The `variableName` is the name we give to our variable. It is like a label on a container.

Once declared, we can assign a value to the variable using the assignment operator (`=`).

```
variableName = value;
```

Variables are essential because they allow us to work with and manipulate data in our programs. Instead of hard-coding specific values directly into our code, we can use variables to store and update information dynamically.

## 🔤 Literals

### Literals

Literals are the raw, straightforward values that we use directly.

Numeric literals are straightforward values like integers that we explicitly write in our code.

```csharp
5
```

```csharp
3.14
```

Character literals represent a single character.

```csharp
'a'
```

```csharp
'$'
```

String literals represent sequences of characters.

```csharp
"Hello World!"
```

```csharp
"Some text"
```

Boolean literals represent the truth values - `true` or `false`.

```csharp
true
```

```csharp
false
```

C# allows us to make numeric literals more readable by using underscores for separation.

```csharp
int largeNumber = 1_000_000; // 👈 1 million
```

```csharp
long creditCardNumber = 1234_5678_9012_3456; // 👈 16-digit credit card number
```

This feature enhances code readability, especially for large numeric values, because the underscores make it easier to read and understand large numeric values by visually separating groups of digits. The underscores do not affect the actual value of the literal.

### Suffix & Prefix

In C# literals, suffixes and prefixes are used to explicitly denote the type or format of a literal value, such as integers, floating-point numbers, and strings. They help the compiler interpret the literal correctly and apply appropriate conversions if necessary. Here’s a breakdown of suffixes and prefixes commonly used in C#:

### Prefixes

1. **0x or 0X**: Indicates a hexadecimal literal. For example, `0xAB` represents the hexadecimal value 171.
   
2. **0b or 0B**: Indicates a binary literal. For example, `0b1010` represents the binary value 10.

### Suffixes

1. **F or f**: Indicates a float literal. For example, `3.14f` explicitly declares the number as a float.

2. **M or m**: Indicates a decimal literal. For example, `123.45m` explicitly declares the number as a decimal.

3. **D or d**: Indicates a double literal. Although not required (as doubles are the default for floating-point literals without a suffix), `3.14d` explicitly declares the number as a double for clarity.

4. **L or l**: Indicates a long integer literal. For example, `123L` explicitly declares the number as a long integer.

5. **U or u**: Indicates an unsigned integer literal. For example, `123U` explicitly declares the number as an unsigned integer.

6. **UL or ul**: Indicates an unsigned long integer literal. For example, `123UL` explicitly declares the number as an unsigned long integer.

These prefixes and suffixes provide clarity and precision in defining the type of literal values in C#, ensuring proper compilation and execution of code.

## 🔢 Integer Data Types

Integers represent whole numbers without any decimal places.

C# provides several basic integer data types, including `byte`, `short`, `int`, and `long`. They allow us to work with numbers that can be counted, such as quantities of items or scores in a game.

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

Integer data types have a specific size, measured in bits, which determines the range of values they can represent. For example, a 32-bit integer can represent values from -2,147,483,648 to 2,147,483,647.

Integer data types can be signed, meaning they can represent both positive and negative numbers, or unsigned, meaning they can only represent positive numbers. Signed integers use one bit to represent the sign (positive or negative).

Choosing the right integer type is about finding a balance between saving memory and accommodating the range of values our program needs.

### Byte & Sbyte

The `byte` data type is the smallest integer type in C#. It can store values from `0` to `255`. Perfect for situations where memory is a precious resource.

```csharp
byte personAge = 25;
Console.WriteLine(personAge);
```

Variable name: `personAge`
Data type: `byte`
Literal: `25`
Description: Stores the age of a person 🧑

### Short & Ushort

The `short` data type provides a bit more range, accommodating values from `-32,768` to `32,767`. Useful when you need a bigger range than a `byte` but want to save memory compared to an `int`.

```csharp
short maximumSpeed = 30000;
Console.WriteLine(maximumSpeed);
```

Variable name: `maximumSpeed`
Data type: `short`
Literal: `30000`
Description: Represents the maximum speed in kilometers per hour of a high-performance sports car 🏎️

```csharp
ushort magicSpellPower = 10000u;
Console.WriteLine(magicSpellPower);
```

Variable name: `magicSpellPower`
Data type: `ushort`
Literal: `10000u`
Description: Represents the power level of a magical spell in a fantasy game ⚔️

### Int & Uint

The `int` data type, short for "integer," is used to store whole numbers. It can handle values from about `-2 billion` to `2 billion`. We could say that other integer data types could be interpreted as variations of the `int` data type.

```csharp
int distanceToMars = 1000000000;
Console.WriteLine(distanceToMars);
```

Variable name: `distanceToMars`
Data type: `int`
Literal: `1000000000`
Description: Stores the distance in kilometers from Earth to Mars 🚀

```csharp
uint quantumBits = 4294967295u;
Console.WriteLine(quantumBits);
```

Variable name: `quantumBits`
Data type: `uint`
Literal: `4294967295u`
Description: Stores the number of qubits in a quantum computer 🌌

### Long & Ulong

When we are dealing with astronomical numbers, we could use the `long` data type. It can hold values ranging from approximately `-9 quintillion` to `9 quintillion`.

```csharp
ulong worldPopulation = 7789654123UL; // 👈 Note the 'UL' postfix
Console.WriteLine(worldPopulation);
```

Variable name: `worldPopulation`
Data type: `ulong`
Literal: `7789654123UL`
Description: Stores the distance in kilometers from Earth to Mars 🌍

## 🚢 Floating-Point Data Types

C# provides two basic floating-point data types - `float` and `double`, which are numbers that have a decimal point.

The `float` data type can handle decimal numbers with single precision. It occupies 4 bytes (32 bits) of memory. It can represent numbers with up to 7 significant digits.

```csharp
float myFloat = 3f;
Console.WriteLine(myFloat);
```

The `double` data type can handle a more extensive range of values and provides higher precision. It occupies 8 bytes (64 bits) of memory. It can represent numbers with up to 15-16 significant digits.

```csharp
double myDouble = 5d;
Console.WriteLine(myDouble);
```

The 'f' and 'd' at the end of a numeric literal indicate the type of the literal:

The **'f' suffix** indicates that the literal is of type `float`. If you don't include the 'f' suffix, the compiler treats the literal as a `double` by default.

The **'d' suffix (optional)** indicates that the literal is of type `double`. However, it's optional because floating-point literals without any suffix are automatically treated as `double` by the compiler.

```csharp
double doubleValue = 3.14; // 'd' suffix (optional) indicates double
```

If we do not include the 'f' or 'd' suffix, the compiler determines the type of the literal based on its value and context. However, it's good practice to explicitly specify the suffix to avoid any confusion and to ensure that the literal is interpreted correctly.

The `float` data type sacrifices some precision for a more compact representation, while `double` provides higher precision at the cost of more memory.

```csharp
double pi = 3.141592653589793238; // Approximate value of Pi
float goldenRatio = 1.6180339887498948482f; // Golden ratio
```

Sometimes numbers get so large or small that scientific notation is more convenient. In C#, you can express floating-point literals using scientific notation, like `1.5e3` for 1500.

### Positive Infinity, Negative Infinity & NaN

In C#, certain floating-point operations can result in special values: Positive Infinity, Negative Infinity, and NaN (Not a Number). These values are used to represent results that exceed the limits of what can be represented in a floating-point type, as well as undefined or unrepresentable results.

**Positive Infinity**:

- **Representation**: `Double.PositiveInfinity`, `Single.PositiveInfinity`
- **Meaning**: Represents a value greater than any other number.
- **Usage**: Occurs in operations where the result exceeds the maximum representable value, such as dividing a positive number by zero or an overflow in arithmetic operations. Indicates a value greater than any other number.
- **Example**:

```csharp
double positiveInfinity = Double.PositiveInfinity;
double result = 1.0 / 0.0; // The result is `PositiveInfinity`
```

**Negative Infinity**:

- **Representation**: `Double.NegativeInfinity`, `Single.NegativeInfinity`
- **Meaning**: Represents a value less than any other number.
- **Usage:** Occurs in operations where the result is less than the minimum representable value, such as dividing a negative number by zero or an underflow in arithmetic operations. Indicates a value less than any other number.
- **Example**:

```csharp
double negativeInfinity = Double.NegativeInfinity;
double result = -1.0 / 0.0; // The result is `NegativeInfinity`
```

**NaN**:

- **Representation**: `Double.NaN`, `Single.NaN`
- **Meaning**: Represents an undefined or unrepresentable value.
- **Usage**: Occurs in operations that do not yield a defined numeric result, such as dividing zero by zero, taking the square root of a negative number, or invalid arithmetic operations.
- **Example**:

```csharp
double nanValue = Double.NaN;
double result = 0.0 / 0.0; // result is NaN
```

These special values help handle exceptional cases in floating-point arithmetic and ensure that operations return predictable results even when they encounter limits or undefined conditions.

```csharp
// Positive Infinity
double positiveInfinity = 1.0 / 0.0;
Console.WriteLine(positiveInfinity); // Output: Infinity

// Negative Infinity
double negativeInfinity = -1.0 / 0.0;
Console.WriteLine(negativeInfinity); // Output: -Infinity

// NaN (Not a Number)
double nanValue = 0.0 / 0.0;
Console.WriteLine(nanValue); // Output: NaN

// Checking for Infinity and NaN
Console.WriteLine(Double.IsInfinity(positiveInf)); // Output: True
Console.WriteLine(Double.IsPositiveInfinity(positiveInf)); // Output: True
Console.WriteLine(Double.IsNegativeInfinity(negativeInf)); // Output: True
Console.WriteLine(Double.IsNaN(nanValue)); // Output: True
```

### Examples

```csharp
double ageOfUniverseInYears = 13.8e9;  // 🕰️ Approximate age of the universe in years
```

```csharp
float depthOfMarianaTrenchInKm = 10.994f; // 🌊 Maximum depth of the Mariana Trench in kilometers
```

```csharp
// 🎨 Mixing Colors in Design
float redIntensity = 0.8f;    // Intensity of red in RGB color model
double greenSaturation = 0.55; // Saturation of green
```

```csharp
// Exploring Planetary Distances 🪐
double distanceToSunInKm = 149_600_000; // Distance from Earth to Sun
double distanceToNeptuneInAU = 30.07;    // Distance from Earth to Neptune in Astronomical Units
```

## 🤔 Precision, Accuracy & Computer Memory

Computers were invented for scientific purposes.

While computers are incredibly precise and accurate in performing numerical calculations, there are cases where unexpected or inaccurate results can occur. This is often due to limitations in how numbers are represented and stored in computer memory, as well as the way arithmetic operations are performed.

Limitations in numerical representation and computation can lead to inaccuracies or unexpected results in calculations performed by computers or calculators.

Examples why strange behavior or inaccuracies can occur in numerical calculations:

- **Floating-Point Representation**: Floating-point numbers, which represent real numbers with decimal points, have limited precision due to the way they are stored in memory using a fixed number of bits for the mantissa (significand) and exponent. This can lead to rounding errors and inaccuracies, especially when performing arithmetic operations on numbers with vastly different magnitudes. Computers use a finite number of bits to represent numbers, which means they can only represent a finite range of values with a certain level of precision. For very large or very small numbers, or numbers with many decimal places, the limited precision can lead to rounding errors or loss of accuracy. If we try to calculate the result of \( \frac{1}{3} \) using a calculator that displays only a limited number of decimal places, we might get a result like 0.333. However, the actual result is an infinitely repeating decimal (0.333333...). The limited precision of the calculator's display leads to an approximation of the true value. Consider the expression \( 0.1 + 0.2 \). In many programming languages using floating-point arithmetic, the result might not be exactly 0.3 due to the limitations of floating-point representation. Instead, it might be a slightly different value, such as 0.30000000000000004, due to round-off errors.
- **Round-off Errors**: Arithmetic operations involving floating-point numbers may introduce round-off errors, where the result is slightly different from the mathematically exact result due to limitations in precision. These errors can accumulate over multiple calculations and affect the final result. Let's say we calculate \( \sqrt{2} \) using the formula \( \sqrt{2} = 2^{1/2} \). While mathematically, the square root of 2 is an irrational number (approximately 1.41421356237), the result obtained from a computer calculation might be a rounded value like 1.414, due to round-off errors in the computation.

Precision refers to how finely a value can be expressed, while accuracy relates to how closely the represented value matches the true value.

Floating-point numbers, like `float` and `double`, offer precision but with limitations. Due to the nature of binary representation, some decimal fractions cannot be precisely represented.

```csharp
// Example 1: Multiplying a large number by 2 using float
float result1_float = 99999999999999999999999f * 2;
Console.WriteLine("Result of multiplying a large number by 2 using float: " + result1_float);
// Expected result: 2.0E+23
```

```csharp
// Example 1: Multiplying a large number by 2 using double
double result1_double = 99999999999999999999999d * 2;
Console.WriteLine("Result of multiplying a large number by 2 using double: " + result1_double);
// Expected result: 2.0E+23
```

```csharp
// Example 2: Adding 1 to a very large number using float
float result2_float = 10000000000000000000000000f + 1;
Console.WriteLine("Result of adding 1 to a very large number using float: " + result2_float);
// Expected result: 1.0E+25
```

```csharp
// Example 2: Adding 1 to a very large number using double
double result2_double = 10000000000000000000000000d + 1;
Console.WriteLine("Result of adding 1 to a very large number using double: " + result2_double);
// Expected result: 1.0E+25
```

```csharp
Console.WriteLine(0.1 + 0.2);
Console.WriteLine(0.3);
```

While computers strive to perform calculations as accurately as possible, it's important for developers to be aware of these potential sources of error and to take steps to mitigate them when necessary. This may involve using appropriate numerical algorithms, choosing suitable data types, and carefully handling edge cases and exceptional conditions in code.

## 🚀 Decimal Precision Data Type

Unlike `float` and `double`, `decimal` is designed to represent decimal fractions with high precision.

Memory is a precious resource, and choosing the right data type involves trade-offs. While `float` and `double` are more memory-efficient, they sacrifice some precision. On the other hand, `decimal` provides precision but at the cost of increased memory usage.

In financial calculations, where precision is crucial, using the `decimal` type ensures accurate representation of monetary values, avoiding potential rounding discrepancies.

```csharp
decimal productPrice = 49.99m;
Console.WriteLine(productPrice);
```

The 'm' at the end indicates it's a decimal literal.

Imagine calculating the total cost of items in a shopping cart. With `decimal`, you ensure that the calculated total accurately reflects the sum of individual item prices, avoiding rounding errors.

Suppose you're calculating interest rates over time. With `decimal`, you ensure that each fractional interest is accurately represented, providing trustworthy results over extended periods.

It's ideal for situations where exact representation of decimal numbers (e.g., currency values) is required, as it avoids rounding errors associated with binary floating-point representation. However, it requires more memory and is generally slower in performance compared to `float` and `double`.

While `decimal` offers unparalleled precision, it comes with a cost—increased memory usage. When using `decimal`, be mindful of memory constraints. It's a trade-off between precision and memory efficiency.

Examples:

**Financial Applications**
In financial applications such as banking software, accounting systems, and e-commerce platforms, the `decimal` data type is used to represent monetary values with precise decimal precision.
Examples include storing and processing amounts for transactions, calculating interest rates, handling currency conversions, and performing tax calculations.

2. **Retail and Inventory Management**:
   - In retail and inventory management systems, the `decimal` data type is used to represent prices, costs, and quantities with exact decimal precision.
   - Examples include storing and managing product prices, calculating total costs for purchases, handling discounts and promotions, and tracking inventory levels.
4. **Medical and Healthcare Systems**:
   - In medical and healthcare systems, the `decimal` data type is used to represent patient data, medication dosages, laboratory results, and billing information with accurate decimal precision.
   - Examples include storing and managing patient records, calculating medication doses based on body weight, analyzing diagnostic test results, and generating billing statements for healthcare services.

5. **Real Estate and Property Management**:
   - In real estate and property management applications, the `decimal` data type is used to represent property values, rental rates, mortgage payments, and financial transactions with precise decimal precision.
   - Examples include storing and managing property listings, calculating mortgage payments and loan amortization schedules, analyzing rental income and expenses, and generating financial reports for property owners.

Overall, the `decimal` data type is widely used in various industries and applications where precise decimal precision is required for storing, processing, and calculating monetary values, measurements, and other numeric data.


### Example 1: Financial Calculation for a Space Travel Agency 🚀
```csharp
decimal spaceshipCost = 1_000_000.50m; // Cost of purchasing a spaceship
decimal fuelCost = 500_000.75m; // Cost of fuel for the journey
decimal totalCost = spaceshipCost + fuelCost; // Total cost of the space mission
```

### Example 2: Calculating the Price of Rare Gemstones 💎
```csharp
decimal emeraldPricePerCarat = 5_000.25m; // Price per carat for emerald gemstones
decimal diamondPricePerCarat = 10_000.75m; // Price per carat for diamond gemstones
decimal totalValue = (emeraldPricePerCarat * 10) + (diamondPricePerCarat * 5); // Total value of gemstones
```

### Example 3: Financial Planning for a Robot Repair Shop 🤖
```csharp
decimal robotPartCost = 250.50m; // Cost of a single robot part
decimal repairServiceFee = 100.75m; // Fee for repairing a robot
decimal totalRevenue = (robotPartCost * 20) + (repairServiceFee * 15); // Total revenue for the month
```

### Example 4: Budgeting for a Deep Sea Exploration 🌊
```csharp
decimal submarineCost = 5_000_000.75m; // Cost of purchasing a submarine
decimal researchEquipmentCost = 2_500_000.50m; // Cost of research equipment
decimal totalBudget = submarineCost + researchEquipmentCost; // Total budget for the expedition
```

### Example 5: Pricing Rare Books in a Vintage Library 📚
```csharp
decimal ancientManuscriptPrice = 20_000.25m; // Price of an ancient manuscript
decimal firstEditionBookPrice = 15_000.75m; // Price of a first edition book
decimal totalValue = ancientManuscriptPrice + firstEditionBookPrice; // Total value of rare books
```

### Example 6: Cost Estimation for Building a Time Machine ⏳
```csharp
decimal fluxCapacitorCost = 1_000_000.50m; // Cost of the flux capacitor
decimal plutoniumCost = 500_000.75m; // Cost of plutonium for fuel
decimal totalCost = fluxCapacitorCost + plutoniumCost; // Total cost of building the time machine
```

### Example 7: Pricing Exotic Fruits in a Futuristic Market 🍍
```csharp
decimal durianPricePerKg = 50.25m; // Price per kilogram of durian fruit
decimal dragonFruitPricePerKg = 100.75m; // Price per kilogram of dragon fruit
decimal totalRevenue = (durianPricePerKg * 30) + (dragonFruitPricePerKg * 20); // Total revenue for the day
```

### Example 8: Calculating the Cost of a Luxury Yacht 🛥️
```csharp
decimal yachtCost = 10_000_000.50m; // Cost of purchasing a luxury yacht
decimal maintenanceCostPerYear = 500_000.75m; // Annual maintenance cost
decimal totalCostOver5Years = yachtCost + (maintenanceCostPerYear * 5); // Total cost over 5 years
```

### Example 9: Estimating Expenses for a Virtual Reality Gaming Center 🎮
```csharp
decimal VRHeadsetCost = 1_500.25m; // Cost of a virtual reality headset
decimal gamingConsoleCost = 1_000.75m; // Cost of a gaming console
decimal totalExpenses = (VRHeadsetCost * 20) + (gamingConsoleCost * 30); // Total expenses for the center
```

### Example 10: Budgeting for a High-Tech Laboratory 🧪
```csharp
decimal laboratoryEquipmentCost = 2_000_000.50m; // Cost of high-tech laboratory equipment
decimal researchGrantAmount = 1_500_000.75m; // Amount received as a research grant
decimal remainingFunds = laboratoryEquipmentCost - researchGrantAmount; // Remaining funds needed
```

These examples showcase the versatility of the decimal data type in handling precise financial calculations and measurements in various real-world scenarios.

## 🌓 Boolean Data Type

The term `boolean` itself is derived from the surname of George Boole, the mathematician who developer `Boolean Algebra`. Boole's work laid the foundation for symbolic logic and provided a systematic way to represent and manipulate logical statements using algebraic techniques.

Boole introduced the concept of variables that can have only two possible values: `true` or `false`. These values are often represented by the binary digits `1` and `0`, respectively, in computer science. Boolean algebra allows for the manipulation of these variables through logical operations such as `AND`, `OR`, and `NOT`.

In C#, the `bool` data type is used to declare a `boolean` variable that could store one of the two possible values: `true` or `false`.

When a `boolean` variable is declared but not explicitly initialized, it defaults to `false`.

```csharp
bool isWarm; // 👈 Default value: false
isWarm = true;
```

```csharp
bool isSunny = true;
Console.WriteLine(isSunny); // 👈 Prints: True

bool isRaining = false;
Console.WriteLine(isRaining); // 👈 Prints: False
```

An expression that could be evaluated to `true` or `false` is called a `boolean` expression.

Imagine a smart home system. Using `boolean` values, we can represent whether lights are on or off, doors are locked or unlocked, and create smart rules based on these conditions.

Functions can return `boolean` values, indicating the success or failure of an operation. For example, a function to check if a user is authenticated might return `true` if authentication is successful.

## 🔣 Character Data Type

Characters represent individual symbols, letters, or digits.

```csharp
char symbol;
symbol = '$';

char letter = 'A';
char emoji = '😊';
```

Behind the scenes, characters in C# are represented using Unicode. Unicode allows the representation of a vast array of characters, including international symbols, emojis, and special characters.

Escape sequences provide a way to represent special characters in your code. For example, `'\n'` represents a newline character, and `'\t'` represents a tab.

// TODO: Add examples.

## 🔣 Character Data Type

In programming, a character data type is used to represent single characters, like letters, numbers, or symbols. It's like a small box where we can store one piece of information, such as the letter 'A', the digit '5', or the punctuation mark ','.

#### What is a Character?

A character is a single unit of information that can be displayed on a screen or printed on paper. It can be a letter of the alphabet (like 'A' or 'z'), a digit (like '0' or '9'), or a special symbol (like '$' or '%').

#### Using Characters in Programming

In programming languages like C#, characters are represented using a data type called `char`. You can think of a `char` as a little container that holds one character. Here's how you can declare and use characters in C#:

```csharp
`char letter = 'A'; // This stores the letter 'A' in the variable named "letter" char digit = '5'; // This stores the digit '5' in the variable named "digit" char symbol = '$'; // This stores the symbol '$' in the variable named "symbol"`
```

#### Operations with Characters

You can perform various operations with characters in your programs. For example, you can compare characters to see if they are equal, or you can convert characters to their corresponding ASCII values (which are numeric representations of characters). Here's a simple example:

```csharp

`char firstLetter = 'A'; char secondLetter = 'B';  bool areEqual = (firstLetter == secondLetter); // This checks if the characters are equal int asciiValue = (int)firstLetter; // This converts the character to its ASCII value`
```
 
ASCII (American Standard Code for Information Interchange) is officially documented, primarily overseen by the American National Standards Institute (ANSI). You can find information about ASCII on the official ANSI website at [https://www.ansi.org](https://www.ansi.org). While the ANSI website may not have ASCII documentation as a standalone resource, it serves as a reputable source for standards-related information, including the ASCII standard. In addition to ANSI's resources, you can also explore other online sources such as Wikipedia, tutorials, reference guides, and technical documents for comprehensive information about ASCII and related topics. If you're looking for in-depth technical details, academic papers, computer science textbooks, and technical manuals related to character encoding and text processing can also be valuable resources.

ASCII (American Standard Code for Information Interchange) is a character encoding standard that assigns numeric codes to characters in the English alphabet, digits, and a few other symbols. Here are some additional details about ASCII:

1. **Character Range**: ASCII codes represent 128 characters, including control characters (non-printable) and printable characters. These characters range from 0 to 127 in decimal or 00 to 7F in hexadecimal.

2. **7-Bit Encoding**: ASCII uses 7 bits to represent each character, allowing for a total of 128 unique characters. The eighth bit is not used in ASCII, which distinguishes it from later character encoding standards like UTF-8.

3. **Standardization**: ASCII was first published as a standard by the American National Standards Institute (ANSI) in 1963 and later updated in 1967. It has since become one of the fundamental building blocks of modern computing.

4. **Universal Adoption**: ASCII quickly became widely adopted and remains a fundamental part of most computer systems and programming languages, particularly in the English-speaking world.

5. **Extended ASCII**: While the original ASCII standard only included 128 characters, various extensions have been developed to accommodate additional characters for different languages and special symbols. These extensions, known as Extended ASCII, vary between different implementations and are not part of the official ASCII standard.

6. **Compatibility**: Due to its widespread adoption, ASCII remains compatible with almost all modern computing systems. Virtually all modern text-based communication protocols, file formats, and programming languages rely on ASCII or its compatible extensions.

7. **ASCII Art**: ASCII art is a form of digital art that uses ASCII characters to create images, designs, or illustrations. It has been popular since the early days of computing and is still appreciated as a creative expression in online forums, social media, and other digital platforms.

8. **Limitations**: One limitation of ASCII is its focus on the English alphabet and lack of support for characters from other languages. This limitation led to the development of Unicode and other character encoding standards capable of representing a broader range of characters from various languages and writing systems.
Certainly! Here's the rewritten version with examples for C#:

1. **Text Representation**: ASCII characters are used to represent text in various digital contexts. For example:
   - The letter 'A' is represented by the ASCII code 65 (or 0x41 in hexadecimal).
   - The digit '0' is represented by the ASCII code 48 (or 0x30 in hexadecimal).
   - The punctuation mark ',' (comma) is represented by the ASCII code 44 (or 0x2C in hexadecimal).

2. **Programming**: ASCII characters are extensively used in programming languages for coding and processing textual data. For instance:
   ```csharp
   // In C#, ASCII values of characters can be obtained directly.
   char letter = 'A';
   int asciiValue = (int)letter; // asciiValue will be 65
   ```

3. **Digital Art (ASCII Art)**: ASCII characters are creatively utilized to form images or designs, known as ASCII art. Here's a simple example of a smiley face:
   ```csharp
   // Simple ASCII art example - smiley face
   Console.WriteLine(":-)");
   ```
   ASCII art can be much more intricate, with artists using various characters and arranging them in intricate patterns to create detailed images.

4. **Communications Protocols**: ASCII characters are used in communication protocols for encoding textual data. For example:
   - In the HTTP protocol, ASCII characters are used to represent headers and data in requests and responses exchanged between clients and servers.
   - In email protocols like SMTP (Simple Mail Transfer Protocol), ASCII characters are used to encode email messages.

These examples demonstrate the versatile and pervasive nature of ASCII characters in various aspects of digital communication, programming, and art. In C#, you can directly access ASCII values of characters and use them in your code for different purposes.

Characters represent individual symbols, letters, or digits.

```csharp
char symbol;
symbol = '$';

char letter = 'A';
char emoji = '😊';
```

Behind the scenes, characters in C# are represented using Unicode. Unicode allows the representation of a vast array of characters, including international symbols, emojis, and special characters.

Non-printable ASCII symbols are characters that do not represent visible characters or printable characters, but rather control characters used for formatting, communication control, or other purposes. Here are some examples:

10. **Horizontal Tab (HT)** - ASCII code 9 (0x09): Moves the cursor to the next tab stop.

11. **Line Feed (LF)** - ASCII code 10 (0x0A): Moves the cursor to the next line.

12. **Vertical Tab (VT)** - ASCII code 11 (0x0B): Moves the cursor to the next vertical tab stop.

13. **Form Feed (FF)** - ASCII code 12 (0x0C): Advances the paper to the next page or form.

These non-printable ASCII symbols play crucial roles in controlling devices, formatting text, and managing communications but do not have visible representations when printed or displayed.

### Unicode

Unicode is a character encoding standard that aims to represent almost all characters from all writing systems used in the world today. Unlike ASCII, which is limited to 128 characters, Unicode supports over 143,000 characters, including characters from various languages, symbols, emojis, and special characters.

[Unicode Official Website](https://unicode.org/)

This website provides comprehensive documentation, charts, and resources related to Unicode, including the latest standards and updates. You can explore the Unicode character charts to find specific characters and their Unicode code points, as well as learn about Unicode encoding schemes and guidelines for implementation.

### Examples of Unicode:

1. **Basic Latin Characters**: Unicode includes characters from the basic Latin alphabet used in English and many other languages. For example:
   - U+0041: LATIN CAPITAL LETTER A (corresponding to the character 'A')
   - U+0061: LATIN SMALL LETTER A (corresponding to the character 'a')

2. **Latin-1 Supplement**: Unicode extends beyond ASCII to include characters from the Latin-1 Supplement block, which includes accented letters and additional symbols. For example:
   - U+00E9: LATIN SMALL LETTER E WITH ACUTE (corresponding to the character 'é')
   - U+00A3: POUND SIGN (corresponding to the symbol '£')

3. **Emoticons and Symbols**: Unicode includes a wide range of emojis, symbols, and pictographs. For example:
   - U+1F600: GRINNING FACE (😀)
   - U+2600: BLACK SUN WITH RAYS (☀️)

4. **CJK Unified Ideographs**: Unicode also includes characters from various writing systems, such as Chinese, Japanese, and Korean (collectively known as CJK characters). For example:
   - U+4E00: CJK UNIFIED IDEOGRAPH-4E00 (一)
   - U+3042: HIRAGANA LETTER A (あ)

5. **Arabic Characters**: Unicode supports characters from the Arabic script. For example:
   - U+0627: ARABIC LETTER ALEF (ا)
   - U+0646: ARABIC LETTER NOON (ن)

6. **Mathematical Symbols**: Unicode includes a comprehensive set of mathematical symbols. For example:
   - U+221E: INFINITY (∞)
   - U+2206: INCREMENT (∆)

Unicode provides a unified way to represent text in all languages and writing systems, making it essential for internationalization and globalization in software development, communication, and digital content creation.

### Character arithmetics

Character arithmetic, based on ASCII codes, involves performing mathematical operations using the ASCII (American Standard Code for Information Interchange) representation of characters. In ASCII, each character is assigned a numerical value, which allows for operations like addition and subtraction to be performed on characters.

Here's how it works:

1. **Conversion to ASCII**: Each character has a corresponding ASCII code. For example, the ASCII code for 'A' is 65, 'B' is 66, and so on. 

2. **Performing Arithmetic**: Once characters are converted to their ASCII codes, you can perform arithmetic operations just like you would with numbers. For example, if you add 1 to the ASCII code of 'A' (which is 65), you get 66, which corresponds to the character 'B'. Similarly, subtracting 1 from the ASCII code of 'B' gives you 65, which corresponds to 'A'.

3. **Modifying Characters**: By performing arithmetic on ASCII codes, you can modify characters. For example, you can convert lowercase letters to uppercase by subtracting 32 from their ASCII codes.

Examples of character arithmetic using C#:

```csharp
using System;

class Program
{
    static void Main()
    {
        // Convert character to ASCII code
        char myChar = 'A';
        int asciiCode = (int)myChar;

        // Perform arithmetic on ASCII code
        int newAsciiCode = asciiCode + 1;

        // Convert ASCII code back to character
        char newChar = (char)newAsciiCode;

        Console.WriteLine(newChar); // Output: B
    }
}
```

This C# code snippet demonstrates how to perform character arithmetic based on ASCII codes. It converts a character to its ASCII code, performs arithmetic on the ASCII code, and then converts the result back to a character. In this example, it increments the character 'A' to 'B'.

It's important to note that character arithmetic based on ASCII codes has limitations. It works well for basic operations and within the ASCII character set, but may not behave as expected for characters outside the ASCII range or when dealing with extended character sets like Unicode.

# Chapter: Character Data Type 📝

Welcome to the "Character Data Type" chapter, part of the "Data Types and Variables" module in "The Complete C# Course." In this chapter, we'll explore the `char` data type in C#, which is used to store single characters. We'll cover examples, literals, ASCII, Unicode, memory usage, and default values. Let's dive in! 🚀

## 1. What is the `char` Data Type? 🤔

The `char` data type in C# is used to represent a single Unicode character. It can store letters, digits, punctuation marks, symbols, and control characters. Each `char` value occupies 2 bytes (16 bits) of memory.

### Example:
```csharp
char myChar = 'A'; // Stores the character 'A'
```

## 2. Character Literals 📝

Character literals are single characters enclosed in single quotes (`'`). They can represent characters directly using their Unicode code points or by using escape sequences for special characters.

### Examples:
```csharp
char letterA = 'A';    // Direct character representation
char newLine = '\n';   // Escape sequence for newline character
char tab = '\t';       // Escape sequence for tab character
char backslash = '\\'; // Escape sequence for backslash character
```

## 3. ASCII and Unicode 💻

### ASCII (American Standard Code for Information Interchange):
- ASCII is a character encoding standard that assigns numerical values to characters.
- It uses 7 bits to represent 128 characters, including letters, digits, punctuation, and control characters.
- ASCII characters are a subset of Unicode characters.

### Unicode:
- Unicode is a character encoding standard that supports a much larger set of characters from various writing systems and languages.
- It uses 16 bits (2 bytes) to represent characters, allowing for over 65,000 unique characters.
- Unicode provides a unique code point for each character, allowing for internationalization and multilingual support.

## 4. Memory Usage 🧠

Each `char` value in C# occupies 2 bytes (16 bits) of memory. This allows the `char` data type to represent a wide range of characters, including those from different languages and symbol sets.

## 5. Default Values 🗃️

If you declare a `char` variable without initializing it, its default value is `'\0'` (the null character). This is different from an empty character or a space character.

### Example:
```csharp
char myChar; // Default value is '\0'
```

## Summary 📜

In this chapter, we explored the `char` data type in C#, which is used to store single characters. We learned about character literals, ASCII, Unicode, memory usage, and default values. Understanding the `char` data type is essential for working with text and characters in C# programming.

## Next Steps ⏭️

Now that you have a good understanding of the `char` data type, practice using it in your C# programs. Experiment with different characters, explore Unicode characters, and understand how they are represented in memory. In the next chapters, we'll delve deeper into other data types and variables in C#.

Happy coding! 😊💻
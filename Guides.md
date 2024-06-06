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

### Computer Memory (Computer Science)
- **Guide**: Think of computer memory as your computer's workspace where it temporarily stores and retrieves information needed for running programs. It's like a desk with different compartments for storing various items.
- **Best Practices**: Understand the main types of memory: RAM (Random Access Memory) acts like a scratch pad for quick access during program execution, while ROM (Read-Only Memory) holds essential instructions and data that don't change. Manage memory efficiently to ensure smooth performance of your programs.

### Data Types (Computer Science)
- **Guide**: Data types are containers that hold different types of information in your programs. They specify the kind of data a variable can hold, like numbers, text, or true/false values.
- **Best Practices**: Use clear and descriptive names for your variables to make your code easy to understand. Be consistent in your naming style throughout your codebase. Refactor your code if you find better names or if the purpose of a variable changes over time.

### Variables Introduction
- **Guide**: Variables are like labeled boxes where you can store and retrieve data in your programs. Each variable has a name that reflects its purpose and a type that defines the kind of data it can hold.
- **Best Practices**: Avoid using ambiguous or cryptic names for variables. Choose names that clearly convey their purpose and usage. Initialize variables whenever possible to give them meaningful starting values.

### Literals
- **Guide**: Literals are direct representations of values in your code, like numbers or text, that you specify explicitly.
- **Best Practices**: Instead of using magic values directly in your code, assign them to named variables with descriptive names. This improves readability and makes your code easier to maintain.

### Integer Data Types
- **Guide**: Integer data types represent whole numbers without any fractional or decimal part.
- **Best Practices**: When declaring integer variables, choose names that indicate their purpose or usage. Refrain from declaring multiple variables in a single statement to keep your code readable and maintainable.

### Floating-Point Data Types
- **Guide**: Floating-point data types represent numbers with fractional parts, like decimals.
- **Best Practices**: Use the `decimal` data type for handling precise calculations involving monetary values or scientific measurements where exact representation of decimal fractions is crucial. Initialize variables with meaningful values to avoid confusion.

### Precision, Accuracy & Computer Memory
- **Guide**: Precision refers to the level of detail in a measurement, while accuracy indicates how close a measurement is to the true value. Computer memory stores data, but its capacity is finite and needs to be managed efficiently.
- **Best Practices**: Strike a balance between precision and accuracy based on the requirements of your application. Keep track of memory usage to optimize performance and prevent resource wastage.

### Decimal Precision Data Type
- **Guide**: The `decimal` data type is ideal for handling values requiring exact representation of decimal fractions, such as monetary values or scientific measurements.
- **Best Practices**: Use the `decimal` data type when dealing with scenarios where precision is crucial, such as financial calculations. Initialize `decimal` variables with appropriate values to ensure accurate results.

### Boolean Data Type
- **Guide**: Boolean data type represents true or false values, often used for logical comparisons and control flow in your programs.
- **Best Practices**: Choose descriptive names for boolean variables that reflect their purpose or the condition they represent. Avoid cascade assignments to maintain code clarity and readability.

### Character Data Type
- **Guide**: Character data type represents single characters, like letters or symbols, often from a specific character set like ASCII or Unicode.
- **Best Practices**: When working with character data, use clear and consistent naming conventions for variables. Initialize character variables with meaningful values to avoid ambiguity.

### String Data Type
- **Guide**: String data type represents sequences of characters, commonly used for storing text or messages in your programs.
- **Best Practices**: Follow naming conventions for string variables and use descriptive names that convey their contents or purpose. Avoid hard-coding strings directly into your code; instead, use named variables for better readability and maintainability.

### Variables Characteristics
- **Guide**: Variables have different characteristics, such as scope, lifetime, and visibility, which affect how they can be accessed and manipulated in your programs.
- **Best Practices**: Understand the scope and lifetime of variables in your code to ensure proper usage and prevent unintended side effects. Refactor your code as needed to improve variable clarity and organization.

### Variables Declaration & Initialization
- **Guide**: Variables must be declared before they can be used, and optionally initialized with a starting value.
- **Best Practices**: Declare variables with clear and meaningful names that reflect their purpose or usage. Initialize variables when possible to provide meaningful starting values and avoid unexpected behavior in your programs.

### Naming Variables
- **Guide**: Choose descriptive and meaningful names for your variables to enhance code readability and maintainability.
- **Best Practices**: Follow a consistent naming style throughout your codebase, using clear and concise names that accurately describe the variable's purpose. Refactor variable names as needed to improve clarity and understanding.

### .NET Common Type System
- **Guide**: The .NET Common Type System (CTS) defines how data types are declared, used, and managed in .NET applications.
- **Best Practices**: Familiarize yourself with the common data types provided by the .NET CTS and their usage in different programming scenarios. Follow best practices for variable naming and data handling to ensure compatibility and maintainability across .NET languages.
# Chapter: C# Code Writing & Formatting ✍️

Welcome to the "C# Code Writing & Formatting" chapter, part of the "C# Introduction" module in "The Complete C# Course." In this chapter, we’ll cover essential practices for writing clean, readable, and well-organized C# code. We’ll discuss tools like IntelliSense, and concepts such as new lines, tabulations, braces positions, blocks of code, comments, naming conventions, code arranging, readability, and code refactoring. Let's get started! 🚀

## 1. IntelliSense 🧠

**IntelliSense** is a powerful code-completion feature in Visual Studio that helps you write code faster and with fewer errors. As you type, IntelliSense provides suggestions for variable names, methods, properties, and more.

### How to Use IntelliSense:
- Start typing the name of a method, property, or variable, and a list of suggestions will appear.
- Use the arrow keys to navigate through the list.
- Press `Tab` or `Enter` to select a suggestion.

## 2. New Lines and Tabulations 📏

Using new lines and tabulations (indents) helps make your code more readable and organized.

### New Lines:
- Place each statement on a new line.
- Separate logical sections of code with a blank line.

### Tabulations (Indents):
- Use the `Tab` key to indent code blocks inside methods, loops, and conditionals.
- Consistent indentation makes the structure of your code clear.

```csharp
using System;

namespace MyNamespace
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello, World!");

            if (true)
            {
                Console.WriteLine("This is inside an if statement.");
            }
        }
    }
}
```

## 3. Braces Positions and Code Blocks 🧩

The position of braces (`{}`) can affect the readability of your code. In C#, the common practice is to place the opening brace on the same line as the statement that begins the block.

### Example:
```csharp
class Program
{
    static void Main(string[] args)
    {
        if (true)
        {
            Console.WriteLine("Condition is true.");
        }
    }
}
```

### Blocks of Code:
- Code blocks are enclosed in braces `{}`.
- Indent the code within braces to show it belongs to the block.

## 4. Using Comments 🗒️

Comments are notes you can add to your code to explain what it does. They are ignored by the compiler.

### Types of Comments:
- **Single-line comments**: Start with `//` and continue to the end of the line.
- **Multi-line comments**: Enclosed in `/* ... */`.

### Example:
```csharp
// This is a single-line comment

/*
 This is a
 multi-line comment
*/

class Program
{
    // Main method - entry point of the program
    static void Main(string[] args)
    {
        Console.WriteLine("Hello, World!"); // Print message to console
    }
}
```

## 5. Naming Conventions 🏷️

Proper naming conventions improve code readability and maintainability.

### Conventions:
- **Classes and Methods**: Use PascalCase (e.g., `MyClass`, `CalculateTotal`).
- **Variables and Fields**: Use camelCase (e.g., `totalAmount`, `userName`).
- **Constants**: Use all uppercase letters with underscores (e.g., `MAX_VALUE`).

## 6. Code Arranging and Readability 📚

Organize your code logically and consistently to enhance readability.

### Tips:
- Group related code together.
- Use blank lines to separate different sections.
- Keep methods short and focused on a single task.

### Example:
```csharp
class Calculator
{
    // Adds two numbers
    public int Add(int a, int b)
    {
        return a + b;
    }

    // Subtracts the second number from the first
    public int Subtract(int a, int b)
    {
        return a - b;
    }
}
```

## 7. Code Refactoring 🛠️

**Code refactoring** is the process of restructuring existing code without changing its external behavior. This improves the design, structure, and readability of the code.

### Common Refactoring Techniques:
- **Extract Method**: Break down long methods into smaller, more manageable ones.
- **Rename**: Change variable, method, or class names to be more descriptive.
- **Simplify Expressions**: Replace complex expressions with simpler ones.

### Example:
Before refactoring:
```csharp
public void ProcessData(int[] data)
{
    for (int i = 0; i < data.Length; i++)
    {
        if (data[i] % 2 == 0)
        {
            Console.WriteLine(data[i] + " is even.");
        }
    }
}
```

After refactoring:
```csharp
public void ProcessData(int[] data)
{
    foreach (int number in data)
    {
        PrintEvenNumber(number);
    }
}

private void PrintEvenNumber(int number)
{
    if (number % 2 == 0)
    {
        Console.WriteLine(number + " is even.");
    }
}
```

## Summary 📜

In this chapter, we covered the essentials of writing and formatting C# code. We explored IntelliSense, the use of new lines and tabulations, braces positions, blocks of code, comments, naming conventions, code arranging, readability, and code refactoring. By following these guidelines, you'll write clean, maintainable, and professional C# code.

## Next Steps ⏭️

Practice applying these formatting and writing techniques to your code. In the next chapters, we'll dive deeper into more advanced C# concepts and further enhance your coding skills.

Happy coding! 😊💻
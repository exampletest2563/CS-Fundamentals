## 👋 C# & .NET

### 🤔 What is C#?

**C#** (pronounced "c-sharp") is a **modern**, **object-oriented programming language** developed by Microsoft. It is designed to be **simple**, **powerful**, and **versatile**, making it an excellent choice for a wide range of applications.

Key features of **C#**:

- **Object-Oriented**: C# supports concepts like classes, objects, inheritance, and polymorphism, which help in creating reusable and modular code.
- **Strongly Typed**: C# ensures that variables are defined with a specific data type, reducing errors and improving code reliability.
- **Easy to Learn**: C# has a syntax that is clean and straightforward, making it accessible for beginners.

### 🌐 What is .NET?

**.NET** (pronounced "dot net") is a free, open-source, cross-platform framework developed by Microsoft. It provides a large set of libraries and tools that make it easier to develop a wide variety of applications, from desktop and mobile applications to web and cloud-based services.

Key features of **.NET**:

- **Cross-Platform**: .NET supports multiple operating systems, including Windows, macOS, and Linux, allowing developers to create applications that run on any platform.
- **Comprehensive Libraries**: .NET includes a vast collection of libraries that provide functionality for everything from file I/O to web development, saving developers time and effort.
- **Performance**: .NET is optimized for high performance, ensuring that applications run efficiently and quickly.

### 🤝 C# & .NET Work Together

C# and .NET are designed to work seamlessly together. When you write a C# program, you can take advantage of the .NET libraries and runtime to build and run your application.

C# and .NET integrate in the following way:

- **C# Language**: We write our code in C#, leveraging its syntax and features to create our application logic.
- **.NET Libraries**: We use the extensive .NET libraries to perform common tasks, such as accessing databases, handling web requests, and more.
- **.NET Runtime**: The .NET runtime executes your C# code, managing memory, handling exceptions, and ensuring our application runs smoothly.

### 🌟 Why Use C# & .NET?

C# and .NET offer several benefits that make them a popular choice among developers:

- **Productivity**: C# and .NET provide tools and features that enhance developer productivity, such as integrated development environments (IDEs) like Visual Studio, which offer powerful debugging and code analysis tools.
- **Versatility**: With C# and .NET, you can develop a wide range of applications, from web and mobile apps to games and enterprise solutions. This versatility makes them a valuable skillset for any developer.
- **Community and Support**: There is a large and active community of developers who use C# and .NET, providing a wealth of resources, tutorials, and forums where you can get help and share knowledge.
- **Reliability and Performance**: Applications built with C# and .NET are known for their reliability and high performance, making them suitable for mission-critical systems and applications that require robust performance.

## 🛠️ Development Environment Setup

### Microsoft Visual Studio

Microsoft Visual Studio is a powerful **Integrated Development Environment** (IDE) used for developing software applications. It supports a variety of programming languages, including C#, and provides tools to make coding easier and more efficient.

Microsoft Visual Studio is an all-in-one tool. It combines code editing, debugging, and testing in one place, and includes features like IntelliSense (code suggestions), a built-in terminal, and version control integration.

### Setting Up Microsoft Visual Studio

Before diving into coding with C#, it's essential to set up a development environment that will streamline your workflow. The following steps will guide you through the process of setting up Microsoft Visual Studio for C# development.

**Step 1. Download The Installer**

1. **Go to the Visual Studio Website**: Visit [Visual Studio's official website](https://visualstudio.microsoft.com/).
2. **Choose a Version**: There are different editions of Visual Studio. The Community edition is free and suitable for most individual developers and small teams.
3. **Download the Installer**: Click the download button to get the installer file.
4. **Run the Installer**: Open the downloaded file to start the installation process.

**Step 2. Select Workloads**

When you run the installer, you’ll be prompted to select workloads. Workloads are groups of related tools and features tailored for different types of development.

- **For C# Development**:
  - Check the ".NET desktop development" workload.
  - If you're planning to develop web applications, also check the "ASP.NET and web development" workload.
  - For mobile development, check the "Mobile development with .NET" workload.

**Step 3. Install**

1. **Review Selected Workloads**: Make sure the correct workloads are selected.
2. **Start Installation**: Click the "Install" button to begin.
3. **Wait for Completion**: The installer will download and install the necessary components. This might take a while.

**Step 4. Initial Setup**

1. **Launch Visual Studio**: After installation, open Visual Studio.
2. **Sign In**: You can sign in with a Microsoft account to sync your settings across devices.
3. **Choose a Theme**: Select a color theme (Light, Dark, Blue) based on your preference.
4. **Start a New Project**: Click "Create a new project" to begin.

### Creating C# Projects

Here is a step-by-step guide to help you create new projects in Microsoft Visual Studio.

**Step 1. Create A New Project**

1. **Click "Create a new project"**: This will open a new project dialog.
2. **Select a Template**: Choose the "Console App (.NET Core)" template for a simple start.
3. **Configure Your Project**: Select "Do not use top-level statements". Give your project a name and choose a location to save it.
4. **Click "Create"**.

**Step 2. Write Code**

1. **Open the Program.cs File**: This file contains the entry point of your application.
2. **Write Your Code**: Here’s a simple example:

```csharp
using System;

namespace HelloWorld
{
	class Program
	{
		static void Main(string[] args)
		{
			Console.WriteLine("Hello, World!");
		}
	}
}
```

**Step 3. Run Your Project**

1. **Click the "Run" Button**: Located at the top of the IDE, it looks like a green arrow.
2. **See the Output**: A console window will open and display "Hello, World!".

Congratulations! We are done. 🎉

## 📂 C# Projects

C# Desktop Console projects allow us to create simple command-line programs that run on your computer. These projects are a great way to learn C# and practice coding skills.

### 🗂️ Solution Explorer

The **Solution Explorer** is a tool window in Visual Studio that helps us navigate and manage files within a project. It provides a hierarchical view of the solution's structure, displaying folders, files, and projects. 

Follow the steps in order to show the Solution Explorer window:

**Step 1. Open Visual Studio**

1. **Launch Visual Studio**: Open the Visual Studio program on your computer.

**Step 2. Navigate to the View Menu**

1. **Select View**: At the top of the window, click on the **View** menu to open a dropdown list of available views.
2. **Select Solution Explorer**: From the dropdown list, click on **Solution Explorer**. The Solution Explorer window should now appear on your screen.

Developers can use the Solution Explorer to navigate through the solution, add new files or projects, organize existing items, and perform various tasks such as building, debugging, and running the solution.

### 📂 Blank Solutions

A **Blank Solution** refers to a project template in Microsoft Visual Studio that creates an empty solution without any pre-existing projects.

The **Blank Solution** template acts as a folder that helps us organize multiple related projects within a single workspace. It could hold one or more C# projects.

Creating a **Blank Solution** is useful when we want to start from scratch and gradually add projects as needed.

**Step 1. Open Visual Studio**

1. **Launch Visual Studio**: Open the Visual Studio program on your computer.

**Step 2. Create a New Blank Solution**

1. **Go to File Menu**: Click on "File" at the top-left corner of the Visual Studio window.
2. **Select New**: From the drop-down menu, choose "New" and then "Project".
3. **Choose a Project Type**: In the "Create a new project" window, select "Other Project Types" and then "Blank Solution".
4. **Provide a Name**: Give your solution a name and choose a location to save it.
5. **Click Create**: Once you've provided the necessary information, click the "Create" button to create the blank solution.

Once created, we can start adding new projects to the solution by right-clicking on the solution name in the Solution Explorer and selecting **Add** > **New Project...**. This allows us to organize and manage multiple projects within a single solution file.

### Adding a Console Project to the Blank Solution

**Step 1: Right-Click on the Solution**

1. **Right-Click**: In the Solution Explorer window (usually on the right side of the Visual Studio window), right-click on the name of your blank solution.

**Step 2: Add New Project**

1. **Select Add**: From the context menu that appears after right-clicking, choose "Add".
2. **Choose Project Type**: In the submenu, select "New Project".
3. **Select Console App**: In the "Create a new project" window, navigate to "Visual C#" and select "Console App (.NET Core)".
4. **Name Your Project**: Give your project a name and choose a location to save it.
5. **Click Create**: Once you've provided the necessary information, click the "Create" button to add the console project to your blank solution.

After creating the project, it will appear in the Solution Explorer window.

### Writing Code in a Console Project

**Step 1: Open the Program.cs File**

1. **Locate Program.cs**: In the Solution Explorer, find the file named "Program.cs" under your console project.

**Step 2: Write Your Code**

1. **Edit Program.cs**: Double-click on "Program.cs" to open it in the code editor.
2. **Write Your Code**: You can write your C# code in the editor window. Here's a simple example:

```csharp
using System;

namespace MyConsoleApp
{
	class Program
	{
		static void Main(string[] args)
		{
			Console.WriteLine("Hello, World!");
		}
	}
}
```

3. **Save Your Changes**: After writing your code, make sure to save the file by pressing \[Ctrl + S\] or by clicking on the "Save" icon in the toolbar.

### Running Projects

**Step 1: Build Your Project**

1. **Build Solution**: Go to the "Build" menu at the top of the Visual Studio window and click on "Build Solution". This compiles your code into an executable file.

**Step 2: Run Your Project**

1. **Start Debugging**: Press F5 on your keyboard or click on the "Start Debugging" button (looks like a green arrow) in the toolbar.
2. **View Output**: A console window will open and display the output of your program, which in this case will be "Hello, World!".

### 📄 Proper File Naming

Using proper file naming conventions is crucial for maintaining organized and readable code.

The naming convention for naming files and classes in C# is called **PascalCase**, e.g. (`NumbersCalculator`, `HtmlParser`).

When naming files, it is best practice to match the class name and use **PascalCase**, ensuring consistency between the class and its file (e.g., a file containing the class `MyClass` should be named `MyClass.cs`). Remember to include the `.cs` extension.

Some of the benefits of proper file naming include:

- **Readability**: Makes your code easier to read and understand.
- **Maintainability**: Simplifies navigating and maintaining your codebase.
- **Consistency**: Promotes a consistent style throughout your project, making it easier for others to collaborate.

For learning purposes, use the name of the task as the name of your project and C# class or file.

### 🚀 Setting a Project as the Startup Project

If a solution contains more than one project, Visual Studio needs to know which project to start first. We can set a certain project as a startup project. The startup project is the one that will be executed when you press the "Run" button.

**Step 1. Open the Solution Explorer**

**Step 2. Set a Startup Project**

1. In the Solution Explorer, locate the project you want to set as the startup project.
2. Right-click on the project.
3. Select "Set as Startup Project" from the context menu.

Now, when you click on **Run**, Microsoft Visual Studio will run the startup project.

## 💻 C# Console Programs

Console programs are applications that run in a command-line interface (CLI) rather than a graphical user interface (GUI). They interact with the user through text input and output. These programs are typically used for simple tasks, testing, and learning the basics of a programming language.

### 🛠️ Creating a Console Program

Creating a console program in C# is straightforward. Here are the steps to get you started:

**Step 1: Open Visual Studio**

1. Open Visual Studio on your computer.

**Step 2: Create a New Project**

1. In Visual Studio, select "File" > "New" > "Project..."
2. In the "Create a new project" dialog, choose "Console App (.NET Core)".
3. Click "Next."

**Step 3: Configure Your Project**

1. Enter a project name (e.g., `HelloWorld`).
2. Choose a location to save your project.
3. Select "Do not use top-level statements".
4. Click "Create."

**Step 4: Write Your Program**

Once your project is created, Visual Studio will open the main file, typically named `Program.cs`. This file contains a basic structure for a console program.

In the `Main` method, you can write your code. For example:

```csharp
using System;

namespace MyFirstConsoleApp
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello, World!");
        }
    }
}
```

Console programs are simple, text-based applications that run in a command-line interface. Console programs are an excellent way to start learning C# as they allow you to focus on the fundamentals of programming.

### 📝 Breakdown of the "Hello World" Program

Let's break down the syntax of a simple "Hello World" program in C# and explain each part:

```csharp
using System;

namespace HelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello, World!");
        }
    }
}
```

Explanation:

- **`using System;`**: Includes the System namespace, which contains fundamental classes like `Console`. It makes the classes in the `System` namespace available to use in the program.
- **`namespace HelloWorld`**: Defines a namespace called HelloWorld. Namespaces help organize code and prevent naming conflicts.
- **`class Program`**: Defines a class called Program. In C#, every program must have at least one class.
- **`static void Main(string[] args)`**: Defines the Main method, the entry point of the program. When we run the program, the execution starts from this method.
- **`Console.WriteLine("Hello, World!");`**: Prints "Hello, World!" to the console.

Notice the curly braces (`{ ... }`). Curly braces define the beginning and end of a block of code. They are used to group the code in blocks.

### Top-Level Statements

Top-level statements in C# allow developers to write code without enclosing it within a class or a method. It simplifies code by removing unnecessary boilerplate, making it more concise and readable.

This feature is particularly useful for quick scripts, prototypes, and small applications. Here's an example of top-level statements:

```csharp
using System;

Console.WriteLine("Hello world!");
```

In this example, the code directly executes without the need for a containing class or method, demonstrating the simplicity and efficiency of top-level statements.

## 📢 C# Output

When programming, developers often use code written by other developers to save time and effort. This code can come in various forms - libraries, frameworks, modules and packages, open source projects, etc.

In C#, leveraging code authored by others involves integrating external libraries, frameworks, and APIs. This is facilitated through namespaces and references.

In C#, the `using System;` directive imports the `System` namespace, which is fundamental for various functionalities. This includes essential classes and methods for tasks like console input/output, working with data types, managing files, and more.

By including `using System;` developers gain direct access to commonly used classes and methods within the `System` namespace. One of these classes is called `Console`. The `Console` class in C# provides the `Console.WriteLine` and `Console.Write` methods for outputting text to the console window. The string must be enclosed in double quotes.

```csharp
using System;

class Startup
{
    static void Main()
    {
        Console.WriteLine("Hello, World!");
    }
}
```

The `Console.Write` method outputs text without appending a newline character.

```csharp
Console.Write("Hello World!");
```

If `using System;` is not included at the top of our program in C#, we would need to reference the `Console` class with its namespace every time we wish to use it. This means that instead of simply writing `Console.WriteLine`, we would have to specify `System.Console.WriteLine`, indicating that `Console` belongs to the `System` namespace.

```csharp
class Startup
{
    static void Main()
    {
		System.Console.WriteLine("Hello World!");
    }
}
```

## 💭 C# Comments

Comments do not represent actual instructions. They can be used to explain the source code, and to make it more readable.

```csharp
// This is a single-line comment

Console.WriteLine("Hello World!"); // This is a single-line comment

/*
  This is a multi-line comment.
  It is capable of encapsulating comprehensive explanations.
*/

Console.WriteLine("Hello World!");
```

Comments can also be used to prevent execution when testing alternative code.

```csharp
// Console.WriteLine("Hello World!");
Console.WriteLine("Hello World!");
```

We will use comments to highlight important segments of the source code.

```csharp
Console.WriteLine("Hello World!"); // 👈 Prints: "Hello World"
```

## 🧨 Compilation Errors

A compilation error, also known as a compile-time error or syntax error, occurs when the code written by a programmer cannot be translated into machine code by the compiler. This typically happens due to mistakes in the code that violate the rules and syntax of the programming language being used.

Compilation errors prevent the compiler from creating an executable program because it cannot understand the code as written. Instead, the compiler generates error messages that indicate where the problem occurred and what needs to be fixed. These error messages often include information such as the line number, file name, and a description of the issue.

Common causes of compilation errors include:
- `Syntax Errors`: Syntax errors occur when the code violates the syntax rules of the programming language. For example, missing semicolons, parentheses, or curly braces can lead to syntax errors.
- `Type Errors`: Type errors occur when there is a mismatch between the data types used in the code.
- `Undefined Symbols Errors`: Undefined symbols errors occur when the compiler encounters a variable, function, or class that has not been defined or declared before it is used.
- `Missing Libraries`: Missing libraries errors occur when the compiler cannot find the necessary libraries or dependencies required to compile the code.

A missing closing double quote in the `Console.WriteLine` statement results in a compilation error.

```csharp
Console.WriteLine("test);
```

There are many ways to write a statement incorrectly.

```csharp
Console.WriteLine("test") // 👈 There is a missing semicolon
```

```csharp
Console.WriteLine('test'); // 👈 Uses single quotes instead of double quotes
```

```csharp
Console.writeLine("test"); // 👈 The Console.WriteLine method is written incorrectly
```

Compilation errors must be fixed before the code can be successfully compiled and executed. Developers typically review the error messages provided by the compiler, locate and correct the errors in their code, and then attempt to compile the program again until no errors remain.

## 🔍 Debugging

### Introduction to Debugging

Debugging is the process of finding (and potentially fixing) errors or bugs (unwanted and/or unexpected behavior) in the code.

Debuggers are IDE features that could stop a program's execution at a given line. While paused, we could inspect the state of the program. We could execute the program line by line (the program's execution will stop before executing the current line) using the debugger's stepping options.

Debugging is a process that involves:

- Placing breakpoints where it is needed
- Work with the debugger's features
- Using the debugger's stepping options

Debuggers are tools which are made to help developer understand the code execution. Do not be afraid to use them!

### Setting Breakpoints

Breakpoints are markers that you can place in your code to pause the execution of your program at specific points. This allows you to examine the state of your program and investigate its behavior step by step.

Setting a breakpoint could be done by clicking on the margin (the area to the left of the line numbers) next to the line of code where we want to set the breakpoint. A red circle will appear, indicating that the breakpoint has been set.

### Running a Program in Debug Mode

Running your program in debug mode allows you to execute your code step by step, pausing at breakpoints so you can inspect the program's state and behavior.

**Step 1. Start Debugging**

1. Click on the "Start Debugging" button (green arrow) in the toolbar, or press the F5 key on the keyboard.

**Step 2. Navigate Through the Code**

1. The program will start running, and execution will pause at the breakpoints you've set. We can use the debugging toolbar to step through your code one line at a time, examine variables, and inspect the call stack.

## 📝 C# Code Writing & Formatting

In this section, we delve into the best practices for arranging code to maximize readability and improve overall code quality.

### 🧠 IntelliSense

**IntelliSense** is a powerful code-completion feature in Microsoft Visual Studio that helps us write code faster and with fewer errors. As we type, IntelliSense provides suggestions for variable names, methods, properties, and more.

### 📏 New Lines, Tabulations & Spacing

Organize your code logically to guide the reader through the flow of the program. Use meaningful comments and whitespace to break code into logical sections.

Consistency in formatting is key to making your code readable. Using new lines and tabulations (indents) helps make your code more readable and organized.

Best practices:

- Place each statement on a new line.
- Separate logical sections of code with a blank line.
- Use the `Tab` key to indent code blocks.
- Use spaces around operators (`+`, `-`, `=`, etc.).
- Remove any redundant white space characters (new lines, tabulations, spaces).

### 🧩 Braces Positions and Code Blocks

Code blocks are enclosed in braces `{}`.

The position of braces (`{}`) can affect the readability of your code. In C#, the common practice is to place the opening brace on the same line as the statement that begins the block.

```csharp
class Program
{
    static void Main(string[] args)
    {
        if (true)
        {
            Console.WriteLine("Condition is true.");
        }
        else
        {
	        Console.WriteLine("Condition is false.");
        }
    }
}
```

The code inside the braces should be indented. This practice visually connects it to the corresponding block.

### 🗒️ Using Comments

Comments are notes you can add to your code to explain what it does. They are ignored by the compiler.

It is a good practice to include comments when it is necessary.

Add comments to explain why certain decisions were made or to provide context where the code may not be immediately clear. Avoid redundant comments that simply restate what the code does.

You can improve the readability of your code by placing comments directly above the statement they refer to.

### 🏷️ Naming Conventions

Choosing descriptive names for variables, functions, and classes enhances code readability. Aim for names that clearly indicate the purpose or intent of the entity they represent.

The name of the C# file and the name of the class should match.

Do not use generic names like "Test", "Application1" or "MyConsoleApp".

Class names should be nouns or noun phrases that describe the primary purpose of the class (e.g., `Customer`, `DatabaseConnection`).

### 📚 Code Arranging and Readability

Organize your code logically and consistently to enhance readability.

Best practices:

- Group related code together.
- Use blank lines to separate different sections.
- Use meaningful names.

## 📚 C# Documentation

### 🧐 Why Documentation Matters?

Documentation help developers understand the purpose, functionality, and usage of the code. Good documentation can make your code more maintainable, reusable, and easier to debug.

Benefits of Documentation:

- **Clarity**: Explains the purpose and functionality of the code.
- **Maintenance**: Helps future developers understand and update the code.
- **Collaboration**: Makes it easier for teams to work together.
- **Learning**: Assists beginners in understanding the code and learning new concepts.

### 📝 Types of Documentation

Documenting the code could be done in several ways:

- Inline Comments;
- XML Documentation Comments;
- External Documentation.

Inline comments are short notes within the code that explain what specific lines or blocks of code do.

```csharp
// This method adds two numbers and returns the result
public int Add(int a, int b)
{
    return a + b;
}
```

XML documentation comments provide more detailed descriptions of classes, methods, properties, and other code elements. These comments are used to generate external documentation files.

```csharp
/// <summary>
/// Adds two integers and returns the result.
/// </summary>
/// <param name="a">The first integer.</param>
/// <param name="b">The second integer.</param>
/// <returns>The sum of the two integers.</returns>
public int Add(int a, int b)
{
    return a + b;
}
```

External documentation includes manuals, guides, README files, and wikis. These documents provide comprehensive information about the software, including installation instructions, usage examples, and technical details. For instance, `README.md` files and User Manuals/Guides.

### Official C# Documentation

The C# language has official documentation provided by Microsoft. The primary website for accessing C# documentation is the Microsoft Docs website.

Main resources and links:

- **Microsoft Docs - C# Programming Guide**: This comprehensive guide covers various aspects of the C# programming language, including syntax, data types, control flow, object-oriented programming, and more. You can find it at [C# Programming Guide](https://docs.microsoft.com/en-us/dotnet/csharp/).
- **Microsoft Docs - C# Language Reference**: This reference documentation provides detailed information about C# language syntax, keywords, types, and other language elements. You can access it at [C# Language Reference](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/).
- **Microsoft Docs - .NET API Browser**: This tool allows you to explore the .NET Framework and .NET Core APIs, including classes, methods, properties, and events available in C# and other .NET languages. You can access it at [.NET API Browser](https://docs.microsoft.com/en-us/dotnet/api/).
- **Visual Studio IntelliSense**: When working in Visual Studio, you can leverage IntelliSense, a feature that provides context-aware code completion and documentation tooltips as you type. This can be a valuable resource for exploring APIs and understanding their usage directly within your development environment.
- **Community Forums and Stack Overflow**: Additionally, you can seek help and advice from the C# developer community on forums such as the Microsoft Developer Community and Stack Overflow. These platforms are great for asking questions, sharing knowledge, and troubleshooting issues.
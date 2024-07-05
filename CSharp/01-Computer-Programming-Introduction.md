## 🌍 Data, Information & Knowledge

### 📈 Understanding Data

Data refers to a collection of raw facts, often represented in numerical or symbolic form.

Data could refer to anything that could be measured, counted or qualified.

Visualize data as the fundamental building blocks that could be combined or transformed to form something meaningful.

Data comes in various forms, including numbers, text, images, and even sounds.

Examples of data:

- **Numbers**: 23, 42, 7.89
- **Text**: "Hello, world!", "C# programming"
- **Images**: A picture of a sunset 🌅
- **Sounds**: The sound of a bird chirping 🐦

In C#, data is often represented using variables. Variables act as containers for storing different types of data, such as numbers and symbols.

### 💡 Transforming Data Into Information

Information is data that has meaning, context, and purpose.

Information is what we derive when data is collected, analyzed and presented in a meaningful way, order or context.

Examples of transforming data into information:

- **Raw Data**: 25, 30, 35, 40
- **Information**: "The temperatures for the week are 25°C, 30°C, 35°C, and 40°C."

In this example, individual temperature readings (data) are combined to give a summary of the week's weather (information).

Information answers questions like "who," "what," "where," "when," and "how."

Data becomes information by first collecting raw data, then processing it by sorting, filtering, and organizing, and finally presenting it in meaningful ways such as charts, reports, or summaries.

In C#, this involves processing and organizing data through algorithms and logic.

### 🧠 Gaining Knowledge From Information

Knowledge represents the wisdom we gain when we understand and connect different pieces of information.

Knowledge is the deeper understanding or the application of information in a meaningful way that comes from putting together various bits of data and information and making sense of them.

Gaining knowledge involves recognizing patterns, making connections, and applying information to make decisions or solve problems.

Examples of knowledge:

- **Information**: "The temperatures this week are 25°C, 30°C, 35°C, and 40°C."
- **Knowledge**: "It is getting progressively hotter throughout the week, so it might be wise to stay hydrated and wear light clothing."

The data-information-knowledge hierarchy represents the transformation from raw data to valuable knowledge:

- **Data**: Raw facts (e.g., individual temperature readings).
- **Information**: Organized data (e.g., weekly temperature summary).
- **Knowledge**: Insights derived from information (e.g., understanding the weather trend and its implications).

### 💻 Practical Example

The following steps represent a simple example of how we can process data in C# to turn it into information and knowledge.

**Step 1. Collect Data**

```csharp
int[] temperatures = { 25, 30, 35, 40 };
```

**Step 2. Process Data to Create Information**

```csharp
int sum = 0;

for (int counter = 0; counter < temperatures.Length; counter++)
{
    sum += temperatures[counter];
}

double averageTemperature = sum / temperatures.Length;
Console.WriteLine("Average Temperature: " + averageTemperature);
```

**Step 3. Apply Knowledge**

```csharp
if (averageTemperature > 30)
{
    Console.WriteLine("It's a hot week! Stay hydrated. 🥤");
}
else
{
    Console.WriteLine("The weather is moderate. Enjoy your week! 😎");
}
```

In this example, we collected temperature data, calculated the average to create information, and then used that information to gain knowledge about the weather.

## 💻 Computer Programming

### ⌨️ Computer Programming Definition

Computer programming is the process of writing a set of instructions/commands for a computer to follow. These instructions are written in a **programming language**.

Computer programming allow us to solve problems, automate tasks, and bring to life a wide range of creations, from basic applications to complex systems.

Key concepts:

- **Program**: A set of instructions that a computer follows to perform a specific task.
- **Programming Language**: A language used to write programs (e.g., C#, Java, Python, JavaScript).
- **Code**: The actual text written in a programming language.
- **Execution**: When the computer follows these instructions, it "executes" the code.

Programming can be likened to providing a recipe to a chef. In this analogy, the recipe serves as a detailed guide for the chef, instructing them on each step required to prepare a particular dish. Similarly, a computer program functions as a set of instructions that guide the computer through a series of steps, enabling it to successfully execute a given task.

### 🎖️ Learning Computer Programming

There are countless advantages of learning computer programming:

- **Problem-Solving Skills**: Programming enhances one's ability to solve problems logically.
- **Career Opportunities**: There is a high demand for skilled programmers in various industries.
- **Understanding Technology Better**.
- **Automation**: Programming helps automate repetitive tasks, saving time and effort.
- **Creativity and Innovation**: Programming allows one to bring his/her ideas to life, whether it is a game, website, or mobile application.

Countless successful individuals trace their roots back to being developers or engineers. By mastering software engineering, you are setting the stage for a future filled with potential and achievement.

## 🔤 Programming Languages

### 🤝 Interfaces

Programming languages represent sets of rules and symbols used to write instructions (**code**) that computers can understand and execute.

Programming languages act as the bridge (**interface**) between human thought and machine execution. For developers, these languages provide a way to express algorithms and manage data. For computers, they translate human-readable code into machine-readable instructions, enabling the execution of tasks and operations.

Key concepts:

- **Syntax**: The set of rules that defines the combinations of symbols (e.g., **keywords**) considered to be correctly structured programs in a language.
- **Semantics**: The meaning of the symbols, expressions, and statements in a programming language.
- **Compiler**: A program that translates code from a high-level programming language to a low-level machine language that computers can execute.
- **Interpreter**: A program that directly executes instructions written in a programming language without requiring them to have been compiled into machine language.

### ⚖️ Key Differences

Programming languages differ in several key areas:

- **Abstraction** (Low-level and High-level programming languages);
- **Syntax** and **Semantics**;
- **Paradigms** (Programming style, e.g. Object-oriented programming or Functional programming);
- **Performance** (Speed/Efficiency);
- **Type Systems**;
- **Availability of pre-built tools and resources**;
- **Platform Compatibility**;
- **Community and Support**.

**Low-level programming languages** are closer to machine code and provide little abstraction from the hardware.

Examples:

- Machine Language;
- Assembly Language.

**High-level programming languages** are more abstract and easier for humans to read, write and understand. They are designed to be more intuitive and closer to human languages/way of expression.

Examples:

- C#;
- Java;
- Python;
- JavaScript.

Programming languages differ in syntax and semantics, meaning they use different sets of rules and structures for writing code. Each language has its own unique keywords, logic structures, and conventions for organizing and interpreting instructions. These differences can affect how programs are written, understood, and executed.

The programming language's **paradigm** (or paradigms) refers to the supported programming style.

Example:

- Java support **Object-Oriented Programming** (OOP).
- Haskell supports **Functional Programming** (FP).

The programming language's performance refers to the speed and efficiency of code execution. For instance, C is faster than Python.

**Type systems** are concerned with the management of data types within programming languages. Certain programming languages are classified as **statically typed**, whereas others are categorized as **dynamically typed**.

Examples:

- C# and Java are statically typed languages.
- JavaScript is a dynamically typed language.

When writing code, it is common to utilize code that has been previously written by others. The availability of libraries and frameworks, which are pre-built tools and resources, varies across programming languages. Libraries and frameworks can be thought of as **packages** that encompass various **frequently used functionalities**, and they can be conveniently imported into the codebase. This way, the developer uses functionality that is already developed and tested, and there is no need to reinvent the wheel.

The community also plays a role. The size and activity of both user and developer communities can greatly impact the success and growth of a certain technology. This can vary depending on the country in which the language is being used. For instance, there may be extensive support for popular languages like JavaScript, while more niche languages like Rust may have a smaller but dedicated community.

Programming languages also differ in terms of their **platform compatibility**, which refers to their ability to run on **various operating systems and environments**. Some languages are specifically designed for certain operating systems, such as Swift for iOS and Kotlin for Android.

Furthermore, programming languages vary in their intended **purpose**. While some languages are considered **general-purpose**, like C# and Java, others are **domain-specific**.

Examples:

- HTML and CSS are used for creating and styling web applications.
- SQL is used for managing and querying relational databases.

> HTML, CSS and SQL might not meet the criteria to be classified as programming languages; instead, they could be categorized as a markup language (HTML), a stylesheet language (SQL) or query language (SQL).

## 🧪 Algorithms

An **algorithm** is a step-by-step set of instructions designed to perform a specific task or solve a problem. An algorithms consists of a finite set of instructions that, when followed, accomplish a particular task.

The term algorithm may be described as a **procedure** or **formula**.

### 👟 Steps

Algorithms are essentially a series of steps or rules that guide the process of solving a problem or completing a task.

For instance, the algorithm for brushing teeth may involve steps such as wetting the toothbrush, applying toothpaste, brushing teeth, and rinsing the mouth.

Example:

Step 1. Wet the Toothbrush 💦
Step 2. Apply Toothpaste 🪥
Step 3. Brush Teeth 🫧
Step 4. Rinse Mouth 😁

The algorithm, written in C#:

```csharp
WetToothbrush();

ApplyToothpaste();

BrushTeeth();

RinseMouth();
```

### 🚧 Edge Cases

Does the algorithm for brushing teeth address the problem at hand? Indeed, it does. However, it is crucial to consider how we should handle various specific situations or edge cases that may arise.

The initial inquiry revolves around the duration required for brushing teeth.

```csharp
WetToothbrush();

ApplyToothpaste();

BrushTeeth(); // 👈 How long?

RinseMouth();
```

We could solve this problem by introducing a loop.

```csharp
WetToothbrush();

ApplyToothpaste();

while (TeethNotClean())
{
	BrushTeeth();
}

RinseMouth();
```

The subsequent inquiries would revolve around the availability of toothbrushes and/or toothpaste. Are there any alternative methods to accomplish the task?

```csharp
if (!HaveToothbrush())
{
	BuyToothbrush();
}

if (!HaveToothpaste())
{
	BuyToothpaste();
}

WetToothbrush();

ApplyToothpaste();

while (TeethNotClean())
{
	BrushTeeth();
}

RinseMouth();
```

This way, we can continue to ask additional questions: Do we have the money to buy the products? Are they available in the store?

The important thing is to seek optimal solutions to the tasks. Solutions that describe the possible steps we would take, even in the most unconventional situations. It is important to be able to describe problems in depth and solve them comprehensively, covering most side/additional cases.

### 👀 Ask Questions

In order to become a better developer, you need to learn how to ask questions that might give you more information about:

- Solving the problem;
- Considering all edge cases;
- Ensuring the expect results;
- Any performance/platform specificity.

Happy coding and happy brushing! 😊🦷

## 🔧 Integrated Development Environments

**Integrated Development Environments** (IDE) are software applications that combine essential tools for developers, including a **code editor**, **debugger**, **compiler** and more, within a unified platform. Having an IDE eliminates the need for developers to constantly switch between different applications while coding.

An IDE provides various features like **auto-completion** (IntelliSense), **syntax highlighting**, and **error detection**. It could also include built-in debuggers that would allow developers to quickly identify and fix error within the codebase by analyzing the code line by line.

Integrated Development Environments also assist in project organization and management through functionalities like **version control**, **file navigation**, and **task automation**.

An IDE could also offer integrated documentation and help resources, allowing developers to easily access information on functions and libraries without exiting the environment.

Some popular examples of Integrated Development Environments include Microsoft Visual Studio, Microsoft Visual Studio Code, IntelliJ IDEA, Eclipse, PyCharm, and Xcode.

## 🫠 Compilation & Interpretation

### Compilation

**Compilation** is the process of translating human-readable programming code into machine-readable instructions all at once. The machine code can be executed by a computer's CPU. In other words, compilation is the process of turning the code into a form that the computer can understand and execute.

Compilation is typically done by a compiler. A compiler performs lexical, syntax, and semantic analysis, optimization, and code generation.

The compilation process catches many types of errors before the program runs, making it easier to debug and maintain code.

Compiled code is stored in executable files (**.exe** files) and does not need recompilation unless source code changes.

Compiled programs typically run faster because the translation to machine code happens only once.

### Interpretation

Interpretation is the process of executing high-level programming code directly, without translating it into machine code beforehand.

Interpretation is typically done by an interpreter. An interpreter performs lexical, syntax, and semantic analysis and then reads and executes the code line by line in real-time.

Interpreted code can be run on any system with a compatible interpreter, providing platform independence.

Interpreters can execute code immediately, which is useful for scripting and testing small code snippets.

### Compilation & Interpretation In C#

C# is primarily a compiled language, designed to leverage the performance benefits of compilation. However, it also incorporates elements of interpretation through the .NET framework.
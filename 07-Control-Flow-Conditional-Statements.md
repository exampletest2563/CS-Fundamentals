## 💡 Conditional Statements

Conditional statements in C# are programming constructs that allow you to execute different blocks of code based on certain conditions. They enable your program to make decisions and react differently depending on the values of variables or expressions. The most common conditional statements in C# are `if`, `else if`, `else`, and `switch`.

Here’s a brief overview of each:

1. **`if` Statement**: Checks a condition, and if it's true, executes a block of code.
   ```csharp
   int age = 18;
   if (age >= 18)
   {
       Console.WriteLine("You are an adult.");
   }
   ```

2. **`else` Statement**: Follows an `if` statement and executes a block of code if the `if` condition is false.
   ```csharp
   int age = 16;
   if (age >= 18)
   {
       Console.WriteLine("You are an adult.");
   }
   else
   {
       Console.WriteLine("You are a minor.");
   }
   ```

3. **`else if` Statement**: Used after an `if` statement to specify a new condition if the previous `if` condition was false.
   ```csharp
   int score = 85;
   if (score >= 90)
   {
       Console.WriteLine("Grade: A");
   }
   else if (score >= 80)
   {
       Console.WriteLine("Grade: B");
   }
   else if (score >= 70)
   {
       Console.WriteLine("Grade: C");
   }
   else
   {
       Console.WriteLine("Grade: F");
   }
   ```

4. **`switch` Statement**: Selects one of many code blocks to be executed based on the value of a variable.
   ```csharp
   int day = 3;
   switch (day)
   {
       case 1:
           Console.WriteLine("Monday");
           break;
       case 2:
           Console.WriteLine("Tuesday");
           break;
       case 3:
           Console.WriteLine("Wednesday");
           break;
       case 4:
           Console.WriteLine("Thursday");
           break;
       case 5:
           Console.WriteLine("Friday");
           break;
       case 6:
           Console.WriteLine("Saturday");
           break;
       case 7:
           Console.WriteLine("Sunday");
           break;
       default:
           Console.WriteLine("Invalid day");
           break;
   }
   ```

### Why Use Conditional Statements?

- **Decision Making**: They help your program decide what actions to take based on various conditions.
- **Flow Control**: They allow your program to execute different code paths and ensure that the correct logic is applied.
- **Readability**: They make your code easier to read and understand by clearly defining the conditions under which certain code blocks are executed.

### Combining Conditions

You can also combine conditions using logical operators:

- **`&&` (and)**: All conditions must be true.
  ```csharp
  int age = 20;
  bool hasID = true;
  if (age >= 18 && hasID)
  {
      Console.WriteLine("You can enter the club.");
  }
  ```

- **`||` (or)**: At least one condition must be true.
  ```csharp
  bool isWeekend = true;
  bool isHoliday = false;
  if (isWeekend || isHoliday)
  {
      Console.WriteLine("You can relax today.");
  }
  ```

- **`!` (not)**: Inverts the condition.
  ```csharp
  bool isRaining = false;
  if (!isRaining)
  {
      Console.WriteLine("You can go for a walk.");
  }
  ```

Conditional statements are fundamental in C# programming, providing the capability to handle different scenarios and making your programs flexible and powerful.

Conditional statements allow you to execute different code based on certain conditions. In C#, the most common conditional statements are `if`, `else if`, `else`, and `switch`. These statements help control the flow of your program by making decisions based on the values of variables or expressions.

## 1. The `if` Statement

The `if` statement executes a block of code if a specified condition is `true`.

### Syntax
```csharp
if (condition)
{
    // Code to be executed if the condition is true
}
```

### Example
```csharp
int age = 18;

if (age >= 18)
{
    Console.WriteLine("You are an adult.");
}
```

In this example, the message "You are an adult." will be printed because the condition `age >= 18` is `true`.

## 2. The `else` Statement

The `else` statement follows an `if` statement and executes a block of code if the `if` condition is `false`.

### Syntax
```csharp
if (condition)
{
    // Code to be executed if the condition is true
}
else
{
    // Code to be executed if the condition is false
}
```

### Example
```csharp
int age = 16;

if (age >= 18)
{
    Console.WriteLine("You are an adult.");
}
else
{
    Console.WriteLine("You are a minor.");
}
```

In this example, the message "You are a minor." will be printed because the condition `age >= 18` is `false`.

## 3. The `else if` Statement

The `else if` statement allows you to check multiple conditions. It is used when you have more than two possible outcomes.

### Syntax
```csharp
if (condition1)
{
    // Code to be executed if condition1 is true
}
else if (condition2)
{
    // Code to be executed if condition2 is true
}
else
{
    // Code to be executed if none of the above conditions are true
}
```

### Example
```csharp
int score = 85;

if (score >= 90)
{
    Console.WriteLine("Grade: A");
}
else if (score >= 80)
{
    Console.WriteLine("Grade: B");
}
else if (score >= 70)
{
    Console.WriteLine("Grade: C");
}
else
{
    Console.WriteLine("Grade: F");
}
```

In this example, the message "Grade: B" will be printed because the condition `score >= 80` is `true`.

## 4. The `switch` Statement

The `switch` statement selects one of many code blocks to be executed. It is useful when you have multiple conditions based on the value of a single variable.

### Syntax
```csharp
switch (variable)
{
    case value1:
        // Code to be executed if variable == value1
        break;
    case value2:
        // Code to be executed if variable == value2
        break;
    default:
        // Code to be executed if variable doesn't match any case
        break;
}
```

### Example
```csharp
int day = 3;

switch (day)
{
    case 1:
        Console.WriteLine("Monday");
        break;
    case 2:
        Console.WriteLine("Tuesday");
        break;
    case 3:
        Console.WriteLine("Wednesday");
        break;
    case 4:
        Console.WriteLine("Thursday");
        break;
    case 5:
        Console.WriteLine("Friday");
        break;
    case 6:
        Console.WriteLine("Saturday");
        break;
    case 7:
        Console.WriteLine("Sunday");
        break;
    default:
        Console.WriteLine("Invalid day");
        break;
}
```

In this example, the message "Wednesday" will be printed because the value of `day` is `3`.

## Combining Conditions with Logical Operators

You can combine multiple conditions using logical operators like `&&` (and), `||` (or), and `!` (not).

### Example with `&&` (and)
```csharp
int age = 20;
bool hasID = true;

if (age >= 18 && hasID)
{
    Console.WriteLine("You can enter the club.");
}
else
{
    Console.WriteLine("You cannot enter the club.");
}
```

In this example, the message "You can enter the club." will be printed because both conditions `age >= 18` and `hasID` are `true`.

### Example with `||` (or)
```csharp
bool isWeekend = true;
bool isHoliday = false;

if (isWeekend || isHoliday)
{
    Console.WriteLine("You can relax today.");
}
else
{
    Console.WriteLine("You have to work today.");
}
```

In this example, the message "You can relax today." will be printed because at least one of the conditions `isWeekend` or `isHoliday` is `true`.

### Example with `!` (not)
```csharp
bool isRaining = false;

if (!isRaining)
{
    Console.WriteLine("You can go for a walk.");
}
else
{
    Console.WriteLine("You need an umbrella.");
}
```

In this example, the message "You can go for a walk." will be printed because the condition `!isRaining` is `true`.

## Conclusion

Conditional statements are essential for making decisions in your programs. By using `if`, `else if`, `else`, and `switch`, you can control the flow of your code based on various conditions. Combining these statements with logical operators allows you to create more complex decision-making processes.

In any programming language, the code needs to make decisions and carry out actions depending on different inputs. Conditional statements allow our code to make decisions based on specific conditions. Think of them as the gatekeepers or the guards of our code.

`Pseudocode`

```csharp
if (condition)
{
	// Code to be executed if condition is true
}
else
{
	// Code to be executed if condition is false
}
```

In this example the word `condition` could be replaced with one of the following:
- a literal of type `bool`;
- a variable of type `bool`;
- any expression that could be evaluated to a value of type `bool`.

## IF Statement

The IF statement consists of the keyword `if`, a condition enclosed in parentheses, and a block of code to execute if the condition is true.

```csharp
var studentScore = int.Parse(Console.ReadLine());

if (studentScore >= 50)
{
	Console.WriteLine("Pass!"); 
}
```

```csharp
var userAge = int.Parse(Console.ReadLine());

if (userAge >= 18)
{
	Console.WriteLine("You're eligible for access!");
}
```

Formatting doesn't matter.

```csharp
var userAge = int.Parse(Console.ReadLine());

if (userAge >= 18) Console.WriteLine("You're eligible for access!");
```

We can omit the curly brackets.

```csharp
var userAge = int.Parse(Console.ReadLine());

if (userAge >= 18)
	Console.WriteLine("You're eligible for access!");
```

The IF statement executes the first statement written after the condition. The curly brackets are used to wrap statements and execute them at once.

```csharp
var userAge = int.Parse(Console.ReadLine()); // Example: "12"

if (userAge >= 18)
	Console.WriteLine("You're eligible for access!");
	Console.WriteLine("You are older than 18 years old.");
```

The `if` statement is one of the most fundamental tools in programming. It allows you to execute a block of code only if a specified condition is true. This chapter will cover the basic usage of `if` statements, including `else` and `else if` statements, and will provide simple, fun, and easy-to-understand examples.

## 1. Basic `if` Statement

An `if` statement evaluates a condition inside parentheses. If the condition is true, the code block inside the curly braces `{}` is executed. If the condition is false, the code block is skipped.

### Syntax
```csharp
if (condition)
{
    // Code to be executed if the condition is true
}
```

### Example
```csharp
int temperature = 30;

if (temperature > 25)
{
    Console.WriteLine("It's a hot day!");
}
```
In this example, the message "It's a hot day!" will be printed because the condition `temperature > 25` is true.

## 2. Adding `else` Statement

The `else` statement can be used to execute a block of code if the `if` condition is false.

### Syntax
```csharp
if (condition)
{
    // Code to be executed if the condition is true
}
else
{
    // Code to be executed if the condition is false
}
```

### Example
```csharp
int temperature = 20;

if (temperature > 25)
{
    Console.WriteLine("It's a hot day!");
}
else
{
    Console.WriteLine("It's not a hot day.");
}
```
In this example, the message "It's not a hot day." will be printed because the condition `temperature > 25` is false.

## 3. Using `else if` for Multiple Conditions

When you need to check multiple conditions, you can use `else if`. This allows you to specify a new condition to test if the previous condition was false.

### Syntax
```csharp
if (condition1)
{
    // Code to be executed if condition1 is true
}
else if (condition2)
{
    // Code to be executed if condition2 is true
}
else
{
    // Code to be executed if none of the above conditions are true
}
```

### Example
```csharp
int score = 85;

if (score >= 90)
{
    Console.WriteLine("Grade: A");
}
else if (score >= 80)
{
    Console.WriteLine("Grade: B");
}
else if (score >= 70)
{
    Console.WriteLine("Grade: C");
}
else
{
    Console.WriteLine("Grade: F");
}
```
In this example, the message "Grade: B" will be printed because the condition `score >= 80` is true.

## 4. Combining Conditions with Logical Operators

You can combine multiple conditions using logical operators like `&&` (and), `||` (or), and `!` (not).

### Example with `&&` (and)
```csharp
int age = 20;
bool hasID = true;

if (age >= 18 && hasID)
{
    Console.WriteLine("You can enter the club.");
}
else
{
    Console.WriteLine("You cannot enter the club.");
}
```
In this example, the message "You can enter the club." will be printed because both conditions `age >= 18` and `hasID` are true.

### Example with `||` (or)
```csharp
bool isWeekend = true;
bool isHoliday = false;

if (isWeekend || isHoliday)
{
    Console.WriteLine("You can relax today.");
}
else
{
    Console.WriteLine("You have to work today.");
}
```
In this example, the message "You can relax today." will be printed because the condition `isWeekend || isHoliday` is true.

### Example with `!` (not)
```csharp
bool isRaining = false;

if (!isRaining)
{
    Console.WriteLine("You can go for a walk.");
}
else
{
    Console.WriteLine("You need an umbrella.");
}
```
In this example, the message "You can go for a walk." will be printed because the condition `!isRaining` is true.

## 5. Nested `if` Statements

You can place one `if` statement inside another `if` statement to check multiple conditions in a nested manner.

### Syntax
```csharp
if (condition1)
{
    if (condition2)
    {
        // Code to be executed if both condition1 and condition2 are true
    }
}
```

### Example
```csharp
int age = 20;
bool hasTicket = true;

if (age >= 18)
{
    if (hasTicket)
    {
        Console.WriteLine("You can watch the movie.");
    }
    else
    {
        Console.WriteLine("You need a ticket to watch the movie.");
    }
}
else
{
    Console.WriteLine("You are too young to watch this movie.");
}
```
In this example, the message "You can watch the movie." will be printed because both conditions `age >= 18` and `hasTicket` are true.

## Conclusion

The `if` statement is a powerful tool in C# programming that allows you to control the flow of your program based on conditions. By using `if`, `else if`, `else`, and combining conditions with logical operators, you can create complex decision-making structures in your code. Understanding and using `if` statements effectively is crucial for writing flexible and dynamic programs.


## IF-ELSE Statement

IF-ELSE statements enable our programs to take one path if a condition is true and another if it's false. They feature the familiar `if` keyword, a condition in parentheses, a block of code for the true scenario, followed by the `else` keyword and another block of code for the false scenario.

```csharp
var studentScore = int.Parse(Console.ReadLine());

if (studentScore >= 50)
{
	Console.WriteLine("Pass!"); 
}
else
{
	Console.WriteLine("Fail!");
}
```

```csharp
var studentScore = int.Parse(Console.ReadLine());
var output = "";

if (studentScore >= 50)
{
	output = "Pass!";
}
else
{
	output = "Fail!";
}

Console.WriteLine(output);
```

# Chapter: IF-ELSE Statements in C#

The `if-else` statement in C# is a fundamental tool that helps control the flow of your program by allowing you to execute different blocks of code based on certain conditions. This chapter will cover the basic usage of `if-else` statements, providing simple, fun, and easy-to-understand examples.

## 1. Basic `if-else` Statement

An `if-else` statement evaluates a condition. If the condition is true, the code inside the `if` block is executed. If the condition is false, the code inside the `else` block is executed.

### Syntax
```csharp
if (condition)
{
    // Code to be executed if the condition is true
}
else
{
    // Code to be executed if the condition is false
}
```

### Example
```csharp
int temperature = 20;

if (temperature > 25)
{
    Console.WriteLine("It's a hot day!");
}
else
{
    Console.WriteLine("It's not a hot day.");
}
```

In this example, the message "It's not a hot day." will be printed because the condition `temperature > 25` is false.

## 2. Adding `else if` for Multiple Conditions

When you need to check multiple conditions, you can use `else if` to specify a new condition to test if the previous `if` condition was false.

### Syntax
```csharp
if (condition1)
{
    // Code to be executed if condition1 is true
}
else if (condition2)
{
    // Code to be executed if condition2 is true
}
else
{
    // Code to be executed if none of the above conditions are true
}
```

### Example
```csharp
int score = 85;

if (score >= 90)
{
    Console.WriteLine("Grade: A");
}
else if (score >= 80)
{
    Console.WriteLine("Grade: B");
}
else if (score >= 70)
{
    Console.WriteLine("Grade: C");
}
else
{
    Console.WriteLine("Grade: F");
}
```

In this example, the message "Grade: B" will be printed because the condition `score >= 80` is true.

## 3. Combining Conditions with Logical Operators

You can combine multiple conditions using logical operators like `&&` (and), `||` (or), and `!` (not).

### Example with `&&` (and)
```csharp
int age = 20;
bool hasID = true;

if (age >= 18 && hasID)
{
    Console.WriteLine("You can enter the club.");
}
else
{
    Console.WriteLine("You cannot enter the club.");
}
```

In this example, the message "You can enter the club." will be printed because both conditions `age >= 18` and `hasID` are true.

### Example with `||` (or)
```csharp
bool isWeekend = true;
bool isHoliday = false;

if (isWeekend || isHoliday)
{
    Console.WriteLine("You can relax today.");
}
else
{
    Console.WriteLine("You have to work today.");
}
```

In this example, the message "You can relax today." will be printed because the condition `isWeekend || isHoliday` is true.

### Example with `!` (not)
```csharp
bool isRaining = false;

if (!isRaining)
{
    Console.WriteLine("You can go for a walk.");
}
else
{
    Console.WriteLine("You need an umbrella.");
}
```

In this example, the message "You can go for a walk." will be printed because the condition `!isRaining` is true.

## 4. Nested `if-else` Statements

You can place one `if-else` statement inside another `if-else` statement to check multiple conditions in a nested manner.

### Syntax
```csharp
if (condition1)
{
    if (condition2)
    {
        // Code to be executed if both condition1 and condition2 are true
    }
    else
    {
        // Code to be executed if condition1 is true and condition2 is false
    }
}
else
{
    // Code to be executed if condition1 is false
}
```

### Example
```csharp
int age = 20;
bool hasTicket = true;

if (age >= 18)
{
    if (hasTicket)
    {
        Console.WriteLine("You can watch the movie.");
    }
    else
    {
        Console.WriteLine("You need a ticket to watch the movie.");
    }
}
else
{
    Console.WriteLine("You are too young to watch this movie.");
}
```

In this example, the message "You can watch the movie." will be printed because both conditions `age >= 18` and `hasTicket` are true.

## 5. Practical Example: Choosing an Outfit

Let's create a fun example to determine what outfit to wear based on the weather.

### Example
```csharp
string weather = "rainy";

if (weather == "sunny")
{
    Console.WriteLine("Wear sunglasses and a hat.");
}
else if (weather == "rainy")
{
    Console.WriteLine("Don't forget your umbrella.");
}
else if (weather == "snowy")
{
    Console.WriteLine("Wear a warm coat and gloves.");
}
else
{
    Console.WriteLine("Check the weather report for more details.");
}
```

In this example, the message "Don't forget your umbrella." will be printed because the condition `weather == "rainy"` is true.

## Conclusion

The `if-else` statement is a powerful tool in C# programming that helps control the flow of your program based on conditions. By using `if`, `else if`, `else`, and combining conditions with logical operators, you can create complex decision-making structures in your code. Understanding and using `if-else` statements effectively is crucial for writing flexible and dynamic programs.

## Comparing Values

We can compare integers directly.

We can compare decimals with a given value (epsilon).

We can compare characters with characters or integers.

We can compare strings directly.

In C#, comparing values is an essential aspect of making decisions within your programs. It allows you to determine relationships between variables and execute different code based on those relationships. This chapter will cover the various comparison operators available in C#, how to use them, and provide simple, fun, and easy-to-understand examples.

## 1. Comparison Operators

C# provides several comparison operators that you can use to compare values. These operators return a boolean value (`true` or `false`) based on the comparison result.

### List of Comparison Operators

- `==` : Equal to
- `!=` : Not equal to
- `>` : Greater than
- `<` : Less than
- `>=` : Greater than or equal to
- `<=` : Less than or equal to

## 2. Using Comparison Operators

Let's explore each of these comparison operators with examples.

### Equal to (`==`)

Checks if two values are equal.

### Example
```csharp
int a = 5;
int b = 5;

if (a == b)
{
    Console.WriteLine("a is equal to b.");
}
else
{
    Console.WriteLine("a is not equal to b.");
}
```

In this example, the message "a is equal to b." will be printed because the condition `a == b` is true.

### Not equal to (`!=`)

Checks if two values are not equal.

### Example
```csharp
int a = 5;
int b = 10;

if (a != b)
{
    Console.WriteLine("a is not equal to b.");
}
else
{
    Console.WriteLine("a is equal to b.");
}
```

In this example, the message "a is not equal to b." will be printed because the condition `a != b` is true.

### Greater than (`>`)

Checks if the value on the left is greater than the value on the right.

### Example
```csharp
int a = 10;
int b = 5;

if (a > b)
{
    Console.WriteLine("a is greater than b.");
}
else
{
    Console.WriteLine("a is not greater than b.");
}
```

In this example, the message "a is greater than b." will be printed because the condition `a > b` is true.

### Less than (`<`)

Checks if the value on the left is less than the value on the right.

### Example
```csharp
int a = 5;
int b = 10;

if (a < b)
{
    Console.WriteLine("a is less than b.");
}
else
{
    Console.WriteLine("a is not less than b.");
}
```

In this example, the message "a is less than b." will be printed because the condition `a < b` is true.

### Greater than or equal to (`>=`)

Checks if the value on the left is greater than or equal to the value on the right.

### Example
```csharp
int a = 10;
int b = 10;

if (a >= b)
{
    Console.WriteLine("a is greater than or equal to b.");
}
else
{
    Console.WriteLine("a is not greater than or equal to b.");
}
```

In this example, the message "a is greater than or equal to b." will be printed because the condition `a >= b` is true.

### Less than or equal to (`<=`)

Checks if the value on the left is less than or equal to the value on the right.

### Example
```csharp
int a = 5;
int b = 10;

if (a <= b)
{
    Console.WriteLine("a is less than or equal to b.");
}
else
{
    Console.WriteLine("a is not less than or equal to b.");
}
```

In this example, the message "a is less than or equal to b." will be printed because the condition `a <= b` is true.

## 3. Practical Example: Grading System

Let's create a practical example of a simple grading system that uses comparison operators to determine the grade based on a score.

### Example
```csharp
int score = 85;

if (score >= 90)
{
    Console.WriteLine("Grade: A");
}
else if (score >= 80)
{
    Console.WriteLine("Grade: B");
}
else if (score >= 70)
{
    Console.WriteLine("Grade: C");
}
else if (score >= 60)
{
    Console.WriteLine("Grade: D");
}
else
{
    Console.WriteLine("Grade: F");
}
```

In this example, the message "Grade: B" will be printed because the condition `score >= 80` is true.

## 4. Fun Example: Age Comparison

Let's create a fun example where we compare ages to determine who is older.

### Example
```csharp
int ageAlice = 25;
int ageBob = 30;

if (ageAlice > ageBob)
{
    Console.WriteLine("Alice is older than Bob.");
}
else if (ageAlice < ageBob)
{
    Console.WriteLine("Bob is older than Alice.");
}
else
{
    Console.WriteLine("Alice and Bob are the same age.");
}
```

In this example, the message "Bob is older than Alice." will be printed because the condition `ageAlice < ageBob` is true.

## Conclusion

Comparing values is a crucial part of decision-making in programming. C# provides several comparison operators to help you evaluate relationships between variables. By understanding and using these operators, you can create dynamic and flexible programs that react appropriately to different conditions.

## 🧭 Variables Scope & Visibility

Scope defines the region of your code where a variable is accessible.

Local variables live within a specific block of code - the innermost block of code they have been declared in. If we declare a variable inside an `if` statement, it's local to that block.

```csharp
var outerScopeVariable = 20;

if (condition)
{
	// Block-scoped / Local variable
    var innerScopeVariable = 10;
    
    // innerScopeVariable is accessible here
    Console.WriteLine(innerScopeVariable);
    
    // outerScopeVariable is accessible here
    Console.WriteLine(outerScopeVariable);
}

// innerScopeVariable is not accessible here

// outerScopeVariable is accessible here
Console.WriteLine(outerScopeVariable);
```

Understanding the scope and visibility of variables is essential for writing effective and error-free programs. In C#, the scope of a variable determines where the variable can be accessed, while visibility refers to whether the variable is accessible from a certain part of your code.

## 1. What is Scope?

The scope of a variable is the part of the program where the variable is accessible. C# has several types of scopes:

- **Local Scope**: Variables declared inside a method or a block.
- **Class Scope**: Variables declared inside a class but outside any method (also known as fields).
- **Namespace Scope**: Variables declared at the namespace level (rarely used and generally considered a poor practice).

## 2. Local Scope

Variables declared within a method or a block (e.g., within `{}`) have local scope. They can only be accessed within the block where they are declared.

### Example

```csharp
class Program
{
    static void Main(string[] args)
    {
        int x = 10; // x is local to Main method
        if (x > 5)
        {
            int y = 20; // y is local to the if block
            Console.WriteLine(y); // y is accessible here
        }
        // y is not accessible here
        Console.WriteLine(x); // x is still accessible here
    }
}
```

In this example, `x` is accessible throughout the `Main` method, but `y` is only accessible within the `if` block where it is declared.

## 3. Class Scope

Variables declared directly within a class but outside any method are known as fields. They have class scope and can be accessed by any method within the class.

### Example

```csharp
class Program
{
    int z = 30; // z is a field with class scope

    static void Main(string[] args)
    {
        Program program = new Program();
        Console.WriteLine(program.z); // z is accessible here
    }

    void Display()
    {
        Console.WriteLine(z); // z is also accessible here
    }
}
```

In this example, `z` is a field and can be accessed by any method in the `Program` class.

## 4. Understanding Visibility

Visibility is about whether a variable can be accessed from a certain part of your code. This is controlled by access modifiers such as `public`, `private`, `protected`, and `internal`.

### Common Access Modifiers

- **public**: The variable is accessible from any other code.
- **private**: The variable is only accessible within the same class.
- **protected**: The variable is accessible within the same class and by derived classes.
- **internal**: The variable is accessible within the same assembly (project).

### Example

```csharp
class Program
{
    public int publicVar = 10;
    private int privateVar = 20;
    protected int protectedVar = 30;
    internal int internalVar = 40;

    static void Main(string[] args)
    {
        Program program = new Program();
        Console.WriteLine(program.publicVar); // Accessible
        Console.WriteLine(program.privateVar); // Accessible within the same class
        Console.WriteLine(program.protectedVar); // Accessible within the same class
        Console.WriteLine(program.internalVar); // Accessible within the same assembly
    }
}

class DerivedProgram : Program
{
    void AccessVariables()
    {
        Console.WriteLine(publicVar); // Accessible
        // Console.WriteLine(privateVar); // Not accessible
        Console.WriteLine(protectedVar); // Accessible because it's a derived class
        Console.WriteLine(internalVar); // Accessible within the same assembly
    }
}
```

In this example, `publicVar` is accessible from anywhere, `privateVar` is only accessible within the `Program` class, `protectedVar` is accessible within `Program` and any derived classes, and `internalVar` is accessible within the same assembly.

## 5. Practical Example: Bank Account

Let's create a simple example to illustrate variable scope and visibility in a practical context.

### Example

```csharp
class BankAccount
{
    public string AccountHolderName; // Accessible from anywhere
    private double balance; // Accessible only within the BankAccount class

    public BankAccount(string name, double initialBalance)
    {
        AccountHolderName = name;
        balance = initialBalance;
    }

    public void Deposit(double amount)
    {
        if (amount > 0)
        {
            balance += amount;
            Console.WriteLine($"Deposited: {amount}, New Balance: {balance}");
        }
    }

    public void Withdraw(double amount)
    {
        if (amount > 0 && amount <= balance)
        {
            balance -= amount;
            Console.WriteLine($"Withdrawn: {amount}, New Balance: {balance}");
        }
        else
        {
            Console.WriteLine("Invalid withdraw amount");
        }
    }

    public void DisplayBalance()
    {
        Console.WriteLine($"Current Balance: {balance}");
    }
}

class Program
{
    static void Main(string[] args)
    {
        BankAccount account = new BankAccount("John Doe", 500);
        account.Deposit(150);
        account.Withdraw(100);
        account.DisplayBalance();
        Console.WriteLine($"Account Holder: {account.AccountHolderName}");
        // Console.WriteLine($"Balance: {account.balance}"); // Not accessible because balance is private
    }
}
```

In this example, `AccountHolderName` is public and accessible from anywhere, while `balance` is private and only accessible within the `BankAccount` class. This demonstrates the use of scope and visibility to control access to variables.

## Conclusion

Understanding the scope and visibility of variables is crucial for managing and organizing your code. Scope defines where a variable can be accessed, while visibility (controlled by access modifiers) defines whether a variable can be accessed from certain parts of your code. By using these concepts effectively, you can write cleaner, more maintainable, and error-free programs.

## Multiple Conditions

In C#, you often need to evaluate multiple conditions to make decisions within your programs. Combining conditions allows you to create more complex and flexible decision-making logic. This chapter will cover how to use logical operators to combine multiple conditions and provide simple, fun, and easy-to-understand examples.

## 1. Logical Operators

Logical operators are used to combine multiple conditions. The main logical operators in C# are:

- `&&` (AND): Returns true if both conditions are true.
- `||` (OR): Returns true if at least one condition is true.
- `!` (NOT): Inverts the boolean value of a condition.

## 2. Using `&&` (AND) Operator

The `&&` operator allows you to combine two or more conditions that must all be true for the combined condition to be true.

### Syntax
```csharp
if (condition1 && condition2)
{
    // Code to be executed if both condition1 and condition2 are true
}
```

### Example
```csharp
int age = 20;
bool hasTicket = true;

if (age >= 18 && hasTicket)
{
    Console.WriteLine("You can enter the concert.");
}
else
{
    Console.WriteLine("You cannot enter the concert.");
}
```

In this example, the message "You can enter the concert." will be printed because both conditions `age >= 18` and `hasTicket` are true.

## 3. Using `||` (OR) Operator

The `||` operator allows you to combine two or more conditions where at least one of the conditions must be true for the combined condition to be true.

### Syntax
```csharp
if (condition1 || condition2)
{
    // Code to be executed if either condition1 or condition2 is true
}
```

### Example
```csharp
bool isWeekend = true;
bool isHoliday = false;

if (isWeekend || isHoliday)
{
    Console.WriteLine("You can relax today.");
}
else
{
    Console.WriteLine("You have to work today.");
}
```

In this example, the message "You can relax today." will be printed because the condition `isWeekend` is true.

## 4. Using `!` (NOT) Operator

The `!` operator inverts the boolean value of a condition. If the condition is true, `!condition` will be false and vice versa.

### Syntax
```csharp
if (!condition)
{
    // Code to be executed if condition is false
}
```

### Example
```csharp
bool isRaining = false;

if (!isRaining)
{
    Console.WriteLine("You can go for a walk.");
}
else
{
    Console.WriteLine("You need an umbrella.");
}
```

In this example, the message "You can go for a walk." will be printed because the condition `!isRaining` is true.

## 5. Combining Multiple Logical Operators

You can combine multiple logical operators to create complex conditions.

### Example
```csharp
int age = 20;
bool hasTicket = true;
bool knowsPassword = false;

if ((age >= 18 && hasTicket) || knowsPassword)
{
    Console.WriteLine("You can enter the secret event.");
}
else
{
    Console.WriteLine("You cannot enter the secret event.");
}
```

In this example, the message "You can enter the secret event." will be printed because the combined condition `(age >= 18 && hasTicket) || knowsPassword` is true.

## 6. Practical Example: Online Shopping Discount

Let's create a practical example where we determine if a customer is eligible for a discount based on multiple conditions.

### Example
```csharp
bool isMember = true;
int totalPurchase = 120;
bool hasCoupon = false;

if (isMember && (totalPurchase > 100 || hasCoupon))
{
    Console.WriteLine("You get a discount!");
}
else
{
    Console.WriteLine("No discount available.");
}
```

In this example, the message "You get a discount!" will be printed because the combined condition `isMember && (totalPurchase > 100 || hasCoupon)` is true.

## 7. Fun Example: Adventure Game Choices

Let's create a fun example for an adventure game where a player needs certain items to enter a cave.

### Example
```csharp
bool hasKey = true;
bool hasTorch = false;
bool knowsSecretPhrase = true;

if (hasKey && (hasTorch || knowsSecretPhrase))
{
    Console.WriteLine("You can enter the cave.");
}
else
{
    Console.WriteLine("You cannot enter the cave.");
}
```

In this example, the message "You can enter the cave." will be printed because the combined condition `hasKey && (hasTorch || knowsSecretPhrase)` is true.

## Conclusion

Combining multiple conditions using logical operators allows you to create more complex and nuanced decision-making logic in your programs. By understanding and effectively using `&&`, `||`, and `!`, you can write code that responds appropriately to a variety of situations. Mastering these concepts will make your programs more flexible and dynamic.


```csharp
var studentScore = int.Parse(Console.ReadLine());
var output = "";

if (studentScore >= 90)
{
	output = "Excellent!";
}
else if (studentScore >= 50)
{
	output = "Pass!";
}
else
{
	output = "Fail!";
}

Console.WriteLine(output);
```

## Nested Conditional Statements

Nested conditional statements in C# allow you to place one conditional statement inside another. This technique helps you create more complex decision-making logic by evaluating multiple conditions in a hierarchical manner. This chapter will cover the basics of nested conditional statements and provide simple, easy-to-understand examples.

## 1. What are Nested Conditional Statements?

Nested conditional statements involve placing one conditional statement (such as `if`, `else if`, or `else`) inside another. This allows you to evaluate multiple conditions in a hierarchical structure, where the inner conditional statements depend on the outcome of the outer ones.

## 2. Syntax of Nested Conditional Statements

```csharp
if (outerCondition)
{
    // Outer code block

    if (innerCondition1)
    {
        // Inner code block 1
    }
    else if (innerCondition2)
    {
        // Inner code block 2
    }
    else
    {
        // Default inner code block
    }
}
else
{
    // Default outer code block
}
```

In nested conditional statements, the inner `if`, `else if`, or `else` statements are placed inside the code block of the outer conditional statement.

## 3. Example of Nested Conditional Statements

Let's look at a simple example to understand how nested conditional statements work:

```csharp
int age = 20;
bool hasID = true;

if (age >= 18)
{
    Console.WriteLine("You are eligible to enter the club.");

    if (hasID)
    {
        Console.WriteLine("You have your ID. Enjoy your night!");
    }
    else
    {
        Console.WriteLine("Sorry, you need to have your ID with you.");
    }
}
else
{
    Console.WriteLine("You are not eligible to enter the club.");
}
```

In this example:
- The outer `if` statement checks if the person is of legal age to enter the club.
- If they are, it then checks if they have their ID with them using the inner `if` statement.
- Depending on the conditions, different messages are printed to the console.

## 4. Benefits of Nested Conditional Statements

Nested conditional statements provide a way to create more complex decision-making logic by allowing you to evaluate multiple conditions in a structured manner. They help in handling different scenarios and making more nuanced decisions in your programs.

## 5. Practical Example: Ticket Pricing

Let's consider a practical example where we determine ticket pricing based on age and membership status:

```csharp
int age = 25;
bool isMember = true;

if (age >= 18)
{
    Console.WriteLine("You are eligible to buy a ticket.");

    if (isMember)
    {
        Console.WriteLine("As a member, you get a discount. Ticket price: $20");
    }
    else
    {
        Console.WriteLine("Ticket price for non-members: $30");
    }
}
else
{
    Console.WriteLine("You are too young to buy a ticket.");
}
```

In this example:
- The outer `if` statement checks if the person is of legal age to buy a ticket.
- If they are, the inner `if` statement checks if they are a member to determine the ticket price.
- Based on the conditions, different ticket prices are displayed.

We can nest IF statements within each other to create more complex conditions and handle various scenarios.

```csharp
var studentScore = int.Parse(Console.ReadLine());
var output = string.Empty;

if (studentScore >= 0 && studentScore <= 100)
{
	if (studentScore >= 90)
	{
		output = "Excellent!";
	}
	else if (studentScore >= 50)
	{
		output = "Pass!";
	}
	else
	{
		output = "Fail!";
	}
}
else
{
	output = "Invalid Score!";
}

Console.WriteLine(output);
```

```csharp
var studentScore = int.Parse(Console.ReadLine());
var output = "";

if (studentScore < 0 || studentScore > 100)
{
	output = "Invalid Score!";
}
else
{
	if (studentScore >= 90)
	{
		output = "Excellent!";
	}
	else if (studentScore >= 50)
	{
		output = "Pass!";
	}
	else
	{
		output = "Fail!";
	}
}

Console.WriteLine(output);
```

```csharp
var userAge = 22;
var hasAccount = false;

if (userAge >= 18)
{
	if (hasAccount)
	{
		Console.WriteLine("Welcome!");
	}
	else
	{
		Console.WriteLine("You need to create an account.");
	}
}
else
{
	Console.WriteLine("Access restricted to users 18 and older.");
}
```


## Conclusion

Nested conditional statements provide a powerful way to create complex decision-making logic in your C# programs. By organizing your conditions hierarchically, you can handle different scenarios and make more nuanced decisions based on multiple factors. Understanding and effectively using nested conditional statements can make your code more flexible and capable of handling a variety of situations.

## 🛠️ Building Complex Boolean Expressions

We can use logical operators to create complex boolean conditions.

```csharp
var isPremiumMember = true;
var isVipMember = false;

if (isPremiumMember || isVipMember)
{
	Console.WriteLine("You have special privileges!");
}
```

```csharp
bool orderContainsMerchandiseProduct = true;
bool isActivePromotion = true;
bool hasOrderDiscount = orderContainsMerchandiseProduct && isActivePromotion;
Console.WriteLine(hasOrderDiscount);
```

```csharp
var age = 25;
var isAccountActive = true;
var hasMembership = true;

if (age >= 18 && isAccountActive && hasMembership)
{
    Console.WriteLine("Welcome! You have access.");
}
```

Parentheses `()` are essential for clarifying the order of evaluation.

```csharp
var isWeekend = true;
var isHoliday = false;
var temperatureCelsius = 32;

var goOutside = (isWeekend || isHoliday) && (temperatureCelsius > 25);
Console.WriteLine(goOutside); // 👈 Prints "True"
```

Storing the result of the evaluation in an variable may add to the code readability.

```csharp
var age = int.Parse(Console.ReadLine());
var isValid = age >= 1 && age <= 100;

if (!isValid)
{
	Console.WriteLine("Invalid age!");
}
```

```csharp
var age = 22;
var isMember = true;

if ((age >= 18 && age <= 30) || isMember)
{
	Console.WriteLine("You qualify for a discount!");
}
```

```csharp
var isPremiumMember = true;
var isVipMember = false;
var age = int.Parse(Console.ReadLine());
var isAccountBlocked = false;

if ((isPremiumMember || isVIPMember) && age >= 25 && age <= 40 && !isAccountBlocked)
{
	Console.WriteLine("Welcome! You meet the criteria.");
}
```

C# supports short-circuiting, where the second operand is only evaluated if necessary. This can improve performance and prevent unnecessary computations.

The following example will not call the functionality `CheckResourceAvailability()` if the variable `isAvailable` is evaluated to false.

Building complex boolean expressions in C# involves combining multiple conditions using logical operators (`&&`, `||`, `!`) to create more sophisticated decision-making logic. This chapter will cover the basics of constructing complex boolean expressions and provide simple, easy-to-understand examples.

## 1. What are Complex Boolean Expressions?

Complex boolean expressions consist of multiple conditions joined together using logical operators. These expressions allow you to create intricate decision-making logic by evaluating multiple conditions simultaneously.

## 2. Logical Operators

### - `&&` (AND): Returns true if both conditions on the left and right are true.
### - `||` (OR): Returns true if at least one of the conditions on the left or right is true.
### - `!` (NOT): Inverts the boolean value of a condition.

## 3. Constructing Complex Boolean Expressions

To build a complex boolean expression, you combine simple conditions using logical operators. Here's the general syntax:

```csharp
if (condition1 && condition2 || condition3 && !condition4)
{
    // Code to be executed if the complex condition is true
}
```

In this example, `condition1`, `condition2`, `condition3`, and `condition4` represent individual conditions that can be true or false. The logical operators (`&&`, `||`, `!`) allow you to create complex combinations of these conditions.

## 4. Example of Complex Boolean Expression

Let's consider an example where we determine whether a person is eligible for a discount based on their age and membership status:

```csharp
int age = 25;
bool isMember = true;

if ((age >= 18 && age <= 30 && isMember) || age >= 65)
{
    Console.WriteLine("You are eligible for a discount!");
}
else
{
    Console.WriteLine("You are not eligible for a discount.");
}
```

In this example:
- The complex boolean expression `(age >= 18 && age <= 30 && isMember) || age >= 65` combines multiple conditions.
- It checks if the person is between the ages of 18 and 30, is a member, or is 65 years or older.
- Depending on the outcome, different messages are displayed.

## 5. Benefits of Complex Boolean Expressions

Building complex boolean expressions allows you to create more sophisticated decision-making logic in your C# programs. By combining multiple conditions using logical operators, you can handle a wide range of scenarios and make nuanced decisions based on various factors.

## 6. Practical Example: Admission Criteria

Let's consider a practical example where we determine whether a student meets the admission criteria based on their test scores and extracurricular activities:

```csharp
int testScore = 85;
bool hasExtracurricular = true;

if ((testScore >= 80 && testScore <= 100) || (testScore >= 70 && testScore <= 100 && hasExtracurricular))
{
    Console.WriteLine("Congratulations! You are admitted.");
}
else
{
    Console.WriteLine("Sorry, you do not meet the admission criteria.");
}
```

In this example:
- The complex boolean expression `(testScore >= 80 && testScore <= 100) || (testScore >= 70 && testScore <= 100 && hasExtracurricular)` evaluates multiple conditions.
- It checks if the test score falls within certain ranges and if the student has participated in extracurricular activities.
- Based on the conditions, the program determines whether the student is admitted.

## Conclusion

Constructing complex boolean expressions in C# allows you to create sophisticated decision-making logic that can handle a variety of scenarios. By combining simple conditions using logical operators, you can build expressions that make nuanced decisions based on multiple factors. Mastering the creation of complex boolean expressions is essential for writing flexible and robust code.

Certainly! Let's develop the example you provided:

```csharp
bool isAvailable = true;

// Function to check resource availability
bool CheckResourceAvailability()
{
    // Simulating resource availability check
    // For demonstration purposes, always return true
    return true;
}

// Main program logic
if (isAvailable && CheckResourceAvailability())
{
    Console.WriteLine("Resource is available and ready to use.");
    // Additional code can go here
}
else
{
    Console.WriteLine("Resource is not available or cannot be used at the moment.");
    // Additional handling for unavailable resource
}
```

In this example:
- `isAvailable` is a boolean variable indicating whether the resource is available.
- `CheckResourceAvailability()` is a function that checks the availability of the resource. For demonstration purposes, it always returns true.
- The `if` statement checks if `isAvailable` is true and if `CheckResourceAvailability()` returns true.
- If both conditions are met, it prints a message indicating that the resource is available and ready to use.
- If either condition fails, it prints a message indicating that the resource is not available or cannot be used at the moment.

You can replace the `CheckResourceAvailability()` function with your actual logic to check the availability of the resource.

## De Morgan Laws

# Chapter: De Morgan's Laws

De Morgan's Laws are fundamental principles in logic that help in simplifying and understanding complex boolean expressions. This chapter will explain De Morgan's Laws, both in general terms and how they apply specifically to C# programming.

## 1. What are De Morgan's Laws?

De Morgan's Laws are two rules in logic that describe how to negate complex boolean expressions involving conjunctions (AND) and disjunctions (OR). These laws are named after the mathematician and logician Augustus De Morgan.

## 2. De Morgan's Laws in General Terms

### Law 1: Negation of a Conjunction (AND)

The negation of a conjunction is logically equivalent to the disjunction of the negations of the individual statements.

Mathematically:
```
!(A && B) = !A || !B
```

### Law 2: Negation of a Disjunction (OR)

The negation of a disjunction is logically equivalent to the conjunction of the negations of the individual statements.

Mathematically:
```
!(A || B) = !A && !B
```

## 3. De Morgan's Laws in C#

In C# programming, De Morgan's Laws are applied when dealing with boolean expressions.

### Law 1: Negation of a Conjunction (AND)

In C#, when you need to negate a conjunction (AND), you can distribute the negation to each individual condition and change the conjunction to a disjunction (OR).

```csharp
!(condition1 && condition2) == !condition1 || !condition2
```

### Law 2: Negation of a Disjunction (OR)

Similarly, when you need to negate a disjunction (OR), you can distribute the negation to each individual condition and change the disjunction to a conjunction (AND).

```csharp
!(condition1 || condition2) == !condition1 && !condition2
```

## 4. Example: Applying De Morgan's Laws in C#

Let's consider an example where we apply De Morgan's Laws to simplify a complex boolean expression in C#.

```csharp
bool condition1 = true;
bool condition2 = false;

// Original expression
if (!(condition1 && condition2))
{
    Console.WriteLine("Original expression is true.");
}
else
{
    Console.WriteLine("Original expression is false.");
}

// Applying De Morgan's Law 1
if (!condition1 || !condition2)
{
    Console.WriteLine("Expression after applying De Morgan's Law 1 is true.");
}
else
{
    Console.WriteLine("Expression after applying De Morgan's Law 1 is false.");
}

// Applying De Morgan's Law 2
if (!(condition1 || condition2))
{
    Console.WriteLine("Expression after applying De Morgan's Law 2 is true.");
}
else
{
    Console.WriteLine("Expression after applying De Morgan's Law 2 is false.");
}
```

In this example:
- We have an original expression `!(condition1 && condition2)`.
- We apply De Morgan's Law 1 and De Morgan's Law 2 to simplify the expression and compare the results.
- The output will demonstrate the equivalence of the original expression and the simplified expressions after applying De Morgan's Laws.

## Conclusion

De Morgan's Laws are powerful principles in logic that help in simplifying complex boolean expressions. By understanding these laws and applying them appropriately, you can make your code more readable and easier to understand. In C# programming, De Morgan's Laws are particularly useful when dealing with boolean conditions in if statements, loops, and other control structures.

In C#, De Morgan's Laws are principles in Boolean algebra that describe the relationships between logical AND (`&&`), logical OR (`||`), and logical NOT (`!`) operators. These laws provide equivalent expressions for negating compound logical expressions, aiding in simplifying and understanding complex conditions in code.

De Morgan's Laws in C# are as follows:

1. The negation of a conjunction is the disjunction of the negations:
   \[ \neg (A \land B) \equiv \neg A \lor \neg B \]

2. The negation of a disjunction is the conjunction of the negations:
   \[ \neg (A \lor B) \equiv \neg A \land \neg B \]

These laws are beneficial for writing clearer and more concise code when dealing with logical conditions.

Example:

```csharp
bool isSunny = true;
bool isWarm = false;

// Applying De Morgan's Law 1: !(isSunny && isWarm) is equivalent to !isSunny || !isWarm
bool result1 = !(isSunny && isWarm);
bool result2 = !isSunny || !isWarm;

Console.WriteLine("Result 1: " + result1); // Output: Result 1: True
Console.WriteLine("Result 2: " + result2); // Output: Result 2: True

// Applying De Morgan's Law 2: !(isSunny || isWarm) is equivalent to !isSunny && !isWarm
bool result3 = !(isSunny || isWarm);
bool result4 = !isSunny && !isWarm;

Console.WriteLine("Result 3: " + result3); // Output: Result 3: False
Console.WriteLine("Result 4: " + result4); // Output: Result 4: False
```

In the example, De Morgan's Laws are applied to logical expressions involving weather conditions. The results demonstrate the equivalence of the original expressions and their counterparts after applying De Morgan's Laws.

## 🔍 Switch Statement

Sometimes, our code needs to make decisions based on the value of a variable.

`Pseudocode`

```csharp
if (variable == value1)
{
	Console.WriteLine("Case 1");
}
else if (variable == value2)
{
	Console.WriteLine("Case 2");
}
...
else if (variable == valueN)
{
	Console.WriteLine("Case N");
}
else
{
	Console.WriteLine("Default Case");
}
```

The `switch` statement evaluates a variable against multiple possible values and executes the block of code associated with the first matching case.

`Pseudocode`

```csharp
switch (expression)
{
	case value1:
		Console.WriteLine("Case 1");
		break;
	case value2:
		Console.WriteLine("Case 2");
		break;
	...
	case N:
		Console.WriteLine("Case N");
		break;
	default:
		Console.WriteLine("Default Case");
		break;
}
```

```csharp
var dayOfWeek = int.Parse(Console.ReadLine());

switch (dayOfWeek)
{
	case 1:
		Console.WriteLine("Monday");
		break;
	case 2:
		Console.WriteLine("Tuesday");
		break;
	case 3:
		Console.WriteLine("Wednesday");
		break;
	case 4:
		Console.WriteLine("Thursday");
		break;
	case 5:
		Console.WriteLine("Friday");
		break;
	case 6:
		Console.WriteLine("Saturday");
		break;
	case 7:
		Console.WriteLine("Sunday");
		break;
	default:
		Console.WriteLine("Invalid day!");
		break;
}
```

Unlike some other languages, C# switch statements don't automatically fall through to subsequent cases. Each case must end with a `break` or other exit statement.

We can group multiple cases to execute the same block of code.

```csharp
var dayOfWeek = int.Parse(Console.ReadLine());

switch (dayOfWeek)
{
	case 1:
	case 2:
	case 3:
	case 4:
	case 5:
		Console.WriteLine("It's a weekday.");
		break;
	case 6:
	case 7:
		Console.WriteLine("It's the weekend!");
		break;
	default:
		Console.WriteLine("Invalid day!");
		break;
}
```

```csharp
var dayOfWeek = int.Parse(Console.ReadLine());

if (dayOfWeek == 1 || dayOfWeek == 2 || dayOfWeek == 3 || dayOfWeek == 4 || dayOfWeek == 5)
{
	Console.WriteLine("It's a weekday.");
}
else if (dayOfWeek == 6 || dayOfWeek == 7)
{
	Console.WriteLine("It's the weekend!");
}
else
{
	Console.WriteLine("Invalid day!");
}
```

Starting from C# 8.0, we can use switch expressions, a more expressive form of the switch statement.

```csharp
var dayOfWeek = int.Parse(Console.ReadLine());

var dayType = dayOfWeek switch
{
	>= 1 and <= 5 => "Weekday",
	>= 6 and <= 7 => "Weekend",
	_ => "Invalid day!
};

Console.WriteLine(dayType);
```

Switch statements enhance code readability, especially when dealing with multiple possible values. They make our code more structured and easier to maintain.

# Chapter: Switch Statement in C#

The switch statement in C# is a control flow statement that allows you to execute different blocks of code based on the value of a variable or expression. This chapter will cover the basics of the switch statement, how it works, and provide simple, easy-to-understand examples.

## 1. What is a Switch Statement?

A switch statement is a programming construct used to compare the value of a variable or expression against multiple possible values. It provides a concise way to execute different blocks of code based on the matched value.

## 2. Syntax of Switch Statement

The general syntax of a switch statement in C# is as follows:

```csharp
switch (expression)
{
    case value1:
        // Code to execute if expression equals value1
        break;
    case value2:
        // Code to execute if expression equals value2
        break;
    // Additional cases as needed
    default:
        // Code to execute if no case matches
        break;
}
```

## 3. How Switch Statement Works

- The switch statement evaluates the value of the expression.
- It compares the value of the expression against each case value.
- If a case value matches the expression value, the corresponding block of code is executed.
- If no case value matches, the code inside the default block (if present) is executed.
- The `break` statement is used to exit the switch block and prevent fall-through to subsequent cases.

## 4. Example of Switch Statement

Let's consider a simple example where we use a switch statement to determine the day of the week based on a numerical input:

```csharp
int dayOfWeek = 3;
string dayName;

switch (dayOfWeek)
{
    case 1:
        dayName = "Monday";
        break;
    case 2:
        dayName = "Tuesday";
        break;
    case 3:
        dayName = "Wednesday";
        break;
    case 4:
        dayName = "Thursday";
        break;
    case 5:
        dayName = "Friday";
        break;
    case 6:
        dayName = "Saturday";
        break;
    case 7:
        dayName = "Sunday";
        break;
    default:
        dayName = "Invalid day";
        break;
}

Console.WriteLine("The day is: " + dayName);
```

In this example:
- We have an integer variable `dayOfWeek` representing the day as a number.
- The switch statement evaluates the value of `dayOfWeek` and executes the corresponding case block to assign the corresponding day name to the `dayName` variable.
- If the value of `dayOfWeek` does not match any of the cases, the default block is executed, assigning "Invalid day" to `dayName`.

## 5. Benefits of Switch Statement

- Switch statements provide a concise and readable way to handle multiple conditions based on the value of a variable or expression.
- They are especially useful when there are many possible values to compare against.
- Switch statements can improve code readability and maintainability compared to using multiple nested if-else statements.

## Conclusion

The switch statement in C# is a powerful tool for executing different blocks of code based on the value of a variable or expression. By understanding how to use switch statements effectively, you can write cleaner and more organized code that is easier to understand and maintain.

## 🌟 Conditional Operator

The conditional operator, often called the ternary operator, provides a way to make decisions within a single line of code.

`Pseudocode`

```csharp
var result = (condition) ? trueExpression : falseExpression;
```

```csharp
var isDaytime = true;
var output = isDaytime ? "Day" : "Night";

Console.WriteLine(output); // Prints "Day"
```

```csharp
var isDaytime = true;
var output = "";

if (isDayTime)
{
	output = "Day";
}
else
{
	output = "Night";
}

Console.WriteLine(output); // 👈 Prints "Day"
```

```csharp
var itemPrice = 50;
var isMember = true;

var totalPrice = isMember ? itemPrice * 0.8 : itemPrice;
Console.WriteLine(totalPrice); // 👈 Prints "40"
```

```csharp
var number = int.Parse(Console.ReadLine());
Console.WriteLine("The number is " + (number % 2 == 0 ? "even" : "odd") + ".");
```

We can nest conditional operators for more complex scenarios, but be cautious not to sacrifice readability.

```csharp
var temperature = int.Parse(Console.ReadLine()); // 👈 Example: "23"

var weatherType = (temperature > 25) ? "Hot" : (temperature < 10) ? "Cold" : "Moderate";

Console.WriteLine(weatherType); // 👈 Prints "Moderate"
```

In case expressions are too long, we can format the line differently.

```csharp
var result = expression
	? veryLongTrueExpression
	: veryLongFalseExpression;

Console.WriteLine(result);
```
# Chapter: Conditional Operator in C#

The conditional operator, also known as the ternary operator, is a compact way to write conditional expressions in C#. This chapter will cover the basics of the conditional operator, how it works, and provide simple, easy-to-understand examples.

## 1. What is the Conditional Operator?

The conditional operator (`? :`) in C# is a ternary operator, meaning it takes three operands. It provides a concise way to write simple conditional expressions.

## 2. Syntax of Conditional Operator

The general syntax of the conditional operator in C# is as follows:

```csharp
condition ? expression1 : expression2
```

## 3. How Conditional Operator Works

- The conditional operator evaluates the condition.
- If the condition is true, it returns `expression1`.
- If the condition is false, it returns `expression2`.

## 4. Example of Conditional Operator

Let's consider a simple example where we use the conditional operator to determine if a person is eligible to vote based on their age:

```csharp
int age = 20;
string eligibility = (age >= 18) ? "Eligible to vote" : "Not eligible to vote";
Console.WriteLine("Person is " + eligibility);
```

In this example:
- We have an integer variable `age` representing the person's age.
- The conditional operator checks if the age is greater than or equal to 18.
- If the condition is true (age is greater than or equal to 18), it returns "Eligible to vote".
- If the condition is false (age is less than 18), it returns "Not eligible to vote".

## 5. Benefits of Conditional Operator

- The conditional operator provides a concise and readable way to write simple conditional expressions.
- It can be used inline within expressions, making code more compact and expressive.
- It is especially useful for assigning values based on conditions in a single line of code.

## Conclusion

The conditional operator in C# is a powerful tool for writing simple conditional expressions. By understanding how to use the conditional operator effectively, you can write cleaner and more concise code that is easier to understand and maintain.

## 📜 Guides

Always use curly brackets `{}` when declaring a body of a structure or a statement. Always leave an empty line after the closing bracket.

Aim to minimize the scope of your variables. Declare variables in the block of code they are used. The later you declare the variable the better.

Avoid complex nesting and complex conditions.

Use brackets to override the precedence of an operator where needed. Using brackets enhance code readability.

Use the conditional operator when making simple decisions with clear true/false outcomes. This could make your code more compact and readable. For more complex scenarios, consider using other decision-making constructs like if-else statements or switch. In such cases, traditional control flow structures might be more readable.

Certainly! Here's a list of guides and good practices about conditional statements in C#:

1. **Understand the Basics**: Before diving into more complex conditional statements, make sure you understand the basic syntax and logic of if statements, switch statements, and the ternary operator.

2. **Use Clear and Descriptive Conditions**: Write conditions that are easy to understand and clearly convey the logic of your code. Avoid overly complex conditions that may confuse other developers (or even yourself).

3. **Avoid Nested Statements When Possible**: While nested if statements can sometimes be necessary, try to keep them to a minimum to avoid code that is difficult to read and maintain. Consider refactoring nested statements into separate methods or using switch statements instead.

4. **Use Switch Statements for Multiple Conditions**: Switch statements are often a cleaner and more readable choice when you have multiple conditions based on the value of a single variable or expression.

5. **Consider Using Ternary Operator for Simple Conditions**: For simple conditional expressions that assign values based on a condition, consider using the ternary operator (`? :`). It can make your code more concise and expressive.

6. **Handle Default Cases**: Always include a default case in switch statements and consider adding an else statement for if statements to handle unexpected or invalid conditions.

7. **Avoid Using Magic Numbers**: Instead of hardcoding numerical values directly into your conditions, use named constants or enums to make your code more readable and maintainable.

8. **Encapsulate Complex Conditions**: If a condition becomes too complex, consider encapsulating it in a separate method with a descriptive name. This makes your code more modular and easier to test.

9. **Test Edge Cases**: When writing conditional statements, make sure to test both the typical and edge cases to ensure your code behaves as expected in all scenarios.

10. **Follow Coding Standards and Style Guidelines**: If you're working on a team, follow the established coding standards and style guidelines for conditional statements to maintain consistency across the codebase.

11. **Document Your Logic**: If a condition is particularly complex or non-obvious, consider adding comments to explain the logic behind it. This helps other developers understand your code more easily.

12. **Refactor Complex Conditions**: If you find yourself writing long and convoluted conditions, it may be a sign that your code could benefit from refactoring. Break down complex conditions into smaller, more manageable parts.

By following these guides and good practices, you can write clean, readable, and maintainable conditional statements in your C# code.
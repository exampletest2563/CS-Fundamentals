## 🔁 I/O Operations

#### What is I/O?
I/O stands for Input/Output. In programming, it refers to the process of exchanging data with external sources, such as files, databases, or user input/output devices like the keyboard and screen.

#### Types of I/O Operations
1. **Reading Input**: Getting data from external sources into the program.
2. **Writing Output**: Sending data from the program to external destinations.

#### Simple Examples:

### Reading Input

#### Example 1: Reading from the Console
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Enter your name:");
        string name = Console.ReadLine(); // Reads input from the console
        Console.WriteLine($"Hello, {name}!");
    }
}
```

#### Example 2: Reading from a File
```csharp
using System;
using System.IO;

class Program
{
    static void Main()
    {
        string filePath = "input.txt";
        if (File.Exists(filePath))
        {
            string content = File.ReadAllText(filePath); // Reads all text from a file
            Console.WriteLine("File Content:");
            Console.WriteLine(content);
        }
        else
        {
            Console.WriteLine("File not found!");
        }
    }
}
```

### Writing Output

#### Example 1: Writing to the Console
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Hello, World!"); // Writes output to the console
    }
}
```

#### Example 2: Writing to a File
```csharp
using System;
using System.IO;

class Program
{
    static void Main()
    {
        string filePath = "output.txt";
        string content = "This is some text to write to the file.";
        File.WriteAllText(filePath, content); // Writes text to a file
        Console.WriteLine("Data written to file successfully.");
    }
}
```

### Tips for I/O Operations

1. **Error Handling**: Always handle exceptions that might occur during I/O operations to ensure the program behaves gracefully.
2. **Resource Management**: Close or dispose of resources (like file handles) properly after using them to avoid memory leaks.
3. **Buffering**: Consider buffering for improved performance, especially when dealing with large amounts of data.
4. **Encoding**: Pay attention to character encoding when reading or writing text files to ensure proper handling of special characters.

Of course! Let's expand on the "Types of I/O Operations" using simple terms and examples:

### Types of I/O Operations

#### 1. Reading Input

**Definition**: Reading input refers to getting data from external sources into the program.

**Simple Example 1**: Reading from the Console

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Enter your age:");
        int age = Convert.ToInt32(Console.ReadLine()); // Reads input from the console
        Console.WriteLine($"You entered: {age}");
    }
}
```

In this example, the program prompts the user to enter their age using `Console.WriteLine`. It then reads the input from the console using `Console.ReadLine()` and converts it to an integer using `Convert.ToInt32()`.

**Simple Example 2**: Reading from a File

```csharp
using System;
using System.IO;

class Program
{
    static void Main()
    {
        string filePath = "data.txt";
        if (File.Exists(filePath))
        {
            string content = File.ReadAllText(filePath); // Reads all text from a file
            Console.WriteLine("File Content:");
            Console.WriteLine(content);
        }
        else
        {
            Console.WriteLine("File not found!");
        }
    }
}
```

In this example, the program reads data from a file named "data.txt" using `File.ReadAllText()`. If the file exists, it reads the content and displays it on the console.

#### 2. Writing Output

**Definition**: Writing output refers to sending data from the program to external destinations.

**Simple Example 1**: Writing to the Console

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Hello, World!"); // Writes output to the console
    }
}
```

In this example, the program writes the message "Hello, World!" to the console using `Console.WriteLine()`.

**Simple Example 2**: Writing to a File

```csharp
using System;
using System.IO;

class Program
{
    static void Main()
    {
        string filePath = "output.txt";
        string content = "This is some text to write to the file.";
        File.WriteAllText(filePath, content); // Writes text to a file
        Console.WriteLine("Data written to file successfully.");
    }
}
```

In this example, the program writes the text "This is some text to write to the file." to a file named "output.txt" using `File.WriteAllText()`.

### Conclusion
Reading input and writing output are essential aspects of I/O operations in programming. By understanding how to read data from sources like the console or files and write data to destinations like the console or files, you can create programs that interact effectively with users and external data sources.

### Conclusion
I/O operations are essential for interacting with external data sources in C#. By understanding how to read input and write output using simple methods like `Console.ReadLine()` and `File.WriteAllText()`, you can create programs that communicate effectively with users and other systems. Remember to handle errors gracefully and manage resources efficiently for robust and reliable I/O operations.

### Advanced I/O Concepts

#### Streams
- In C#, I/O operations often involve working with streams, which are sequences of data.
- Streams can represent various data sources and destinations, such as files, network connections, and memory buffers.
- The `System.IO` namespace provides classes like `FileStream`, `MemoryStream`, and `NetworkStream` for working with different types of streams.

#### StreamReader and StreamWriter
- These classes are used for reading and writing text data from/to streams, respectively.
- They provide methods for reading and writing characters, lines, and more from/to streams.
- They are often used when dealing with text files or network streams containing text data.

#### BinaryReader and BinaryWriter
- These classes are used for reading and writing binary data from/to streams, respectively.
- They provide methods for reading and writing primitive data types (integers, floating-point numbers, etc.) and byte arrays.
- They are useful when working with binary files or network streams containing binary data.

#### Asynchronous I/O
- Asynchronous I/O allows for non-blocking I/O operations, which can improve the responsiveness and scalability of applications.
- In C#, asynchronous I/O operations are commonly performed using the `async` and `await` keywords along with methods that support asynchronous operations, such as `ReadAsync` and `WriteAsync`.

#### File and Directory Operations
- In addition to reading and writing files, the `System.IO` namespace provides classes for working with files and directories, such as `File`, `Directory`, and `Path`.
- These classes offer methods for creating, deleting, moving, copying, and enumerating files and directories.

### Best Practices for I/O Operations

1. **Use Using Statement**: When working with resources like file streams, use the `using` statement to ensure proper disposal of resources even in case of exceptions.
   ```csharp
   using (FileStream fs = new FileStream("file.txt", FileMode.Open))
   {
       // Read from or write to the file
   }
   ```

2. **Buffering**: Use buffering for improved performance, especially when dealing with large files. For file streams, buffering is often enabled by default, but you can adjust the buffer size for optimal performance.

3. **Error Handling**: Handle exceptions that may occur during I/O operations gracefully to provide meaningful error messages to users and prevent unexpected application crashes.

4. **Security**: Be mindful of security considerations when reading from or writing to files, especially when dealing with user input or sensitive data. Avoid vulnerabilities like path traversal attacks.

5. **Encoding**: Specify the character encoding explicitly when working with text files to ensure proper handling of non-ASCII characters and compatibility across different systems.

### Conclusion
I/O operations are fundamental for interacting with external data sources in C#. By mastering advanced concepts like streams, asynchronous I/O, and file operations, you can build efficient and robust applications that effectively handle input and output tasks. Remember to follow best practices for error handling, security, and performance optimization when working with I/O operations in C#.

### Introduction
Input and Output (I/O) operations are essential parts of any programming language. They allow programs to interact with the outside world, such as reading from or writing to files, taking input from the keyboard, and displaying output on the screen. In this chapter, we will explore how to perform basic I/O operations in C# and handle common tasks efficiently.

### Reading and Writing to the Console
The simplest form of I/O is reading from and writing to the console. The console is the text interface that you see when you run a command-line application.

#### Writing to the Console
To display text on the console, you use the `Console.WriteLine` and `Console.Write` methods.

- `Console.WriteLine`: This method writes a message to the console, followed by a new line.
- `Console.Write`: This method writes a message to the console without adding a new line at the end.

```csharp
Console.WriteLine("Hello, World!"); // Writes "Hello, World!" followed by a new line
Console.Write("This is a test."); // Writes "This is a test." without a new line
Console.WriteLine("Next line."); // Writes "Next line." followed by a new line
```

The `Console.WriteLine` method can also be used with format specifiers to insert values into the output string.

```csharp
int age = 25;
Console.WriteLine("You are {0} years old.", age); // Outputs: You are 25 years old.
```

#### Reading from the Console
To read input from the console, you use the `Console.ReadLine`, `Console.Read`, and `Console.ReadKey` methods.

- `Console.ReadLine`: Reads a line of text input from the user until they press Enter.
- `Console.Read`: Reads the next character from the input stream.
- `Console.ReadKey`: Captures the next key press from the user without waiting for the Enter key.

```csharp
Console.WriteLine("Enter your name:");
string name = Console.ReadLine(); // Reads a line of text from the user
Console.WriteLine("Hello, " + name + "!"); // Greets the user with their name

Console.WriteLine("Press any key to continue...");
Console.ReadKey(); // Waits for the user to press a key
```

You can also capture and process individual key presses using `Console.ReadKey`.

```csharp
Console.WriteLine("Press a key to see its information:");
ConsoleKeyInfo keyInfo = Console.ReadKey();
Console.WriteLine("Key pressed: " + keyInfo.Key + ", Char: " + keyInfo.KeyChar);
```

### Working with Files
In C#, you can also read from and write to files, which allows you to store data permanently. The `System.IO` namespace provides the necessary classes for file operations.

#### Writing to a File
To write text to a file, you can use the `StreamWriter` class or the `File.WriteAllText` method.

Using `StreamWriter`:
- The `StreamWriter` class is used for writing characters to a stream in a particular encoding.

```csharp
using System.IO; // Include the System.IO namespace

string path = "example.txt"; // Path to the file
using (StreamWriter writer = new StreamWriter(path))
{
    writer.WriteLine("Hello, file!"); // Writes a line to the file
    writer.WriteLine("This is a second line."); // Writes another line
}
```

The `using` statement ensures that the `StreamWriter` object is properly disposed of when done, which closes the file and releases any resources.

Using `File.WriteAllText`:
- The `File.WriteAllText` method writes all text to a file in one call. If the file does not exist, it creates the file. If the file exists, it overwrites the content.

```csharp
string path = "example.txt";
string content = "Hello, file!\nThis is a second line.";
File.WriteAllText(path, content); // Writes the content to the file
```

#### Appending to a File
To add text to the end of a file without overwriting the existing content, use `StreamWriter` with the append parameter set to `true` or `File.AppendAllText`.

```csharp
using (StreamWriter writer = new StreamWriter(path, true))
{
    writer.WriteLine("This line is appended."); // Adds a line to the end of the file
}

string appendText = "This is appended text.\n";
File.AppendAllText(path, appendText); // Appends text to the file
```

#### Reading from a File
To read text from a file, you can use the `StreamReader` class or the `File.ReadAllText` method.

Using `StreamReader`:
- The `StreamReader` class is used for reading characters from a stream in a particular encoding.

```csharp
using System.IO;

string path = "example.txt";
using (StreamReader reader = new StreamReader(path))
{
    string line;
    while ((line = reader.ReadLine()) != null)
    {
        Console.WriteLine(line); // Reads and prints each line
    }
}
```

Using `File.ReadAllText`:
- The `File.ReadAllText` method reads all text from a file in one call.

```csharp
string path = "example.txt";
string content = File.ReadAllText(path); // Reads all text from the file
Console.WriteLine(content); // Prints the content
```

#### Reading Lines from a File
To read lines from a file into an array of strings, use the `File.ReadAllLines` method.

```csharp
string[] lines = File.ReadAllLines(path);
foreach (string line in lines)
{
    Console.WriteLine(line); // Prints each line
}
```

### Handling Exceptions
When performing I/O operations, things can go wrong, such as the file not being found or the user entering invalid input. It's important to handle these exceptions to prevent your program from crashing. You can use `try`, `catch`, and optionally `finally` blocks to handle exceptions.

```csharp
try
{
    string path = "nonexistent.txt";
    string content = File.ReadAllText(path); // This might throw an exception if the file doesn't exist
    Console.WriteLine(content);
}
catch (FileNotFoundException e)
{
    Console.WriteLine("The file was not found: " + e.Message);
}
catch (UnauthorizedAccessException e)
{
    Console.WriteLine("You do not have permission to access this file: " + e.Message);
}
catch (Exception e)
{
    Console.WriteLine("An error occurred: " + e.Message);
}
finally
{
    Console.WriteLine("This block runs regardless of whether an exception was thrown.");
}
```

### Summary
In this chapter, we've covered the basics of I/O operations in C#. You learned how to:

- Read from and write to the console using `Console.WriteLine`, `Console.Write`, `Console.ReadLine`, `Console.Read`, and `Console.ReadKey`.
- Handle file operations using `StreamWriter`, `StreamReader`, `File.WriteAllText`, `File.ReadAllText`, `File.AppendAllText`, and `File.ReadAllLines`.
- Manage exceptions using `try`, `catch`, and `finally` blocks.

With these skills, you can make your programs interact with users and other systems more effectively.

## ✍️ Reading User Input

In C#, the `Console` class provides a streamlined mechanism for interacting with the standard input (`Console.In`) and output (`Console.Out`) streams.

```csharp
Console.Write("Enter your name: ");

string username = Console.ReadLine(); // 👈 Example: "John"

Console.WriteLine("Hello, " + username + "!"); // 👈 Prints: "Hello, John!"
```

To work with other data types, converting is required.

The `Console.ReadLine` method reads a line of text entered by the user and returns it as a string.

```csharp
string firstNumber = Console.ReadLine(); // Example: "2"
string secondNumber = Console.ReadLine(); // Example: "3"

Console.WriteLine(firstNumber + secondNumber); // Prints: "23"
```

In order to convert a string to an integer, we can use the `Int32.Parse` method.

```csharp
Console.Write("Enter your age: ");

string userInput = Console.ReadLine(); // 👈 Example: "34"
int userAge = Int32.Parse(userInput); // 👈 Converts "34" to 34

Console.WriteLine(userAge + 10); // 👈 Prints: "44"
```

`Int32` and `int` are aliases.

```csharp
Console.Write("Enter your age: ");

string userInput = Console.ReadLine();
int userAge = int.Parse(userInput);

Console.WriteLine(userAge);
```

We can omit the declaration of the `userInput` variable:

```csharp
Console.Write("Enter your age: ");

int userAge = int.Parse(Console.ReadLine());

Console.WriteLine(userAge);
```

```csharp
Console.Write("Enter your age: ");

int userAge = Convert.ToInt32(Console.ReadLine());

Console.WriteLine(userAge);
```

## 🚫 Invalid Input

### Introduction
Handling invalid input is an important part of making your programs robust and user-friendly. Invalid input can come from users entering unexpected data, such as text instead of numbers, or from files that do not contain the expected information. In this chapter, we will explore techniques for detecting and managing invalid input in C#.

### Basic Input Validation
Input validation is the process of ensuring that the data entered by the user meets certain criteria before the program processes it.

#### Validating Numeric Input
One common type of invalid input is when a user is expected to enter a number but enters something else. To handle this, you can use the `int.TryParse` method, which attempts to convert a string to an integer and returns `true` if successful.

```csharp
Console.WriteLine("Enter a number:");
string userInput = Console.ReadLine();
int number;
if (int.TryParse(userInput, out number))
{
    Console.WriteLine("You entered the number: " + number);
}
else
{
    Console.WriteLine("Invalid input. Please enter a valid number.");
}
```

In this example, `int.TryParse` tries to convert the user's input to an integer. If the conversion is successful, the program continues normally. If the conversion fails, it displays an error message.

#### Validating Other Data Types
You can use similar methods for other data types:

- `double.TryParse` for double-precision floating-point numbers
- `DateTime.TryParse` for date and time values
- `bool.TryParse` for boolean values

```csharp
// Example for double
Console.WriteLine("Enter a decimal number:");
string userInput = Console.ReadLine();
double decimalNumber;
if (double.TryParse(userInput, out decimalNumber))
{
    Console.WriteLine("You entered the decimal number: " + decimalNumber);
}
else
{
    Console.WriteLine("Invalid input. Please enter a valid decimal number.");
}

// Example for DateTime
Console.WriteLine("Enter a date (mm/dd/yyyy):");
userInput = Console.ReadLine();
DateTime date;
if (DateTime.TryParse(userInput, out date))
{
    Console.WriteLine("You entered the date: " + date.ToShortDateString());
}
else
{
    Console.WriteLine("Invalid input. Please enter a valid date.");
}

// Example for bool
Console.WriteLine("Enter 'true' or 'false':");
userInput = Console.ReadLine();
bool booleanValue;
if (bool.TryParse(userInput, out booleanValue))
{
    Console.WriteLine("You entered: " + booleanValue);
}
else
{
    Console.WriteLine("Invalid input. Please enter 'true' or 'false'.");
}
```

### Handling Exceptions
Sometimes, invalid input can cause exceptions to be thrown. You can handle these exceptions using `try` and `catch` blocks to prevent your program from crashing.

#### Example: Handling Divide by Zero
A common exception is dividing by zero. You can catch this exception and handle it gracefully.

```csharp
try
{
    Console.WriteLine("Enter the numerator:");
    int numerator = int.Parse(Console.ReadLine());

    Console.WriteLine("Enter the denominator:");
    int denominator = int.Parse(Console.ReadLine());

    int result = numerator / denominator;
    Console.WriteLine("Result: " + result);
}
catch (DivideByZeroException)
{
    Console.WriteLine("Error: Cannot divide by zero. Please enter a valid denominator.");
}
catch (FormatException)
{
    Console.WriteLine("Error: Please enter valid numbers.");
}
```

In this example, if the user enters a zero for the denominator, a `DivideByZeroException` is caught, and an appropriate error message is displayed. If the user enters non-numeric input, a `FormatException` is caught.

### Validating String Input
When expecting specific text input, you can use conditions to check if the input meets your criteria.

#### Example: Checking for Empty Input
```csharp
Console.WriteLine("Enter your name:");
string name = Console.ReadLine();

if (string.IsNullOrWhiteSpace(name))
{
    Console.WriteLine("Invalid input. Name cannot be empty.");
}
else
{
    Console.WriteLine("Hello, " + name + "!");
}
```

#### Example: Checking for Specific Format
You might expect input in a specific format, such as an email address. While full email validation is complex, you can perform a basic check using string methods.

```csharp
Console.WriteLine("Enter your email address:");
string email = Console.ReadLine();

if (email.Contains("@") && email.Contains("."))
{
    Console.WriteLine("Email is valid.");
}
else
{
    Console.WriteLine("Invalid email address.");
}
```

### Using Regular Expressions
For more complex validation, you can use regular expressions (regex). Regular expressions allow you to define a pattern that the input must match.

#### Example: Validating an Email Address
```csharp
using System.Text.RegularExpressions;

Console.WriteLine("Enter your email address:");
string email = Console.ReadLine();

string pattern = @"^[^@\s]+@[^@\s]+\.[^@\s]+$";
if (Regex.IsMatch(email, pattern))
{
    Console.WriteLine("Email is valid.");
}
else
{
    Console.WriteLine("Invalid email address.");
}
```

In this example, the regular expression `^[^@\s]+@[^@\s]+\.[^@\s]+$` is used to check if the input is a valid email address.

### Summary
Handling invalid input is crucial for creating robust and user-friendly applications. In this chapter, you learned how to:

- Validate numeric, date, and boolean input using `TryParse` methods.
- Handle exceptions to manage unexpected errors gracefully.
- Validate string input for specific criteria and formats.
- Use regular expressions for complex validation needs.

By applying these techniques, you can ensure your program handles invalid input effectively and provides helpful feedback to users.

## 🗝️ Key Events

Sometimes, we want a capture a single keypress instead of a whole line. The `Console.ReadKey` method allows capturing key events.

```csharp
ConsoleKeyInfo keyInfo = Console.ReadKey();
Console.WriteLine("Key pressed: " + keyInfo.KeyChar);
```

In order to check if the user pressed the \[Enter\] key, we can use the `ConsoleKey` enumeration. It includes a variety of keys, from letters and numbers to function keys and modifiers.

```csharp
ConsoleKeyInfo keyInfo = Console.ReadKey();

if (keyInfo.Key == ConsoleKey.Enter)
{
    Console.WriteLine("Enter key pressed!");
}
```

The `Console.ReadKey` method could be used to detect special keys and modifiers, too. Modifiers are accessible via the `ConsoleModifiers` enumeration.

```csharp
ConsoleKeyInfo keyInfo = Console.ReadKey();

if (keyInfo.Key == ConsoleKey.A && keyInfo.Modifiers == ConsoleModifiers.Shift)
{
    Console.WriteLine("[Shift] + [A] pressed!");
}
```

## 📜 Guides

#### I/O Operations

**Overview:**
- I/O (Input/Output) operations in C# involve reading data from input devices like the keyboard and writing data to output devices like the console.

**Reading Input:**
- `Console.ReadLine()`: Reads a line of text from the console.
  ```csharp
  string input = Console.ReadLine();
  ```
- `Console.Read()`: Reads the next character from the input stream.
  ```csharp
  int character = Console.Read();
  ```

**Writing Output:**
- `Console.WriteLine()`: Writes a line of text to the console.
  ```csharp
  Console.WriteLine("Hello, World!");
  ```
- `Console.Write()`: Writes text to the console without a newline.
  ```csharp
  Console.Write("Hello, ");
  Console.Write("World!");
  ```

#### Invalid Input

**Handling Invalid Input:**
- Validate user input to ensure it meets expected criteria.
- Use exception handling to manage errors that arise from invalid input.

**Example of Input Validation:**
- Parse a string to an integer and handle potential errors.
  ```csharp
  Console.WriteLine("Enter a number:");
  string input = Console.ReadLine();
  try
  {
      int number = int.Parse(input);
      Console.WriteLine("You entered: " + number);
  }
  catch (FormatException)
  {
      Console.WriteLine("Invalid input, please enter a valid number.");
  }
  ```

**Using `TryParse` Method:**
- `int.TryParse()`: Tries to parse the input without throwing an exception.
  ```csharp
  Console.WriteLine("Enter a number:");
  string input = Console.ReadLine();
  int number;
  if (int.TryParse(input, out number))
  {
      Console.WriteLine("You entered: " + number);
  }
  else
  {
      Console.WriteLine("Invalid input, please enter a valid number.");
  }
  ```

#### Key Events

**Key Events in Console Applications:**
- Handle key press events using `ConsoleKeyInfo` and `Console.ReadKey()`.

**Capturing Key Presses:**
- `Console.ReadKey()`: Reads the next key pressed by the user.
  ```csharp
  Console.WriteLine("Press any key to continue...");
  ConsoleKeyInfo keyInfo = Console.ReadKey();
  Console.WriteLine("You pressed: " + keyInfo.Key);
  ```

**Key Properties:**
- `Key`: The key pressed by the user.
- `KeyChar`: The Unicode character represented by the key.
- `Modifiers`: Any modifier keys (Shift, Alt, Control) pressed in combination with the key.

**Example of Using Key Events:**
- Detecting specific keys.
  ```csharp
  Console.WriteLine("Press 'X' to exit.");
  while (true)
  {
      ConsoleKeyInfo keyInfo = Console.ReadKey(true);
      if (keyInfo.Key == ConsoleKey.X)
      {
          Console.WriteLine("Exiting...");
          break;
      }
      else
      {
          Console.WriteLine("You pressed: " + keyInfo.Key);
      }
  }
  ```

**Note:**
- Key events are more commonly used in GUI applications with event-driven programming. In console applications, key handling is limited to basic key press detection.
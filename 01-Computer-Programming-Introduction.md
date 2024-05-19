# 🎓 Computer Programming Introduction

## 🌍 Data, Information & Knowledge

Data refers to a collection of raw facts, often presented in numerical or symbolic form. Data could refer to anything that could be measured, counted or qualified.

In C#, data is often represented using variables. Variables act as containers for storing different types of data, such as numbers and symbols.

Information is data that has meaning, context, and purpose. Information is what we derive when data is collected, analyzed and presented in a meaningful way, order or context.

In C#, this involves processing and organizing data through algorithms and logic.

Knowledge represents the wisdom we gain when we understand and connect different pieces of information. Knowledge is the deeper understanding or the application of information in a meaningful way that comes from putting together various bits of data and information and making sense of them.

## 💾 Data Storage

Computers use two main storage components:
- `RAM` (Random Access Memory);
- `HDD` (Hard Disk Drive) or `SSD` (Solid State Drive).

Both components are physical components used for data storage. The main difference between `RAM` and `HDD` is the type of storage.

`HDD` stores data permanently. It is responsible for storing all data no matter if the machine is turned on or off.

`RAM` stores data temporarily. It is responsible for all applications that run on the computer.

// TODO: Add information how brain works.
The brain stores data and information through a process called memory encoding, which involves the conversion of sensory input into a form that can be stored within the brain's neural circuits. This process can be broken down into several stages:

Encoding: Information from the outside world is perceived through the senses and then processed and interpreted by the brain. During encoding, this sensory input is transformed into a neural code.

Storage: Encoded information is stored in the brain through changes in the strength of synaptic connections between neurons. This involves processes such as synaptic plasticity, where the efficiency of synaptic transmission is modified. Long-term potentiation (LTP) is one mechanism believed to underlie long-term memory storage, enhancing the synaptic connections between neurons over time.

Consolidation: Stored memories are stabilized and integrated with existing knowledge. This process often occurs during sleep and involves the transfer of information from short-term memory in the hippocampus to long-term memory storage in the cortex.

Retrieval: Stored information is accessed and brought back into conscious awareness when needed. This involves reactivating the neural circuits that were involved in the initial encoding and storage of the memory.

Memories can be categorized into different types, such as:
- Short-term memory: Temporary storage of information for seconds to minutes.
- Long-term memory: More permanent storage, which can last from days to a lifetime.
- Declarative (explicit) memory: Memories of facts and events that can be consciously recalled.
- Procedural (implicit) memory: Memories of skills and habits that are performed automatically.

## 💻 Computer Programming

Computer programming is the art of instructing computers to perform specific tasks. It's a creative process where we communicate with machines using a set of instructions.

## Programming Languages

Programming languages act as the bridge (interface) between human thought and machine execution. They represent sets of rules and symbols used to write instructions (code) that computers can understand and execute.

Programming paradigms define the style of programming. C# supports imperative, declarative and object-oriented paradigms.

// TODO: Languages are interfaces for both sides.
Programming languages are interfaces for both developers and computers. They allow developers to write instructions that computers can execute. For developers, these languages provide a way to express algorithms and manage data. For computers, they translate human-readable code into machine-readable instructions, enabling the execution of tasks and operations. Thus, programming languages bridge the gap between human logic and computer functionality.

// TODO: Differences between languages.
Programming languages differ in several key areas: syntax, which dictates the rules and structure for writing code; semantics, which define the meaning of constructs and commands; and paradigms, which support various programming styles such as object-oriented or functional. They vary in performance, with some languages executing faster than others. Type systems also differ, with languages being either statically or dynamically typed. The availability of libraries and frameworks, community and support, and platform compatibility further distinguish them, influencing the choice of language based on project requirements and developer preferences.

- Syntax: Rules and structure for writing code (e.g., Python uses indentation, C++ uses braces).
- Semantics: Meaning of the constructs and commands (e.g., how loops and conditionals function).
- Paradigms: Programming styles supported (e.g., object-oriented in Java, functional in Haskell).
- Performance: Speed and efficiency of code execution (e.g., C is faster than Python).
- Type Systems: Handling of data types (e.g., statically typed in Java, dynamically typed in JavaScript).
- Libraries and Frameworks: Availability of pre-built tools and resources (e.g., NumPy for Python, STL for C++).
- Community and Support: Size and activity of user and developer communities (e.g., extensive for JavaScript, niche for Rust).
- Platform Compatibility: Ability to run on different operating systems and environments (e.g., Swift for iOS, Kotlin for Android).

## 🧪 Algorithms

## 🔧 Integrated Development Environments

// TODO: Why we do not use text editors?
We use Integrated Development Environments (IDEs) for programming because they provide advanced features that significantly boost productivity and code quality. Unlike basic text editors, IDEs offer syntax highlighting, code completion, debugging tools, and integrated version control. These capabilities enable us to identify errors early on, streamline coding tasks, and enhance overall efficiency, making IDEs the preferred option for software development.

// TODO: Compilers / Interpreters. PC < C/I > Developer.
**Compilers:**  
A compiler translates high-level source code into machine code or bytecode before execution. It performs lexical, syntax, and semantic analysis, optimization, and code generation. Compiled code is stored in executable files and does not need recompilation unless source code changes.

**Interpreters:**  
An interpreter executes source code line by line without prior compilation. It reads, interprets, and executes code immediately, allowing for rapid development and testing. Interpreted code may run slower than compiled code due to on-the-fly translation during runtime.

For developers, compilers offer advantages in terms of performance and efficiency. Compiled languages typically run faster because the source code is translated into machine code beforehand, reducing the overhead during runtime. This makes compiled languages like C, C++, and Java preferable for applications requiring speed and optimization, such as games or system software.

On the other hand, interpreters offer flexibility and ease of use. They allow for quick development and testing as changes in the source code can be immediately executed without the need for recompilation. Interpreted languages like Python, JavaScript, and Ruby are favored for rapid prototyping, scripting, and web development due to their agility and dynamic nature.

Ultimately, the choice between compilers and interpreters depends on the specific requirements of the project, including performance considerations, development speed, and the target environment. Many developers leverage both compilers and interpreters in their toolkit to harness the benefits of each approach as needed.


// TODO: Compile time and runtime.
Compile time is the stage during software development where source code is converted into machine code or bytecode by a compiler. This process checks for syntax errors and translates human-readable code into a format that the computer can understand and execute.

Runtime, also known as execution time, happens when the compiled code is actually run by the computer's processor. It encompasses the entire duration of the program's execution, from start to finish, including any input, processing, and output operations that occur during this time. During runtime, the program interacts with the computer's hardware and peripherals to perform the tasks defined by the code.
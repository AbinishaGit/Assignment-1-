# 1.Compiler vs Interpreter Based Language
## Compiler:
A compiler translates the entire source code into machine code (or an intermediate code) before execution.
The compiled code is typically stored in a separate file, which can be executed directly by the machine.

**Examples:** C, C++, Rust.

## Interpreter:
An interpreter translates and executes the source code line by line at runtime.
There is no separate compilation step; the code is executed directly from the source.
**Examples:** Python, Ruby, JavaScript.

# Key Differences:

**Execution Speed:** Compiled languages generally execute faster because the code is already translated into machine language. Interpreted languages may be slower due to the overhead of translating code at runtime.

**Portability:** Interpreted languages are often more portable because the interpreter can run on different platforms, whereas compiled code is platform-specific.

**Development Cycle:** Interpreted languages usually have a faster development cycle since there’s no need to compile the code before running it.

# 2.How a C Program is Compiled

The compilation process of a C program typically involves several stages:
## Preprocessing:
The preprocessor handles directives like #include, #define, and #if.
It expands macros, includes header files, and processes conditional compilation.
**Output:** A preprocessed source code file (usually with a .i extension).

## Compilation:
The compiler translates the preprocessed source code into assembly language.
**Output:** An assembly code file (usually with a .s extension).

## Assembly:
The assembler converts the assembly code into machine code (object code).
**Output:** An object file (usually with a .o or .obj extension).

## Linking:
The linker combines one or more object files and libraries into a single executable file.
It resolves references to external functions and variables.
**Output:** An executable file (e.g., a.out or program.exe).

# 3. C Program Memory Structure
The memory layout of a C program typically consists of the following segments:

## Text Segment:
Contains the compiled machine code of the program.
This segment is read-only and shared among processes.

## Initialized Data Segment:

Stores global and static variables that are initialized with a value.

This segment is further divided into:

**Initialized Read-Only Data:** Constants.

**Initialized Read-Write Data:** Variables that can be modified.

**Uninitialized Data Segment (BSS):** Stores global and static variables that are not initialized.

The memory is initialized to zero by the OS.

**Heap:** Used for dynamic memory allocation (e.g., malloc, calloc, realloc).

The heap grows upwards in memory.

**Stack:** Used for function call management, including local variables and return addresses.

The stack grows downwards in memory.

## 4. How to Swap 2 Variables (Apart from *, /, and +/- Operators)
 
 can swap two variables using the XOR bitwise operator:

**#include <stdio.h>**

**int main()**

**{**

    **int a = 5, b = 10;**
    
    **printf("Before swap: a = %d, b = %d\n", a, b);**
    
    // Swapping using XOR
    
    **a = a ^ b;**
    
    **b = a ^ b;**
    
    **a = a ^ b;**
    
    **printf("After swap: a = %d, b = %d\n", a, b);**
    
    **return 0;**
    
**}**

## 5. Create a Git Account

To create a Git account (specifically on GitHub, which is a popular platform for Git repositories):

**Visit GitHub:**
**Go to GitHub's website.**

**Sign Up:** Click on the "Sign up" button.
Enter your email address, create a username, and set a password.

**Verify Your Email:**
GitHub will send a verification email to the address you provided.
Click the link in the email to verify your account.

**Complete Setup:**
Follow the on-screen instructions to complete your profile setup.
You can choose a free plan or a paid plan depending on your needs.

**Start Using Git:**
Once your account is set up, you can create repositories, clone existing ones, and start collaborating on projects.

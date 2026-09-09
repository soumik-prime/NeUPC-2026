# Level 0 - Programming Fundamentals

## 1. What is Programming?
* **What a computer program actually is**
  * Instructions executed sequentially by a machine
  * Source code $ightarrow$ compiler $ightarrow$ machine code $ightarrow$ execution
  * Understanding that a computer only does exactly what it's told, in order
* **Setting up the environment**
  * Installing a compiler (`g++`) or using an online judge/IDE (Codeforces, OnlineGDB, VS Code)
  * Writing and running the first program (*Hello World*)
  * Reading and interpreting basic compiler error messages

---

## 2. C - Core Syntax & Foundations
* **Structure of a C program**
  * `#include`, `main()`, `return` statement
  * `printf()`, `scanf()` basics
  * How a program starts and ends execution
* **Variables & Data Types**
  * `int`, `float`, `double`, `char`
  * Declaration, initialization, naming rules
  * Type sizes and `sizeof()`
  * Constants (`const`, `#define`)
* **Operators**
  * Arithmetic (`+`, `-`, `*`, `/`, `%`)
  * Relational (`==`, `!=`, `<`, `>`, `<=`, `>=`)
  * Logical (`&&`, `||`, `!`)
  * Assignment (`=`, `+=`, `-=`, `*=`, `/=`)
  * Increment/decrement (`++`, `--`), pre vs post
  * Operator precedence basics
* **Input/Output**
  * `scanf`/`printf` format specifiers (`%d`, `%f`, `%c`, `%s`)
  * Reading multiple inputs on one line
  * Common formatting mistakes (missing `&`, mismatched specifiers)
* **Conditionals**
  * `if`, `if-else`, `else if` ladder
  * `switch` statement
  * Nested conditionals
* **Loops**
  * `for`, `while`, `do-while`
  * `break`, `continue`
  * Nested loops
  * Loop-based patterns (counting, summing, iterating ranges)
* **Functions**
  * Function declaration vs definition
  * Parameters, return types, `void` functions
  * Pass by value
* **Arrays (C-style)**
  * 1D array declaration, indexing, iteration
  * 2D arrays (basic grid concept)
  * Array-function interaction (passing arrays to functions)
* **Strings (C-style)**
  * `char` arrays, null terminator `\0`
  * Basic `<string.h>` functions: `strlen`, `strcpy`, `strcmp`
* **Pointers (Introductory)**
  * What a pointer is, `&` and `*`
  * Pointer to a variable, pointer arithmetic basics

---

## 3. Problems

### C - Core Syntax
* Simple calculator (arithmetic on two numbers)
* Even/odd, positive/negative/zero checker
* Grade calculator using `if-else`/`switch`
* Sum/average of $n$ numbers using loops
* Factorial and Fibonacci using loops
* Largest/smallest of $n$ numbers using arrays
* Reverse an array
* Basic string operations: length, copy, compare without built-ins
* Swap two numbers with and without a third variable, and using pointers
* Simple function-based programs (e.g., check prime, check leap year)

### Star/Character Patterns
* Solid square, solid triangle (right-angled)
* Inverted triangle
* Pyramid (centered triangle)
* Diamond pattern

---

## 4. Transitioning to C++
* **Why C++ over C for CP**
  * STL availability, faster I/O, cleaner syntax
  * What "competitive programmers mostly write C++" actually means in practice
* **`cin`/`cout`**
  * Replacing `scanf`/`printf`
  * `cin >>`, `cout <<`, chaining
  * `endl` vs `"
"`
* **Namespaces**
  * `using namespace std;` - what it means and why it's used
* **References**
  * `&` as reference (vs pointer)
  * Pass by reference in functions
* **`std::string` (C++ class)**
  * Difference from C-style `char` arrays
  * Concatenation, comparison, `.length()`, `.substr()`
  * Why `string` replaces manual `char` array handling

---

## 5. Basic Class Concept
* **What a class is**
  * Grouping data (members/attributes) and behavior (member functions) together
  * Difference between a `struct` and a `class` (default access: `public` vs `private`)
* **Defining a simple class**
  * Member variables, member functions
  * `public`/`private` basics
* **Objects**
  * Creating an object, accessing members with `.`
* **Constructors (introductory)**
  * Default constructor concept
  * Initializing an object's data on creation

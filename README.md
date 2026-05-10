📘 Ham++ Language Guide
Welcome to Ham++! This is a simple, fast, and powerful scripting language designed for learning programming concepts and writing practical scripts. Below is a complete guide to getting started, syntax, and examples.

🚀 Quick Start
1. Installation & Compilation
Save the code in a file named hampp.cpp and compile it:

Bash


g++ hampp.cpp -o hampp -std=c++17
You can run it in two ways:

Interactive Mode:

Bash






./hampp
(Type exit to quit)

File Execution:

Bash






./hampp script.hampp
📝 Core Syntax & Commands
1. Variables
Use the var keyword to define variables. Ham++ automatically infers the type (number or string).

Hampp


var x = 10
var y = 3.5
var name = "Ham++"
2. Operators
Supports standard arithmetic and logical operators.

Type	Operator	Example	Description
Arithmetic	+, -, *, /, %	a + b	Add, Subtract, Multiply, Divide, Modulo
Comparison	==, !=, <, >, <=, >=	x > 5	Equal, Not Equal, Less Than, Greater Than
Logical	and, or, not	x > 0 and y < 10	AND, OR, NOT
3. Printing Output
Use the print command to display output to the console.

Hampp


var score = 100
print score
print "Your score: " + score  // Concatenation works
4. Control Flow
if and else Statements
Hampp


var age = 18

if (age >= 18) {
    print "You are an adult"
} else {
    print "You are a minor"
}
while Loops
Hampp


var i = 5
while (i > 0) {
    print i
    i = i - 1
}
// Output: 5, 4, 3, 2, 1
5. Functions
Define functions with parameters and return values.

Hampp


func add(a, b) {
    return a + b
}

func greet(name) {
    print "Hello " + name
}

var result = add(5, 10)
print result  // Output: 15

greet("Ali")
💡 Practical Examples
Example 1: Factorial (Recursion)
Hampp


func factorial(n) {
    if (n <= 1) {
        return 1
    }
    return n * factorial(n - 1)
}

print factorial(5)  // Output: 120
Example 2: Print Even Numbers
Hampp


var i = 1
while (i <= 20) {
    if (i % 2 == 0) {
        print i
    }
    i = i + 1
}
Example 3: Simple Number Guessing
Hampp


var secret = 7
var guess = 5

if (guess == secret) {
    print "Congratulations! You guessed it."
} else if (guess < secret) {
    print "The number is larger."
} else {
    print "The number is smaller."
}
⚠️ Important Notes & Limitations
Data Types: Ham++ currently supports Integers and Floats. Strings are supported for printing and concatenation but cannot be used in arithmetic operations.

Function Returns: Functions support return, but complex return value handling in nested loops is basic.

Error Handling: If you use an undefined variable or divide by zero, the program will stop with an error message.

Standard Library: Built-in libraries (advanced math, file I/O) are not yet included.

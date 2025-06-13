# COMPILER-DESIGN-BASICS

COMPANY : CODTECH IT SOLUTION

NAME : PRASHANT KUMAR SINGH

INTERN ID : CT04DF551

DOMAIN : C++ PROGRAMMING

DURATION : 4 WEEKS

MENTOR : NEELA SANTHOSH

 Task Overview – Task 4: Compiler Design Basics
👨‍💻 Internship Task Title:
Task-4: Compiler Design Basics

📝 Objective:
The objective of this task was to build a basic arithmetic expression parser and evaluator using C++. This task aims to simulate the core functionality of a simple compiler, particularly focusing on the expression evaluation phase, which includes lexical analysis, parsing, operator precedence, and expression evaluation.

As part of CodTech’s Internship Program, this task serves as an introduction to Compiler Design fundamentals and emphasizes how programming languages process arithmetic expressions during compilation.

🧠 Problem Statement:
Implement a simple compiler-like tool in C++ that:

Takes an arithmetic expression as input from the user (e.g., 3 + 4 * 2)

Parses the expression character by character

Handles operator precedence (* and / before + and -)

Evaluates and prints the correct result

The tool should also support multi-digit integers, whitespace handling, and ideally, parentheses for grouped operations.

🛠️ Approach and Methodology:
To solve this problem, we implemented an infix expression evaluator using the stack-based approach, which mimics how most real-world compilers handle expressions. Here are the key components of the solution:

Lexical Scanning: The input string is scanned character by character. If a number is encountered, the full number (possibly multi-digit) is extracted. Whitespace is ignored.

Parsing and Precedence Handling: Two stacks are used—one for operands (numbers) and one for operators (+, -, *, /, (, )). Operators are pushed based on their precedence. When a lower-precedence operator is encountered, the previous higher-precedence operators are applied first, respecting BODMAS rules.

Parentheses Support: Parentheses are parsed such that sub-expressions are evaluated first before integrating with the rest of the expression. This is essential for complex arithmetic logic and closely aligns with compiler design principles.

Evaluation: As operators and operands are processed from the stacks, the corresponding arithmetic operation is executed, and the result is pushed back to the value stack.

Error Handling: The enhanced version includes error checks for:

Invalid characters

Mismatched parentheses

Division by zero

Incomplete expressions

Modularity: The code is broken into reusable functions for precedence, applyOp, and evaluate, making the structure clean, readable, and scalable.

🔍 Sample Features:
Supports expressions like 3 + 4 * 2, (3 + 5) * (10 - 4), etc.

Handles spacing, multi-digit numbers, and nested brackets.

Reports invalid expressions with custom error messages.

Avoids division by zero by throwing exceptions.

👇 Sample Input & Output:
Input:
(3 + 5) * 2
Output:
Result = 16
Input:
10 / (5 - 5)
Output:
Error: Division by zero.
💡 Learnings & Skills Gained:
Through this task, I gained hands-on experience with:

Compiler expression parsing logic

Stack-based evaluation algorithms

Implementing BODMAS (operator precedence)

Error handling in parsing

Modular coding in C++

This task served as an excellent foundation to understand how expressions are parsed and evaluated inside a compiler, one of the core topics in Compiler Design.

OUTPUT

![Image](https://github.com/user-attachments/assets/98fcb5bd-68aa-42d8-8c7e-20511f36457a)


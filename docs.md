# AHLL Documentation

**Andy's Happy Little Language** - A whimsical programming language designed to make coding fun and happy!

## Table of Contents

1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [Variables](#variables)
4. [Lists and Collections](#lists-and-collections)
5. [Math Operations](#math-operations)
6. [Input and Output](#input-and-output)
7. [Conditionals](#conditionals)
8. [Functions (Concepts)](#functions-concepts)
9. [File I/O](#file-io)
10. [Shell Integration](#shell-integration)
11. [Advanced Features](#advanced-features)
12. [Complete Examples](#complete-examples)

---

## Introduction

AHLL (Andy's Happy Little Language) is a fun, whimsical programming language with English-like syntax. It features playful commands that make coding memorable and enjoyable.

### Features

- Whimsical syntax with memorable command names
- Variables, lists, math operations
- Input/output capabilities
- Conditionals and functions
- File I/O operations
- Shell command integration

---

## Getting Started

### Installation

```bash
# Option 1: Build Debian package
./builder
sudo dpkg -i ahll_1.0-1_all.deb

# Option 2: Manual installation
sudo cp usr/bin/ahll /usr/local/bin/
sudo cp usr/bin/bananacat /usr/local/bin/
sudo chmod +x /usr/local/bin/ahll /usr/local/bin/bananacat
```

### Running Programs

```bash
# Using ahll interpreter
ahll program.ahll

# Using bananacat wrapper (more fun!)
bananacat program.ahll
```

### File Extension

AHLL programs use the `.ahll` extension.

---

## Variables

Variables in AHLL are created in a three-step process using whimsical terminology.

### Creating Variables

```ahll
// Step 1: Create a classroom (namespace)
create_new_classroom_named_("my_vars")

// Step 2: Add a student (variable name) to the classroom
add_new_student_with_name_of_("x")_to_classroom_("my_vars")

// Step 3: Teach the student a value
teach_("x")_a_bit_of_(42)_from_classroom("my_vars")
```

### Accessing Variables

```ahll
// Use square brackets to access variable values
write_this([x])

// Variables in expressions
write_this([x + 10])
```

### Variable Types

AHLL supports various types:

```ahll
// String
create_new_classroom_named_("strings")
add_new_student_with_name_of_("greeting")_to_classroom_("strings")
teach_("greeting")_a_bit_of_("Hello, World!")_from_classroom("strings")
write_this([greeting])

// Number (integer)
create_new_classroom_named_("numbers")
add_new_student_with_name_of_("count")_to_classroom_("numbers")
teach_("count")_a_bit_of_(100)_from_classroom("numbers")
write_this([count])

// Boolean (stored as string)
create_new_classroom_named_("flags")
add_new_student_with_name_of_("is_ready")_to_classroom_("flags")
teach_("is_ready")_a_bit_of_("true")_from_classroom("flags")
```

### Example: Variable Demonstration

```ahll
write_this("=== Variables Demo ===")

create_new_classroom_named_("person_data")
add_new_student_with_name_of_("name")_to_classroom_("person_data")
add_new_student_with_name_of_("age")_to_classroom_("person_data")

teach_("name")_a_bit_of_("Alice")_from_classroom("person_data")
teach_("age")_a_bit_of_(25)_from_classroom("person_data")

write_this("Name: ")
write_this([name])
write_this("Age: ")
write_this([age])
```

**Output:**
```
=== Variables Demo ===
Name: 
Alice
Age: 
25
```

---

## Lists and Collections

Lists in AHLL are called "classrooms" and contain "students" (items).

### Creating Lists

```ahll
// Create an empty list
create_new_classroom_named_("my_list")
```

### Adding Items to Lists

```ahll
// Add individual items
add_new_student_with_name_of_("apple")_to_classroom_("my_list")
add_new_student_with_name_of_("banana")_to_classroom_("my_list")
add_new_student_with_name_of_("cherry")_to_classroom_("my_list")
```

### Accessing List Items

```ahll
// Access items directly by name
write_this([apple])
write_this([banana])
write_this([cherry])
```

### Removing Items from Lists

```ahll
// Remove a specific item from a list
nuke_notes_("banana")_from_classroom_("my_list")
```

### Deleting Entire Lists

```ahll
// Delete an entire list
nuke_list_("my_list")
```

### Example: List Operations

```ahll
write_this("=== Lists Demo ===")

create_new_classroom_named_("colors")
add_new_student_with_name_of_("red")_to_classroom_("colors")
add_new_student_with_name_of_("green")_to_classroom_("colors")
add_new_student_with_name_of_("blue")_to_classroom_("colors")

write_this("Colors in list:")
write_this([red])
write_this([green])
write_this([blue])

// Remove blue
nuke_notes_("blue")_from_classroom_("colors")

write_this("After removing blue:")
write_this([red])
write_this([green])
```

**Output:**
```
=== Lists Demo ===
Colors in list:
red
green
blue
After removing blue:
red
green
```

---

## Math Operations

AHLL supports standard mathematical operations using square bracket syntax.

### Basic Operations

```ahll
// Addition
write_this([1 + 1])

// Subtraction
write_this([10 - 5])

// Multiplication
write_this([2 * 3])

// Division
write_this([10 / 2])

// Complex expressions
write_this([2 * 3 + 4])
write_this([(10 - 5) / 2])
write_this([(5 + 3) * (10 - 2)])
```

### Math with Variables

```ahll
create_new_classroom_named_("math_vars")
add_new_student_with_name_of_("a")_to_classroom_("math_vars")
add_new_student_with_name_of_("b")_to_classroom_("math_vars")

teach_("a")_a_bit_of_(10)_from_classroom("math_vars")
teach_("b")_a_bit_of_(5)_from_classroom("math_vars")

write_this([a + b])
write_this([a * b])
write_this([a / b])
```

### Example: Math Demo

```ahll
write_this("=== Math Operations Demo ===")

write_this("1 + 1 = ")
write_this([1 + 1])

write_this("2 * 3 + 4 = ")
write_this([2 * 3 + 4])

write_this("(10 - 5) / 2 = ")
write_this([(10 - 5) / 2])

write_this("100 / 10 * 5 = ")
write_this([100 / 10 * 5])
```

**Output:**
```
=== Math Operations Demo ===
1 + 1 = 
2
2 * 3 + 4 = 
10
(10 - 5) / 2 = 
2.5
100 / 10 * 5 = 
50.0
```

---

## Input and Output

### Output (Printing)

```ahll
// Print a string message
write_this("Hello, World!")

// Print variable values
write_this([my_variable])

// Print expressions
write_this([10 + 5])
```

### Input (User Interaction)

```ahll
// Ask for user input (stores in [answer])
ask_this("What is your name? ")

// Use the answer
write_this("Nice to meet you, ")
write_this([answer])
```

### Example: Input/Output Demo

```ahll
write_this("=== Input/Output Demo ===")

ask_this("What's your name? ")
write_this("Hello, ")
write_this([answer])
write_this("!")

ask_this("How old are you? ")
write_this("You are ")
write_this([answer])
write_this(" years old.")
```

**Output:**
```
=== Input/Output Demo ===
What's your name? Alice
Hello, 
Alice
!
How old are you? 25
You are 
25
 years old.
```

---

## Conditionals

AHLL provides conditional statements for decision making.

### Basic Conditionals

```ahll
// Simple equality check
If_<("status")_is_("ready")>_then_do:
    write_this("Status is ready!")
```

### Negative Conditions

```ahll
// Check if something is NOT true
but if_<the_following_thing_is_not_true_lol_<("status")_is_("done")>>_do:
    write_this("Status is NOT done")
```

### Complete Conditional Example

```ahll
write_this("=== Conditionals Demo ===")

create_new_classroom_named_("test")
add_new_student_with_name_of_("status")_to_classroom_("test")
teach_("status")_a_bit_of_("ready")_from_classroom("test")

If_<("status")_is_("ready")>_then_do:
    write_this("Status is ready!")

but if_<the_following_thing_is_not_true_lol_<("status")_is_("done")>>_do:
    write_this("Status is NOT done")

// Test with different value
teach_("status")_a_bit_of_("done")_from_classroom("test")

If_<("status")_is_("done")>_then_do:
    write_this("Status is now done!")

but if_<the_following_thing_is_not_true_lol_<("status")_is_("ready")>>_do:
    write_this("Status is NOT ready")
```

**Output:**
```
=== Conditionals Demo ===
Status is ready!
Status is NOT done
Status is now done!
Status is NOT ready
```

### Nested Conditionals

```ahll
create_new_classroom_named_("nested")
add_new_student_with_name_of_("x")_to_classroom_("nested")
add_new_student_with_name_of_("y")_to_classroom_("nested")

teach_("x")_a_bit_of_(5)_from_classroom("nested")
teach_("y")_a_bit_of_(10)_from_classroom("nested")

If_<("x")_is_(5)>_then_do:
    If_<("y")_is_(10)>_then_do:
        write_this("Both x=5 and y=10!")
```

---

## Functions (Concepts)

Functions in AHLL are called "concepts" and are defined using indented blocks.

### Defining a Concept

```ahll
// Define a concept (function)
create_new_concept_("greet")
define_concept_("greet")_here:
    write_this("Hello from concept!")
    write_this("This is a function in AHLL")
```

### Calling a Concept

```ahll
// Concepts are called automatically when defined
// (In AHLL, concepts execute when reached)
```

### Example: Concept Demo

```ahll
write_this("=== Functions (Concepts) Demo ===")

create_new_concept_("say_hello")
define_concept_("say_hello")_here:
    write_this("Hello, World!")

create_new_concept_("add_numbers")
define_concept_("add_numbers")_here:
    write_this("Calculating 5 + 3 = ")
    write_this([5 + 3])

create_new_concept_("personal_greeting")
define_concept_("personal_greeting")_here:
    ask_this("What should I say? ")
    write_this([answer])
```

**Output:**
```
=== Functions (Concepts) Demo ===
Hello, World!
Calculating 5 + 3 = 
8
What should I say? Hello!
Hello!
```

### Concepts with Multiple Statements

```ahll
create_new_concept_("complex_task")
define_concept_("complex_task")_here:
    write_this("Starting complex task...")
    ask_this("Enter a number: ")
    write_this("You entered: ")
    write_this([answer])
    write_this("Task complete!")
```

---

## File I/O

AHLL supports basic file operations.

### Writing Data to Files

```ahll
// Create a list with data
create_new_classroom_named_("data_list")
add_new_student_with_name_of_("item1")_to_classroom_("data_list")
add_new_student_with_name_of_("item2")_to_classroom_("data_list")

// Save the list to a file
file_document_("data.txt")_as_("data_list")
```

### Deleting Files

```ahll
// Delete a file
burn_papers_("data.txt")
```

### Example: File I/O Demo

```ahll
write_this("=== File I/O Demo ===")

// Create data to save
create_new_classroom_named_("notes")
add_new_student_with_name_of_("note1")_to_classroom_("notes")
add_new_student_with_name_of_("note2")_to_classroom_("notes")
add_new_student_with_name_of_("note3")_to_classroom_("notes")

write_this("Saving notes to file...")

file_document_("my_notes.txt")_as_("notes")

write_this("Notes saved to my_notes.txt!")

// Later, you can delete the file
// burn_papers_("my_notes.txt")
```

**Output:**
```
=== File I/O Demo ===
Saving notes to file...
Notes saved to my_notes.txt!
```

### Reading Files

Note: AHLL currently focuses on writing data. For reading, you can use shell commands (see below).

---

## Shell Integration

AHLL can execute shell commands using the `use_cheating_` function.

### Running Shell Commands

```ahll
// List files in current directory
use_cheating_("ls -la")

// Show current directory
use_cheating_("pwd")

// Create a directory
use_cheating_("mkdir my_folder")

// Any shell command works
use_cheating_("echo 'Hello from shell!'")
```

### Example: Shell Integration Demo

```ahll
write_this("=== Shell Integration Demo ===")

write_this("Current directory:")
use_cheating_("pwd")

write_this("Listing files:")
use_cheating_("ls -la *.ahll")

write_this("Date and time:")
use_cheating_("date")
```

**Output:**
```
=== Shell Integration Demo ===
Current directory:
/home/user/projects/ahll
Listing files:
-rw-r--r-- 1 user user  456 Jan 15 10:30 example.ahll
-rw-r--r-- 1 user user  234 Jan 15 10:32 demo.ahll
Date and time:
Wed Jan 15 10:32:45 PST 2025
```

### Useful Shell Commands

```ahll
// Check Python version
use_cheating_("python3 --version")

// Show system info
use_cheating_("uname -a")

// Count lines in a file
use_cheating_("wc -l example.ahll")
```

---

## Advanced Features

### Happy Children Prison

A special list for uninitialized variables:

```ahll
write_this("=== Happy Children Prison Demo ===")

// Add variables without assigning values
add_new_student_with_name_of_("bob")_to_happy_children_prison_LOL
add_new_student_with_name_of_("alice")_to_happy_children_prison_LOL

write_this("Variables in Happy Children Prison:")
write_this([bob])
write_this([alice])
```

### Comments

Use `//` for single-line comments:

```ahll
// This is a comment
write_this("This is not a comment")  // This is also a comment
```

### Indentation

AHLL uses indentation to define blocks (for functions, conditionals):

```ahll
create_new_concept_("my_function")
define_concept_("my_function")_here:
    write_this("This is inside the function")
    write_this("So is this")

write_this("This is outside the function")
```

---

## Complete Examples

### Example 1: Interactive Calculator

```ahll
write_this("=== Interactive Calculator ===")

ask_this("Enter first number: ")
create_new_classroom_named_("calc")
add_new_student_with_name_of_("num1")_to_classroom_("calc")
teach_("num1")_a_bit_of_([answer])_from_classroom("calc")

ask_this("Enter second number: ")
add_new_student_with_name_of_("num2")_to_classroom_("calc")
teach_("num2")_a_bit_of_([answer])_from_classroom("calc")

write_this("Sum: ")
write_this([num1 + num2])

write_this("Product: ")
write_this([num1 * num2])
```

### Example 2: Todo List Manager

```ahll
write_this("=== Todo List Manager ===")

create_new_classroom_named_("todos")
add_new_student_with_name_of_("task1")_to_classroom_("todos")
add_new_student_with_name_of_("task2")_to_classroom_("todos")
add_new_student_with_name_of_("task3")_to_classroom_("todos")

teach_("task1")_a_bit_of_("Learn AHLL")_from_classroom("todos")
teach_("task2")_a_bit_of_("Build something")_from_classroom("todos")
teach_("task3")_a_bit_of_("Share with friends")_from_classroom("todos")

write_this("Your todo list:")
write_this([task1])
write_this([task2])
write_this([task3])

// Complete task2
nuke_notes_("task2")_from_classroom_("todos")

write_this("After completing task 2:")
write_this([task1])
write_this([task3])

// Save to file
file_document_("todo.txt")_as_("todos")
write_this("Todo list saved to todo.txt")
```

### Example 3: Guessing Game

```ahll
write_this("=== Guessing Game ===")

create_new_classroom_named_("game")
add_new_student_with_name_of_("secret")_to_classroom_("game")
teach_("secret")_a_bit_of_(7)_from_classroom("game")

ask_this("Guess a number between 1 and 10: ")
add_new_student_with_name_of_("guess")_to_classroom_("game")
teach_("guess")_a_bit_of_([answer])_from_classroom("game")

If_<("guess")_is_(7)>_then_do:
    write_this("You got it! The secret number is 7.")

but if_<the_following_thing_is_not_true_lol_<("guess")_is_(7)>>_do:
    write_this("Wrong! The secret number was 7.")
```

### Example 4: Data Processor with Shell Commands

```ahll
write_this("=== Data Processor ===")

create_new_classroom_named_("data")
add_new_student_with_name_of_("entry1")_to_classroom_("data")
add_new_student_with_name_of_("entry2")_to_classroom_("data")
add_new_student_with_name_of_("entry3")_to_classroom_("data")

teach_("entry1")_a_bit_of_("Apple: $1.50")_from_classroom("data")
teach_("entry2")_a_bit_of_("Banana: $0.75")_from_classroom("data")
teach_("entry3")_a_bit_of_("Cherry: $3.00")_from_classroom("data")

write_this("Processing data...")

// Use shell to show data file info
file_document_("data.csv")_as_("data")
use_cheating_("wc -l data.csv")
use_cheating_("cat data.csv")

write_this("Data processing complete!")
```

### Example 5: Complete Program

```ahll
write_this("=== Complete AHLL Program ===")
write_this("Welcome to Andy's Happy Little Language!")
write_this("")

// Variables
create_new_classroom_named_("user_info")
add_new_student_with_name_of_("username")_to_classroom_("user_info")
add_new_student_with_name_of_("user_age")_to_classroom_("user_info")

ask_this("What is your name? ")
teach_("username")_a_bit_of_([answer])_from_classroom("user_info")

ask_this("How old are you? ")
teach_("user_age")_a_bit_of_([answer])_from_classroom("user_info")

write_this("")
write_this("Hello, ")
write_this([username])
write_this("!")

// Simple age check
If_<("user_age")_is_("18")>_then_do:
    write_this("You just turned 18!")

but if_<the_following_thing_is_not_true_lol_<("user_age")_is_("18")>>_do:
    write_this("Nice to meet you at age ")
    write_this([user_age])

write_this("")
write_this("Thank you for trying AHLL!")
write_this("Goodbye from AHLL!")
```

**Sample Output:**
```
=== Complete AHLL Program ===
Welcome to Andy's Happy Little Language!

What is your name? Alice
How old are you? 25

Hello, 
Alice
!
Nice to meet you at age 
25

Thank you for trying AHLL!
Goodbye from AHLL!
```

---

## Quick Reference

| Feature | Syntax | Example |
|---------|--------|---------|
| Print | `write_this("text")` | `write_this("Hello!")` |
| Input | `ask_this("prompt")` | `ask_this("Name? ")` |
| Variable | `create_` + `add_` + `teach_` | See variables section |
| List | `create_new_classroom_named_` | `create_new_classroom_named_("my_list")` |
| Math | `[expression]` | `[1 + 2 * 3]` |
| If | `If_<()_is_()>>_then_do:` | `If_<("x")_is_(5)>_then_do:` |
| Not | `the_following_thing_is_not_true_lol_` | `the_following_thing_is_not_true_lol_<(...)>` |
| Function | `create_new_concept_` + `define_concept_` | See functions section |
| File Write | `file_document_("path")_as_("list")` | `file_document_("a.txt")_as_("data")` |
| File Delete | `burn_papers_("path")` | `burn_papers_("a.txt")` |
| Shell | `use_cheating_("command")` | `use_cheating_("ls")` |

---

## Tips and Best Practices

1. **Use descriptive names**: Choose meaningful names for your classrooms and students
2. **Comment your code**: Use `//` to explain complex logic
3. **Indent properly**: Use consistent indentation for functions and conditionals
4. **Test frequently**: Run your code often to catch errors early
5. **Have fun**: AHLL is designed to be whimsical and enjoyable!

---

## Troubleshooting

### Common Errors

1. **"File not found"**: Check that your `.ahll` file exists
2. **Syntax errors**: Ensure proper indentation and parentheses
3. **Variable not found**: Make sure you created the variable before using it
4. **Math errors**: Check for division by zero

### Getting Help

- Run `bananacat --help` for command options
- Check `example.ahll` for working examples
- Review this documentation for syntax references

---

## License

AHLL is licensed under the MIT License. See LICENSE file for details.

---

*"Make coding fun again!"* - andy64lol 🌻



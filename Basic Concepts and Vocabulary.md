## Programming Languages

#### What is a programming language?
- A programming language is a set of rules for giving instructions to a computer
- It provides the syntax for giving instructions and specifies the ways to store information, and it controls the order in which instructions are executed in a program

#### What is unique about Python?
- Python is a high-level programming language, which means it takes care of many low-level tasks for you so you can focus on solving problems
- For example, when you assign a value to a variable, Python deletes the variable automatically when it is no longer needed, sparing you from having to manage memory

#### How does a programming language affect how we think about solving problems?
- Every language has unique features that lead to characteristic programming styles and philosophies
- Python focuses on simplicity, readability, and getting the job done

## Operating Systems

#### What is an operating system?
- The operating system(OS) is the software that controls the computer's inner functionality

#### What does an operating system do?
- An operating system performs low-level functionality, such as reading from and writing to memory and interacts with hardware devices, like hard drives, RAM, CPU, graphics processors, displays, batteries, and other external devices 
- Major Operating Systems include Windows, macOS, and Linux (such as Ubuntu and Fedora)

#### How does Python interact with the operating system?
- Python is a cross-platform programming language
- The OS module, in Pythons standard utility modules, provides functions for interacting with the operating system by providing a portable way of using operating system-dependent functionality

## Terminal

#### What is a terminal?
- A terminal is a program that allows you to interact with the OS
- It is often referred to as the console or command line
- You use a terminal (rather than going through a GUI) to issue clear, concise, text-based commands to the OS to perform tasks quickly and efficiently

#### How do you run a Python program from a terminal?
- You can run a Python program from a terminal using a command like this:
```
# create a file - hello_world.py with your python code
$ python hello_world.py
```

#### How do you start a Python session from a terminal?
- In a Python terminal session, each line of code executes as soon as you enter it:
```
$ python
>>> print(“Hello, terminal world!”)
Hello, terminal world!
```
## Text Editors

#### What is a text editor?
- A text editor is a program designed for writing and editing code

#### What is syntax highlighting?
- Most text editors have features to make writing and editing code easier
- Syntax highlightings, for example, colours your code so you can quickly recognize different parts of a program – a string might be green, a method might be purple

#### What are some beginner-friendly text editors?
- Sublime Text, Atom, and Geany are some commonly used beginner-friendly text editors because of their ease of use and familiar interfaces
- They also have powerful features that help you work more efficiently

#### What are some more advanced text editors?
- Emacs and Vim are advanced text editors introduced in the 1970s
- Their learning curve is steep, but once you learn to use them well, writing and editing code is incredibly efficient
- Most Linux systems install Vim, or its predecessor vi, by default

## IDEs

#### What is an IDE?
- An integrated development environment is a text editor with powerful project management features

#### What are some typical features of IDEs?
- They include
     - debugging tools
     - auto-filing for certain code elements
     - ability to catch errors as you are entering code
- For projects that span multiple files, the IDE looks through the files and helps maintain consistency across the project
- IDES can make code testing easier and identify portions of your code that you could refactor
- IDEs help you interact with other project elements, such as HTML and JavaScript, in a web application and help you work with a database

#### What IDEs are best for Python?
- Popular Python IDEs include
    - PyCharm
    - PyDev
    - SPyder
    - Visual Studio

## Comments

#### What are comments?
- Comments are readable lines in a program that the compiler/interpreter ignores during execution
- They allow you to add notes about how the program works to help you and other developers understand the code
```
#This is a comment
print("Hello, World!")
```

#### Why are comments beneficial in programming?
- Document the functionality of a program, classes or functions
- To explain the role of variables when you introduce them
- Used to prevent execution of unwanted code
- How do you provide a solution for a problem after considering multiple approaches

#### What kinds of comments should you write?
- Writing comments will remind you of the code functionality when you return to it later
- Comments also help teams of programmers collaborate effectively

## Style Guide

#### What is a style guide?
- A style guide offers direction on creating consistency in your code, such as how far you indent lines, your maximum line length, or how you break lengthy lines

#### What kinds of recommendations are made in style guides?
- A style guide is not a set of rules: if you break the guidelines but follow the syntax rules, your code will still run
- When you follow a style guide, your code will be consistent, and it will be easier for you and others to focus on what it does rather than what it looks like

#### Where can you find the Python style guide?
- Pythons design ensures that programmers write more readable code with it than with other languages
- Be sure to read the Python style guide, PEP 8, for suggestions on how to create clean and consistent code

## Project Specifications

#### What is a project specification?
- A project specification, or spec, lists requirements for what a program needs to do

#### Why is a project specification important?
- Clear specifications are necessary for projects of all sizes to have a solid idea of what to aim toward and whether your project is successful
- Without a clear spec, you will waste time and risk the failure of your project
- A project specification indicates the problems that need solving and how users will interact with the program
- It should specify what kinds of inputs your program will deal with, as well as the outputs the program needs to generate

#### Who writes project specifications?
- When learning to program, each exercise you attempt is a mini spec
- Well-specified problems are more manageable to solve than poorly specified exercises
- A good programmer looks for a spec when collaborating on an existing project and develops a full spec before committing to a new project

## Syntax

#### What is syntax?
- It is a set of rules for how to write instructions in that language
- Syntax for code is akin to grammar for a language
- The syntax rules tell you how to store data, respond to specific conditions, and control the flow of execution in the language

#### What is a syntax error?
- A syntax error occurs when a program does not follow the syntax rules
- The language does not understand how to execute the code, even if only a minor mistake like a missing parentheses or comma

#### What is a logical error?
- A logical error occurs when your program follows the syntax rules and runs but does not do what you want it to do
- You will know you have a logical error when your project generates output, but it does not match the project spec
- You will need to reevaluate your approach to the program and then modify that approach

## Debugging

#### What is a bug?
- A bug is a program in the way a program runs
- Debugging is the process of identifying the cause of a bug and modifying code to fix the issue

#### What does debugging mean?
- One of the first steps in debugging is to understand error messages
- They tell you where the interpreter had a problem and what kind of problem occurred

#### How do you debug a program?
- Logical errors do not result in error messages, so you need to look at the program execution to resolve them
- To debug logical errors, examine the value of variables at different points during the program execution
- Do this by inserting print() calls into the code at strategic points, logging the values of vital variables during execution, or using the debugging tools available in most IDEs
- Also, write tests for your code to see which parts are working and which are not

## Refactoring 

#### What is refactoring?
- Refactoring is the process of rewriting parts of a working program to make it simpler, more efficient, and easier to work with

#### When and why should you refactor code?
- Consider refactoring code when you’ve solved the same problem in multiple places
- This approach follows the don’t repeat yourself, or DRY,  principle
- Code repetition presents opportunities for errors, makes programs harder to modify, and makes programs longer and harder to read

#### What is the DRY principle?
- The DRY principle is stated as "Every piece of knowledge must have a single, unambiguous, authoritative representation within a system"
- When the DRY principle is applied successfully, a modification of any single element of a system does not require a change in other logically unrelated elements

#### How do you refactor code?
- To refactor code, place a repeated block of code into a separate function
- Then replace the repeated code with a function call
- When you need to improve that code, you only need to change the code in the function for it to work throughout the program
- Refactoring can help you find more efficient ways to solve problems, and separating code into different modules makes it easier to work with

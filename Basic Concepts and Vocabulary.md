## Programming Languages

#### What is a programming language?
- A programming language is a set of rules for giving instructions to a computer
- It provides the syntax for giving instructions and specifies the ways to store information
- It controls the execution order of a program

#### What is unique about Python?
- Python is a high-level programming language, which means it takes care of many low-level tasks for you so you can focus on solving problems
- For example, when you assign a value to a variable, Python deletes the variable automatically when it is no longer needed, sparing you from having to manage memory

#### How does a programming language affect how we think about solving problems?
- Every language has unique features that lead to characteristic programming styles and philosophies
- Python focuses on simplicity, readability, and getting the job done

## Operating Systems

#### What is an operating system?
- The operating system(OS) is the software that controls the inner functionality of a computer

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
- Consider refactoring code when you have solved the same problem in multiple places
- This approach follows the do not repeat yourself (DRY)  principle
- Code repetition presents opportunities for errors, makes programs harder to modify, and makes programs longer and harder to read

#### What is the DRY principle?
- The DRY principle is stated as - every piece of knowledge must have a single, unambiguous, authoritative representation within a system
- When the DRY principle is applied successfully, a modification of any single element of a system does not require a change in other logically unrelated elements

#### How do you refactor code?
- To refactor code, place a repeated block of code into a separate function, then replace the repeated code with a function call
- When you need to improve that code, you only need to change the code in the function for it to work throughout the program
- Refactoring can help you find more efficient ways to solve problems, and separating code into different modules makes it easier to work with

## Modules

#### What is a module?
- In python, a module is a file that contains code
- Modules are used to break up large programs into smaller parts for more manageable coding

#### Why are modules important?
- Modules compartmentalize complex programs
- Programmers break up larger projects into different files, each of which focuses on one aspect of the project
- his makes large projects easier to write and collaborate on in teams: each programmer can focus on only the modules they’re responsible for

#### How do you use a module in a program?
- To create a module, you move code that has a particular aim into a separate file
- To use a module, import it into the file you’re working on to make the code available
- You can import the entire module or just the parts you need


## Standard Library

#### What is a standard library?
- A standard library is the set of tools included in any language standard installation
- It comprises core data structures and tools for working with data in your program

#### What constitutes a standard library?
- Python standard library encloses the following tools:
     - Working with a variety of data types and text
     - Mathematical functions
     - Work with files and dates and times
     - Make graphical user interfaces (GUIs)
     - Work with networks and multimedia
     - Test and debug your code and handle errors
     - Distribute your programs

#### What is not a part of a standard library?
- Seldom does a standard library include specialized data analysis tools, game frameworks, web application frameworks, and other application-specific libraries 
- These are available through external libraries that are updated more often than the language as a whole
- Once you understand a languages core syntax and rules become familiar with the language standard library tools, these can help you write code efficiently

## Thrid-party Libraries

#### What is a third-party library?
- A third-party library provides additional functionality not covered by a language standard library

#### What is a package?
- To understand Python packages, we will briefly look at scripts and modules 
    - A script is something you execute in the shell to accomplish a defined task 
    - To write a script, you would type your code into your favourite text editor and save it with the .py extension 
    - You can then use the python command in a terminal to execute your script
- A module is a Python program that you import, either in interactive mode or into your other programs 
    - It is an umbrella term for reusable code
    - A Python package usually consists of several modules 
    - Physically, a package is a folder containing modules and maybe other folders that themselves may have more folders and modules
    - Conceptually, it is a namespace
    - Package modules can be referenced by a package name that they are bound by

#### What is a package manager?
- Package Managers are tools that help you manage the dependencies for your project
- A dependency is code that is required for your program to function as required that often are in the form of packages

#### What kinds of third-party libraries are available for Python?
- Third-party libraries, or packages, are installed through an automated package manager, such as pip,  for consistent and secure installation
- A package manager also helps keep the libraries you have installed up-to-date
- More than 100,000 packages are available through the Python package manager
- For example, the requests package helps you write programs to access online resources, Pillow helps to work with images, SQLAlchemy makes it easier to work with databases, and Numpy offers tools for working with numerical data

## Frameworks 

#### What is a framework?
- A framework is a larger package that helps solve a particular problem
- Some frameworks help you build games, data visualizations, and web applications
- A framework includes tools that handle common tasks within a problem area
- For example, a game framework often provides a way to determine when a collision between two game elements has occurred
- A web application framework usually provides a way to extract information from a database
- Simple frameworks leave it to you to make many problem-solving decisions; larger frameworks have more default approaches to common situations

#### What kinds of frameworks are available for Python?
- Popular python web frameworks include Django, a large framework that provides tools to build web applications, and Flask, a bare-bones web application framework that leaves many decisions up to you
- Popular game frameworks include Pygame, Kivy, and Piglet

## Error Handling

#### What is error handling?
- Error handling refers to writing code that anticipates errors that are likely to occur and then responds to those errors

#### Why is error handling important?
- To run successfully, a program needs the correct set of inputs and the ability to do its work, and it must return its output appropriately
- Errors can happen during any of these stages
- Well-written programs have error-handling code that anticipates and deals with errors that might occur at each stage
- Error handling can just be code that checks certain values and conditions before proceeding
- If the values and conditions are appropriate, execution continues along one path
- If not, it follows a different path

#### How do you handle errors in a program?
- One common approach is to check whether the input is in the correct format
- When a user inputs their age, you expect a positive number
- You can add code to check for a positive number before continuing and then raise an exception if anything else is entered

#### What is an exception?
- An exception is a special error condition that responds to a specific kind of error

## Version Control 

#### What is version control?
- Version control is the process of saving different versions of your project as it evolves
- If you break a program, you can return to a previously working version, or you can simply examine how your program worked in a previous version

#### What is a commit?
- Version control systems work by allowing you to make a commit, which saves the current state of all the files in your project
- You can make a commit after implementing a new feature

#### What does it mean to “check out” a commit?
- If you make a mistake and can’t figure out how to fix your program, you can check out the previous commit and start again from a working version of your project

#### What is a repository?
- A repository is the collection of all commits you’ve made to a project; it contains other resources required to manage your project as well

#### Why is version control important?
- Version control is important to keep track of changes — and keep every team member working on the right version
- You should use version control software for all code, files, and assets that multiple team members will collaborate on

#### What is distributed version control?
- A distributed version control system allows multiple people to make commits on the same project and provides tools for resolving conflicts in collaborative projects
- Git and Mercurial are the most common version control systems at the time of this writing

## Testing 

#### What is a test?
- A test is code outside your program that runs some of your program code to check whether it works correctly

#### How do you write a test?
- Each part of a program solves one aspect of a larger problem your problem aims to solve
- You can write tests that prove each part of your code behaves properly
- To write a test, you import the code you want to test, set up sample data, and run the code using that data
- Then you can make assertions about the results

#### What is an assertion?
- An assertion is a statement about what a value or condition should be
- For example, you might assert that the value of the variable age is greater than 18
- If the code acts as it should, the test passes
- If it doesn’t, the test fails
```
def test_sum():
    assert sum([10, 20, 70]) == 100, "Should be 100"

test_sum()
print("sum = 100")     # will print sum = 100 only if the assert statement in test_sum() passes
```

#### How do tests help you add new features to a project?
- A good set of tests helps you find bugs before your users do
- It also helps ensure that when you add new features to your projects, the code doesn’t affect the behaviour of existing features and your program still works

## User Interfaces 

#### What is an application programming interface?
- An application programming interface (API) is a specification for how one program asks another program for information

#### What is a graphical programming interface?
- A graphical user interface (GUI) is an easy-to-use interface that lets users click elements on the screen

#### What is a command programming interface?
- A command-line interface (CLI) allows users to interact with a program by entering commands in a terminal

#### Why is each of these important?
- Using GUI is the simplest way for non-technical users to interact with a program
- For example, a weather website would present information in a browser (a GUI) for general users, but it might also provide an API that technical users can work with to build projects that use real-time weather data
- APIs allow you to pull in data from external resources
- Developers working on large, collaborative projects can build their APIs to design how each program in the project communicates
- Designing and building a good API requires experience and planning, but learning to use an API is much simpler
- A CLI enables automation and scripting in a more customizable fashion than with GUIs


## Databases

#### What is a database?
- A database is a program that allows you to store and retrieve information
- Good databases are highly optimized to do this efficiently and reliably with large amounts of data

#### Why are databases important?
- Databases store the application information
- Retrieving information from a website or posting on a website means that information is being read from or written to a database
- Many of the programmers working on a project interact with a database

#### What is SQL? How do you communicate with a database?
- Structured Query Language (SQL) is a language written to interact with databases, but you don’t need to know SQL to work with a database
- Many languages and frameworks generate SQL for you so you can work with the database through those languages
- The application server can communicate only through the intermediary of a database driver (SQL)
- A database driver is software that acts as an interpreter between the application server and the database
- After the driver establishes communication, the query is executed against the database and a recordset is created

#### What are some common databases?
- These are the most common databases used in programming
     - SQLite
     - PostgreSQL
     - MySQL
     - SQL Serve
     - Oracle 

## Data Structures and Types 

#### What are data structures?
- Data structures define how you store and organize data efficiently in any programming language
- Every programming language has a core set of data structures
- They allow you to access and perform operations on the data

#### What are data types?
- Data types refer to the data structures you are using or the kind of information stored in those data structures
- The most common data types include
     - int
     - float
     - complex
     - str

#### Why are data structures important?
- Much of programming focuses on handling data
- How much you represent data through code impacts what you can do with the data - if you model your data well, your program is easier to work with
- Choosing a specific approach to data modelling portrays how you think about data, so knowing the available data structures in a programming language will help you best represent the information in your project

#### What are the most common kinds of data structures?
- Data structures offer different ways of storing data based on our requirements
     - Mutability
          - It refers to the ability to change an object after its creation
          - Mutable objects can be modified, added, or deleted after they’ve been created
          - Immutable objects cannot be modified after their creation
     - Access requirements
          - It relates to whether we require the position of an element to access the element
- The most common data structures include
     - Lists
     - Dictionaries 
     - Sets
     - Tuples

## Variables 

#### What is a variable?
- A variable is a name attached to a piece of data
- Simply put, it is a container to store data
- First define a variable, then use that name when you refer to that piece of data
- They reserve some space in memory to store data and can hold a small piece of information, or it can hold many gigabytes of data
```
# int data type 
age = 24  

# float data type 
distance   = 20.86  

# string data type
emp_one    = "John Doe"  
emp_two = 'Jane Doe'

# Python variables support multiple assignments
a = b = c = 24
print(a)      # 24
a, b = 12, 24
print(a, b)   # 12 24
``` 

#### What are the rules for naming a variable?
- Variable names in python follow two main rules:
     - They must contain only letters, underscores, and numbers
     - They must start with a letter or underscore
- Good variable names are short but descriptive:
```
First_name = ‘albert’
Last_name = ‘einstein’
Username = ‘einsteina’
Age = 42
```

#### Why are variables important?
- Variables are crucial because they help to measure concepts in a study
- Used to retrieve data throughout the program without having the remember the value of the data stored
- Used to perform, store and reuse the outputs of operations
- They improve code readability 

#### What is a statistically typed language?
- In statistically typed languages, you must declare the kind of data a variable represents when you define it
- Status languages prioritize processor efficiency over a programmer's time
- Programs are longer and more verbose in status languages but can be highly optimized
- Type-checking is done during compile-time

#### What is a dynamically typed language?
- In a dynamically typed language, you do not have to declare the kind of data a variable will represent
- Dynamic languages prioritize a programmer's time over efficient use of the processor, but they can still be fast and efficient when used properly
- Type-checking is done during run-time

#### What makes Python a dynamic language?
- In Python, the interpreter examines the data associated with the variable throughout the life of the program and manages type issues for you
```
# declaring a string variable
name = 'Jane'
type(name)      # str

# reassigning a boolean value to 'name'
name = True
## reassigning a value to the 'x'
type(name)      # bool
```

## Saving State

#### What is a program’s state?
- The state of a program is the set of values of all the variables at a given moment
- Saving state refers to saving these values so they can be recovered if the program crashes or the user closes it

#### What is the JSON format? Why is JSON used to save a state?
- A common way to save a program’s state is to write the current values to a JSON file
- JSON (JavaScript Object Notation) is a way of storing data that’s easy for programs to read back
- Originally developed for use in JavaScript programs, JSON is now used by many programming languages
- The JSON format can be read by programs and by humans
- Some simple JSON data files look just like Python code
- Python has libraries you can use to simplify reading and writing JSON files

# Python Basics

## [Data Types in Python](https://github.com/DasikaMadhu/WQU-ADSL-Notes/blob/main/Basic%20Concepts%20and%20Vocabulary.md#data-structures-and-types)
| Type          | Second Header |
| ------------- | ------------- |
| Text          | str           |
| Numeric       | int, float    |
| Sequence      | list, tuple   |
| Mapping       | dict          |
| Set           | set           |
| Boolean       | bool          |

**1. Text Data Types**
   - ### str
     - **What is a string?**
         - Strings are a ordered sequence of characters that are enclosed within 'single' or "double" quotes 
         - There is no limit on the length of a string
     - **How do you store a string in a variable?**
         - In this example, “I love Python!” is a string assigned to the variable message:
            ```
            message = “I Love Python!”
	         print(message)                  # prints - I Love Python!
            
            my_string = 'Hello, world!'      # prints Hello, world!
            print(my_string)
            
            print("Okay, see you again.")    # prints Okay, see you again.

            ```
         - Strings support being encased by single and double quotes, so you can use nested quotes to print strings with quotes
           ```
           python_quote = ‘ I said, “I love Python!” ’
           print(python_quote)              # prints I said, “I love Python!”
           ```
     - **How do you include tabs and newlines in a string?**
         - Insert tabs and newlines into strings using the special sequences \t and \
           ```
           message = “Grocery list:\n\tmilk\n\teggs”
           print(message)
           # prints Grocery list:
	        #          milk
	        #          eggs
           ```
     - **What is a string method?**
         - A string method is a function that performs an action on a string
         - They are useful for presenting data in a certain format or cleaning up user-submitted data
     - **How do you change the case of a string?**
         - To change the case of a string, use the methods **title()**, **upper()**, and **lower()**
           ```
           name = ‘ella fitzgerald’
           name.title()              # ‘Ella Fitzgerald’
           name.upper()              # ‘ELLA FITZGERALD’
           name.lower()              # ‘ella fitzgerald’
           ```
     - **How do you strip whitespace from a string?**
         - The **lstrip()**, **rstrip()**, and **strip()** methods remove extra whitespace from strings, helpful for cleaning up date:
            ```
           name = ‘  jordan  ‘
           name.lstrip()              # ‘jordan  ‘
           name.rstrip()              # ‘   jordan’
           name.strip()               # ‘jordan’
           ```
     - **How to check if a variable is of type string?**
         - Using the **type()** with the string variable name as a parameter returns the type 'str'
           ```
           var = 'This is a string'
           type(var)                  # str 
           ```
     - **How to check the length of a string?**
         - Using the **len()** with the string variable name as a parameter returns the length of the string
           ```
           var = 'This is a string'
           len(var)                   # 16  
           ```
     - **How to index and slice a string?**
         -  Indexing a string allows accessing individual characters in a string directly by using a numeric value
         -  String indexing is zero-based: the first character in the string has index 0, the next is 1, and so on
         -  Strings supoort negative indexing
            ```
            my_string = 'new string'
            my_string[0]                  # 'n'
            my_string[1]                  # 'e'
            my_string[4]                  # ' '
            my_string[-1]                 # 'g'
            my_string[-4]                 # 'r'
            ```
         -  
**2. Numeric Data Types**
   - int
   - float

**3. Sequence Data Types**
   - list
   - tuple

**4. Mapping Data Type**
   - dict

**5. Boolean Data Type**
   - bool

## Conditional Statements
   

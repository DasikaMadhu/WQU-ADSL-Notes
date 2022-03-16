# Python Basics

## [Data Types in Python](https://github.com/DasikaMadhu/WQU-ADSL-Notes/blob/main/Basic%20Concepts%20and%20Vocabulary.md#data-structures-and-types)
| Type          | Second Header |
| ------------- | ------------- |
| Text          | [str](https://github.com/DasikaMadhu/WQU-ADSL-Notes/blob/main/Python%20Basics.md#str)           |
| Numeric       | int, float    |
| Sequence      | list, tuple, complex   |
| Mapping       | dict          |
| Set           | set           |
| Boolean       | bool          |

**1. Text Data Types**
   - ### str
     - **What is a string?**
         - Strings are an ordered sequence of characters that are enclosed within 'single' or "double" quotes 
         - There is no limit on the length of a string
     - **How do you store a string in a variable?**
         - In this example, “I love Python!” is a string assigned to the variable message:
            ```
            message = “I Love Python!”
	         print(message)                  # prints - I Love Python!
            
            my_string = 'Hello, world!'      # prints Hello, world!
            print(my_string)
            
            print("Okay, see you again.")    # prints Okay, see you again.
	    
	       # multi-line string
	       print("""This is line one.
	                 This is in line two!
                     Is this line three?
		     """)                         # prints This is line one.
	                                              This is in line two!
                                                  Is this line three?
					      
		   print('''This is line one.
		             This is in line two!
			         Is this line three?
			     ''')                    # prints This is line one.
	                                              This is in line two!
                                                  Is this line three?
            ```
         - Strings support being encased by single and double quotes, so you can use nested quotes to print strings with quotes
           ```
           python_quote = ‘ I said, “I love Python!” ’
           print(python_quote)              # prints I said, “I love Python!”
           ```
     - **How do you include tabs and newlines in a string?**
         - Insert tabs and newlines into strings using the special sequences \t and \n
         - These are called escape characters
         - Common escape characters include 
   			| Escape Character  | Use                        |
 			|-------------|----------------------------------|
			| \'          | single quote                     |
			| \\          | backslash                        |
			| \n          | new line                         |
			| \r          | carriage return                  |
			| \t          | tab                              |
			| \b          | backspace                        |
			| \f          | form feed                        |
			| \ooo        | octal values                     |
			| \xhh        | hexadecimal values               |			
           ```
           message = “Grocery list:\n\tmilk\n\teggs”
           print(message)
           # prints Grocery list:
	        #          milk
	        #          eggs
           ```
     - **What is a string method?**
         - A string method is a function that acts on a string
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
         -  Python supports negative indexing
            ```
            my_string = 'new string'
            my_string[0]                  # 'n'
            my_string[1]                  # 'e'
            my_string[4]                  # ' '
            my_string[-1]                 # 'g'
            my_string[-4]                 # 'r'
            ```
        -  String slicing is the process of extracting substrings from the main string
        -  Python supports negative slicing
           ```
	       # string slicing syntax - string_name[start : stop : step]
	       
	       my_string = 'This is a string'
	       my_string[:2]                        # 'Th'
	       my_string[:6]                        # 'This i'
	       my_string[2:]                        # 'is is a string'
	       my_string[4:len(s)]                  # ' is a string'
	       my_string[:2] + s[2:]                # 'This is a string'
	       my_string[:]                         # 'This is a string'
	       my_string[-8:-1]                     # 'a strin'
	       my_string[:-1]                       # 'This is a strin'
	       my_string[::-1]                      # 'gnirts a si sihT'
	       my_string[::-5]                      # 'gsiT'
	       my_string[:3:-2]                     # 'git  i'
	       my_string[2::2]                      # 'i sasrn'
	       ```
      -  **How to replace strings with other strings?**
         - Using the **replace()** method helps you replace a string with another string
            ```
            my_string = "Hello, World!"
	       my_string.replace("H", "J")          # 'Jello, World!'
            ```    
      -  **How to split strings?**
         - Using the **split()** method splits the string into substrings
         - You can assign the split parts to other strings
            ```
            my_string = "Hello, World!"
	       my_string.split(","))                                    # ['Hello', ' World!']
	       
	       my_string = "Hi, these are my Python notes!"
	       first_string, second_string = my_string.split(", ")
	       first_string                                             # Hi
	       second_string                                            # these are my Python notes!
            ```  
         - Using the **splitlines()** method splits a string into a list
            ```
	            my_string = "Thank you for perusing my notes. Feel free to check out the rest."
                print(my_string.splitlines())                          # ['Thank you for perusing my notes. Feel free to check out the rest.']
	       ```
      -  **How to count the occurrence of specific characters in a string?**
         - Using the **count()** method returns the first occurrence of the specified value
            ```
	       # string count syntax - string.count(value, start, end)
	       my_string = "Hi, these are my Python notes!"
	       my_string.count("Python")
	       my_string.count("n")
	       my_string.count("n",0,10)
            ```    	
      -  **What is the difference between index() and find()?**
         - The **index()** and **find()** methods both return the first occurrence of the specified value
         - However, the find() method returns -1 if the value is not found
         - The index() method  raises an exception if the value is not found
            ```
	       # string index syntax - string.index(value, start, end)
            my_string = "Hi, these are my Python notes!"
	       my_string.index("a")                # 10
	       my_string.index("!")                # 2
	       my_string.index("!")                # 29
	       my_string.index("x")                # ValueError: substring not found
	       my_string.find("x")                 # -1
            ```
      -  **How to partition a string?**
         - Using the **partition()** method searches for a specified string, and splits the string into a tuple containing three elements
            ```
	       # string index syntax - string.index(value, start, end) 
	       my_string = "Hi, these are my Python notes!"
	       my_string.partition("Python")            # ('Hi, these are my ', 'Python', ' notes!')
	       my_string.partition("n")                 # ('Hi, these are my Pytho', 'n', ' notes!')
	       my_string.partition("notes")             # ('Hi, these are my Python ', 'notes', '!')
            ```
      -  **What is string concatenation?**
         - String concatenation appends two strings together
         - It binds a number of string variables together, creating one string from two or more individual strings
            ```
	       string_one = "Hello, "
	       string_two = "world!"
	       my_string =  string_one + string_two           # Hello, world!
	       
	       string_one = "Okay,"
	       string_two = "bye!"
	       my_string =  string_one + " " + string_two     # Okay, bye!
            ```
      -  **What is string interpolation?**
         - Inject a variable into your string for printing
         - Substitute values of variables into placeholders in a string
         - String interpolation can be done in three ways
         	+ using placeholders % 
         	        - A placeholder can interpolate different types of data into a string literal
         	        - Placeholders can be any one of the following -
				| Placeholder | Data Type                        |
				|-------------|----------------------------------|
				| %d or %i    | integer                          |
				| %f          | float                            |
				| %e          | exponential                      |
				| %s          | string                           |
				| %c          | single character                 |
				| %g          | rounded off version of %f and %e |
				| %r          | raw data                         |
				| %o          | octal                            |
				| %x          | hexadecimal                      |        	       
         	+ .format()
           		- A placeholder {} is used to interpolate data into a string literal based on their index position
         	+ f-strings 
         	 	- They are formatted string literals provide the option to format strings with minimal code
         	 	- Require Python 3.6 or higher
         	 	- They are faster than the above two options
            ```
	       # regular string interpolation
	       string_name = "John"
	       print("Hello, " + string_name)                                # Hello John
	       
	       # using placeholders - print("String literal %format-specifier-placeholder" % "variable list")
	       print("Hello, %s" % "Jane")                                   # Hello Jane 
	       print("Hello %s, you are at %s" % ("Jane", "work"))           # Hello Jane, you are at work
	       print("Hello %s, you are %d years old" % ("Jane",24))         # Hello Jane, you are 24 years old
	       
	       # using .format()
	       print('String format - {}'.format('one'))                                           # String format - one
	       print('String format - {} {} {}'.format('part 1','part 2','part 3'))                # String format - part 1 part 2 part 3
	       print('the {} {} {}'.format('fox','quick','brown'))                                 # the fox quick brown
	       print('the {1} {2} {0}'.format('fox','quick','brown'))                              # the quick brown fox
	       print('the {1} {1} {1}'.format('fox','quick','brown'))                              # the quick quick quick
	       print('the {q} {b} {f}'.format(f='fox',q='quick',b='brown'))                        # the quick brown fox
	       print("result = {r}".format(r=result))                                              # result = 0.1287001287001287
	       print("result = {r:1.3f}".format(r=result))                                         # result = 0.129
	       print("result = {r:10.3f}".format(r=result))                                        # result =      0.129
	       print("Hello, my name is {n}. My age is {a}.".format(n="Jane",a=52))                # Hello, my name is Jane. My age is 52.	
	       
	       # using f-strings
	       name_one="Dave"
	       name_two="Alex"
	       print("These are my brothers %s and %s" %(name_one,name_two))                       # These are my brothers Dave and Alex
	       print(f"{name_one!r} is a python developer")                                        # 'Dave' is a python developer
            ```
      -  **How can we check if a certain character is present or not in a string?**
         - Using the **'if "character" in my_string'** or **'if "character" not in my_string'** searches for the presence of the required character in a string
         - If the character is present, **'"character" in my_string'** returns a True boolean value
         - If the character is present, **'"character" not in my_string'** returns a False boolean value
           ```
	       my_string = "Learning is free!"
	       
	       if "free" in my_string: 
           print(my_string)                                             # Learning is free!
			       
	       if "free" not in my_string: 
           print("Required character is not present")                   # Required character is not present
	   
           print("free" in my_string)                                   # True           

           print("expensive" in my_string)                              # False
 
           print("free" not in my_string)                               # False

           print("expensive" not in my_string)                          # True 
     	   ``` 

[:arrow_up:](https://github.com/DasikaMadhu/WQU-ADSL-Notes/blob/main/Python%20Basics.md#python-basics)
<hr>

**2. Numeric Data Types**
   - ### int
     - **What is an int?**
         - An integer, or int, is a whole number, positive or negative, without decimals, of unlimited length
         - There is no limit on the length of a string

[:arrow_up:](https://github.com/DasikaMadhu/WQU-ADSL-Notes/blob/main/Python%20Basics.md#python-basics)
<hr>

   - ### float
     - **What is a float?**
         - Strings are an ordered sequence of characters that are enclosed within 'single' or "double" quotes 
         - There is no limit on the length of a string

[:arrow_up:](https://github.com/DasikaMadhu/WQU-ADSL-Notes/blob/main/Python%20Basics.md#python-basics)
<hr>

   - ### complex
     - **What is a complex?**
         - Strings are an ordered sequence of characters that are enclosed within 'single' or "double" quotes 
         - There is no limit on the length of a string

[:arrow_up:](https://github.com/DasikaMadhu/WQU-ADSL-Notes/blob/main/Python%20Basics.md#python-basics)
<hr>

**3. Sequence Data Types**
   - ### list
     - **What is a list?**


[:arrow_up:](https://github.com/DasikaMadhu/WQU-ADSL-Notes/blob/main/Python%20Basics.md#python-basics)
<hr>

   - ### complex
     - **What is a tuple?**
         - 

[:arrow_up:](https://github.com/DasikaMadhu/WQU-ADSL-Notes/blob/main/Python%20Basics.md#python-basics)
<hr>

**4. Mapping Data Type**
   - ### dict
     - **What is a dict?**
         - 

[:arrow_up:](https://github.com/DasikaMadhu/WQU-ADSL-Notes/blob/main/Python%20Basics.md#python-basics)
<hr>

**5. Boolean Data Type**
   - ### bool
     - **What is a bool?**
         - 


[:arrow_up:](https://github.com/DasikaMadhu/WQU-ADSL-Notes/blob/main/Python%20Basics.md#python-basics)
<hr>

## Conditional Statements

   
[:arrow_up:](https://github.com/DasikaMadhu/WQU-ADSL-Notes/blob/main/Python%20Basics.md#python-basics)
<hr>
 			

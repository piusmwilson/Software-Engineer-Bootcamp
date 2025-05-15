# PYTHON PROGRAMMING LANGUAGE

A high-level interpreted programming language, known for its simplicity and readability, that works on many platforms that is used to develop various desktop and mobile applications, websites, and software interfaces. It emphasizes code readability and encourages a clean and concise coding style.

## Table of Contents

- [Python Learning Roadmap](#python-learning-roadmap)
- [Introduction](#introduction)
- [The Key Features of Python](#the-key-features-of-python)
- [Pep 8](#pep-8)
- [Python Datatypes](#python-datatypes)
- [Typecasting](#typecasting)
  - [What is Python Type Casting](#what-is-python-type-casting)
    - [Implicit and Explicit Python Type Casting](#implicit-and-explicit-python-type-casting)
- [Python Developer](#python-developer)
  - [Technical skills needed to become a competent Python developer](#technical-skills-needed-to-become-a-competent-python-developer-)
- [Object Oriented Python](#object-oriented-python)
- [Python Libraries](#python-libraries)
- [Python Frameworks](#python-frameworks)
- [Conclusion](#conclusion)
- [References](#references)
- [Keywords](#keywords)


## Python Learning Roadmap

### package managers

- pip
- conda
- PyPI

### Basics

- basic Syntax
- variables
- data types
- conditionals
- Typecasting
- functions
- loops
- exceptions
- lists, tuples, sets
- Dictionaries

### Advanced

- List & Comprehensions
- Generators
- Expressions
- Paradigms
- Regex
- Decorators
- Iterators
- Lambdas
- Functional Programming
- Map, reduce, filters
- Threading

### Web Frameworks

- Flask
- FastAPI
- Django
- Tornado

### OOP

- Classes
- Inheritence
- Methods (_Including Dunder Methods_)

### Data Science

- NumbPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow
- PyTorch

### Testing

- Unit Testing (_unitest_, _pytest_).
- Intergration Testing.
- End-to-end Testing(_Selenium, PyAutoGUI_).
- Load Testing
- Test-Driven Development (TDD)

### Automation

- File Manipulations (_os, shutil, pathlib_)
- Web Scraping (_BeautifulSoup, Scrapy_)
- GUI Automations (_PyAutoGUI_)
- Network Automation

### Data Structures and Alogrithms (DSA) 

- Arrays & Linked lists
- Heap,Stacks,Queues
- Hash Tables
- Binary Search Trees
- Recursion
- Sorting Alogrithms

### Covers

- The universal concepts of computer programming;
- The syntax and semantics of the Python language;
- practical skills in resolving typical implementation challenges;
- how to use the most important elements of the Python Standard Library;
- how to install your runtime environment;
- how to design, develop, test, and debug simple Python programs.

## **Introduction**

Python is a simple, case sensitive, general-purpose programming language(Also object Oriented)developed by Guido Van Rossum, and released in 1991, going on to become one of the most popular languages among software and web professionals.

It gives developers the kind of versatility to work on many tasks like;- _Web Development, Web Application, Software Developent, AI & Machine Learning, System Scripting, Design Web Frameworks for new codes, Workflows, Prototyping, Automation, Deployment Services, Data Analysis, Data Visualisation, Web Scraping, Mathematics._

The Python REPL: REPL (_from Read, Evaluate, Print and Loop_) is a environment that you can use to program small snippets of Python code. Run exit() to leave the REPL.

Although Python developers will typically do back-end/server-side development, work on coding, debugging errors, deploying services, and designing projects, the arrival of machine learning and data science has extended their reach, helping them use their programming and coding skills to combine software components and enhance features, data privacy, and security.

Python developers can now perform a wide range of tasks with the work scope varying, depending on the needs of a company, employer or task at hand. Some Python developers are freelancers doing various tasks for different organizations and clients.

## The Key Features of Python

Python is has an easy to read syntax, dynamic typing, automatic memory management, extensive standard library, and support for multiple programming paradigms.

## PEP 8 

PEP 8 is the official style guide for python code that provides guidance on how to format pyhton code to enhance readability and maintain consistency across projects.

## Python Modules

Python Modules are files containing python code that defines functions, classes, and variables. They allow code reuse and organisation, making it easier to manage and maintain larger projects.

## Python Packages

A Python package is a way to organise related modules into a directory hierarchy, allowing for logical grouping of modules, making it easier to manage and distribute code.

## Commenting in Python

Comments in python are denoted by the ``#`` character. Anything after the ``#`` is considered a comment and is ignored by the python interpreter.

## Python Datatypes

Data types are data items that have been classified or categorized into things like numbers, integers, strings, and so on. A data type isn’t just a category of data, but it also informs what operations can be performed on a particular set of data.

Every value in Python has a data type and Python Data Types are used to define the type of a variable.

Without data types at play, you could set a variable, but Python wouldn’t know what to do with it. For example, if you didn’t have data types, you might set x = 2 and y = 10, but if you try to add those together with a function, Python wouldn’t know they were numbers so it wouldn’t be able to make the calculation. And that is why data types are important.

There are different types of data types in Python.

**Some built-in Python data types are:**

- Numeric data types: int, float, complex
- String data types: str
- Sequence types: list, tuple, range
- Binary types: bytes, bytearray, memoryview
- Mapping data type: Dictionary(_dict_)
- Boolean type: _bool_
- Set data types: set, frozenset

You will also notice that some of those types include different “sub-types”

## Typecasting

Type casting is the process of converting an object of one type into another in programming.

In Python there are different data types, such as numbers, sequences, mappings etc and often times, there are situation where, you have the available data of one type but you want to use it in another form thus the use of _**Python Type Casting**_.

### What is Python Type Casting

Python Type Casting is a process in which we convert a literal of one data type to another data type.

Fore example, say you have a program where a user has input a _string_ and you want to use it as a _number_,python's type casting mechanism will help with that.

### Implicit and Explicit Python Type Casting

- **Python Implicit Casting**

When any language compiler/interpreter automatically converts object of one type into other, it is called automatic or implicit casting. Python is a strongly typed language. It doesn't allow automatic type conversion between unrelated data types. For example, a string cannot be converted to any number type. However, an integer can be cast into a float. Other languages such as JavaScript is a weakly typed language, where an integer is coerced into a string for concatenation.

Note that memory requirement of each data type is different. For example, an integer object in Python occupies 4 bytes of memory, while a float object needs 8 bytes because of its fractional part. Hence, Python interpreter doesn't automatically convert a float to int, because it will result in loss of data. On the other hand, int can be easily converted into float by setting its fractional part to 0.

Implicit int to float casting takes place when any arithmetic operation on int and float operands is done.

- **Python Explicit Casting**

Although automatic or implicit casting is limited to int to float conversion, you can use Python's built-in functions int(), float() and str() to perform the explicit conversions such as string to integer.

## Python Developer

### Technical skills needed to become a competent Python developer;-

- Back-end and front-end Tools. front-end includes JavaScript, HTML, CSS, etc.
- Knowledge of Version control.
- A proper understanding of the automation framework for debugging errors, using different tools proficiently and managing other routine tasks thus managing toll and enhancing your speed and accuracy.
- A good grasp of Data Algorithms and Structures.

## Object Oriented Python

Object-oriented programming (OOP) is a programming paradigm in which programs are designed using classes and objects. This design allows related functions and data to be grouped together in self-contained and reusable units.

A class is a template or blueprint from which objects are made from. Classes define the properties and methods that an object can have, and objects are unique instances of a class.

For example, let's say you want to create a life simulation game where players can adopt and raise pets. You would have a "Pet" class that defines the properties of each pet (like "name" and "age"), as well as behaviors they can do (like "speak" and "eat").

You could then create objects, or instances, of this class for each specific pet. Each object could have its own values for each property. For example, you could have a 2-year-old pet named "Winston", & a 1-year-old pet named "Wesley"; both initialized from the "Pet" class.

Object-oriented programming has 4 main principles; _Encapsulation, Inheritance, Abstraction, and Polymorphism_.

- **Encapsulation** hides internal details but exposes data & methods via a public interface, preventing unintentional changes. E.g. — a player can view a pet's age but can't accidentally change it. But they can run methods avail on the public interface like changing a pet's name.

- **Inheritance** allows classes to inherit properties and methods from other classes, making code reusable and organized. E.g. — A "SuperPet" class that extends from "Pet "and would inherit "age", "name", "eat", and "speak"; while defining new behaviors like "fly"

- **Polymorphism** is a principle that enables objects to change their form by extending or overriding existing methods. E.g. A "Dog" & "Cat" class that extended from the "Pet", shouldn't share the same "speak" method. You'd override it to have its own logic like "woof" or "meow"

- **Abstraction** reduces complexity by only surfacing the information needed for a given context or use case. E.g. A “Player” class doesn’t need to know how the “eat” method works in the “Pet” class, it just needs to know how to interact with it — i.e. its input and output.

OOP provides a way to design your program that makes it reusable, secure, stable, and easy to understand. But it isn't without disadvantages. A couple of arguments against it are that it can lead to over-engineering and complexity on a large scale.

## Python Libraries

- Python + Pandas = Data Manupulation.
- Python + Scikit-Learn = Machine Learning.
- Python + Tensorflow = Deep Learning.
- Python + Matplotlib = Data Visualisation.
- Pyhton + Seaborn = Advanced Visualisation.
- Python + Flask = Advanced Visualisation & Web.
- Python + Pygame = Game Development.
- Python + Kivy = Mobile App Development.
- Python + Tkinter = GUI Development.

### Python Frameworks

One of the things to learn in Python after the fundamentals are **Python Frameworks** — toolkits developers can use to create software products quickly and efficiently. Using frameworks, python developers can focus on implementing application business logic without reinventing many common functions, including data storage, security layers, application routing, and many more. The two main types of frameworks are full-stack and micro-frameworks([reference](https://www.knowledgehut.com/blog/programming/how-to-become-a-python-developer)).

A link to a good Python roadmap;- [Step by step guide to becoming a Python developer](https://roadmap.sh/python).

Python fundamentals are like a foundation for any programming language whose basic concepts developers starting out should master.

All in all, key focus areas when starting out are;-

- Introduction to Python and computer programming
- Data types, variables, basic input-output operations, and basic operators;
- Boolean values, conditional execution, loops, lists and list processing, logical and bitwise operations;
- Functions, tuples, dictionaries, exceptions, and data processing.

A Python developer is responsible for writing server-side web application logic. Python web developers usually develop back-end componenets, connect the application with other(often third party) web services, and support the front-end developers by integrating their work with the Python Application.


## Conclusion

Python stands out with its simplicity, readability, and easy to understand syntax. It has a large and active community, extensive libraries, and is widely used in various domains such as web development, data analysis and scientific computing.

Type casting is the method to convert the Python variable datatype into a certain data type in order to perform the required operation by users. And Python supports two types of casting;- Implicit type casting and Explicit type casting.

## References

- [Python Developer](https://roadmap.sh/python)
- [Kaggle's Python](https://www.kaggle.com/learn/python)
- [Python](https://www.python.org/)
- [Real Python](https://realpython.com/)
- [The Python Tutorial](https://docs.python.org/3/tutorial/index.html#tutorial-index)
- [The Python Standard Library](https://docs.python.org/3/library/index.html)
- [The Python Language Reference](https://docs.python.org/3/reference/index.html#reference-index)
- [Python library reference](https://docs.python.org/3/library/stdtypes.html#numeric-types-int-float-complex)
- [Learn Object Oriented Programming With Python](https://www.freecodecamp.org/news/learn-object-oriented-programming-with-python/)
- [Object-Oriented Programming in Python – Explained in Plain English](https://www.freecodecamp.org/news/object-oriented-programming-python/)
- [Learn Python](@python.science)
- [Python sys library](https://docs.python.org/3/library/sys.html)
- [Python dictionaries Library](https://docs.python.org/3/library/stdtypes.html#mapping-types-dict/)
- [How to Write Unit Tests in Python – with Example Test Code](https://www.freecodecamp.org/news/unit-testing-in-python/)
- [Python Data Types](https://www.digitalocean.com/community/tutorials/python-data-types)
- [Python for Beginners: Data Types](https://thenewstack.io/python-for-beginners-data-types/)
- [Python - Type Casting](https://www.tutorialspoint.com/python/python_type_casting.htm)
- [Type Casting in Python (Implicit and Explicit) with Examples](https://www.geeksforgeeks.org/type-casting-in-python/amp/)

## Keywords

``Python``, ``Python Programming``, ``Python OOP``, ``Object-Oriented Programming in Python``, ``Variables``, ``Datatype``, ``Python Data Types``, ``Python Casting``, ``Type Casting``, ``Python Type Casting``, ``Implicit``, ``Python Implicit Type Conversion``, ``Explicit``, ``Python Explicit Type Conversion``

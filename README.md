## Introduction

Python is a versatile, high-level programming language known for its readability, simplicity, and broad applicability. It was created by Guido van Rossum and first released in 1991. Python's design philosophy emphasizes code readability and ease of use, making it a popular choice for beginners and experienced developers alike.

Here's a brief introduction to key aspects of Python:

1. **Syntax:**
Python uses a clean and straightforward syntax that emphasizes readability. It uses indentation to define code blocks, eliminating the need for braces or other explicit block delimiters.
Example:

```{python}
if x > 0:
    print("Positive number")
else:
    print("Non-positive number")
```
2. **Interpreted and High Level:**
Python is an interpreted language, meaning that it does not need to be compiled before execution. This makes development and debugging more interactive. It is also a high-level language, abstracting away many low-level details, which simplifies programming.

3. **Dynamic Typing:**
Python is dynamically typed, meaning you don't need to explicitly declare variable types. The interpreter infers types during runtime. Example :

```{python}
x = 5           # Integer
y = "Hello"     # String
z = 3.14        # Float
```

4. **Rich Standard Library:**
Python comes with a comprehensive standard library that includes modules for various tasks, such as file I/O, regular expressions, networking, and more. This reduces the need for external dependencies.
5. **Object-Oriented:**
Python supports object-oriented programming (OOP), encapsulating data and behavior into objects. It allows for the creation and manipulation of classes and objects.
Example:

```{python}
class Dog:
    def __init__(self, name):
        self.name = name

    def bark(self):
        print(f"{self.name} says Woof!")

my_dog = Dog("Buddy")
my_dog.bark()

```
6. **Community and Ecosystem:**
Python has a large and active community of developers. The Python Package Index (PyPI) hosts a vast collection of third-party libraries and frameworks that extend Python's capabilities, making it suitable for a wide range of applications.
7. **Versatility:**
Python is used in various domains, including web development, data science, artificial intelligence, machine learning, automation, scripting, and more. It is often considered a "glue" language due to its ability to integrate components written in different languages.
8. **Popular Frameworks:**
Python has popular frameworks and libraries that simplify complex tasks. Some examples include Django and Flask for web development, NumPy and Pandas for data science, TensorFlow and PyTorch for machine learning, and many more.

## Getting Started 
To get started with Python, you need to install the Python interpreter on your system. You can download it from the official Python website. Once installed, you can run Python scripts from the command line or use integrated development environments (IDEs) like VSCode, PyCharm, or Jupyter notebooks for interactive development.
On a personal note, I like Jupyter notebook a lot, because besides providing a neat IDE for executing and debugging code, it comes pre-installed with lots of modules like Numpy, Pandas, Matplotlib, Seborn, Scikitlearn etc. 

## Installation
1. Install a Python interpreter : https://www.python.org/
2. Install Jupyter notebook : 

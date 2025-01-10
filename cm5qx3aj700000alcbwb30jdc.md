---
title: "Learning Python: My First Step Towards Mastering Machine Learning"
seoTitle: "My Journey into Python and Machine Learning"
seoDescription: "Beginner's guide to Python for machine learning: libraries, packages, IDEs, data types, control flows, and functions"
datePublished: Fri Jan 10 2025 15:33:43 GMT+0000 (Coordinated Universal Time)
cuid: cm5qx3aj700000alcbwb30jdc
slug: learning-python-my-first-step-towards-mastering-machine-learning
tags: ai, programming-blogs, python, machine-learning, python3

---

As I mentioned in my previous blog, I started learning Python. In this blog, I will share my learnings in the easiest and simplest way possible. So, let’s get started!

### Before diving into Python concepts, let’s understand some important terms:

#### **1\. Library/Libraries**

Imagine you’re trying to build a chair. For that, you need tools like a hammer and screwdrivers. Now, you have two options:

1. Buy a toolkit that already has these tools.
    
2. Make them from scratch.
    

Most of us would choose the toolkit, wouldn’t we? It’s easier to use and saves us the hassle of creating tools from scratch! Similarly, in programming, libraries are like toolkits—collections of pre-written code that we can reuse to save time and effort. Libraries include functions, classes, or modules that make coding faster and more efficient.

In short, a **library** is like a toolkit for programmers. Pretty cool, right?

---

#### **2\. Package**

Now let’s talk about packages. Imagine you bought two different types of toolkits from an online shop. When your order arrives, everything is neatly packed in a box with all the toolkits inside. That box is a package.

In programming, a **package** is like that box—it contains libraries (and sometimes other resources) bundled together in an organized way. Packages make it easy to find, use, and share libraries. Wouldn’t you agree it’s better to use toolkits and neatly packed boxes than reinvent the wheel every time?

---

#### **3\. IDE (Integrated Development Environment)**

Let’s continue with our chair analogy. Imagine you’re building the chair, but all the tools, wood, and instructions are scattered everywhere. Wouldn’t it be great to have a workshop where everything is in one place? That’s what an **IDE** is for a programmer!

An IDE is like your programming workshop. It brings everything you need into one spot:

* **Tools** (e.g., compiler, debugger to run and fix your code)
    
* **Materials** (e.g., files and folders to organize your project)
    
* **Instructions** (e.g., syntax highlighting, code suggestions to guide you)
    

Whether you’re a beginner or a pro, an IDE makes coding easier, faster, and more efficient. It’s your trusty workshop for building amazing things!

---

#### **4\. Distribution**

Now imagine you’re building the chair again, and instead of going to multiple stores to buy wood, nails, and tools, you order a complete DIY chair kit online. This kit arrives with everything you need—tools, materials, and instructions—all in one neat box. Isn’t that convenient?

In programming, a distribution like **Anaconda** works the same way. Instead of downloading and installing each tool, library, and resource separately, it bundles them all together. For example, Anaconda includes:

* Python
    
* Essential libraries (e.g., NumPy, Pandas, Matplotlib)
    
* Tools (e.g., Jupyter Notebook)
    

In short, a distribution saves you time and effort by giving you everything you need in one place— just like a DIY kit.

---

### Why I Chose Anaconda

I’m using Anaconda, which is a distribution that includes tools, libraries, and frameworks for data science, machine learning, and scientific computing. You might wonder, **"Why use Anaconda and not just an IDE?"** Great question! Here’s what I found:

#### **Advantages of Anaconda:**

1. **Pre-installed Libraries**:
    
    * Anaconda includes libraries like NumPy, Pandas, Matplotlib, Scikit-learn, and TensorFlow, saving time and effort.
        
    * Tools like Jupyter Notebook provide an interactive coding environment ideal for data exploration.
        
    * With IDEs, we’d need to manually install and configure these libraries, which can be time-consuming and prone to errors.
        
2. **Environment Management**:
    
    * Anaconda allows us to create isolated environments with specific library versions, helping us:
        
        * Avoid version conflicts between projects.
            
        * Use different Python versions for different projects.
            
    * IDEs don’t manage environments directly; we’d need additional tools (e.g., Docker).
        
3. **Simplified Library Management**:
    
    * Anaconda uses the **Conda** package manager, which makes installing, updating, and managing libraries super easy. For example: Installing TensorFlow or Pandas requires just one command, and all dependencies are handled automatically.
        
    * With IDEs, we rely on `pip`, which can sometimes lead to dependency conflicts.
        

---

### My Installation Process

Here’s how I got started with Anaconda:

1. I downloaded Anaconda from its official website (I’m using Windows).
    
2. After completing the installation, I opened the `Anaconda Prompt`.
    
3. In the terminal, I typed `jupyter notebook` and pressed Enter.
    
4. That’s it! The Jupyter Notebook interface opened in my browser, and I was ready to code interactively.
    

Once inside the Jupyter Notebook:

1. I clicked `New` to create a new folder.
    
2. After creating the folder, I selected it and clicked `New` again to open a Python notebook.
    
3. A new tab opened with the notebook interface.
    
4. To kick things off, I wrote my very first Python line of code: `print("Hello World")`.
    
5. Pressing `Shift + Enter` ran the code, and voila—"Hello World" appeared as the output!
    

---

### Python Basics: Data Types

Like other programming languages, Python has data types that classify items and determine what operations can be performed on them. Here’s a quick overview:

#### **1\. Numeric**

Numeric types represent numbers. Python has three numeric types:

* **int**: Whole numbers (e.g., 5, -10)
    
* **float**: Decimal numbers (e.g., 3.14, -2.5)
    
* **complex**: Numbers with real and imaginary parts (e.g., 2+3j)
    

**Use in Machine Learning:**

* **int**: Discrete values like class labels or iterations.
    
* **float**: Continuous values like weights or probabilities.
    
* **complex**: Advanced areas like signal processing.
    

---

#### **2\. Sequence Types**

Sequence types store multiple items in an ordered way. Key types:

* **list**: Mutable collections (e.g., `[1, 2, 3]`)
    
* **tuple**: Immutable collections (e.g., `(1, 2, 3)`)
    
* **string**: Text data (e.g., `'Hello'`)
    

**Use in Machine Learning:**

* **list**: Datasets, predictions.
    
* **tuple**: Fixed configurations.
    
* **string**: Text data in NLP tasks.
    

---

#### **3\. Dictionary**

A collection of key-value pairs (e.g., `{'key': 'value'}`). Keys are unique, values can vary.

**Use in Machine Learning:**

* Storing hyperparameters or mappings (e.g., class labels).
    

---

#### **4\. Boolean**

Booleans represent `True` or `False` values.

**Use in Machine Learning:**

* Control flow (e.g., stopping conditions).
    
* Binary classification results.
    

---

#### **5\. Set Types**

* **set**: Unordered unique items.
    
* **frozenset**: Immutable set.
    

**Use in Machine Learning:**

* Unique elements (e.g., dataset labels).
    

---

So, to get familiar with these data types, I practised their syntax and explored some commonly used functions. Here’s a sneak peek into what I learned and how I experimented with them:

1. **List -**
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1735813702471/a691b71d-54cb-4668-b835-32632b3ea30d.png align="center")
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1735813715307/9c50b5a9-aff2-4926-afe8-4f0b838295cb.png align="center")
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1735813726846/1a2a87f9-4884-4a70-8665-b43fa11cc815.png align="center")
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1735813735215/c094b66f-9615-4f30-8d53-33c2e7b8b4fd.png align="center")
    
2. **Tuple -**
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1735951547047/b429dc1c-6743-4d74-b99f-ab80959e3d54.png align="center")
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1735951560468/a4ba8a4f-2716-4eaf-b77b-c120702d6260.png align="center")
    
    Tuples are **immutable** in Python, which means once they are created, their elements cannot be changed, added, or removed. Because of this immutability, methods like `pop()` or `remove()` that modify the content of a collection do not exist for tuples.
    
3. **String -**
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736078809283/4bde74f3-92a2-42ec-b7d5-10af91343254.png align="center")
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736078824864/14ba319c-c844-4835-a228-985f9e80765b.png align="center")
    
4. **Dictionary -**
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736084661832/18dbbd8e-4bd2-4a39-8991-cd8fc44de2d5.png align="center")
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736084704943/3a9580e9-fcec-48dd-b8c1-4284b5d4c1bf.png align="center")
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736084721442/56b330ab-253e-4f8e-a210-9c86e285beb7.png align="center")
    
5. **Set and frozenset -**
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736086782077/0da5a18e-97e7-4ee9-9ff6-822cb0c5158f.png align="center")
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736086832194/44607e7c-3cb2-47cb-9044-28f8d6f53baa.png align="center")
    

---

### Control Flows :

When I first started coding, I was fascinated by how a program could "think." I mean, imagine your code deciding what to do based on input or repeating tasks without you manually writing every step! That’s where **control flows** come in—they’re like the brain of your program, guiding it to make decisions, repeat actions, and even handle unexpected hiccups.

Python's control flow structures include:

1. **Conditional Statements**: `if`, `elif`, `else`
    
2. **Loops**: `for`, `while`
    
3. **Break and Continue**: Alter the flow of loops.
    
4. **Exception Handling**: `try`, `except`, `finally`, `raise`
    

---

### 1\. **Making Decisions: Conditional Statements**

Conditional statements let your code make decisions based on certain conditions, guiding it to follow one path or another.

#### General Syntax:

```python
if condition:
    # Code block to execute if condition is True
elif another_condition:
    # Code block to execute if the second condition is True
else:
    # Code block to execute if none of the above conditions are True
```

**Explanation**:

* `if` checks the first condition. If it's `True`, the code inside it runs.
    
* `elif` (else if) checks another condition if the first one isn't met.
    
* `else` runs the code when none of the previous conditions are true.
    

Example:  
Let's write a simple program that tells you what to wear based on the temperature:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736263234606/f2cdedb1-ab72-4c2c-b202-dca3b4062abe.png align="center")

---

### 2.Repeating Tasks: Loops

Loops are our best friend when we want to repeat actions multiple times, whether it's processing data or just performing a task over and over.

#### General Syntax:

##### **For Loop** (when we know how many times to repeat):

```python
for variable in iterable:
    # Code block to repeat
```

**Explanation**:

* The loop goes through each item in the `iterable` (like a list, string, or range).
    
* The `variable` takes each value from the iterable, and the loop runs the code inside for each value.
    

##### **Example for a For Loop**:

Let's print a list of movies:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736263426547/040fda6e-4d27-4baf-b9b8-6353a7c05e7b.png align="center")

##### **While Loop** (when we don’t know how many times to repeat):

```python
while condition:
    # Code block to repeat while the condition is True
```

**Explanation**:

* The `while` loop keeps running the code inside as long as the `condition` remains `True`.
    

##### **Example for a While Loop**:

Let’s guess a number until we get it right:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736263646850/5e1ad93f-b5d6-46da-9891-dbbd692e330a.png align="center")

Sometimes, we want to skip parts of a loop or exit early. That’s where `break` and `continue` come in.

#### General Syntax:

##### **Break** (to exit a loop early):

```python
for item in iterable:
    if some_condition:
        break  # Exit the loop
```

##### **Continue** (to skip the current iteration and continue the loop):

```python
for item in iterable:
    if some_condition:
        continue  # Skip to the next iteration
```

**Explanation**:

* `break` stops the loop completely.
    
* `continue` skips the current iteration and moves to the next one.
    

##### **Example with Break**:

Searching for the item eraser in the list of items:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736263799065/3c08c6b8-e8ca-41ed-979f-d10268c0a727.png align="center")

##### **Example with Continue**:

Skipping even numbers:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736263844556/6539a22f-fc79-4a6c-ba60-17d6029c6e84.png align="center")

---

### 3.Handling Errors: Exception Handling

Sometimes, things go wrong in our code. Instead of crashing, exception handling lets us handle errors gracefully.

#### General Syntax:

```python
try:
    # Code block where you expect an error might occur
except ExceptionType:
    # Code block to run if an exception occurs
else:
    # Code block to run if no exception occurs
finally:
    # Code block that always runs, regardless of whether an exception occurred
```

**Explanation**:

* `try` is where we place code that could throw an error.
    
* `except` catches and handles the error if one occurs.
    
* `else` runs if no error occurs.
    
* `finally` runs no matter what, even if there’s an error.
    

##### **Example**:

Here’s a simple program where we ask the user for a number and handle the case where they don’t enter a valid number:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736264189932/03391b88-9974-4519-a572-29c71115707b.png align="center")

---

***NOTE*** \- *Some common exceptions in Python:*

1. `ZeroDivisionError`*: Raised when we try to divide a number by zero.*
    
2. `IndexError`*: Raised when we try to access an index in a list or tuple that is out of range.*
    
3. `ValueError`*: Raised when a function receives an argument of the correct type but an inappropriate value.*
    
4. `TypeError`*: Raised when an operation or function is applied to an object of inappropriate type.*
    
5. `FileNotFoundError`*: Raised when trying to open a file that doesn’t exist.*
    
6. `KeyError`*: Raised when trying to access a dictionary with a key that doesn’t exist.*
    
7. `AttributeError`*: Raised when an invalid attribute reference or assignment is made on an object.*
    
8. `ImportError`*: Raised when an import statement fails to find the module or when a module or object cannot be imported.*
    
9. `OverflowError`*: Raised when a numeric operation exceeds the range that can be represented.*
    
10. `MemoryError`*: Raised when an operation runs out of memory.*
    
11. `NameError`*: Raised when a local or global name is not found.*
    
12. `NotImplementedError`*: Raised when a method or operation is not implemented, typically in abstract classes.*
    
13. `AssertionError`*: Raised when an* `assert` *statement fails, indicating that the condition being tested is false.*
    
14. `TimeoutError`*: Raised when a system function timed out at the operating system level.*
    
15. `KeyboardInterrupt`*: Raised when the user interrupts the program's execution, often by pressing* `Ctrl+C`*.*
    

*These exceptions are part of Python's built-in error handling mechanism, helping developers manage and respond to different types of errors in a program.*

---

### 4.Organizing Code: Functions

Functions are like mini-programs inside our program. They allow us to group code that we want to reuse and make our code more organized and readable

#### General Syntax:

```python
def function_name(parameters):
    # Code block to execute
    return value  # Optional, depending on whether you want to return something
```

**Explanation**:

* `def` is the keyword used to define a function.
    
* `function_name` is the name you give your function (choose a descriptive name).
    
* `parameters` are the values that the function will take when called (can be empty if needed).
    
* The `return` statement is optional and is used to return a result from the function to the caller.
    

#### Example:

Let's define a simple function that greets the user.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736265856594/28f861e8-02ca-48d8-892c-3098606b5d26.png align="center")

We can define functions with more than one parameter. It’s like giving the function multiple pieces of information to work with.

#### General Syntax:

```python
def function_name(parameter1, parameter2, ...):
    # Code block to execute using parameter1, parameter2, etc.
    return value  # Optional
```

#### Example:

Let’s define a function that calculates the area of a rectangle.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736266007056/fc56cc8f-0f90-4cbb-9043-9b198340d6cc.png align="center")

Sometimes, we might want to have default values for parameters. This allows us to call the function without specifying those parameters each time.

#### General Syntax:

```python
def function_name(param1=default_value, param2=default_value, ...):
    # Code block to execute using the parameters
    return value  # Optional
```

#### Example:

Let’s create a function that prints the full name of a person, where the last name is optional.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736266184665/fa3c2e85-65a9-46b8-af4f-ed2253ba6947.png align="center")

The `return` statement is used to send back a value from a function. We can return values of any type—like integers, strings, lists, or even other functions!

#### Example:

Here’s a function that returns the square of a number.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736266243866/69ec52fb-1aac-4908-8974-6b0623327a46.png align="center")

---

### 5\. File Handling in Python: Reading from and Writing to Files

In many programs, we'll need to work with files—whether it’s reading data, storing logs, or saving output. Python makes file handling easy with functions like `open()`, `.read()`, `.write()`, and more.

I have created a file named `example.txt` whose content is as follows:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736519676811/05ed52ba-bc7b-445c-8b86-c802c8c50978.png align="center")

**Opening a File:**

The `open()` function is used to open a file. It takes two main parameters: the `filename` and the `mode` in which you want to open the file (read, write, etc.).

#### General Syntax:

```python
file = open("filename", "mode")
```

**Explanation**:

* `"filename"` is the name of the file you want to open.
    
* `"mode"` specifies the action (e.g., read, write, append). The most common modes are:
    
    * `"r"`: Read (default, file must exist).
        
    * `"w"`: Write (creates a new file or overwrites an existing file).
        
    * `"a"`: Append (adds to the end of the file).
        
    * `"rb"`, `"wb"`: Read or write in binary mode.
        

**Reading from a File:**

Once a file is open, we can read its content using different methods.

#### General Syntax for `.read()`:

```python
content = file.read()  # Reads the entire file
```

#### Example:

Reading the entire content of a file:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736520327644/cfc0cbdc-38ec-40f9-8f5b-9df9385c9c8e.png align="center")

**Closing the File:**

After we finish working with a file, it's important to close it using `.close()`. This frees up the resources and ensures the file is saved properly.

**Writing to a File:**

We can use the `.write()` function to write data to a file. We need to be careful because this will **overwrite** any existing content in the file (unless we use append mode).

#### General Syntax:

```python
file = open("filename", "w")  # Open file in write mode
file.write("Your content here")  # Write to the file
file.close()  # Close the file after writing
```

#### Example:

Writing to a file:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736520719764/a400080b-68da-4ae7-bebc-1e6693422d64.png align="center")

The file `new_file.txt` gets created and the content is as follows :

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736520665157/b921be7e-43f1-4dd7-be71-71b8011e1578.png align="center")

**Appending to a File:**

If we don’t want to overwrite a file but instead add to it, we can open the file in append mode (`"a"`).

#### General Syntax:

```python
file = open("filename", "a")  # Open file in append mode
file.write("Additional content\n")  # Add to the file
file.close()
```

#### Example:

Appending to a file:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736520863025/d5e28708-f940-44ec-a8fb-f662c4bfd2c2.png align="center")

The new content of the file `example.txt` is as follows:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736520988071/3bc29ab6-8def-40df-86d6-7b6a7a4a66ec.png align="center")

If we want to read a file line by line, we can use `.readlines()`.

#### General Syntax:

```python
lines = file.readlines()  # Returns a list of lines in the file
```

#### Example:

Reading a file line by line:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736521237678/6a0e560a-f037-4537-801e-5f08bdf9d45d.png align="center")

---

### 6\. **The** `os` Library: File and Directory Management

The `os` library is essential when we need to interact with the operating system—whether it's to work with files, directories, or environment variables. It allows us to do everything from creating files to checking if a file or directory exists. Let’s dive into some common tasks.

#### a) **Checking if a File/Directory Exists**

We can use `os.path.exists()` to check if a file or directory exists on our system.

The `os.mkdir()` function allows us to create a new directory.

#### General Syntax:

```python
import os
os.mkdir("directory_name")
```

#### General Syntax:

```python
import os
os.path.exists("path/to/file_or_directory")
```

#### Example:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736519114597/4975cb75-b2ed-46b7-bc97-708154a3cc40.png align="center")

#### b) **Listing Files in a Directory**

We can list all the files in a directory using `os.listdir()`.

#### General Syntax:

```python
import os
os.listdir("path/to/directory")
```

#### Example:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736519219653/c6baf281-8076-4b3f-aa48-acfac6830d29.png align="center")

#### c) **Renaming or Removing Files**

We can rename files using `os.rename()` and remove them using `os.remove()`.

#### General Syntax for Renaming:

```python
os.rename("old_filename", "new_filename")
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736519256303/0761a005-3b8d-4dd2-afc1-290d76bda95b.png align="center")

#### General Syntax for Removing:

```python
os.remove("filename_to_remove")
```

---

These are just some of the concepts I’ve explored so far in my journey with Python. My approach is to learn on the go and dive deeper into topics as I progress. In the next blog, I’ll be exploring how to visualize data using Python — an essential skill for data analysis and machine learning.

If you have any suggestions, tips, or feedback that could help enhance my understanding, please feel free to share in the comments. Your input will not only help me but also benefit others on the same journey.

Let’s grow and learn together!
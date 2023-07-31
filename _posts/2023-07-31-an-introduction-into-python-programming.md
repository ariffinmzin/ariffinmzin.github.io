---
title: "An Introduction into Python Programming"
author: ariffin
date: 2023-07-31 23:06:00 +0800
categories: [Blogging, Python]
tags: [Python]
---

# An Introduction into Python Programming 🐍
Hello there, you adventurous souls! 💫 Today, we're going to take an exciting journey into the heart of Python, one of the most loved programming languages out there. So buckle up! 😁

## Overview
Python, not to be mistaken with the slithering reptile, is a high-level, interpreted programming language known for its simplicity and elegance. 🎩 Much like the perfect cup of coffee, it's strong (in capabilities), sweet (in syntax), and a favorite amongst many programmers, both beginners and veterans alike! ☕

Created with the philosophy of "Code readability matters", Python's syntax is designed to be easy-to-understand, clean, and intuitive. This allows developers to focus more on solving problems than on trying to understand the language itself. 🧐

## History of Python 🏛️
So, where did Python come from? Python was created by Guido van Rossum, a Dutch programmer who started working on the language back in the late 1980s as a Christmas 🎅 hobby project! He wanted to create a language that was easy-to-read and easy-to-write, borrowing elements from various other languages like ABC, Modula-3, C, C++, Unix shell, and even English itself. Fun fact: Python is named after the British comedy troupe Monty Python, not the snake. So, if you were hoping to become a snake charmer, I'm sorry for the letdown. 😅

Python was publicly released in 1991, and since then, it has grown rapidly, mainly due to its simplicity and the ever-expanding standard library which is like a vast treasure chest for programmers. 🏴‍☠️

## Python Identifiers 🏷️
In Python, identifiers are the names used to identify a variable, function, class, module, or other object, which is like giving a name to our pet. 🐶 So, how do we name our Python pets?

Here are some rules:

1. Identifiers can be a combination of lowercase (a to z) or uppercase (A to Z) letters, digits (0 to 9), or an underscore (_). For instance, `snake_case`, `MACRO_CASE`, `camelCase`, `CapWords` are all valid Python identifiers.
2. An identifier cannot start with a digit. `1variable` is incorrect, while `variable1` is perfectly fine.
3. Keywords cannot be used as identifiers. We can't name our pet "None", "True", or "False" (sorry, Boolean fans!). 😅
4. Identifiers can be of any length. But remember, too long might confuse you later, and too short might not be descriptive. Strike a balance! 🎯

## Naming Conventions 📛
In Python, naming conventions are a bit like fashion trends - you can technically wear whatever you want, but certain styles just fit better for specific occasions. 😉

* Use `lowercase` with words separated by underscores for variables and functions: `my_variable`, `compute_average`.
* Use `PascalCase` for class names: `MyAwesomeClass`.
* Use `ALL_CAPS` for constants: `PI`, `MAX_OVERFLOW`.
* If you're using a variable that's supposed to be "private" (not directly accessed), prefix it with a single underscore: `_my_secret_var`.
* If an identifier starts with two leading underscores, it's a strongly private identifier: `__really_secret_var`.
* An identifier that starts and ends with two underscores is a language-defined special name: `__init__`, `__main__`.

## Lines and Indentation ⏩
Python uses indentation to define blocks of code. Other languages might use curly braces `{}`, but Python's like, "Nah, I'm good. I'll stick with spaces and tabs." 😉 Each level of indentation is four spaces (preferred) or one tab.

```python
def greet(name):
    print(f"Hello, {name}!")  # This line is indented!

greet("Alice")
```

In the above code, the `print` statement is part of the `greet` function because it's indented under the function definition. Pretty neat, eh?

## Script Mode and Interactive Mode 💻
Python can be run in two modes: script and interactive. In *interactive mode*, you type Python commands one at a time at the `>>>` prompt, and they get executed immediately. It's like having a conversation with Python! 😊

```python
>>> print("Hello, World!")
Hello, World!
```

In *script mode*, you write your Python code in a file (ending with .py) and then run it with Python. It's more like writing a letter 💌 to Python.

```python
# save this as hello_world.py
print("Hello, World!")

# run the script
$ python hello_world.py
Hello, World!
```

This marks the end of our Python exploration today. Stay tuned for more riveting Python adventures. Until then, keep coding, keep exploring, and remember - Python is more enjoyable with friends. 🥳
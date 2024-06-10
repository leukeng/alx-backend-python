# Aynchronous Programming in Python

<img src=https://camo.githubusercontent.com/828f2fb0743c07e1c3e65431eb9692cda313f137d10ecde9dbaeb02ca4bc560a/68747470733a2f2f7265616c707974686f6e2e636f6d2f63646e2d6367692f696d6167652f77696474683d3936302c666f726d61743d6175746f2f68747470733a2f2f66696c65732e7265616c707974686f6e2e636f6d2f6d656469612f556e6465727374616e64696e672d4173796e6368726f6e6f75732d50726f6772616d6d696e672d696e2d507974686f6e5f57617465726d61726b65642e3462353930633763303365612e6a7067>
Async programming allows you to write concurrent code that runs in a single thread. The first advantage compared to multiple threads is that you decide where the scheduler will switch from one task to another, which means that sharing data between tasks it's safer and easier.

## Concurrency vs Parallelism
Concurrency and parallelism can sound really similar but in programming there is an important difference. Immagine you are writing a book while cooking, even if it seems like you are doing both tasks at the same time, what you are doing is switching between the two tasks, while you wait for the water to boil you are writing your book, but while you are chopping some vegetables you pause your writing. This is called concurrency. The only way to do these two tasks in parallel is having two people, one writing and one cooking, which is what multicore CPU do.

### Concurrency
<img src=https://camo.githubusercontent.com/543ab4f3a024d9b8138a9adf5fbd6a0e35abbf6da79c11630f0f925df59cbcda/68747470733a2f2f7265732e636c6f7564696e6172792e636f6d2f70726163746963616c6465762f696d6167652f66657463682f732d2d643238665530674b2d2d2f635f6c696d6974253243665f6175746f253243666c5f70726f6772657373697665253243715f6175746f253243775f3838302f68747470733a2f2f6465762d746f2d75706c6f6164732e73332e616d617a6f6e6177732e636f6d2f692f6564757a6d70347a7433383938787a35646669612e6a706567>

### Parellelism
<img src=https://camo.githubusercontent.com/543ab4f3a024d9b8138a9adf5fbd6a0e35abbf6da79c11630f0f925df59cbcda/68747470733a2f2f7265732e636c6f7564696e6172792e636f6d2f70726163746963616c6465762f696d6167652f66657463682f732d2d643238665530674b2d2d2f635f6c696d6974253243665f6175746f253243666c5f70726f6772657373697665253243715f6175746f253243775f3838302f68747470733a2f2f6465762d746f2d75706c6f6164732e73332e616d617a6f6e6177732e636f6d2f692f6564757a6d70347a7433383938787a35646669612e6a706567>

## Resources
- Async with python

- Getting started with async

- AsyncIO in python

- Async python doc

## Learning Objectives
- async and await syntax
- How to execute an async program with asyncio
- How to run concurrent coroutines
- How to create asyncio tasks
- How to use the random module

## Coroutines
A coroutine is the result of an asynchronous function which can be declared using the keyword async before def
```
async def my_func(args):
    return args**2

routines = my_func(args)
```
When we declare a function using the async keyword the function is not run, instead, a coroutine object is returned.

## Project Requirements
- A README.md file, at the root of the folder of the project, is mandatory
- Allowed editors: vi, vim, emacs
- All your files will be interpreted/compiled on Ubuntu 18.04 LTS using python3 (version 3.7)
- All your files should end with a new line
- All your files must be executable
- The length of your files will be tested using wc
- The first line of all your files should be exactly #!/usr/bin/env python3
- Your code should use the pycodestyle style (version 2.5.x)
- All your functions and coroutines must be type-annotated.
- All your modules should have a documentation (python3 -c 'print(__import__("my_module").__doc__)')
- All your functions should have a documentation (python3 -c 'print(__import__("my_module").my_function.__doc__)'
- A documentation is not a simple word, it’s a real sentence explaining what’s the purpose of the module, class or method (the length of it will be verified)

# summery 
## Classes and Objects
![image](https://miro.medium.com/max/3840/1*3nVcGlo7ijlMgyjfWj0QxA.png)
#### Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.
#### let's take an example to be clear more 
`` class MyClass:``
    ``variable = "blah"``

    def function(self):
         print("This is a message inside the class.")  
     
#### now to assign the above class(template) to an object you would do the following:     
``class MyClass:``
    ``variable = "blah"``

    def function(self):
        print("This is a message inside the class.")

``myobjectx = MyClass()``
#### To access the variable inside of the newly created object "myobjectx" you would do the following:

``myobjectx.variable``
#### So for instance the below would output the string "blah":
``print(myobjectx.variable)``
#### You can create multiple different objects that are of the same class like here 
``class MyClass:``
    ``variable = "blah"``

    def function(self):
        print("This is a message inside the class.")

``myobjectx = MyClass()``
``myobjecty = MyClass()``

``myobjecty.variable = "yackity"``
#### To access a function inside of an object you use notation similar to accessing a variable:
``myobjectx.function()``

## now let's move to another topic the Thinking Recursively in Python
![image2](https://files.realpython.com/media/fixing_problems.ffd6d34e887e.png)
#### This is the typical structure of a recursive algorithm.
![image](https://files.realpython.com/media/elves_7.8d1af1cd85c8.png)
#### Recursion is a common mathematical and programming concept. It means that a function calls itself. This has the benefit of meaning that you can loop through data to reach a result.

#### This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result. All recursive functions share a common structure made up of two parts: base case and recursive case.

#### Behind the scenes, each recursive call adds a stack frame (containing its execution context) to the call stack until we reach the base case. Then, the stack begins to unwind as each call returns its results.

#### Recursive functions are common in computer science because they allow programmers to write efficient programs using a minimal amount of code. The downside is that they can cause infinite loops and other unexpected results if not written properly.

## now our last topic for today is Python Testing with pytest: Fixtures and Coverage
![image](https://files.realpython.com/media/Intermediate-Advanced-PyTest-Features_Watermarked.2d8ace6b71be.jpg)
##### Pytest is a robust Python testing tool, pytest can be used for all types and levels of software testing. pytest can be used by development teams, QA teams, independent testing groups, individuals practicing TDD, and open source projects. In fact, projects all over the Internet have switched from unittest or nose to pytest, including Mozilla and Dropbox. Why? Because pytest offers powerful features such as ‘assert‘ rewriting, a third-party plugin model, and a powerful yet simple fixture model that is unmatched in any other testing framework.

### Fixtures
#### If your tests need to work on data you typically need to set them up. This is often a process that has to be repeated and independent for each test. This often leads to duplicate code.

#### The @pytest.fixture decorator provides an easy yet powerful way to setup and teardown resources. You can then pass these defined fixture objects into your test functions as input arguments.

#### In pytest, you define fixtures using a combination of the pytest.fixture decorator, along with a function definition. For example, say you have a file that returns a list of lines from a file, in which each line is reversed:

``def reverse_lines(f):
    return [one_line.rstrip()[::-1] + '\n'
       for one_line in f]``
#### If you're going to test this function, you'll need to pass it a file-like object. But rather you can create a fixture that'll provide your test with the appropriate object at the right time.

``@pytest.fixture
    def simple_file():
        return StringIO('\n'.join(['abc', 'def', 'ghi', 'jkl']))``































``# Then print out both values``
``print(myobjectx.variable)``
``print(myobjecty.variable)``

# summery

## In Tests We Trust — TDD with Python
##### Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.

##### ok let give an example to be clear 
`` def test_should_return_female_when_the_name_is_from_female_gender():
    detector = GenderDetector()
    expected_gender = detector.run(‘Ana’)
    assert expected_gender == ‘female’ ``
    
##### There are some details to pay attention
1. *the test name*. The tests can be considered as your alive documentation. We need to be descriptive about it and to say what is expected and what we are testing.
2. The test file name should follow the same name of module name
3. Other thing to care about is the structure
- Arrange: you need to organize the data needed to execute that piece of code (input);
- Act: here you will execute the code being tested (exercise the behaviour);
- Assert: after executing the code, you will check if the result (output) is the same as you were expecting.
#### now let's talk about The Cycle
![image](https://miro.medium.com/max/1033/1*ZPQ7IoHWm0yG0SIbjZxQ9w.png)

- 🆘 Write a unit test and make it fail (it needs to fail because the feature isn’t there, right? If this test passes, call the Ghostbusters, really)
- ✅ Write the feature and make the test pass! (you can dance after that)
- 🔵 Refactor the code — the first version doesn’t need to be the beautiful one (don’t be shy)
#####   now let’s do the cycle!
1.first We made our test fail
2. Now it’s time to implement the feature . our implementation should follow the same rule, ok
3. We just need to write the method that returns the right answer
4. then if you run  tests again. It’s green!!! 🍀
#### now let's have some fun and remember things
![image2](https://miro.medium.com/max/875/1*dTd_0x8gdefpRt9tUtekPQ.png)
- The greatest advantage about TDD is to craft the software design first
- Your code will be more reliable: after a change you can run your tests and be in peace
- Beginning may be hard — and that’s fine. You just need to practice!

## now let"s move to another topic ..... the Recursion

##### The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. Using recursive algorithm, certain problems can be solved quite easily. 
### What is base condition in recursion? 
##### In the recursive program, the solution to the base case is provided and the solution of the bigger problem is expressed in terms of smaller problems. 
### What is the difference between direct and indirect recursion?
##### A function fun is called direct recursive if it calls the same function fun. A function fun is called indirect recursive if it calls another function say fun_new and fun_new calls fun directly or indirectly.
### How memory is allocated to different function calls in recursion?
##### When any function is called from main(), the memory is allocated to it on the stack. A recursive function calls itself, the memory for a called function is allocated on top of memory allocated to calling function and different copy of local variables is created for each function call. When the base case is reached, the function returns its value to the function by whom it is called and memory is de-allocated and the process continues.























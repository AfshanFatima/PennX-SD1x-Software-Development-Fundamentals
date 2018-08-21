### Week 2: Testing and Debugging

### Unit Testing

**Problem 1a**

Select all the benefits/advantages of Junit testing.

Test that all pieces of a software fits together.

Make life easier for regression testing. -correct

Make it easier to locate a bug. -correct

Tells if the software is compliant with user specification.

Makes development process more clear. -correct

Explanation: 
Regression test is functional rather than unit testing, but Junit can be used to write separate unit tests which eases the process. Junit helps point out cases where the code fails.

**Problem 1b**

Writing unit tests for every method in a Java program ensures that the program works?

True

False -correct

Explanation:
Regression test is functional rather than unit testing, but Junit can be used to write separate unit tests which eases the process. Junit helps point out cases where the code fails.

![code snippet](https://prod-edxapp.edx-cdn.org/assets/courseware/v1/275f50ddca07a7c69c0b94e9a4f73429/asset-v1:PennX+SD1x+2T2017+type@asset+block/Quiz2.1Problem2.png)

**Problem 2**

Given the above class and tests, which test method will fail?

testDeposit

testOwner1

testOwner2 -correct

testOwner3 

Explanation:
When comparing two objects, == will not work. == will compare the address of the two objects.

![code snippet](https://prod-edxapp.edx-cdn.org/assets/courseware/v1/34df338ab4e3ff3168759d16255a1321/asset-v1:PennX+SD1x+2T2017+type@asset+block/Quiz2.1Problem3.png)

**Problem 3**

How many test cases would you recommend for the above method?

Answer Correct: 4 or 5
 
Explanation:
You need unit test cases for each possibility such as when req's getMethod returns "GET", "HEAD", "POST", some other value or null. For each, response(returned value) can be checked.

**Problem 4**

Why does TDD want you to write the tests before the code?

Testing needs to be done anyway, so might as well do it at the beginning.

Writing a test helps you discover edge cases even before you start coding. -correct

Writing a test helps break the program into testable units. This helps with the design of your code. -correct

It is the prevailing trend in the software engineering industry.

Explanation:
Testing helps break down the code into components each satifying a condition including edge cases.

### Debugging

**Problem 1**

Match the definition of the following terminologies: 

1 step over,

2 step into,

3: step return

(a) You're done debugging this method step-by-step, and you just want the debugger to run the entire method until it returns as one entire step.

(b) A method is about to be invoked, but you're not interested in debugging this particular invocation, so you want the debugger to execute that method completely as one entire step.

(c) A method is about to be invoked, and you want to debug into the code of that method, so the next step is to go into that method and continue debugging step-by-step.

Correct Answer:

1 step over:
 b or (b) or B or (B)

2 step into:
   c or (c) or C or ©

3: step return
  a or (a) or A or (A)

Explanation:
Step over is for the method about to be invoked. Step return is jump out from the method and let it return as one step. Step into is to jump into the method to debug step by step.

**Problem 1**

Match the definition of the following terminologies: 

1 step over,

2 step into,

3: step return

(a) You're done debugging this method step-by-step, and you just want the debugger to run the entire method until it returns as one entire step.

(b) A method is about to be invoked, but you're not interested in debugging this particular invocation, so you want the debugger to execute that method completely as one entire step.

(c) A method is about to be invoked, and you want to debug into the code of that method, so the next step is to go into that method and continue debugging step-by-step.

Answer Correct:

1 step over:
   b or (b) or B or (B)
   
2 step into:
   c or (c) or C or (C)
   
3: step return
   a or (a) or A or (A)
   
Explanation:
Step over is for the method about to be invoked. Step return is jump out from the method and let it return as one step. Step into is to jump into the method to debug step by step.

**Problem 2**

If we want to run intermediate computations while we are in the midst of debugging, the view we need is:

Console

Error Log

Display -correct

Tasks

Explanation:
Display window will show intermediate computations.




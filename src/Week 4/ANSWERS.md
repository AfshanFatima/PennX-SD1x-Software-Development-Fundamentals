### Week 4 : Polymorphism

### Overloading

**Problem 1**

Select correct statements from the following list:

In Java, signature of a method includes method name, return type, number of arguments and type of arguments (order of arguments matter).

System.out.println() is heavily overloaded in Java. correct

You can not overload constructor.

An overloaded method can call another method with the same method name but different arguments. -correct


Explanation:
The signiture of the method does not include the return type; System.out.println() can take int, string, and other data types. So it is heavily overloaded in java.
        

### Overriding

![Code Snippet](https://prod-edxapp.edx-cdn.org/assets/courseware/v1/1753c66acdb5065db328be587cded346/asset-v1:PennX+SD1x+2T2017+type@asset+block/Quiz4.2Problem2.png)

In main method, what gets printed in each of the following print statements?

**Problem 2.1**

System.out.println(e1 == e2);

 Answer Correct:  true
 
Explanation:
e1 is assigned to e2. Both e1 and e2 refer to the same spot in memory. Comparing them gives you the same result.


**Problem 2.2**

System.out.println(s1.equals(s2));

Answer Correct:true

Explanation:
s1 is "bla"; s2 is "bl" + "a", which is also "bla"; So they are equal.


**Problem 2.3**

System.out.println(s1 == s2);

Answer Correct:  false

Explanation:
For string, == compares the address of the two strings. Since they are stored at different places in memory, it will return false.


**Problem 2.4**

System.out.println(e1);

Answer Correct: ID: 0; Name: oops or ID: 0; NAME: oops or id: 0; name: oops

Explanation:
When toString() method is overrided, it will not print the address of the class but how a programmer want it to be. In this case, it will print ID: 0; Name: oops.

**Problem 2.5**

System.out.println(e1.tostring());

Answer Correct: Name: oops or name: oops

Explanation:
tostring() is different from toString(). In this case, tostring() is called, so it will only print: Name: oops or name: oops

**Problem 2.6**

System.out.println("look: " + e1);

Answer Correct: look: ID: 0; Name: oops or look:ID: 0; Name: oops

Explanation:
Same as 2.4, since toString() method is overrided, when call System.out.println(), it will print "look: " and what should be printed in the toString() method.

![Code Snippet](https://prod-edxapp.edx-cdn.org/assets/courseware/v1/7e50a69a86218a93639b5815d87926ad/asset-v1:PennX+SD1x+2T2017+type@asset+block/Quiz4.1P2.1.png)

**Problem 3.1**

In the code snippet above, when animal.speak() is called, what is the name, the power, and do we get to see 'Here comes the King' being printed out. In order to answer this please give your answer as name followed by space followed by the power followed by either the word Yes or the word No.

 Answer Correct: DEFAULT_NAME 3 no or DEFAULT_NAME 3 No or DEFAULT_NAME 3 NO
 
Explanation:
The constructor takes an int 3, which calls the 4th constuctor. In the constructor, it assigns 3 to the instance variable called field. So when speak() is called, the name will still be the default name, but the power will be 3. Here comes the king will not be printed because Animal is the super class and it will not inherit anything from the subclass.


**Problem 3.2**

In the code snippet above, when lion1.speak() is called, what is the name, the power, and do we get to see 'Here comes the King' being printed out. In order to answer this please give your answer as name followed by space followed by the power followed by either the word Yes or the word No.


Answer Correct: DEFAULT_NAME 10 Yes or DEFAULT_NAME 10 yes or DEFAULT_NAME 10 YES

Explanation:
The constructor of lion1 does not take any parameters. So it will call the default constructor of its super class, which is Animal. In the default constructor of Animal, name is DEFAULT_NAME, power is 10. lion1 therefore inherits the two attributes. "Here comes the king!!!" is printed because it overrides the method called speak in the Animal class.


**Problem 3.3**

In the code snippet above, when lion2.speak() is called, what is the name, the power, and do we get to see 'Here comes the King' being printed out. In order to answer this please give your answer as name followed by space followed by the power followed by either the word Yes or the word No.

Answer Correct: DEFAULT_NAME 10 Yes or DEFAULT_NAME 10 yes or DEFAULT_NAME 10 YES

Explanation:
The second constructor of lion2 is called. It takes a string; however, this value is not assigned to any attributes because super(string) is not called in the second constructor. "Here comes the king!!!" is printed because it overrides the method called speak in the Animal class.


**Problem 3.4**

In the code snippet above, when lion3.speak() is called, what is the name, the power, and do we get to see 'Here comes the King' being printed out. In order to answer this please give your answer as name followed by space followed by the power followed by either the word Yes or the word No.

Answer Correct: DEFAULT_NAME 99 Yes or DEFAULT_NAME 99 yes or DEFAULT_NAME 10 YES

Explanation:
The third constructor of lion3 is called. It takes an int and super(power) is called. In its parent class, the forth constructor is called. It assigns value to the power attributes.

**Problem 3.5**

In the code snippet above, when lion4.speak() is called, what is the name, the power, and do we get to see 'Here comes the King' being printed out. In order to answer this please give your answer as name followed by space followed by the power followed by either the word Yes or the word No.


Answer Correct: Simba 100 Yes or Simba 100 YES or Simba 100 yes

Explanation:
The last constructor of lion4 is called. super(name, power) will call the last constructor of its super class, which assign a value to the name attribute and a value to the power attribute. "Here comes the King!!!" will be printed for the same reason.

### Abstract classes and interfaces

**Problem 1**


All methods in an abstract class are abstract.

True

False -correct

Explanation:
An abstract class is any class that has at least one abstract method. But you could declare a class to be abstract even if you don't have abstract methods.


**Problem 2**

An abstract class can implement an interface.

True -correct

False

Explanation:
An abstract class can implement an interface.


**Problem 3**


Assume there is a method called "public double doThis(int x)" in an interface In order to implement this interface, we can define a method as:

public double doThis(int z) -correct

public int doThis(int y) 

private double doThis(int x)

public int doThis (int x, int y)

Explanation:
When implementing an interface, the method signature must be the same. The method accessor must be public.

 
**Problem 4**

Which of the following statements are correct?
In an abstract class, all its methods must also be abstract.

You can not create an instance of an interface, however, you can create an instance of an abstract class.

You can declare a class to be abstract even if it doesn’t have any abstract methods. -correct

When a class extends an abstract class, it must define all the abstract methods.

Usually, abstract class can be used as an “adaptor class” between interface and concrete class, if the author of the concrete class doesn’t want to define all the interface methods. -correct


Explanation:
In an abstract class, not all of its methods should be abstract. You cannot instantiate an abstract class.

 
**Problem 5**

Which of the following statements are FALSE?

Sometimes we make an interface method private. -correct

An interface doesn’t have any instance variables, because there won’t be any instance of an interface.

In Java, a class can extend only one superclass, but implement as many interfaces as you want.

If your class wants to implement an interface without defining all the interface methods, your class must be abstract.

Explanation:
All methods declarations in an interface must be public.
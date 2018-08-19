#### Week 3 : Collections and Object Oriented Design


##### Variable length arrays - ArrayLists

Problem 1

Which one of the following statements is wrong?
ArrayList is basically an Array that can resize itself.

A 2-dimensional ArrayList would be appropriate to represent a chess board. -correct

When an Array is full but we want to keep adding elements to it, we need to initiate a new Array with larger size and copy all elements from the old Array to the new Array.

Each row in a 2-dimensional Array doesn’t have to be the same length.
    

Explanantion: To represent a chess board, it is better to use a 2d array.


Problem 2

Select all the lines of code that would NOT compile from the following list. (Assume all necessary packages are imported. There might be more than one answer.)

ArrayList< String> stringList = new ArrayList<>();

ArrayList< int> intList = new ArrayList<>(); correct

int[ ] array = new int[3];

int[ ] array = new int[ ] {1, 2, 3};

int[ ] array = new int[ ]; -correct

Explanation:
Java syntaxes


![Code Snippet](https://prod-edxapp.edx-cdn.org/assets/courseware/v1/a951233c79bad3c9644478b5b69c7cb2/asset-v1:PennX+SD1x+2T2017+type@asset+block/Quiz3.1Problem3.png)

Problem 3

Which lines in the code snippet 1 would CAUSE ConcurrentModificationException?

7

7, 8

9

10

11 

11, 12 -correct

Explanation:
Java does not allow you to loop an ArrayList and modify it at the same time. If you do this, it will throw you the ConcurrentModificationException.

##### Access modifiers

![Code Snippet](https://prod-edxapp.edx-cdn.org/assets/courseware/v1/f082c547611ac77a8149c8c114e9b4e2/asset-v1:PennX+SD1x+2T2017+type@asset+block/Quiz_3.2.png)

**Problem 1**

What will be printed to console by the code snippet 1?

0, 1

1, 2

0, 679

1, 680

1, 681 -correct

1, 679


Explanation:
Static field is shared among all instances of the same class.

**Problem 2**

What gets printed if you remove the static keyword in the very first line (code snippet 1)?

0, 1

1, 1 -correct

0, 679

1, 680

1, 681

1, 679

Explanation:
Non-static field is not shared among all instances of the same class.

**Problem 3**

Select the correct statements from the following list:

When we want to access a private instance variable from outside the class, we can change it to private.

From the class-as-a-service point of view, Javadoc for private methods is not necessary. -correct

Generally, getter methods shouldn’t have side effects on the state of instance variables. -correct

Helper methods are usually private. -correct

Explanation:
When we want to access a private instance variable from outside the class, we can use the public getter method.
## SD1x SOFTWARE DEVELOPMENT FUNDAMENTALS

**week 1: Java Basics**

**Conditionals and Loops**

**Problem 1**

Choose all statements that would give you compile error.

double d = 2;

int n = 1.27; -correct

String s = 'I am a string';  -correct

String s = “I am another string”;

boolean b = true && “what?”;  -correct

boolean b = false || true;

String s = true;  -correct

Answer Correct:
Float or double hold decimal values. Char can have only single character.Integer cannot hold decimal values. String takes in a sequence of characters specified within double quotes. true is boolean when specified without quotes.

```
public static void main(String[] args) {
    int n = 93;
    double d = 1.27;
    double result = n - d;
    if (result > 0) {
        boolean b = result < 0;
        if (b) {
            System.out.println("this cannot be true!");
       }
     } else {
     String s = "wow";
     if (result >= 0 ) {
         s = "bravo!";
         System.out.println(s);
     } else {
         System.out.println(s);
    }
  }
}
``` 
    

**Problem 2**

What will be printed to console by the above code snippet 1? If nothing is printed, please respond with the word Nothing.

Answer Correct:
Blank or Nothing

Explanation:
result is larger than 0, thus enter the first if block; variable b's value is false, so do not enter the sub-block and do not print anything. 
    
```
    for (int i = 0; i < 0; i++) {
        System.out.println("wow");
    }
```
    
**Problem 3**

How many times is “wow” printed to console when the above code snippet 2 loop is executed?

0 -correct

1

Infinity 

Explanation:
It will not enter the for loop because i is not less than 0.

    
 ```
    int i = 0;
     while (i <10) {
         System.out.println("wow again");
     }
 ```
     

**Problem 4**

How many times is “wow again” printed to console when the above code snippet 3 loop is executed?

9

10

11 

Infinity -correct

Explanation:
i is not increased and it will be always be less than 10, and hence it is an infinite loop.

```
int j = 0;
for  (int i = 0; i < 93; i++) {
    j = i + 1;
}
int i = j;
System.out.println(i);
```

**Problem 5**

What number is printed to console when the above code snippet 4 is executed?

0

1

93 -correct

94

Answer
Correct: When i increments to 93, it will break the for loop. The last valid i to enter the for loop is i = 92. So j = 92+1=93. Then give the j's value to i. So i is 93 too.

**Classes**

**Problem 1**

In the Car example (discussed in the video), if we add a method to get the odometer reading before we fuel the car, what's the return type of this method?

void

int

double -correct

String

Answer
Correct: Odometer is usually a number with decimals, which is the type of double in java


**Problem 2**

What is the return type of the constructor for Car class?

Car

void incorrect

Object

no return type -correct

Ferrari

Explanation:
A constructor has no return type.


**Problem 3**

Could a constructor be parameter-less?

Yes  -correct

No

Answer
Correct: A constructor can have no parameters.

**Problem 4**

Will the following line of code be compiled: 

int this = 5;

True

False -correct

Answer
Incorrect: this is a reserved keyword in java. It refers to the current instance of the class, which is an object rather than a primitive type.

**Data Collections**

**Problem 1**

How do you declare an array of integers of size 10?

array int[ ] = 10;

int array = new int(9);

int[ ] array = int[10];

int array = new int[9];

int array[ ] = new int[10]; correct

Answer
Correct: This is the one of the syntaxes of declaring an array, which include: type, size, "new" key word and correct places of putting "[ ]"

**Problem 2**

What is largest index in an array of size n?

  Answer Correct: n-1 or n - 1
  
Explanation:
Java uses 0 based index.


```
public static void main(String[] args) {
    inst[] score = new int[] {88, 55 71, 98, 93};
    ArrayList<Integer> decentScores = new ArrayList<>();
    for (int i = 0; i < scores.length; i++) {
       if (scores[i] > 90) {
           decentScores.add(i);
       }                                                        
    }
    System.out.println(decentScores.get(1));
 }
   ``` 

**Problem 3**

What is printed to console by the code snippet 1?

98

93

4 -correct

5 

Explanation:
Java uses 0 based index; the index is being added to the ArrayList. It returns the second element (with index 1) from the ArrayList.

```
int[] arr = new int[] {8, 5, 15,23, 1,7};
for (int i = arr.length - 1; i > 0; i--) {
arr[i - 1] = arr[i];
}
System.out.println(arr[0]);
```

**Problem 4**

What does the code snippet 2 print out?

Answer Correct:
    7
 
Explanation:
After the for loop, all elements in the array becomes 7.




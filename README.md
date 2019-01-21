Question: Match the access modifier with its visibility.
The correct answers for this question are public : “visible by all classes in all packages”, private : “visible only in the class in which its defined”, default : “visible within the class in which it's defined, as well as by classes within the same package”, and protected : “visible within the class in which it's defined, by classes within the same package, and by subclasses of the class in which it's defined” This is the correct answer because the definition of each class tells us what the access modifiers can do. Default and protected classes are both “package-level access” classes, meaning that only classes in the same package can access it.

Question Consider the following requirements for a method I need to write.
Accepts a single parameter
If that parameter is a whole number, return the parameter unchanged.
If that parameter contains a fractional component, return the next largest whole number.
Here's my method definition.
public double mystery(double x) {

}
Which single line of code will adequately complete this method?:
The correct answer is return Math.ceil(x);. This is because the ceiling function always rounds up to the largest whole number when it is given a fraction. The floor function does the opposite and the round function is dependant on whether the fraction is above .5 or not.

Question: Consider the following method definition.
public static void saySomething(String something) {
   System.out.println(something);
}
Now, consider the following usages of this method.
saySomething("hello, there.");        // first usage
 
String message = "hello, there.";     // second usage
saySomething(message);
 
String something = "hello, there.";   // third usage
saySomething(something);
From the perspective of what is output to the console, what is the difference between the three ways in which the method is called?
The correct answer for this question is There is no difference. This is because all of the strings go through the same class and all say the same thing. The second choice is correct because, even though the string is now called message, it goes in the saySomething class and gets transfered into the string something, which then prints out the message.
 
Question: When writing a method, you must always include a(n)                             [ Select ]                          ["static identifier", "visibility indicator", "access modifier", "dynamic key"]           , a(n) return value , and the method name (in that order). Together, this is known as the method's                             [ Select ]                          ["method signature", "method name", "method identifier"]            

The correct answer is an access modifier because every method will start with an access modifier. This will tell the objects and classes which things it can access. The next answer is the return type. The return type is the data type that is required from the method that it will return. The return type can be null if needed. The last value is the method signature which is the name for the method. 

Question: Consider the following code snippet.
String str = "Hello, there. My name is Joseph. What's yours?";
char c = str.charAt(7);
What is the value of c after running this code? 
The correct answer is 't'. The reason it is ‘t’ is because char c = str.charAt(7); is a character data type. A character data type will be store with ‘’ and since the 7th index in String str = "Hello, there. My name is Joseph. What's yours?" is t, that is what you get.


Question: Consider the following method definition.
public long multiply(int a, int b, int c) {

}
Modify the following method definition so that it accepts three integers in the form of parameters, computes their product, and prints it to the console. The method should not return a value.:
The correct answer is public void multiply(int a, int b, int c) {System.out.println(a * b * c);} because it accepts the 3 integers and does not need to return anything. The other answers are wrong because the method either isn’t void, meaning that it must return a value, or doesn’t print out the answer.

Question: Consider the following method definition.
public int add(int x, int y) {
   return x + y;
}
Assuming I've created an object of the class in which this method is defined called test, how can I use this method to compute and store the sum of two integers?
The correct answer is int sum = test.add(123, 456);. This is because the answer initializes the sum, and then puts 2 different integers into the method that mentions the class it is in. The other answers are wrong because they dont do those 3 things.

Question: Consider the following method definition.
public double randomNumber(int seed) {
   if (seed > 1000) {
       return Math.random() * seed;
   } else if (seed > 500) {
       return Math.random() * seed * -1;
   }
}
I keep getting an error message telling me that my method must return a value of type double. What's wrong with my code?
The correct answer is For seed values less than or equal to 500, the method does not return a value. This is because the if statements both have conditions where seed is more than 500, but there is no condition if that is not true. The other statements are not right about the code.

Question: Let's assume I've got my Scanner object setup as shown below.
import java.util.Scanner;

public class Example {

   public void getInput() {
       Scanner s = new Scanner(System.in);

       // read user input (first and last name, then age)
       // TODO

       // print user input to the console
       System.out.println("Hello, " + name ". You're " + age + " years old.");
       s.close();
   }
}
Given the text printed to the console and the implied data types, which methods of the Scanner class should I use and how do I use them?
The correct answer is String name = s.nextLine();
int age = s.nextInt();. This is because the answer correctly uses the scanner functions and codes them correctly. The other answers do not have the right syntax to call the functions.

Question I want to print each character of a String one-by-one on a separate line. The number of characters in the String is unknown. You may assume the String is stored in a variable called str. How can I do this? Select all that apply.: 

The correct answer is for (int i = 0; i < str.length(); i++) {System.out.println(str.charAt(i));} and int i = 0; int length = str.length();
while (i < length) {
   System.out.println(str.charAt(i));
}. These are right because he is using System.out.println and it is printing each character individually on a line. The others are wrong because they don't go through the whole string, they start at the second character.

Question: Methods that return a value allow us to use them to perform some computation, and store (and later use!) the result of that computation.

The Correct Answer is True because one of the uses of a method is to create a collection of statements in order to recall and use later. 
False is not correct because it does not follow the definition of a method. 

Question: Which of the following are valid access modifiers for methods in Java? Select all that apply.
The Correct Answer is default, private, protected, and public because java access modifiers for methods include public, private, protected, and default.
The other answers are incorrect as package, dynamic, and static because they are not java access modifiers. . 

Question: public int add() 

}
The correct answer is 0 as a parameter is the type of data that a method can receive and this line of code is not a method. 
The other answers are incorrect as anything else than a 0 would mean that this line of code would be a method which it is not.


Question Consider the following lines of code,
String s = "abcdefg";
String sub1 = s.substring(s.indexOf("c"));
String sub2 = s.substring(s.indexOf("e"), s.indexOf("g"));
What are the values of sub1 and sub2 after running this code?
The correct answer is cdefg and ef because the first string sub 1 pulls the letter c and any characters to the end of the string while  string sub2  pulls the letter e and any letters until the letter g is met and which is also not included. 

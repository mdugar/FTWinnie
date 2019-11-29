# Sprint 09: Simple Java Program Structure

In our first program, we displayed a single message on the computer. We did this using the `System.out.println()` statement. This is a command in Java that we can use to perform certain actions.

Well, actually, `println()` is the statement really. `System.out` is the class that contains the `println()` statement we run. And every statement in Java ends with a semicolon. Every. One. It is like the period for a sentence.

You see, almost everything in Java is saved in something called a class. A class defines the rules for how parts of our program works. Later, you will learn how to work with classes more, and even how to make your own. For now, we will need to just work with the ones that we already have available to us.

When we run our code from before...

```java
System.out.println(“Hello, world!”);
```
...there are a few things that are going on.

First, everything around this line of code sets up our project in Java. Let’s look at it briefly:

```java
public class Main {  

    public static void main(String[] args) {  
        System.out.println("Hello, World");  
    }  
}  
```

In this example code, our `Hello, World` statement is within two specific code blocks. A code block is defined using a pair of curly braces, or `{ }`. These group the contents within them into a block.

Blocks have some rules around them, but we’ll cover those later. For now, just know that you can take blocks and put them inside of one another. So, in this example, we have a `public class Main` code block that starts on line 1 and ends on 6. We then have `public static void main` code block that starts on 3 and ends on 5.

Our code is within this inner code block.

The outer block defines the overall wrapper for our program, called a class. While the name of the class can vary, all Java programs must have a `public static void main` block to run. Java looks for this to execute when it builds and runs the program.

Until we get to object-oriented programming, all of your code will be in the Main.java file. Soon, we will also create code outside of the `public static void main` code block.

Those public, class, static, void statements? Just ignore them for now and focus on what we put into the constructor. Everything will make sense in time.

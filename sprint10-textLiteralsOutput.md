# Sprint 10: Text Literals and Output

Computers take things literally. Like, literally. So much that there are things actually called literals.

Literally.

"Hello, World" is a literal. A text literal to be precise.

A text literal contains letters and numbers and is denoted by a pair of quotation marks. The quotes mark the beginning and the end of the literal.

## Text Output

When you run a statement like `println()` it is looking for something called a string. A string is another word for text. Think of it like a sequence of letter beads on a string.

When you provide a string to a statement that uses a string, it will do something with it. In the case of `println()` it will print it to the screen, and then move to the next line.

So, if you have the following statements:

```java
System.out.println("Hello");
System.out.println("World");
```

This would output as:

```
Hello
World
```

Displaying both on two lines.

But there is another statement you can use, `print()`. This works the same way, but you don’t move to the next line after the text displays.

So, if you have the these statements:

```java
System.out.print("Hello");
System.out.print("World");
```

This would output as:

```
HelloWorld
```

Putting both characters on the same line.

## Escape Sequences

Text literals can contain special characters as well. Take the previous example:

```java
System.out.print("Hello");
System.out.print("World");
```

If you wanted to include a new line in the text literal itself, you can add it using the two-letter sequence `\n`.

This is called the newline character. And will create a line break in your text:

```java
System.out.print("Hello\n");
System.out.print("World");
```

Is essentially the same as: 

```java
System.out.print("Hello\nWorld");
```

And displays this on the screen:

```
Hello
World
```

How about this one?

If you wanted to display the following line, how would you do it?

```
Mike said, "Hey!"
```

This line of text has a quote in it, so if we created a text literal with it we would have:

```
"Mike said, "Hey!""
```

But the computer, again, is dumb. So, it will think that the quote before the H in Hey is the end of the literal.

Not what we wanted.

To get around this, we can use a escape sequence to tell the program that the quotes around Hey are part of the literal, not the boundaries of it:

```
"Mike said, \"Hey\""
```

Now the slash quote two-character sequence can allow the literal to include the quote.

There are others you can use too, including the tab space sequence.

The tab sequence, `\t` adds a tab space in your text. This is sometimes helpful to align things into columns if you get the right sequence set up.

Like this one:

```
"First\tMiddle\tLast"
"R.\tDouglas\tWinnie"
```

This would display as:

```
First   Middle		Last
R.      Douglas	    Winnie
```

The tab space shifts over to help line things up when you stack statements on top of one another.
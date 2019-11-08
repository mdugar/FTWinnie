# Sprint 06: How Java Works

Java is a unique programming language due to the “write once, run anywhere” mantra that was part of the original vision. How it makes this vision come to life is important to understanding how you work as a programmer.

## The Problem with Compiled Languages

Compiled programming languages generally have a big limitation. When you convert your code to an executable program, the compiler reads the code and creates a binary file that is specific to a processor architecture.

So, if I used a language like C or C++ to compile a program on my 32-bit Windows PC, that program can’t run on a Mac, nor can it run on a 64-bit Windows PC. It can only run on a 32-but Windows PC.

Every processor and operating system are expecting a program to meet extremely specific requirements. The way the program accesses the hardware is vastly different between Intel processors, ARM-based processors (like those found on phones and tablets), and other processor types like RISC architectures. (Older Macs used this type of architecture using chips called PowerPC chips like the G5 or G4.)

Even 32-bit Intel processors and 64-bit Intel processors operate completely differently. So 64-bit programs can’t run on 32-bit computers, and 32-bit programs can’t run natively on 64-bit computers.

When you expand to other types of computers like servers, the number of processor types and architectures can get even more complex.

Web and application servers can use vastly different architecture types like Sparc, Xeon, Itanium, and other types over the last couple of decades.

So, the folks at Sun Microsystems, when they designed Java, wanted to get past this limitation, so they created an innovative way to get around it.

## The JVM and JRE

When you run a Java program, you aren’t just running the program, you are running a few things at the same time.

For multiple platforms, Oracle has created a set or technologies called the Java Runtime Environment and the Java Virtual Machine. These are built so that the specific architectures of the hardware including Intel, ARM, 64-bit, 32-bit, and more can run Java programs.

These runtimes are installed on the system and stay resident, waiting for a Java program to be executed.

When a Java program is called to run, the Java Runtime Environment, or JRE kicks in, and opens the compiled program. The runtime environment then captures the instructions of the program and converts them to native executions on the computer. So, if the program requests to find the square root of a value, on a 32-bit machine, it will call the processor directive to calculate it. On a 64-bit machine, it will call the directive that is unique to that architecture.  

![Java architecture](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/javaArch.PNG)

This is what has made Java so universal. Wherever Oracle has created a JRE, you can run Java programs.

## Compiling Java Bytecode

When you create your Java program, there are a few things in play when you create your code, called source code or source.

![Java lifecycle](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/javaLifecycle.PNG)

First, when you create your program, you are writing a plain text file. There is no formatting, special characters, graphics, or anything other than letters and numbers. When you save this file to your computer, it is a `.java` file, meaning that the file extension is `.java`.

When you are finished coding your program, you take the file and send it to the compiler. The compiler takes the instructions you created and converts them to Java Bytecode, which the JRE can read and understand. The Java Bytecode (sometimes referred to a JBC) is a concise and compressed file that isn’t human readable but is designed to be understood and executed quickly by the JRE.

The JRE then takes those bytecode instructions and sends them to the native hardware to execute the program on the machine.

When you compile your program, you are creating these Java Bytecode files, called `.class` files and they will run in the JRE against the native hardware of the architecture.

## Pre-Compiled Files

Sometimes, you will want to have files that you use repeatedly in your program. These generally are sections of code that will never change but contain pre-built actions that you can execute and use in your own custom code.

Maintaining these files can be extensive, and when you make improvements to this code, you want to find a way to make it easy to take those improvements and bring them to other programs.

To make this easier, Java supports combining pre-compiled code into something called a JAR, or Java Archive. This is a single module that you can then bring into any program and access the actions and functions within it just as if they were part of your code.

If you ever want to update or change the JAR, you can just change that single reference, or overwrite the JAR file that your program points to and the updates are made.

## OpenJRE

Java is an open-source language, meaning that the community can build, change, and improve the language and the compiler.

As part of this, Oracle has created the OpenJRE and OpenJDK for the community to build and enhance. Oracle can then take contributes made by the open-source community and bring it into the official Oracle Java JDK and JRE. 

Oracle then adds additional security and other protections to ensure the applications that run on it are safe and secure. Because it is a packaged platform, this security is applied to any hardware, server or cloud infrastructures.

Android is largely built on Java, and starting with Android N, or Android Nougat, Google switched to the OpenJDK due to litigation with Oracle.

In the end, to you, it doesn’t matter which version of Java you are running. When you install any JDK and JRE, the source code, compiled files and execution of the programs is essentially the same.
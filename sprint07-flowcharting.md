# Sprint 07: Flowcharting

Programming and coding are just as much about thinking and planning as it is about sitting in front of a keyboard. Often, a developer needs to plot out in their mind or on paper how a program is going to work. This can make the coding process much easier, especially if you are working together with others on a project.

A flowchart is a common way to sketch out your program. It is exactly as it sounds: a chart that visually shows the flow of a program. In a flowchart, you connect various steps, decisions, and actions together into a string that follows the flow of how the program will operate.

Because the computer is so literal with how it processes your actions and code, a flowchart makes it easier to code more accurately the first time versus having to debug and thrash your way through code. Trust me, it is tempting to ditch the flowchart and go straight to the code, but if you are new, or relatively new to coding, it will save you a ton of time and force you to stop, pause, and sketch things out before you go to the keyboard.

## Flowcharting tools

There are a bunch of flowcharting tools you can use, some are pen and paper, and some are online.

### Paper

Just like how a writer journals in a notebook, or a designer sketches in a sketchbook, a developer can often sketch a flowchart using pen and paper. Sometimes making things tangible and tactile helps slow your brain down and be more thoughtful with your code and program.

If you want to go with the paper approach, you can get a stencil the help with your work. It helps make things a bit cleaner.

### Tablet and Stylus

If you have a tablet or laptop that supports a stylus like an iPad, Surface, or 2-in-1 laptop, there are lots of sketching apps that you can use for your flowcharting including OneNote, Adobe Illustrator Draw, Autodesk SketchBook, and more. Some specialized tablet apps can even detect the shapes you draw and convert them to template shapes.

### Apps

Apps like OmniGraffle, Sketch, Adobe XD, Visio, PowerPoint, and Illustrator are examples of apps you can download or purchase and use to build your flowcharts. These apps vary in what they can do, but they all can work for building a flowchart.

I use Visio a lot, and it has a cool feature where you can create the steps for your flowchart in Excel, and then import them into Visio to automatically create the flowchart. You can then resync the chart if you make changes in Excel.

## Flowcharting Basics

Flowcharts use different shapes to represent unique types of steps in the program or process flow. These shapes then determine what steps are being taken, and can also affect the direction the program flow can take

### Terminus

![Terminus](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/terminus.PNG)

A basic flowchart starts with the pill shape, this is called a terminus shape and is used when you start and end your flowchart. Inside, you write in either “Start” or “Stop” and can optionally define how the program does this in the shape.

Then you draw a line, with an arrow, pointing to the next step in the flowchart.

### Process / Action

![Process / Action](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/process.PNG)

An action, sometimes called a process, is represented by a simple rectangle. You create a single rectangle for every individual step that needs to be part of your program. We often combine multiple steps in our mind and think of them as a single action. So, something simple might seem like a single step, but it involves multiple actions.

You then create more steps in your flowchart and connect them using lines with arrows. They can turn and twist. They can be vertical or horizontal. It is entirely up to you.

### Input and Output

![Input and Output](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/io.PNG)

In your program, you will often need to get input from the user, or display output to them. These steps are represented by a parallelogram to distinguish them from other steps, and you describe it like any other action.

### Decisions

![Decision](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/decision.PNG)

Decisions branch the flow of a program based on the results of a question. The question must be answered with a “Yes” or “No” response. (You’ll find out why later in the class).

A decision step uses a diamond shape and has two paths that come off of it. One for “Yes”; one for “No.” You then connect these paths to different actions based on the results of the question.

These separate paths may reconnect at a later point, but that is all based on your program and when you want to make that happen.

### Annotations

Sometimes you can't fit everything into a shape, so it is fine to add annotations or notes to the flowchart. These can either be added descriptions or details about the step, or programming and coding notes for you or others when the coding starts.

### Other Shapes

There are other shapes for working with data, creating subprocesses, and other actions, but we will cover those later when we need them. For now, we will stick with these four basic shapes.

## Take out the trash

Let’s take a look at an example flowchart and you can see how this all comes together:

![Taking out the trash](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/flowchart.PNG)

The flowchart starts with a terminus, or terminal shape, labeled start.

Then an action is performed, “Open trash can”.

Next, we reach a decision. The answer to the question needs to be yes, or no. “Is the trash full?” If it is, you follow the yes path. If it isn’t, you follow the no path.

Depending on the path you take, you will continue from step to step following each action.

This chart has the decision paths meet back up to a single point, which is totally fine with a flowchart.

It then ends with the stop terminus.

## But is it really that simple?

No. It isn’t. Because we make assumptions all the time, and often those assumptions lead us into problems.

Part of a programmer’s job is to take complicated tasks and break them down into individual steps that can’t be broken down any further.

It is like looking at water and drilling down to the molecules and then the atoms that form it. You dive down to the smallest element that forms the basis of the object. Now take that principle and apply it to an action. We take for granted many steps that are part of a group of actions.

Let’s look at our previous example: Let’s take out the trash.

The phrase “take out the trash” probably conjures up a few things in your mind. If someone tells me, “Hey Doug, can you take out the trash please?” there are certain steps that already form in my head around what I have to do.

For my home, these are the steps I need to do.

First, I need to go to the kitchen and grab the full garbage bag out of the trash can, then I take it around the house and empty the smaller trash cans in the bedroom and bathroom into it. Then I take it to the curbside can and put it inside.

That’s it! I took out the trash.

But are those all of the steps? Did I break down everything enough to make sure that everything happens that needs to happen? What if I took the steps I mentioned and wrote them down and had someone follow them to-the-letter? Would they do what I expected?

No, they probably wouldn’t, because even with those steps there are some assumptions that I didn’t think of. For instance, if it is the day before trash pickup I need to put the curbside can on the street. When I say “trash” I see it as trash and recycling, but someone that would take me literally might not see that.

As a programmer, you need to be as accurate and literal as possible with your code. Breaking down actions into smaller actions is critical to being successful. With each line of code that you write, like “take out the trash” you need to define each statement or action that needs to happen within that to fulfill everything that you expect and for the action to be executed correctly.

So, when you break down a process or a task, put yourself in someone else’s shoes to see if the steps you outlined would make sense. If not, add the clarity and details you need to make it foolproof to get the desired results.
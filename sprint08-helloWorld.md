# Sprint 08: Hello, World

Coding requires knowing what to code, but also, how to combine the tools you use together to make the project work and share with others.
Before we start getting into some heavy coding, we should work on exactly how you should use the tools together.

Our workflow

For this class, we have the following tools available to us:

- GitHub
- IntelliJ
- Java JDK
- Email

Using these tools, we can create projects and share them with others, specifically me for when you are ready to turn in your homework.

The general workflow you'll use for project will be this:

1.	Create a new project in IntelliJ
2.	Code your project
3.	Compile and test/run your project
4.	Create a repo on GitHub
5.	Upload your code to GitHub
6.	Repeat 2-3-4-5 as necessary
7.	Share your repo directory

This sprint will go through the details of how to build your project step-by-step.

## Create your IntelliJ Java project

First, we need to create the basic structure for our project. To do that, we need to go into IntelliJ and create a new Java project using specific project templates.

### IntelliJ IDEA

When you launch IntelliJ for the first time, you will see the welcome screen. You can also open this screen from the **File > Open** menu item.

![IntelliJ Welcome window](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/welcomeWindow.PNG)

From here, we need to create a new project, so select, you guessed it, **"Create New Project"** from the window.

You will then see the New Project window. From here, you will define the parameters for your project and set up the initial folder structure and starter code to begin coding and building your project.

### First Time Only: Configure the JDK

One important component of your project is connecting it to the JDK. This isn't done automatically and needs to be done the first time you create a project and may need to be repeated each time you update the JDK on your machine.

The process is pretty simple:

At the top of the New Project window, click the **"New…"** button:

![New Project window](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/newProject.PNG)
 
When you click the **"New…"** button, you need to tell IntelliJ where the JDK is installed. On a Windows machine, it is usually located in the **"Program Files"** folder, on macOS, it is usually in the **"Library"** folder.
Select the location of the JDK and the main folder of the JDK, and then select **OK**:

![Select JDK folder](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/selectJDK.PNG)

You'll then see the version of the JDK appear at the top of the New Project window.

### Create Project

When you have the JDK configured, get started by having Java selected on the left and keep the library and framework options unchecked.

Click **Next** to continue from the New Project window.

On the next screen, you will configure the project template:

![Project templates](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/projTemplates.PNG)

Check **"Create project from template"** and then select **"Command Line App"**

![Template selections](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/templateSelection.PNG)

Click **Next** to continue.

Now you need to give your project a name. It is highly recommended to not have any special characters or spaces in your project name. Usually for homework, you can use the name that was part of the assignment. For now, we will use **"HelloWorld"**

Then you need to select where to save your project. You can choose the default folder, and when you create the project name it will create a subfolder for you. If you don't see it, create one under the IdeaProjects folder.

The third option is for the base package. The default package is called `com.company`, but we aren't going to use that so remove that and make sure the field is blank.

When you are done, you should see this: 

![New Project name and location](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/firstView.PNG)
 
Click **Finish** when you are ready.

IntelliJ will come to life and create the project structure, and a stub code file to help you get started.

### About Your Project

When the project is ready, you will see the IntelliJ interface display your main project code file, named `Main.java`. This file is where you will be building most of your project code in class assignments and homework.

On the right is the main coding area. This is where you will type your code in and you can see syntax errors, get contextual help with the features built-in to IntelliJ.

On the left is the project explorer. You can open and close this using the Alt-1 or Cmd-1 keyboard shortcuts.

The Project panel displays all the files that are in your project. The top level-folder is called the same name as the project you created. Inside, you will see a `src` folder. This contains the source code for your project. If you expand this, you will see more details of the files that are in your project, including the `Main.java` file that is already open on the right.

You will see other items here as well. The `.idea` folder contains project settings for IntelliJ that help reconfigure the IDE to your previous settings when you open the project again.
The External Libraries section displays all the Java archive files, or JARs that are part of your project. Remember that the Java JDK includes all the tools for Java in JAR files. If you expand this disclosure triangle, you can see all of them.
 
![The Project panel](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/projPanel.PNG)

With the initial framework of the project created, we can now write the code for our program and work with our local development environment that we have created in IntelliJ.

## Coding your project

In IntelliJ, you will write all your project code in the code panel. Each code file is opened in a tab. Double-clicking a file in the Project panel will open it up as a new tab.

When you create a new project, you will already have a tab open for the `Main.java` file. 

### Writing Your First Program

I know, I know. So much talking/writing/reading, and not enough coding. Let's put that frustration to rest by writing our first program.

Now, this program isn't going to do much. But that's ok. Keep it simple for now, and we will get more complex in time. Trust me.

In your code panel, you will see a line that says:

```java
// write your code here
```

Well, guess what? That's where your code goes!

Place your cursor at the end of that line of text and press Enter or Return.

Now, write the following line of code, making sure it is spelled, capitalized, and punctuated exactly as it displayed below:

```java
System.out.println("Hello, World!");
```

When you are finished writing that line of code, the code panel should look like what is shown in Figure 9.

With the program code complete, we can now compile, build, and run the program right inside of IntelliJ.

![Finished Main.java file](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/finishedMain.PNG)
 
### Compile and Run Your First Program

Open **Run > Run 'Main'** from the menu. This will compile your program into Java Bytecode, building a `.class` file that will be added to your Project panel.

You will see the program begin to compile and a new panel will open at the bottom, the Run panel. This will display the results of the compilation. If there are any errors, it will list them out. In this case, there are no errors and the program runs, displaying the text `Hello, World!` on the screen.

Congrats! You have built and run your first Java Program.

![Output of first program](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/firstRun.PNG)

There are some things we should look at in the Project panel however.  You'll see a new folder called `out`. This folder contains the compiled bytecode for your project.

You will see a file called `Main.class`. If you remember, this file is the compiled Java bytecode that runs in the JRE. This is stored here in your project to then run on the computer. The output of the program is directed to the Run (sometimes called the Output) panel.

Now that we have a successfully running project, we should save the code to GitHub if we ever need to go back to this point later if we make changes.

## Create your repo in GitHub

With our code saved on our local computer, we need to create a repo in GitHub for us to work with changes to our code and share it with other people.

First, open a browser and go to www.github.com. From there, we will create a new repo and upload our code.

Log into your account and you should see the dashboard, like the one that is shown below:

![GitHub.com Dashboard](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/ghDash.PNG)

From here, click the green **New** button on the left, or click the plus button next to your account gravatar and select **New repository**.

Give your repository a name, usually defined in the homework or assignment. For this example, we will use **HelloWorld**.

Give your repo a description, like **"First project in GitHub"**.

Keep the project Public and check the **Initialize this repository with a README** option. We will be using the README to share information about our project.

You can leave all of the other options as is. Your page should look like the one below:

![New repository settings](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/newRepoSettings.PNG)

Click the **Create repository** button at the bottom of the page.

You will now see the repository landing page, and you will see a single file, **README.md** has been created and added to your repository.

We can edit this file directly in GitHub. Click the pencil icon in the right side of the title bar where the **README.md** section starts.
 
![Editing README.md](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/editReadme.PNG)

This is in a special format called Markdown. We will learn more about Markdown later, but for now, you can add more details and notes about your project on this page.

Add this to the bottom of the file **"Serra High School, AP CompSci"**

At the bottom, you can now save this change, or commit it to the repository. Add a summary of the change, and then add an optional description like this:

![Commit change information](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/commitChangeInfo.PNG)

Then click the **Commit Changes** button at the bottom.

You will now see the changes shown on the page:

![Seeing changes made to README.md](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/readmeChanges.PNG)

You have just created your first commit. Commits are changes that you wish to add to your project and track changes over time.

## Upload your code to GitHub

Now that you have your repo created, you can upload your code and keep it online to share and track changes and versions.

First, make sure you are at the main landing page for your repo. On this page, click the **Upload Files** button on the page.

![Upload files button](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/uploadFiles.PNG)

Now, you can drag and drop files to the area on the page, or click the **choose your files** link and browse using the Explorer or Finder dialog box.

One trick to find your code file is to go back to IntelliJ.

From there, go to your Project panel and right click the code file you want to upload. Select **Show in Explorer** or **Show in Finder** option:
 
![Show in... Option](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/showIn.PNG)

That will then open a window and display the file. You can now drag and drop that into GitHub in the browser.

You will see the file added to the bottom of the file drop target zone:

![File ready to commit](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/fileReady.PNG)

Now, we can commit our changes. For the summary, put **"First code commit"** and then for extended description **"Display a statement on the screen"**.

Press the green **Commit Changes** button when you are finished.

GitHub will then process your changes and then display them in the repository window.
Sharing program output

In addition to your code, it is very important that you share the output from your program when you turn it in. To do that, we will create a text file and copy and paste the contents from the Run panel into the text file.

To start, create a new file in your repo, call it `output.txt`:

![Creating a text file](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/createTextFile.PNG)

From IntelliJ, go to your HelloWorld project and click inside the Run panel. If the panel isn't open, run the program again to display it.

Press Control-A or Command-A to select all, and then copy to the clipboard. Then go back to the new text file in GitHub and paste:

![Pasted output text](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/pasteOuput.PNG)

Go to the bottom of the page and press the **Commit new file** button.

## Share your repo

Now that your program is in GitHub, you can share the repo web address when you submit your homework assignment.

When you send the assignment, I will be able to see your program file, any notes or information you put in the `README.md` file, as well as the program output, all in one place.

I can then add comments to the commits and files in your repository.

As you make changes to your code, you can reupload and create new commits, updating the materials that are in GitHub. You can then look at previous commits and download files at different points in time if you need to get something that was lost or changed.
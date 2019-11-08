# Sprint 03: Setting Up GitHub

When you code, you need to have a location to store it and share that code with others to work with it and review it. Tools called code repositories are ideal ways to do this and there are several different types that are available for developers to use.

## GitHub

The one that we will use is called GitHub. GitHub is a free public code platform that developers use to build, archive, and manage coding projects for individual or group collaboration. It is built on the Git technology that is ordinarily used for private, internal projects, but GitHub build their public platform on Git to make it available to anyone.

To create a GitHub account is simple. Go to http://www.github.com/ and create an account there. For our use in class, please create your account as your Serra email address so I can easily identify your account.

When you create your account, be sure to go to GitHub Desktop to download the desktop client for Windows or macOS. You can download the installer here: https://desktop.github.com/

Install the client and sign into your account. You can then create a repository to keep track of the changes you make in your classwork projects. You can either create a single project to capture all of your homework assignments, or you can create an individual repository for each project. Whichever you choose is up to you.

## How GitHub Works

GitHub and Git create a special directory that it uses to keep track of all changes that you make to the files inside of it. When you make a change to a file, it tracks what the change was and notes that.

This is different than a backup. A backup creates a copy of everything that is in a folder. A change in Git and GitHub only records what changed, which can save a lot of space, and is much faster to process.

There are many advanced workflows and automations that you can tie into Git and GitHub, but we will only be using the platform to store and share projects and homework assignments.

There are ways to tie in GitHub directly into the IntelliJ IDEA IDE, but for simplicity, we will use the GitHub Desktop client to make, track, commit and sync changes to our GitHub account. Then you can send the URLs from your GitHub repository to me when you submit your homework.

## Lifecyle of a Repository

A repository, or repo, starts with the master branch, sometimes known as a trunk. For individual developers, or small teams, projects might only use a master branch and never create alternate versions of it. 

As the program evolves and new changes are made, they are saved to the repository by making a commit. A commit contains the changes to the code and a brief comment and description made by the developer on what changed for future reference. Over time, there will be dozens or hundreds of commits on a repository over time.

At some point a repository will need to split in some way. Either there needs to be simultaneous work and they don’t want to have code conflict with others, or a project needs to maintain an existing version and they want to do something else with it. In that case, a branch is created from the main trunk and development can happen in parallel with the original code.

At some point, a branch will need to rejoin the main development, and this is done by merging that branch back into the master trunk.

For open-source repositories it is common for a developer to find a helpful framework and want to add it to their own development environment. To do that, they would fork the repository, creating a copy in their own environment to work with and potentially make changes.

When a developer makes changes or improvements to a forked repository, they might want to contribute those changes back to the main repository they forked from. To do that, they submit a pull request back to the original repository. As part of this pull request, the developer outlines the changes that were made, and the person that receives the requests can compare the proposed changes to the repo by performing a diff, that shows the changes side by side from one another. 

![Figure 1: Repository lifecycle](https://github.com/sfdesigner/FTWinnie/blob/master/diagrams/fig1.PNG)

Repositories can vary in complexity from something very simple with a single or a handful of developers, to a large open-source project with tens of thousands of developers. Code repos are the core of how software developers work together on projects of any size.
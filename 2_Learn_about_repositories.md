# Learn about Repositories

>Create a new git repository on your computer

## Repositories

A repository is a collection of related items. In our case, it is a collection of files related to our engineering project. You can imagine it as a project folder with all the relevant files inside of it. In fact, that's what it will look like on your computer anyways. Sometimes they're called "repos" for short.

![repos](images/repos.png)

You tell Git what your project is and Git will start tracking all of the changes to that folder. This makes it a Git repository: a folder of items being tracked by Git. Git tracks when files are added, subtracted or even a single letter in a single file is changed. All of this plus who did it and when is tracked by Git. In software, tracking changes like this is called version control.

## Using Terminal

Terminal (or Bash) is a way to instruct your computer to do things by typing commands rather than clicking applications with your mouse. You can rename files, open files, create new folders, move between directories (folders) and more all by running typed commands. You can even use a text editor for code (like Vim or Nano) in your terminal and never have to leave!

Besides navigating your computer, you can also use programs in Terminal that have a command-line interface (CLI), meaning they can be run with commands in terminal. Git is one of these. The first part of the command lets your computer know you're talking to Git. The parts following that are the commands and the different options you want Git to act on.

In this tutorial you'll learn a few basic command-line actions (in addition to Git commands) for navigating your computer. Using a command line is a very important skill to have. It loads faster than a GUI and you can run commands fast without having to fiddle around with a mouse.

## Completing the Goal

You're going to create a new project folder and then initialize it as a Git repository. We'll name the folder 'hello-world' for this challenge.

Time to open up that terminal!

In your terminal window, type these commands, one at a time, pressing enter/return after each.

First, make a new folder:

```bash
mkdir hello-world
```

Then go into that folder:

```bash
cd hello-world
```

Finally, tell Git to initialize (start tracking) the folder you are now in:

```bash
git init
```

The last command should return something starting with "Initialized empty Git repository". The others commands do not return anything.

To double check the repository exists you can use the command `ls -a` and see the .git file or use the command `git status`.

You did it, Get checked and then move to commit!

>Show that you made a git repo successfully

### Handy Tips

Make a new folder (aka make directory)

```bash
mkdir <FOLDERNAME>
```

Navigate into an existing folder (aka change directory)

```bash
cd <FOLDERNAME>
```

List the items in a folder

```bash
ls
```

List hidden items in a folder

```bash
ls -a
```

Turn Git on for a folder

```bash
git init
```
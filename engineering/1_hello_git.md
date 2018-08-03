# Hello Git

Git is an open source distributed version control system. Which means...

* Open Source
  * You are free to use, alter, edit, resell, and mess around with Git however you see fit.
* Distributed
  * No single point of failure. If you are using Git to collaborate, everyone
    on your team has a full backup of the entire project.
* Version Control
  * Git remembers the history of all your files so you don't have to!
    This makes reverting to previous versions easy and losing files hard.

Git should probably already be installed on your raspberry pi. Type `git --version` in your terminal and if it returns a version number higher than 1.7.10, you're set!

Your probably filling out forms in all your other classes to let your teachers know who you are. So might as well do the same with Git?

Set your name:

```bash
git config --global user.name "Your Name"
```

Set your email:

```bash
git config --global user.email "youremail@example.com"
```

And just so that we're all on the same page set Nano to the default editor for git:

```bash
git config --global core.editor "nano"
```

So now that Git knows who you are let's make a repository.

A repository is a collection of related files and in most cases it's a folder for storing a project. You can store code, pictures, and even 3D parts in a repository!

![repos](../images/repos.png)

In order for Git to start tracking a repository you need to tell it to do so. Make a new directory called hello-world and go into it. Once inside use this command to start tracking this repository:

```bash
git init
```

If you don't see something that starts with "Initialized empty Git repository" that may be a problem.

If not congradulations you just made your first Git repository! To double check the repository exists you can use the command `git status`.

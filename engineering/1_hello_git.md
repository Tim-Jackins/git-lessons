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

Git should already be installed on your Raspberry Pi. Run the command
`git --version` in your terminal and make sure it returns a version number
higher than 1.7.10.

You haven't introduced yourself to Git yet! Let's do that now. Git doesn't
really care what your name or email is, but it's helpful for your teammates
to see who wrote which pieces of code.

Set your name and email:

```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```

And just so that we're all on the same page, set Nano to the default editor for git:

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

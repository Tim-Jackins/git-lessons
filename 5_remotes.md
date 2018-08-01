# Bring a Remote Into the Mix

When you put something on GitHub that copy lives on one of GitHub's servers. This makes it a remote repository because it is not on your computer, but on a server, "remote" and somewhere else. By pushing your local (on your computer) changes to it, you keep it up to date.

Others can always then get the latest from your project by pulling your changes down from the remote (and onto their computer). This is how everyone can work on a project together without needing access to your computer where your local copy is stored.

![remotes](images/remotes.png)

## Create a Remote Repository

You want to sync your local version with one stored on GitHub.com. First create a new remote repository on GitHub.com. Sorry for the following annoyingly itemized steps:

1. Go to github.com, log in, and click the '+' in the top right and then click 'New repository'.
2. Give it a name that matches your local repository's name, 'hello-world', and a short description.
3. Make it public. This means it'll be listed on your public profile.
4. Don't initialize with a README because we already have a file, locally, named 'readme.txt'. This is a helper option from GitHub if you hadn't already made it.
5. Leave '.gitignore' and 'license' set to 'none'. We won't use them in this tutorial.
6. Click create repository!

## Connect your Local to your Remote

Now you've got an empty repository started on GitHub.com. At the top you'll see 'Quick Setup', make sure the 'HTTPS' button is selected and copy the address. This is the address of your repository on GitHub's servers.

Back in your terminal, and inside of the 'hello-world' folder that you initialized as a Git repository in the earlier lesson, you want to tell Git to remember the address of the remote version on GitHub's servers. You can have multiple remotes so each requires a name. The primary remote is typically named origin.

To add a remote named 'origin' to your repository:

```bash
git remote add origin <URLFROMGITHUB>
```

Your local repository now knows where your remote repository, named 'origin', lives on GitHub's servers. Think of it as adding a name and address on speed dial now when you need to send something there, you can.

## Push your work to your Remote

Next you want to push (send) everything you've done locally to your remote repository on GitHub. This is something you'll do often so that your remote version is up to date and matching the state of your local version.

Git has a branching system so that you can work on different parts of a project at different times. We'll learn more about that later, but by default the first branch is named 'master'. When you push (and later pull) from a project, you tell Git the branch name you want and the name of the remote that it lives on.

In this case, we'll send our branch named 'master' to our remote on GitHub named 'origin'.

```bash
git push origin master
```

Upon putting in this command it may ask you for a username and password. This is so that GitHub knows that you have permission to push to this remote. To store your credentials use this command:

```bash
git config credential.helper store
```

If it doesn't work don't worry about it.

Now go to your remote repository's page on GitHub.com and refresh the page. Wow! Everything is now the same locally as it is remotely. Congrats on your first public repository!

>Show that you have a public repo

### Handy Tips

Add remote connections

```bash
git remote add <REMOTENAME> <URL>
```

Set a URL to a remote

```bash
git remote set-url <REMOTENAME> <URL>
```

Pull in changes

```bash
git pull <REMOTENAME> <BRANCHNAME>
```

View remote addresses

```bash
git remote -v
```

Push changes

```bash
git push <REMOTENAME> <BRANCH>
```

What are...

* README
  * A README explains what the project is, how to use it, and often times, how to contribute (though sometimes there is an extra file, 'CONTRIBUTING.md', for those details).

* .gitignore
  * A .gitignore is a list of files that Git should not track for instance, files with passwords!

* LICENSE
  * A LICENSE file is the type of license you put on your project. This lets others know how they can use it. Information on the types is here: choosealicense.com.

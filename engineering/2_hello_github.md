# Hello GitHub

Now that you've got a repository started, let's create a text file in it (nano `<your filename>`). Call it something fun and write something cool in it. Now let's check out some of that Git file tracking.

First, use this command to have Git let you know what it's seeing:

```bash
git status
```

Hmm, Git saw that your file exists but it still isn't tracking it. You need to `add` the file you made  and `commit` your changes to the repository.

```bash
git add <the name of your file>
git commit -m "<a brief description of your work (ei: I just made a new file!)>"
```

Okay, now go back to that file and add a line of text--or remove a line--and try this command:

```bash
git diff
```

Pretty cool, right? Git remembered what your file looked like the last time you committed, and is showing you the changes you made to your file since then.

Now that Git is fully tracking that file you can use `add` and `commit` changes. Let's check the status of our repo (*pst:* `git status`). Interesting, instead of telling us that the file you made is untracked Git is it's been modified. From here on out when you use the `add` command you will be adding specific changes inside of files, not the files themselves. The `diff` command is what you can use to double check changes that Git sees before you `add` and `commit` them. So now let's save those changes:

```bash
git add <the name of your file>
```

The command looks similar to the first add right? By adding with the filename you are telling Git to `add` all the changes to that file. Now let's `commit`, this command is the same as it was above:

```bash
git commit -m "<a brief description of your work (ei: Added some changes to a file)>"
```

## Bringing a Remote Into the Mix

What's more fun than a repo stored in one place? A repo stored in two places! In order to share your code with teammates, you'll need to put it somewhere *remote*ly where you can both reach it. GitHub provides this service for free! Once your repo is on GitHub, other people, can pull (copy and download) changes from the remote and, if you let them, push (copy and upload) their changes to the remote.

![remotes](/images/remotes.png)

This is the structure Git uses for online collaboration.

"Did someone say online collaboration? I already know how to collaborate online, I'll make a Drive folder and share it with everyone but wait... How am I going to get code from my Pi onto Drive?"

While Drive works well for sharing in some cases, Git has a better way of going about it, especially relating to code.

You're going to need to [make a GitHub account](https://github.com/join) to use their services. Once that's done, go ahead and [make an new empty repo](https://github.com/new) on GitHub. Name it `hello-world` and do not initialize with a README, LICENSE, or a .gitignore!

If you make it succesfully, then you should see a screen talking about 'Quick Setup' and showing you an HTTPS link. That link points to an empty space, on GitHub's servers, that GitHub has allocated for your repo. Now we have to give our repository directions on where to push commits so that they get saved in this new space. This is called adding a remote and here's the command to do it:

```bash
git remote add origin <URL from GitHub>
```

`origin` is that name that we are assigning to the remote. You can name your remote anything but for the sake of convention we are calling it origin.

So now let's push our local repository to the remote.

```bash
git push origin master
```

Your terminal is going to ask you to put in your GitHub username and password so that it push code to your remote repo.

Now go to your remote repository's page on GitHub.com, and refresh the page. Wow! Everything is now the same locally as it is remotely. Congrats on your first public repository!

Going forward you may want to keep all your code backed up with Git on GitHub, whether it's for a project or just a lesson, just in case your Raspberry Pi fails.

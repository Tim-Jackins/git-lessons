# Hello GitHub

Now that you've got a repository started, let's create a text file in it (`nano <your filename>`). Call it something fun and write something cool in it. Now let's check out some of that Git file tracking.

First, let's ask Git what's going on in your repository:

```bash
git status
```

Hmmm, Git saw that your file exists, but it still isn't tracking it. You need to `add` the file you made and `commit` your changes to the repository. The `git commit` command will open your default editor, nano, and prompt you to enter a commit message. This message should be brief but describe the changes you made in the commit. For example: `Created <the name of your file>`.

```bash
git add <the name of your file>
git commit
```

Okay, now go back to that file and add a line of text--or remove a line--and try this command:

```bash
git diff
```

Pretty cool, right? Git remembered what your file looked like the last time you committed, and is showing you the changes you made to your file since then.

Let's check the status of our repo (*pst:* `git status`). Hmmm, interesting, instead of telling us that your file is untracked, Git just says it's been modified. Once Git is tracking a file, `git add` will add specific changes inside of the file, not the file itself. Now `add` and `commit` your changes.

## Bringing a Remote Into the Mix

What's more fun than a repo stored in one place? A repo stored in two places! In order to share your code with teammates, you'll need to put it somewhere *remote*ly where you can both reach it. GitHub provides this service for free! Once your repo is on GitHub, other people, can pull (copy and download) changes from the remote and, if you let them, push (copy and upload) their changes to the remote.

![remotes](/images/remotes.png)

This is the structure Git uses for online collaboration.

"Did someone say online collaboration? I already know how to collaborate online, I'll make a Drive folder and share it with everyone but wait... How am I going to get code from my Pi onto Drive?"

While Drive works well for sharing in some cases, Git has a better way of going about it, especially relating to code.

You're going to need to [make a GitHub account](https://github.com/join) to use their services. Once that's done, go ahead and [make a new empty repo](https://github.com/new) on GitHub. Name it `hello-world` and do not initialize with a README, LICENSE, or a .gitignore!

If you make it successfully, then you should see a screen talking about 'Quick Setup' and showing you an HTTPS link. That link points to an empty space, on GitHub's servers, that GitHub has allocated for your repo. Now we have to give our repository directions on where to push commits so that they get saved in this new space. This is called adding a remote and here's the command to do it:

```bash
git remote add origin <URL from GitHub>
```

`origin` is the name that we are assigning to our remote. If you add other remotes later you would switch out `origin` for a different name when you run this command.

So now let's push our local repository to the remote.

```bash
git push origin master
```

Git will prompt you for your GitHub username and password in order to authorize the push. Keep in mind that these credentials are case-sensitive.

Now go to your remote repository's page on GitHub.com, and refresh the page. Wow! Everything is now the same locally as it is remotely. Congrats on your first public repository!

Going forward you may want to keep all your code backed up with Git on GitHub, whether it's for a project or just a lesson, just in case your Raspberry Pi fails.

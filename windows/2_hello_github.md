# Hello GitHub

Now that you've got a repository started, let's create a text file in it (`nano <your filename>`). Call it something fun and write something cool in it. Now let's check out some of that Git file tracking.

First, let's ask Git what's going on in your repository:

```bash
git status
```

Hmmm, Git saw that your file exists but it still isn't tracking it. You need to `add` the file you made and `commit` your changes to the repository. The `git commit` command will open your default editor, nano, and prompt you to enter a commit message. This message should be brief but describe the changes you made in the commit. For example: `Created <the name of your file>`.

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

You may be used to using Drive for collaboration in some cases; however, Git has a better way of going about it, especially relating to code.

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

This year we are going to move away from using the wiki and instead are going to make your engineering notebook a repo! This means two things:

You must...

- make a new repo called `Engineering-4-notebook` and push it to GitHub
- store all of your lessons, and your write-ups in this repo

I suggest ordering your notebook like so, see below, but you can order it however you like.

```bash
Engineering-4-notebook
├── Bash
│   └── hello_world.sh
├── Python
│   ├── calculator.py
│   └── dice_roller.py
└── README.md
```

You might be wondering "Hey wait a minute what's that .md file?" All the stuff you would normally put in your sigma wiki will instead be in the .md file. To make your file look pretty [use this guide](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

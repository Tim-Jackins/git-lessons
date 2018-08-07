# Hello GitHub

Now that you've got a repository started, let's add a text file to it. Call it something fun and write something cool in it. Now let's check out some of that Git file tracking.

First, try this command:

```bash
git status
```

Hmm, Git saw your file but it still isn't tracking it. You need to `add` the changes you made in that file and `commit` your changes to the repository.

```bash
git add <Filename>
git commit -m "<insert a brief description of your work>"
```

Okay, now go back to that file and add a line of text--or remove a line--and try this command:

```bash
git diff
```

Pretty cool, right? Git remembered what your file looked like the last time you committed, and is showing you the changes you made to your file since then.

## Bring a Remote Into the Mix / Hello GitHub

What's more fun than a repo stored in one place? A repo stored in two places! In order to share your code with teammates, you'll need to put it somewhere *remote*ly where you can both reach it. GitHub provides this service for free! Once your repo is on GitHub, other people, can pull/(copy and download) changes from the remote and (if you let them) push/(copy and upload) their changes to the remote.

![remotes](../images/remotes.png)

You're going to need to [make a GitHub account](https://github.com/join) to use their services. Once that's done, go ahead and [make an new empty repo](https://github.com/new) on GitHub.

If you make it succesfully, then you should see a screen talking about 'Quick Setup' and showing you an https link. That links points to your empty space that GitHub has allocated for your repo. So here's how you tell your local repo to treat that space as its remote.

```bash
git remote add origin <URL from GitHub>
```

So now let's push our local repository to the remote.

```bash
git push origin master
```

Now go to your remote repository's page on GitHub.com, and refresh the page. Wow! Everything is now the same locally as it is remotely. Congrats on your first public repository!

Going forward you may want to keep all your code backed up with Git on GitHub, whether it's for a project or just a lesson, just in case your Raspberry Pi fails.

There are a lot of really cool Git features that we skipped over for the sake of time. If you're curious, there are [plenty of online resources](http://try.github.io/) to help you learn more. GitHub also has some [handy functionality](https://guides.github.com/) that could be useful to your project.

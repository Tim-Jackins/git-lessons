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

Here comes the distributed part of Git. So in order to collaborate with teamates you'll need to put it somewhere *remote*ly where you can both reach it. GitHub provides these services for free! Once your repo is on GitHub anyone, who has premission to, can pull/(copy and download) changes from the remote and push/(copy and upload) their changes to the remote.

![remotes](../images/remotes.png)

You're going to need to make a GitHub account to use their services. Once that's done go ahead and make an new empty repo on GitHub.

If you make it succesfully then you should see a screen talking about 'Quick Setup' and showing you an https link. That links points to your empty space that GitHub has allocated for your repo. So here's how you tell your local repo to treat that space as it's remote.

```bash
git remote add origin <Url from GitHub>
```

So now let's push our local repository to the remote.

```bash
git push origin master
```

Now go to your remote repository's page on GitHub.com and refresh the page. Wow! Everything is now the same locally as it is remotely. Congrats on your first public repository!

Going forward you may to keep all your code, whether it's for a project or for the lesson, backed up with Git on GitHub just in case your Raspberry Pi fails.

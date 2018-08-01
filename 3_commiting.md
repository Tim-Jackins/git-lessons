# Commit *this* to memory

>Stage changes and make a commit to your repository

## Create a new File

Now that you've got a repository started let's add a file to it.

Open your text editor and create a new empty file. If you don't know how to do this check the [tips section](#handy-tips). Now write a little bit of text, perhaps type "Hello!", and save the file as 'readme.txt' in the 'hello-world' folder you created in the last challenge.

## Check Status + Stage/Add and Commit Changes

Next check the status of your repository to find out if there have been changes. You know you have changed something, but does Git?

Make sure you're still within your 'hello-world' directory when you're running these commands. Use Git to see what changed in your repository:

First, check the status:

```bash
git status
```

Git should tell you that a file has been added.

Then add the file you just created so that it becomes a part of the changes you will commit (aka save) with Git:

```bash
git add readme.txt
```

Finally, commit those changes to the repository's history with a short message describing the updates.

```bash
git commit -m "Created readme"
```

## Make More Changes

Now add another line to 'readme.txt' and save the file again.

In terminal, you can view the difference between the file now and how it was at your last commit.

Tell Git to show you the diff:

```bash
git diff
```

Look at the info you get and think about what each number might mean. Play around a little adding and removing text and try to understand this print out. When you finish exploring commit your changes and get checked.

>Show that your changes are up to date and that you looked at the `git diff` print out.

### Handy Tips

Open file with Nano

```bash
nano <FILENAME>
```

Save changes and then exit while in Nano

```console
Ctrl + o
Enter/return
Ctrl + x
```

Check status of changes to a repository

```bash
git status
```

View changes to files

```bash
git diff
```

Add/Stage a file's changes to be committed

```bash
git add <FILENAME>
```

To add all files changes

```bash
git add -A
```

To commit (aka save) the changes you've added with a short message describing the changes

```bash
git commit -m "your commit message"
```

To commit with a longer message (this will automatically open up your git text editor)

```bash
git commit
```

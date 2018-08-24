# Forking and Cloning

Now you know how to make a repo, attach a remote, and put your work on GitHub! As impressive as this is, it's only half the fun. The other half is collaborating with others online.

Let's look at [cool-repo](https://github.com/chssigma/cool-repo). Look through its contents to get a sense of what you need to add. I'll give you a hint: it's your GitHub info and name to a particular table. So now you know what you need to add... but can you? You can't push commits to this repo, because you haven't been added as a collaborator, but that won't stop you from collaborating!

It's time to fork and clone!

## Fork

Forking is when you copy a repo to a different location on GitHub's servers. Because you have ownership over this copy, you can push commits to it.

Click on the "Fork" button in the top right corner of the [webpage](https://github.com/chssigma/cool-repo). Once the animation is finished, look at the top left corner of the screen. If you see something saying "forked from chssigma/cool-repo", you have successfully forked your first repo.

## Clone

Cloning is when you make a local copy of a repo. As a bonus, it stores the URL you used to clone in a remote named "origin".

Pull up your Git bash terminal in an empty folder, and clone your fork of `cool-repo` over HTTPS with this command:

```bash
git clone https://github.com/<your GitHub Username>/cool-repo.git
```

You now have a local copy of your fork of `cool-repo`! Add your name to the appropriate table and commit and push your changes to `origin master`. Here's a cool diagram describing what you did:

![clone](/images/clone.png)

So now you need a way to get the changes you just committed back into the main repository owned by chssigma. Lucky for you, GitHub has a way to do this built-in, it's called a pull request.

Head back to your fork of `cool-repo`, should be `https://github.com/<your username>/cool-repo/`, click on "Pull requests" in the menu bar near the top of the screen, and then click on "New pull request".

Double check that your changes are listed correctly and then create your pull request! Once you've done that, you simply have to wait for a collaborator, Mr. Timmins, on `chssigma/cool-repo` to pull in your changes.

Here's your diagram:

![pullrequest](/images/pullrequest.png)

Either Mr. Timmins will approve your pull request or he will leave a comment explaining what you need to fix. You can check on your request [here](https://github.com/chssigma/cool-repo/pulls/). If you end up having to make changes, all you need to do is edit your repo locally and then add, commit, and push them.

The fork, clone, and pull request method is how most strangers collaborate with each on GitHub. Congratulations, you have the tools to become an open source collaborator!

There are a lot of really cool Git features that we skipped over for the sake of time. If you're curious, there are [plenty of online resources](http://try.github.io/) to help you learn more. GitHub also has some [handy functionality](https://guides.github.com/) that could be useful to your project.

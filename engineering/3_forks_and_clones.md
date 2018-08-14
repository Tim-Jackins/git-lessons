# Forks and Clones

Now you know how to make a repo, attach a remote, and put your work on GitHub! As impressive as this is it's only half the fun. The other half is collaborating with others online.

"Online collaboration with classmates? Ugh, that means we have to pass around my laptop and have everyone slowly type their emails into a drive folder... Right?"

While this is the norm for services like drive, Git has a different way of going at it.

Let's look at [cool-repo](https://github.com/chssigma/cool-repo). Look through it's contents to get a sense of what you need to add. I'll give you a hint it's your GitHub info and name to a particular table. So now you know what you need to add... but can you? You can't commit changes to this repo, because you haven't been added as a collaborator, but there is an interesting work around.

It's time to fork and clone!

Fork

Forking is when you make an editable copy a repo to a different location on GitHub's servers.

Click on the "Fork" button in the top right corner of the webpage. Once the animation is finished you should see your new forked repo!

Clone

Cloning is when you make a local copy of a repo. As a bonus it comes with an "origin" remote already setup.

Pull up a terminal on your pi, head to the home directory (`cd ~`), and clone the repo over HTTPS with this command:

```bash
git clone https://github.com/<your GitHub Username>/<your repos name>.git
```

You now have your very own copy of cool-repo! add your name to the appropriate table and commit and push your changes.

You're a majority of the way done with the tutorial! Here's a cool diagram describing what you did:

![clone](/images/clone.png)

So now you need a way to get the changes you just commited back into the main repository owned by chssigma. Lucky for you Git has a way to do this built in, it's called a pull request.

Head back to your fork of cool-repo, should be `https://github.com/<your username>/cool-repo/`, click on "Pull requests" in the the menu bar near the top of the screen, and then click on "New pull request".

Double check that your changes are listed correctly and then create your pull request! Once you've done that you simply have to wait for a collaborator on chssigma/cool-repo to pull in your changes. Here's your diagram:

![pullrequest](/images/pullrequest.png)

The fork, clone, and pull request method is how most strangers collaborate with each on GitHub. So congradulations you have the tools to become an open source collaborator!

There are a lot of really cool Git features that we skipped over for the sake of time. If you're curious, there are [plenty of online resources](http://try.github.io/) to help you learn more. GitHub also has some [handy functionality](https://guides.github.com/) that could be useful to your project.

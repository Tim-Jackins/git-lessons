# Getting GitHub

The repository you've created so far is just on your computer, which is handy, but makes it pretty hard to share your work and collaborate with others. No worries, that's what GitHub is for!

GitHub is a website that allows people everywhere to upload what they're working on with Git so that everyone can easily work together on the same project. GitHub acts as the central repository for you and everyone else to share. You push your changes to it and pull down changes from others.

## Create a Github Account

Visit [github](https://github.com) and sign up for a free account.

## Add GitHub username to your Git Config

Save it exactly as you created it on GitHub and capitalize where capitalized. Note, you don't need to enter the "<" and ">".

Add your GitHub username to your Git configuration:

```bash
git config --global user.username <Username>
```

You can double check what you have set in your Git config by typing:

```bash
git config --global user.username
```

>Show that you have git configured correctly and that you have a github account
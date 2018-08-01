# Getting Started

>Install and configure git

## Install

Already have Git or not sure? Type git --version in your terminal and if it returns a version number higher than 1.7.10, you're set! For more information, visit the Git website.

## Verify

Once Git is installed, open your terminal. You can verify that Git is really there by typing:

```bash
git --version
```

This will return the version of Git on your computer and look something like this:

```bash
git version 2.17.1
```

Next, configure Git so it knows to associate your work to you:

Set your name:

```bash
git config --global user.name "Your Name"
```

Now set your email:

```bash
git config --global user.email "youremail@example.com"
```

And just so that we're all on the same page set Nano to the default editor for git:

```bash
git config --global core.editor "nano"
```

You're done with your first challenge!

>Show that your name, email, and editor have all been configured correctly

P.S. At the end of every lesson in order to move on you must get checked by Dr. Shields or Jack. The thing needing to be checked will appear in qoute style (like the above objective).

### Handy Tips

Set your name:

```bash
git config --global user.name "Your Name"
```

View your name:

```bash
git config --global user.name
```

Set your email:

```bash
git config --global user.email "youremail@example.com"
```

View your email:

```bash
git config --global user.email
```

Universally most configs can be displayed by simply not type the text after the command.
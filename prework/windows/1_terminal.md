Setup for Windows
-----------------

This guide will help you setup a software development environment on [Windows 7](http://windows.microsoft.com/en-us/windows/home) and above. By the end, your computer will be configured with the same state-of-the-art tools used by professional software developers.

This guide is mostly compatible with older versions of Windows. So follow along as best you can while Googling any problems you come across.


### The Terminal

Included in Windows is the **Terminal**—an app that runs a Unix shell.

A **Unix shell** is a command line user interface between you and your computer's operating system. You're probably most familiar with the graphical user interface of your computer's operating system. While that's technically a shell too, most programmers think of the textual, command line interface when they hear to word _shell_.

Sadly, Windows **does not** include a Unix shell. Let's fix that.

CAVEAT: Until Windows adopts more Unix standards, please be aware that any Unix-based tools written for Windows will inevitably have some quirks.


### Install Git for Windows

[Git for Windows](http://msysgit.github.io/) is a lightweight, native set of tools that bring the full feature set of Git to Windows. It includes **Bash**, a popular Unix shell, which you'll use to run the `git` command line just like other Unix environments.

To get started, download and install [Git for Windows](http://msysgit.github.io/). There are a bunch of installation options, but you can use the defaults if you're feeling overwhelmed.

Once installed, use the Start Menu to launch Git Bash.

![](https://i.imgur.com/9CKUGs5.png)

**TIP:** Don't be distracted by the **Git GUI** program.

Once launched, you'll see something like this.

![](https://i.imgur.com/hyjvQkW.png)

Ignoring the welcome message and the git help, here's a quick break down of what you're seeing in the Terminal app.

| Component             | Description                            |
| --------------------- | -------------------------------------- |
| `Ryan Sobol`          | Name of your user account              |
| `PHOTON-PC`           | Name of your computer                  |
| `~` (home directory)  | Name of your working directory         |
| `$`                   | Prompt symbol                          |

Any characters you type will appear after the `$` prompt symbol. Go ahead and type `uname`. After pressing the Enter key, you'll see something like this.

![](https://imgur.com/muRRwcK.png)

Here's what happened:

1. The shell waited for you to type a command.
1. You then typed the word `uname` which appeared after the prompt.
1. You pressed the Enter key which triggered the shell to accept your input.
1. The shell searched for a program called `uname`.
1. Once found, the shell launched the `uname` program and handed it control over the Terminal.
1. While running, the `uname` program told the Terminal to display the word `MINGW32_NT-6.1`.
1. Once finished, the `uname` program exited and handed control of the Terminal back to the shell.
1. The shell told the Terminal to display another prompt.
1. Once displayed, the shell began waiting for your next command.

Simply stated, a Unix shell works like a read-evaluate-print loop or **REPL**.


### Change the Terminal

The default Terminal app in Windows has no support for copy and paste keyboard shortcuts. Weak! Let's change that.

To get started, download [Console](http://sourceforge.net/projects/console/)—a modern Terminal app for Windows. Once downloaded, extract the app to `C:\Program Files` like this.

![](https://i.imgur.com/YQwoRp5.png)

Once extracted, add a shortcut the Start Menu.

![](https://i.imgur.com/KzFbpDI.png)

Launch the Console app and ignore the security warning. Navigate to the `Edit > Settings` menu item and check the box on the **bottom left** to "save settings to user directory".

![](https://i.imgur.com/bk1epeX.png)

Click the OK button to save and close the Console app for now.

Back in the original Git Bash window, run the following command.

```
curl -fsSL http://git.io/Fafs | sh
```

**TIP:** To paste, right click the title bar and choose `Edit > Paste`.

Now, relaunch the Console app—ignoring the security warning again—and you'll see something like this.

![](https://i.imgur.com/Ip6ulxi.png)

Finally, close Git Bash and delight in your new Terminal app that has proper copy and paste support. :tada:


### [Next ⇒](2_sublime_text.md)

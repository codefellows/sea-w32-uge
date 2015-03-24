### Install Fish

Using APT, you can now install [Fish](http://fishshell.com/), a smart and user-friendly command line shell. Remember, a shell is simply the user interface between you and your computer's operating system.

There are many command line shells availabe to choose from, each with their own strengths. Since it's easy to switch back and forth at any time, we recommend you give Fish a try for this workshop.

To get started, run the following commands.

```
sudo apt-get install -y fish git
```

Finally, run this command to make Fish your default shell.

```
chsh -s /usr/bin/fish
```

**TIP:** This will also require your account password which **will not** appear on the screen as you type.

Now, restart Ubuntu, relaunch your Terminal, and you'll see something like this.

![](https://i.imgur.com/WyUWiaK.png)

Welcome to Fish! :tropical_fish:


### Improve the prompt

The prompt is the visual cornerstone of any shell, so let's change it to be both functional and glamorous. :nail_care:

To download and install a better prompt, run the following command.

```
curl -fsSL http://git.io/beJs | ruby
```

To verify the new prompt is installed correctly, relaunch the Terminal. You'll see something like this.

![](https://i.imgur.com/e1Rdz6H.png)

Here's a quick break down of what you're seeing.

| Component             | Description                            |
| --------------------- | -------------------------------------- |
| `~` (home directory)  | Name of your working directory         |
| `$`                   | Prompt symbol                          |


### Update the auto-completions

Fish's auto-completions enhance the user experience of most command line tools.

To update fish's completions, run the following command.

```
fish_update_completions
```

And you'll see something like this.

![](https://imgur.com/weyOeJW.png)

To try out auto-completions, start typing the following command.

```
sudo apt-get c
```

And press the Tab key and you'll see something like this.

![](https://i.imgur.com/Xq4MDsz.png)

Finish typing the following command and press the Enter key.

```
sudo apt-get check
```

**TIP:** This may require your account password which **will not** appear on the screen as you type.

And you'll see something like this.

![](https://i.imgur.com/vUJpOzC.png)


### Leverage your history

Fish keeps a record of every command you've ever run. You can use that history to your advantage.

Start by typing the following command one more time.

```
sudo apt-get c
```

This time you'll see an auto-suggestion based on the most recent matching command.

![](https://i.imgur.com/VfgM4Zw.png)

To use the auto-suggestion, press the right arrow ➡ key and hit the Enter key.

![](https://i.imgur.com/aj9rzhz.png)

**TIP:** Use the up arrow ⬆ and the down arrow ⬇ keys to cycle through your entire history of commands.


### [⇐ Previous](2_apt.md) | [Next ⇒](4_sublime_text.md)

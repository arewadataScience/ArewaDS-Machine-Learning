# Set-up instructions for MacOS

Welcome to the **MacOS set up** repository!

Your first step in this journey is to **carefully read** the steps in this tutorial. You'll learn how to set up your computer - follow the link to your MacOS type :arrow_right:

- [MacOS Intel Setup](#MacOS-Intel-Setup)
- [MacOS M1 Setup](#MacOS-M1-Setup)

### MacOS Intel Setup

Some of the steps in the following sections will require `Homebrew` for MacOS. `Homebrew` is a package manager - it helps you installing software. Installing `Homebrew` will make it easier to install software that we will use later on.

**Step 1:** Open a terminal in one of the following ways:
* In Finder <img src='media/finder.png' alt='Finder' width="4%" />, open the `/Applications/Utilities` folder, then double-click `Terminal`.
* Press <kbd>cmd</kbd> + <kbd>space</kbd> then type `terminal` and press <kbd>enter</kbd>.

    The terminal should now be open:

    <img src='media/mac_terminal.png' width="50%" />

**Step 2:** To install `Homebrew` for MacOS, copy and paste the following line in the terminal:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

**Step 2.1:** Sometimes it's necessary to install `xcode command line utils`. To do so, execute the following command before installing `Homebrew`:

```bash
xcode-select --install
```

You may be prompted to install the `Command Line Developers Tools`. Confirm and once it finishes, continue installing `Homebrew` by pressing <kbd>enter</kbd> again.

**Step 3:** Open a terminal and run the following command to update `Homebrew`. The verbose option means that `Homebrew` will tell you what it's doing - you will see a lot of text output in your terminal:

```bash
brew update --verbose
```

**Step 4:** Now run the following command to install `git`. `Git` is a version control software that facilitates collaboration of people working together on the same code and keeps track of the versions as the code changes. You will learn more about `git` in this course.

```bash
brew install git
```

**Step 5:** Now run the following command to install `Python 3.8`:

```bash
brew install python@3.8
```

**Step 6:** then run the following command to set the default `python3` version to 3.9:

```bash
brew link python@3.9
```

And you're done! Go back continue with setting up Git and GitHub in step 3.

### MacOS M1 Setup

So you've got the new M1 and you're super happy with how fast it is. Unfortunately dealing with Apple silicon requires a little detour. But don't worry, we'll be able to get there in the end.

**Step 1:** Open a terminal in one of the following ways:
* In Finder <img src='media/finder.png' alt='Finder' width="4%" />, open the `/Applications/Utilities` folder, then double-click `Terminal`.
* Press <kbd>cmd</kbd> + <kbd>space</kbd> then type `terminal` and press <kbd>enter</kbd>.

    The terminal should now be open:

    <img src='media/mac_terminal.png' width="50%" />

**Step 1.1:** To use Intel-based software, you'll need `Rosetta2`. Most of you should already have it installed. If you don't have it yet, simply run the following line in the terminal:

```bash
softwareupdate --install-rosetta
```

This will launch the rosetta installer and you’ll have to agree to a license agreement.

**Step 2:** To install `Homebrew x86` version, aka `ibrew` for MacOS, copy and paste the following line in the terminal. `Homebrew` is a package manager - it helps you installing software. Installing `Homebrew` will make it easier to install software that we will use later on.

```bash
arch -x86_64 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

**Step 2.1:** Sometimes it's necessary to install `xcode command line utils`. To do so, execute the following command before installing `Homebrew`:

```bash
xcode-select --install
```

**Step 3:** Add an alias with `ibrew` to your `$PATH` (so that you computer can find `ibrew` when you call it from the terminal):

```bash
echo 'alias ibrew="arch -x86_64 /usr/local/bin/brew"' >> ~/.zshrc
```

**Step 4:** Activate the alterations done to the `.zshrc` file:
```bash
source ~/.zshrc
```

**Step 5:** Install `Python 3.8` with `ibrew`:

```bash
ibrew install python@3.8
```

**Step 6:** Add `Python 3.8` to `$PATH`:

```bash
export PATH="/usr/local/opt/python@3.8/bin:$PATH" >> ~/.zshrc
```

**Step 7** Re-activate the alterations done to the `.zshrc` file:
```bash
source ~/.zshrc
```

And you're done! Go back to the main menu and continue with setting up Git and GitHub in step 3.

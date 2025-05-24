# Set-up instructions for Windows 10/11

Welcome to the Windows 10/11 setup guide for the Arewa Data Science Fellowship. The primary goal of this tutorial is to equip you with the necessary tools and knowledge to prepare your Windows 10/11 environment for data science activities. By the end of this guide, you will have successfully installed and configured the [Windows Subsystem for Linux (WSL)](https://docs.microsoft.com/en-us/windows/wsl/install), [Git](https://git-scm.com/download/win), and [Python 3.8](https://www.python.org/downloads/release/python-380/), along with essential tools like [pip](https://pip.pypa.io/en/stable/installation/) and [venv](https://docs.python.org/3/library/venv.html). These installations are crucial for your data science journey, as they provide a robust and flexible development environment. This setup will enable you to run Linux command-line tools directly in Windows, facilitating a seamless integration of Linux-based data science tools and workflows.

 `Windows Subsystem for Linux (WSL)` enables you to run Linux command line inside Windows. You can follow a Youtube tutorial [here](https://www.youtube.com/watch?v=bRW5r7TK6KM)

**Step 1:** Follow **[this guide](guides/Windows_Subsystem_for_Linux_Installation_Guide_for_Windows_10.md)** to setup `WSL` on Windows 10/11.

**Step 2:** Open a terminal (remember **[this](guides/Windows_Subsystem_for_Linux_Installation_Guide_for_Windows_10.md#Opening-the-WSL-terminal)**!!) and run the following command. It will install `git`. `Git` is a version control software that facilitates collaboration of people working together on the same code and keeps track of the versions as the code changes. You will learn more about `git` in the coming weeks.

```bash
sudo apt update && sudo apt upgrade && sudo apt install git
```

**Step 3:** Open a terminal (remember **[this](guides/Windows_Subsystem_for_Linux_Installation_Guide_for_Windows_10.md#Opening-the-WSL-terminal)**!!) and check if you already have `python3.8` by usind the command below. If your version is `Python 3.9.x` (`x` = any number), you can skip to step 4, otherwise continue with step 3.1 and 3.2.

```bash
python3.9 --version
```

**Step 3.1:** Run the following commands to set up `Python 3.9` (if you get an error with this command, check [this](troubleshooting.md/#6-when-setting-up-python-38-i-get-an-error)). First, add the `deadsnakes repository` - a place from where you will download `Python 3.9`:

```bash
sudo add-apt-repository ppa:deadsnakes/ppa
```

**Step 3.2:** Run the following commands to install `Python 3.9`:

```bash
sudo apt update && sudo apt install python3.9 -y
```

**Step 4** Run the following command to get `pip` and `venv`. `pip` is a package manager - it will help you easily install software. `venv` is a software for creating virtual environments (we will come back to what this means in the next set up step):

```bash
sudo apt update && sudo apt upgrade && sudo apt install python3-pip python3.9-venv -y
```
And you're done! Go back to the main menu and continue with setting up Git and GitHub in step 3.

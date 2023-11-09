# Set-up instructions for Linux

Welcome to **Linux/Ubuntu set up** repository!

Your first step in this journey is to **carefully read** the steps in this tutorial. You'll learn how to set up your environment.

So you're using Ubuntu, huh? Well, kudos to you. You just need to install a couple of packages.


**Step 1:** Open a terminal and check what version of Python you have by using the command below. If your version is `Python 3.8.x` (`x` = any number), you can skip to step 2, otherwise continue with steps 1.1 and 1.2

```bash
python3.8 --version
```

**Step 1.1:** Run the following commands to setup `Python 3.8` (if you get an error with this command, check [this](troubleshooting.md#6-when-setting-up-python-38-i-get-an-error)
). Add the `deadsnakes repository`:

```bash
sudo add-apt-repository ppa:deadsnakes/ppa
```

**Step 1.2:** Run the following commands to install `Python 3.8`:

```bash
sudo apt update && sudo apt install python3.8 -y
```

**Step 2** Run the following command to get `pip` and `venv`. `pip` is a python package manager - it will help you easily install python packages. `venv` is a software for creating virtual environments (we will come back to what this means in the next set up step):

```bash
sudo apt update && sudo apt upgrade && sudo apt install python3-pip python3.8-venv -y
```

And you're done! Go back to the main menu and continue with setting up Git and GitHub in step 3.

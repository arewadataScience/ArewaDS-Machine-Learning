# Set-up instructions for Linux


## Objective

Welcome to the Linux/Ubuntu setup guide for the Arewa Data Science Fellowship. This tutorial aims to equip you with the necessary tools and configurations for a productive data science environment on Linux/Ubuntu. By the end of this guide, you will have:

- Installed and configured [Python 3.8](https://www.python.org/downloads/release/python-380/), an essential programming language for data science.
- Set up [pip](https://pip.pypa.io/en/stable/installation/), the Python package manager, for managing software packages.
- Configured [venv](https://docs.python.org/3/library/venv.html), a tool for creating isolated Python environments, crucial for project-specific dependencies.

So you're using Ubuntu, huh? Well, kudos to you. You just need to install a couple of packages.

**Step 1:** Open a terminal and check what version of Python you have by using the command below. If your version is `Python 3.8.x` (`x` = any number), you can skip to step 2, otherwise continue with steps 1.1 and 1.2

```bash
python3.8 --version
```

**Step 1.1:** Run the following commands to setup `Python 3.8`. Add the `deadsnakes repository`:

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

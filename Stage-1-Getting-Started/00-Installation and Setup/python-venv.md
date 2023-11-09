# Python virtual environment

In this section, you'll learn how to create and manage Python virtual environments for data science projects using conda. This knowledge is vital for maintaining organized, conflict-free, and reproducible data science projects. We will use [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/), a minimal installer for conda, to manage our virtual environments and dependencies. By the end, you will understand:

- Understanding Virtual Environments: Understanding their role in isolating dependencies for individual projects.
- Conda Environment Setup: creating and maintaining a virtual environment using conda
- Conda Package Management: Using Conda for installing and updating packages.
- Activating Environments: How to activate and work within these environments.

## Python Virtual Environment with Conda

Python virtual environments are like a "room" where you gather all the Python packages that you will need to work on your Python project. You can have many virtual environments on your computer. Every time you work on a project, you activate the corresponding virtual environment with all the necessary software packages. The virtual environments are independent of each other. The advantage is also that your OS Python installation is unaffected - Ubuntu needs Python and if you break your OS Python installation, you can break Ubuntu. Check out more information [here](https://realpython.com/python-virtual-environments-a-primer/#what-is-a-virtual-environment).

We will use the `conda` software package to create the virtual environment. The virtual environment will be just a folder on your computer where all the necessary software packages are installed. We will be using the same environment for the whole course and install all the packages at the beginning. 


Conda is an open-source package management system and environment management system that runs on Windows, macOS, and Linux. It can install, run, and update packages and their dependencies. It can create, save, load, and switch between environments on your local computer. It was created for Python programs but can package and distribute software for any language (such as R, Ruby, Lua, Scala, Java, JavaScript, C/ C++, FORTRAN). Below is a step-by-step guide on setting up and using a Conda environment:


**Step 1:** Start by ensuring that the Python packages `pip`, `setuptools`, and `wheel` are up to date:

```bash
python3.8 -m pip install --user --upgrade pip setuptools wheel
```

**Step 2:** Create a virtual environment with the name `prep-venv` in the `.virtualenvs` folder:

```bash
python3.8 -m venv ~/.virtualenvs/prep-venv
```

**Step 3:** Activate the environment:

```bash
source ~/.virtualenvs/prep-venv/bin/activate
```

After you activate your virtual environment you should see at the leftmost of your command line the name of your virtual environment surrounded by parenthesis, like this:

```bash
`(prep-venv) mig@macbook-pro %`
```

**Step 4:** Update `pip`:

```bash
pip install -U pip
```

**Step 5:**: Navigate to your workspace folder and install the Python packages from the `requirements.txt` file:

```bash
cd ~/projects/ds-prep-workspace
pip install -r requirements.txt
```
Congratulations! You are now all set up and you can continue to the last step in the main menu - step 6, testing the weekly workflow with `SLU00 - Jupyter Notebook` from `Week 00`.

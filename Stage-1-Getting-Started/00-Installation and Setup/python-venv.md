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


## Conda Setup and Virtual Environment Management

**Step 1:**  Download and Install Miniconda:

Visit the Miniconda download page [here](https://docs.conda.io/projects/miniconda/en/latest/) and choose the appropriate installer for your operating system.

Follow the installation instructions provided on the download page or in the installer to install the Miniconda.

**Step 2:**  Create a Conda environment:


```bash
conda create --name datascience python=3.8
```

This creates an environment named datascience with Python 3.8.


**Step 3:**  Activate the enviroment


```bash
conda activate datascience

```

After activation, your command prompt should reflect the active environment:

You'll see (ds-datascience) in your command prompt, indicating that the environment is active as shown below

```bash
(prep-env) your_username@your_machine %

```
For example:

```bash
`(datascience) mig@macbook-pro %`
```

**Step 4:** It's a good practice to ensure that conda is up-to-date:


```bash
conda update -n base -c defaults conda

```

**Step 5:**  Manage packages with Conda::

Install packages as needed. For example, to install NumPy:


```bash
conda install numpy

```

If you have a requirements.txt file, you can install the required packages using:


```bash
conda install --file requirements.txt

```

**Step 4:** Deactivate the environment when finished:

```bash
conda deactivate

```



**Step 4:** Update `pip`:

```bash
pip install -U pip
```


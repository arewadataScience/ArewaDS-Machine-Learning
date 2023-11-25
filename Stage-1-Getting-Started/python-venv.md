# Python virtual environment

Python virtual environments are like a "room" where you gather all the Python packages that you will need to work on your Python project. You can have many virtual environments on your computer. Every time you work on a project, you activate the corresponding virtual environment with all the necessary software packages. The virtual environments are independent of each other. The advantage is also that your OS Python installation is unaffected - Ubuntu needs Python and if you break your OS Python installation, you can break Ubuntu. Check out more information [here](https://realpython.com/python-virtual-environments-a-primer/#what-is-a-virtual-environment).


In this section, you'll learn how to create and manage Python virtual environments for data science projects using conda. This knowledge is vital for maintaining organized, conflict-free, and reproducible data science projects. We will use [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/), a minimal installer for conda, to manage our virtual environments and dependencies. By the end, you will understand:

- Understanding Virtual Environments: Understanding their role in isolating dependencies for individual projects.
- Conda Environment Setup: creating and maintaining a virtual environment using conda
- Conda Package Management: Using Conda for installing and updating packages.
- Activating Environments: How to activate and work within these environments.

![virtual_env](https://github.com/arewadataScience/ArewaDS-Machine-Learning/blob/main/Stage-1-Getting-Started/python_virtual_enviment.png)

![virtual_env](https://github.com/arewadataScience/ArewaDS-Machine-Learning/blob/main/virtual_env_issue.png)



## Python Virtual Environment with Conda


We will use the `conda` software package to create the virtual environment. The virtual environment will be just a folder on your computer where all the necessary software packages are installed. We will be using the same environment for the whole course and install all the packages at the beginning. 

![conda](https://github.com/arewadataScience/ArewaDS-Machine-Learning/blob/main/Stage-1-Getting-Started/conda.png)


We can also use pip to install the package if it is not available in the conda. See here on [pip vs conda](https://stackoverflow.com/questions/54834579/specific-reasons-to-favor-pip-vs-conda-when-installing-python-packages). 


## Conda Setup and Virtual Environment Management

**Step 1:**  Download and Install Miniconda:

Visit the Miniconda download page [here](https://docs.conda.io/projects/miniconda/en/latest/) and choose the appropriate installer for your operating system.

Follow the installation instructions provided on the download page or in the installer to install the Miniconda.

**Step 2:**  Create a Conda environment:


```bash
conda create --name datascience python=3.8
```

This creates an environment named datascience with Python 3.9.


**Step 3:**  Activate the enviroment


```bash
conda activate datascience

```

After activation, your command prompt should reflect the active environment:

You'll see (datascience) in your command prompt, indicating that the environment is active as shown below

```bash
(datascience) your_username@your_machine %

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

## Conda vs Pip 

### pip

- **Primary Focus**: pip is the package installer for Python. It is specifically designed to manage Python packages.
- **Package Sources**: It installs packages from the Python Package Index ([PyPI](https://pypi.org)) and other indexes.
- **Package Types**: pip is used for installing and managing Python libraries.
- **Environment Management**: While pip can be used alongside virtual environment managers like `venv` to create isolated Python environments, it does not manage environments by itself.
- **Dependency Resolution**: pip resolves dependencies purely within the Python ecosystem.

### conda

- **Primary Focus**: conda is a package and environment management system. It is designed to handle packages in any language, with a particular focus on Python, R, Ruby, Lua, Scala, Java, JavaScript, C/ C++, FORTRAN.
- **Package Sources**: It installs packages from the [Anaconda repository](https://anaconda.cloud/package-categories) and can also integrate with PyPI. It is often used for data science and machine learning projects, particularly those that require complex dependencies.
- **Package Types**: conda is used for installing both Python and non-Python packages.
- **Environment Management**: conda excels in creating, exporting, listing, removing, and updating environments that have different versions of Python and/or packages installed.
- **Dependency Resolution**: conda resolves dependencies across all the software in an environment, not just Python packages. This makes it more suitable for complex projects where non-Python packages are a requirement.


### Key Differences

1. **Scope**: `pip` is Python-specific, while `conda` handles packages in multiple languages.
2. **Environment Management**: `conda` includes environment management, unlike `pip`.
3. **Dependency Management**: `conda` offers comprehensive dependency management across Python and non-Python packages.
4. **Source of Packages**: `pip` primarily uses PyPI, whereas `conda` uses the Anaconda repository and can integrate with PyPI.
   
| Task | Conda Command | Pip Command |
|------|---------------|-------------|
| Install a package | `conda install package_name` | `pip install package_name` |
| Uninstall a package | `conda remove package_name` | `pip uninstall package_name` |
| Update a package | `conda update package_name` | `pip install --upgrade package_name` |
| List installed packages | `conda list` | `pip list` |
| Search for a package | `conda search search_term` | `pip search search_term` |
| Create a virtual environment | `conda create --name env_name` | `python -m venv env_name` |
| Activate a virtual environment | `conda activate env_name` | `source env_name/bin/activate` (Linux/Mac), `.\env_name\Scripts\activate` (Windows) |
| Deactivate a virtual environment | `conda deactivate` | `deactivate` |




## Resources

1. [Conda CheetSheet](https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf)
2. [The definitive guide to Python virtual environments with conda](https://whiteboxml.com/blog/the-definitive-guide-to-python-virtual-environments-with-conda)

3. [Python Virtual Environments: A Primer](https://realpython.com/python-virtual-environments-a-primer/)
4. Youtube: [Python - Setup Visual Studio Code with Anaconda](https://www.youtube.com/watch?v=sts3CFewvkY)




# Python virtual environment

Virtual environments are like rooms designed to work on a specific project. For instance, you could have a room for painting with all your painting tools and another room for sewing with all your sewing tools. Each room is like a world on it's own - you go to a specific room to work on a specific project with a specific set of tools.

Python virtual environments are like a "room" where you gather all the Python packages that you will need to work on your Python project. You can have many virtual environments on your computer. Every time you work on a project, you activate the corresponding virtual environment with all the necessary software packages. The virtual environments are independent of each other. The advantage is also that your OS Python installation is unaffected - Ubuntu needs Python and if you break your OS Python installation, you can break Ubuntu. Check out more information [here](https://realpython.com/python-virtual-environments-a-primer/#what-is-a-virtual-environment).

We will use the `venv` software package to create the virtual environment. The virtual environment will be just a folder on your computer where all the necessary software packages are installed. We will be using the same environment for the whole course and install all the packages at the beginning. (In the Academy, there will be a different virtual environment for each learning unit.)

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

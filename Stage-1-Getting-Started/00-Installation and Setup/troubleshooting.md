# Troubleshooting

[1. When I open Windows Explorer through Ubuntu, it goes to a different folder than in the guide](#1-when-i-open-windows-explorer-through-ubuntu-it-goes-to-a-different-folder-than-in-the-guide)   
[2. Ubuntu on Windows 10 high CPU usage, crashes](#2-ubuntu-on-windows-10-high-cpu-usage-crashes)   
[3. When I pull from the `ds prep course-2023` repository, I get an error](#3-when-i-pull-from-the-ds-prep-course-2023-repository-i-get-an-error)   
[4. When I try to open `jupyter notebook`, I get an error](#4-when-i-try-to-open-the-jupyter-notebook-i-get-an-error)   
[5. When I use the `cp` command the `>` sign appears and the command does not execute](#5-when-i-use-the-cp-command-the--sign-appears-and-the-command-does-not-execute)   
[6. When setting up python 3.8 I get an error](#6-when-setting-up-python-38-i-get-an-error)   
[7. Nothing happens when I type my password](#7-nothing-happens-when-i-type-my-password)   
[8. I still have a NotImplemented error](#8-i-still-have-a-notimplemented-error)   
[9. Tutorial videos from Prep Course 2020](#9-tutorial-videos-from-prep-course-2020)

### 1. When I open Windows Explorer through Ubuntu, it goes to a different folder than in the guide

Please make sure:

- you are running the command `explorer.exe .` including the dot at the end.
- you are running Windows 10 version `1909` or newer.

### 2. Ubuntu on Windows 10 high CPU usage, crashes

- Make sure you are running Windows 10 version `1909` or newer.
- Then, try following [these steps](https://teckangaroo.com/enable-windows-10-virtual-machine-platform/)

### 3. When I pull from the `ds-prep-course-2023` repository, I get an error

If you get an error like the following when pulling:

```
error: Your local changes to the following files would be overwritten by merge:
<some files>
Please commit your changes or stash them before you merge.
Aborting
```

what `git` is telling you is that changes were made by you to the files in the `~/projects/ds-prep-course-2023` folder, and therefore it is not pulling the changes made by the instructors because they would overwrite the changes made by you.

To fix this do the following:

1. Make sure that any changes you made to the files in `~/projects/ds-prep-course-2023`  (that you don't want to lose) are saved in your `~/projects/ds-prep-workspace` repository (refer to [Updates of the learning units](weekly-workflow.md#14-updates-of-the-learning-units) on how to do this). If you don't want to keep the changes you made to these files, just continue on to the next step.
2. Go to the `~/projects/ds-prep-course-2023` folder and run:

    ```bash
    cd ~/projects/ds-prep-course-2023
    git stash
    ```

3. Now you can pull from the `ds-prep-course-2023` repository:

    ```bash
    git pull
    ```

### 4. When I try to open the jupyter notebook, I get an error

Make sure that your virtual environment is activated **before** opening the jupyter notebook.

```bash
source ~/.virtualenvs/prep-venv/bin/activate
```

### 5. When I use the `cp` command the `>` sign appears and the command does not execute

```bash
cp -r ~/projects/ds-prep-course-2023/“Week 00" ds-prep-workspace
>
```

Make sure to use this type of quotes `"` and not these ones `“`.

### 6. When setting up python 3.8 I get an error

When I run this command:

```bash
sudo add-apt-repository ppa:deadsnakes/ppa
```

I get this error:

```bash
W: GPG error: http://apt.postgresql.org/pub/repos/apt focal-pgdg InRelease: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 7FCC7D46ACCC4CF8
```

Solution: Take the id in front of `NO_PUBKEY` (in my case it's `7FCC7D46ACCC4CF8`) and run the following command:

```bash
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 7FCC7D46ACCC4CF8
```

### 7. Nothing happens when I type my password

When you type your password in the terminal, it is not visible. This is normal, just type the password and hit <kbd>enter</kbd>.

### 8. I still have a NotImplemented error

I've completed the exercise in the Exercise Notebook but when I run the cell I get a **NotImplementedError**.

Solution:
The `raise NotImplementedError()` is added to the exercise cell as a placeholder for where you're supposed to add your solution/code. It is meant to be removed!

### 9. Tutorial videos from Prep Course 2020

🎁🎬 Check the **tutorial videos** if you have any doubts after following this tutorial. These videos were made for the **Prep Course of year 2020**, so there may be some differences.

- [Setup guide for Windows - Part 1](https://www.youtube.com/watch?v=fWi3bYoHW18)
- [Setup guide for Windows - Part 2](https://www.youtube.com/watch?v=bnJOQHh9pJ4)
- [Setup guide for Mac](https://www.youtube.com/watch?v=qs0z4ibMFdU)
- [Updates to Learning Units guide for Windows 10](https://www.youtube.com/watch?v=Q2Cezm6ufrE)
- [Updates to Learning Units guide for Mac](https://www.youtube.com/watch?v=-fzIDfNBZ0I)

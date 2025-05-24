# Basic Command Line Tutorial for Beginners

Welcome to this beginner-friendly tutorial on using the command line. This guide aims to introduce you to the basics of command line operations. Learning the command line is crucial in data science for enhancing efficiency and handling complex tasks. Key reasons include:

1. **Speed**: Command line operations often execute tasks faster than graphical interfaces.
2. **Automation**: Scripts in the command line allow for automating repetitive tasks.
3. **Handling Big Data**: The command line is effective for processing large datasets.
4. **Access to Tools**: Many specialized data science tools are optimized for command line usage.
5. **Advanced Features**: Certain advanced functions are more accessible or exclusively available through the command line.
6. **Version Control**: Command line proficiency is essential for using version control systems like Git, which are vital in collaborative data science projects.
7. **Understanding Systems**: Using the command line offers deeper insights into the workings of computers and software, beneficial for troubleshooting and optimization.

Overall, command line skills significantly contribute to the efficiency, power, and versatility of data science workflows.


<table>
  <tr>
    <td>
        <a href="vscode.md">
            <img src="media/commandline.png" alt="VSCode setup" style="max-width: 100%; height: auto;"/>
        </a>
    </td>
  </tr>
</table>


## Introduction to the Command Line

The command line, also known as the terminal or shell, is a text-based interface to the system. You can perform almost all the tasks that you do with a GUI, but using text commands can often be more efficient.

## Opening the Terminal

Before navigating the file system, you need to know how to open the terminal on your operating system:

### Windows
- Press `Windows + R`, type `cmd`, and press `Enter`. This opens the Command Prompt.
- Alternatively, you can search for "Command Prompt" in the Start menu.

### MacOS
- Open `Finder`, go to `Applications > Utilities`, and double-click on `Terminal`.
- Alternatively, you can use `Spotlight` by pressing `Command + Space`, typing `Terminal`, and pressing `Enter`.

### Linux
- Usually, you can open the terminal with a shortcut, typically `Ctrl + Alt + T`.
- Alternatively, you can find it in your applications menu, the location of which varies by distribution.


## Navigating the File System

### Displaying the Current Directory

- **Command:** pwd (Linux/Mac) or cd (Windows, without arguments)
- **Purpose:** To display the path of the current directory.
- **Usage:**

```bash
pwd
```

### Listing Files and Directories

- **Command**: `ls` (Linux/Mac) or `dir` (Windows)
- **Purpose**: Lists all files and directories in the current directory.
- **Usage**:

```bash
ls
```
A full list of `ls` command options is available [here](https://www.computerhope.com/unix/uls.htm).
  
### Changing Directories

- **Command:** cd <directory>
- **Purpose:** To change your current directory.
- **Usage:**

```bash
cd Documents

```

## File Operations

Managing files is a frequent task in the command line.

### Creating a New File

- **Command:** touch <filename> (Linux/Mac) or type nul > <filename> (Windows)
- **Purpose:** To create a new, empty file.
- **Usage:**

```bash
touch newfile.txt
```

### Creating a New Directory

- **Command:** mkdir <directoryname>
- **Purpose:** To create a new directory.
- **Usage:**
  
  ```bash
  mkdir NewFolder
  ```

### Deleting Files and Directories

- **Command:** rm <filename> (file) or rm -r <directoryname> (directory, Linux/Mac) and del <filename> (file) or rmdir /s <directoryname> (directory, Windows)
- **Purpose:** To delete files or directories.
- **Usage:**

```bash
rm unwantedfile.txt
rm -r OldFolder
```

## Viewing and Editing Files

- **Command:** cat <filename> (Linux/Mac) or type <filename> (Windows)
- **Purpose:** To display the content of a file.
- **Usage:**

```bash
cat example.txt
```


This tutorial has covered the basics of using the command line, providing you with the foundational skills necessary for many tasks in software development, data science, and system management. As you gain more comfort with these commands, you'll find the command line to be a powerful tool in your toolkit.


## Resources

- Youtube: [Command Line Crash Course For Beginners | Terminal Commands](https://www.youtube.com/watch?v=uwAqEzhyjtw)

- Youtube: [Beginner's Guide to the Bash Terminal](https://www.youtube.com/watch?v=oxuRxtrO2Ag)
- Udemy : [Linux Command Line Basics](https://www.udemy.com/course/linux-command-line-volume1/) This is an introductory course to the Linux command Line. It's great for both Linux beginners and advanced Linux users. It is 5 hours on-demand video. This is not free. 


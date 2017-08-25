##### Python for data science workshop

## Common Python Data Tools

<!--
##### Learning Objectives
By the end of this section you will be able to:
* Identify common tools used by data scientists.
* Define the terminal and give examples of why it is useful.
* Define common text editors and their purpose.
* Define open-source tools, including Jupyter Notebooks, along with their benefits.

----------------------------------

## Python Tool Types

### In order to do work with python over time, you'll need a set of tools at your disposal
These tools allow you to create and distribute the code necessary to complete all the steps of a python development workflow. We will look at:

- The terminal (also referred to as Command Line or Command Prompt).
- Text editors, including Sublime and Atom.
- Open-source tools such as the Jupyter Notebook IDE
- Python environments such as Anaconda  

----------------------------------
-->


### In order to do any work with python, you'll need a set of tools at your disposal
The tools discussed in this section allow you to create, compile, and distribute the code necessary to complete all the steps of a python development workflow

#### By the end of this section you will be able to...

+ Discuss common python tools used by data scientists
+ Define the terminal, explain its features, and give examples of why it is useful.
+ Define common text editors and their purpose
+ Define open-source tools, including Jupyter Notebooks and Anaconda along with their benefits

----------------------------------

## Interacting with Python on Computers: The Command Line Interface

**Whenever we use a computer, we need a way to "talk to it" so that we can tell it what to do.**
There are several ways to do this:
- GUI (Graphical User Interface): This is what you're most familiar with. It's any system that allows you to interact with information by clicking, dragging, or otherwise arranging and selecting objects, usually with a combination of the mouse and keyboard. They're (ideally) visually appealing and intuitive to understand.
- CLI (command line interface): Computers didn't always come with a GUI. Instead, everyone interacted with the computer using text commands in what we call a Command Line Interface (CLI). While you may not have seen it as a casual computer user, the command line still exists, and using it becomes essential as you program more.
![alt text](assets/cli.png "The Command Line Interface")
- Shell: This is simply a type of command line program. Once you've booted up into your GUI-based operating system, if you want to interact with the command line, you'll need to open a program designed to do so. On a Mac, the default CLI shell is called the "terminal," and in Windows, it's the "Command Prompt."
![alt text](assets/terminal.png "Terminal")

Examples of command line interfaces: Terminal app on Macs and [Git Bash on windows](https://git-for-windows.github.io/) 
<!--
*NOTE: The following slides include commands that may behave differently on Windows computers. [Bash](https://www.gnu.org/software/bash/) is a free Unix shell that allows the Windows command line to use many of the same commands. You can also [learn more about the Windows CLI itself](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=3&cad=rja&uact=8&ved=0ahUKEwjX1vz4n8rUAhXC7D4KHfVaBZcQFggsMAI&url=https%3A%2F%2Fcommandwindows.com%2Fcommand3.htm&usg=AFQjCNGWUZPreYMfxE_IbAljVKcC5gXspA&sig2=axivxJhs6yrk1_FepckxzQ), if you'd rather go that route.*


----------------------------------

_Slide Title_:  Navigating in the CLI: Paths

Every file or folder in a file system can be read, written, and deleted by referencing its position inside the file system.

When we talk about the position of a file or a folder in a file system, we refer to its "path." There are a couple of different kinds of paths we can use to refer to a file: the absolute path and the relative path.

- **Absolute path:** The  specific location of a file or folder from the root directory, typically shown as /. The root directory is the starting point from which all other folders are defined. It is *not* normally the same as your home directory, which is usually found at `/Users/[Your Username]`.
- **Relative path:** A reference to a file or folder relative to your current position or the present working directory (`pwd`).

In the CLI:
- `pwd` (stands for "print working directory") shows you the absolute path of the directory you are currently in.
- `cd` is the command to "change directory."
  - By itself, `cd` takes you back to the home directory.
  - `cd` + *path* will navigate from wherever you are to the new path — so, if you're in folder A and want to navigate into folder B, type `cd B`.
  - `cd ..` will navigate you one directory back up the path.
  - To indicate the absolute path (and jump directly to any directory without navigating through each folder), add a */* to the beginning of the path. Without a */*, the CLI will interpret the path as looking for a subfolder.
- `~` (tilde) is a reference to the home directory, so ```cd ~``` takes you "home," and ```~/directoryname``` takes you to a directory branching off the home directory.

----------------------------------
-->
<!--
### Examples of Absolute and Relatives Paths

#### Below are some examples that use relative and absolute paths to complete the same action:
1. My present location is ```/folder/subfolder``` and now I want to change directory to ```/folder```
- Using a relative path: ```cd ..```
- Using an absolute path: ```cd /folder```
2. My present location is ```/folder/subfolder``` and I want to change the location to ```/folder/othersubfolder```
- Using a relative path: ```cd ../othersubfolder```
- Using an absolute path: ```cd /folder/othersubfolder```


*Note: Directory is an important term that's often used interchangeably with folder. Although they are not exactly the same, when we say "navigate to your project directory," think of it as "navigate to your project folder."*

----------------------------------
_Slide Title_:  Useful Commands in the CLI

_Slide Content_:

Here are some useful commands to use within the CLI:
 - To stop a script that is currently running, press `Ctrl-C`. (Try this out by typing `ping 127.0.0.1`, which basically sends a message to your computer asking if it's awake. It will keep pinging until you type `Ctrl-C`.)
 - To open a file, use `open` and then the file name (or path, if you're not already in that folder): `open file.txt` or `open subfolder/file.txt`.
 - `ls` lists the files and directories in the current folder (or any folder if you list the path as well: ```ls /Applications```)
  - `ls -a` also shows the files that are currently hidden.
 - Create a new file: ```touch filename```
 - Remove a file: ```rm filename```
 - Create a new directory: ```mkdir foldername```
 - Remove a directory: ```rm -r foldername``` (the ```-r``` tells the computer to remove the folder AND any files/folders within it)
 - The asterisk (&ast;) indicates a wildcard character: ```ls *;i*;``` looks for any file or directory with the letter "i" in the name.

 -->
 
----------------------------------

## Ok, but why use command line?

### The command line is a very different way of doing things than you may be used to
<br>
The key benefit to you as a coder is that the command line gives you a whole set of new, powerful tools. Everything on the computer is scripted, which means it's all bits of code. This code can be run, examined, and manipulated within the command line. As a result, you can understand and even change what's happening in the programs you run, and especially those you create.
<br>
<br>
Using the CLI also allows you to write your own code and run it without building your own GUI.
<br>
<br>
You can also automate processes within the command line to simplify many tasks, such as running a script at a certain time or looping an action (e.g., refreshing the internet every 30 seconds).
<br>
<br>
You'll find many other reasons to interact with the command line throughout your coding endeavors. Most people you ask who have been in the field for awhile will tell you that they frequently use this tool. So, whether or not it seems useful to you now, it will be soon!

----------------------------------



## Text Editors

### Not everything you want to do can be accomplished through the command line. So, rather than writing complex scripts in real time there, coders often use text editors.

**What is a Text Editor?**

- It provides an interface for viewing and modifying text files.
- Text files are files containing text that's readable by humans.
- Text files are encoded via ASCII or Unicode characters.
- There are different kinds of text editors:
  - Terminal/command line-based: Vim, Emacs, GNU nano
  - Window-based: Sublime, Atom, Notepad++

You may also be familiar with programming that's done via online applications, such as JS Bin and Codepen. These applications allow you to write code using a web-based text editor; in other words, within your web browser. When you're comfortable writting code on your code on your own, you'll probably work in a stand-alone text editor.
<br>
We will be using ??? for this workshop so we can focus as much as possible on learning Python today rather than the installation and mechanics of stand alone editors.


----------------------------------

## Modern Text Editors

### Text editors are very handy programs. They can:

- Open a file or directory.
- Understand context.
  - Offer context-sensitive help.
  - Highlight errors or bad practices in your code.
  - Adapt to different file formats.
  - Provide syntax highlighting.

Extensions and plugins are used to add additional features to a text editor.

<!--
----------------------------------

## Types of Text Files

### Text editors can understand, interpret, and edit a wide variety of text files.

Some examples are:
- Plaintext (`.txt`)
- Markdown (`.md`)
- CSV (`.csv`)
- Various programming languages, each with their own set of rules, keywords, operators, and syntax:
  - Python
  - CSS
  - JavaScript
  - Ruby
  - BASH
  - SQL
-->

----------------------------------

## Common Text Editors

### People use a variety of text editors. There's always a debate over [the best](http://blog.liveedu.tv/10-best-text-editors-programming-2016/)

**These are some of the most popular text editors among programmers below. You will want to download one of these and become familiar with it over time.**

1. [Sublime](https://www.sublimetext.com/): This is a very popular text editor, mostly because of its many features. It's efficient and versatile, and a variety of plugins have been developed to add to its functionality. However, it is not free, so many people turn to other editors.
2. [VIM](http://www.vim.org/): This is one of the older text-editing programs available and is completely customizable, so it's popular among enthusiasts. It is very efficient, can be used completely without a mouse, and comes standard on most Unix-based computers. It is open source and free to use but is less intuitive than other editors and can be difficult to learn.
3. [Atom](https://atom.io/): One of the newer editors on the market, Atom has already proven to be quite popular. It's "hackable," in that it can be developed for and customized as much as the user wants. There are also many, many plugins available on the internet. Atom is free to use and easy to pick up for beginners. The downside is that it's not very efficient, consumes a lot of memory, and can have some difficulty with large files. For a beginning programmer, however, Atom is a great resource.
4. [Notepad ++](https://notepad-plus-plus.org/features/): This is another open-source editor and is very agile. It's also simplistic, resembling the familiar Notepad program. It supports most programming languages without any installation or plugins and can manage large files with ease. The interface is not very intuitive, however, and lacks helpful features for beginning coders that the other applications include.

GA often recommends Atom as their text editor of choice, as most of the necessary features are available in the trial version, but you're welcome to use any of the above (or others) if you have a preference.

----------------------------------

## Other Open-Source tools

### Other tools you'll encounter in Python development and in data science are:

- [Git and GitHub](www.github.com): This version control software is used by individual programmers to track the progress of their projects and by teams to collaborate in an organized way. You will become more familiar with this program throughout the course, but, for now, consider it a way to organize and share files that preserves the history of their changes and keeps them safer.
- [Jupyter Notebooks](jupyter.org/): Found in the Anaconda suite of tools (which is worth exploring in itself), the Jupyter Notebook tool allows you to create your code in organized "notebooks," which can intersperse code chunks (that can run individually in any order) with markdown text, allowing for easy annotation and clear, organized scripts. Jupyter offers an alternative to a text editor and is what is know as an integrated development environment (IDE), in which script can easily be written and executed. Throughout this course, we'll often present materials in a Jupyter Notebook to allow for easy demonstration of code, as well as offer well-formatted explanatory text, images, and videos.
- [Anaconda data science environment](https://www.continuum.io/what-is-anaconda)
Keep in mind that many open-source tools are created as plugins for text editors or libraries for programming languages. So many have been created by the data science and programming communities at large that you can nearly always find something to help you meet your goal. Keep an eye on blogs to see what others are using, and don't try to reinvent the wheel — if there's a tool you wish you had, Google it to see if someone's already created it!


----------------------------------

## Review: Your available tools

#### You are now aware of the tools necessary for completing most steps of the data science workflow
To review, we discussed:
- Navigating your computer and running scripts with the *command line*.
- Creating code and complex scripts in your choice of *text editors*.
- Upgrading your toolkit with open-source content such as plugins for text editors and interfaces including Jupyter Notebook..
With these tools at your disposal, you'll be in great shape as you progress your Python capabilities!

We will work today with tools from the [Anaconda environment](https://www.continuum.io/) environment on your laptop

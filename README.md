# Exercise 0.1 - Sandbox

This is the first exercise folder of this course. In this exercise, you'll familiarize yourself with the development environment and get everything set up.

You can use this sandbox folder to try out different things later on. When you encounter something new in the material, try it out in the sandbox first, and then solve the exercises on the topic.

This guide will assume you are using either a Linux environment or Windows Subsystem for Linux. If you are in a Linux environment, you can safely ignore the references to Windows directories.

## Installing Windows Subsystem for Linux (WSL)

You can find installation instructions for WSL [here](https://docs.microsoft.com/en-us/windows/wsl/install-win10).

You will need administrative access to your machine and the ability to run PowerShell commands.

Choose `Ubuntu 18.04` for your distro.

## Setting up a development environment in WSL

In this guide you will set up a folder called `python-programming` in `Documents` and use it for your development environment. We will also assume that your primary drive is `C:\`.

Go into your file explorer, find the `Documents` directory and right-click to create a New Folder called `python-programming`. *Don't use spaces in the name of this directory.*

Open up your WSL environment and enter the following commands at the prompt:

```bash
ln -s /mnt/c/Users/<your machine username>/Documents/python-programming python-programming
```

remembering to replace <your machine usename> with your username.

*Hint: If you press Tab after typing Users/ it will offer autocomplete suggestions.*

Once this is done, type

```bash
cd python-programming
```

to enter the `python-programming` directory.

Clone the `sandbox` and `exercises` repositories from Github using the following commands:

```bash
git clone https://github.com/den01-python-programming/sandbox/
git clone https://github.com/den01-python-programming/exercises/
```

Type `ls` at the command prompt. You should see the following output:

```plaintext
sandbox    exercises
```

You can use the `sandbox` repo to try things out in Python throughout this course. Think of it as a directory for testing things.  

## Downloading the exercises

Enter the exercises directory using

```bash
cd exercises
```

Type `ls` at the command prompt. You should see the following output:

```plaintext
README.md   dl_exercises.sh     exercise-list.dat
```

The `dl_exercises.sh` file uses the `exercise-list.dat` file to download each part's exercises from the repos. We can *run* the `dl_exercises.sh` script as follows:

```bash
./dl_exercises.sh
```

You will be asked some questions as the script runs through depending on your scenario.

Once the exercise files for each part are downloaded, you can use this directory as your main development environment.

If you type `ls` at the prompt, you should now see the exercises that were downloaded by the script.

You can enter any of the directories using `cd`.

If you would like to examine the inner workings of this script, you can check it out using:

```bash
cat dl_exercises.sh
```

Don't worry too much at the moment about how this works - it will probably become clearer as you go through the course!

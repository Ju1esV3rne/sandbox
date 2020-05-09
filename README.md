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

Make another directory called `exercises` using:

```bash
mkdir exercises
```

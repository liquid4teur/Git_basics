# Presentation

This repo is here to document the essential commands used to correctly configure Git through command line & Github.

# Installation

## Create your Github repo

# Configuration

## SSH credentials

You have to take the SSH key from your github account and save it into your computer in order to "autorize" the computer to use your Github account.  

## Configure your profile through Git CMD

First, you have to configure the gitconfig file (/etc/gitconfig) in order to use your Github account.
You have to fill your Github username & email:

>git config --global user.name "your_username"
>git config --global user.email your_email

Then, if you want to verify the configuration, you can do it through the command:

>git config --list

It will list you all the parameters saved into the gitconfig file.

## Configure your editor

You can easily configure your text editor if you don't want to use Vi or Vim.
Personnaly, I use Visual Studio Code so the command to configure it will be:

>git config --global core.editor "code --wait"

Other text editor could also be usable, like Atom or Sublim Text:

>git config --global core.editor "atom --wait"
>git config --global core.editor "'C:/Program Files (x86)/sublime test 3/subl.exe' -w"

Then in your command prompt, to open a file, you can use directly the command:

>code nameofyourfile

## Creating a repository

The first thing people usually do is to create the repo on which you will put your project and work on it.

# Use Case

## Clone your Repo

Once, you configured your machine with your Github account, you are now able to work on it.
After creating the repository on which you will work on, you have to clone the concerned repository.

## Working from different machines

In my case, I work from 3 different machines (1 Mac & 2 Windows). Also, I have my repositories saved into Github and cloned on the 3 different machines.
For example, during the week I am working on one of my 2 Windows machine.
Then, during the week-end, I need to work on my Mac. So, the question is, how will I gather all the modifications I made during the week-end ?
Simply by doing:

## Undo git add

To undo "git add" before a commit, it's possible to unstage changes:

- For a single file:

>git reset <file> 

- To unstage all changes: 

>git reset

# Other useful command

## Delete a folder (with files inside)

- To force removing of a folder (containing files):

>rm -rf
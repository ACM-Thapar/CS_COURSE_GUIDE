# How to write your .bashrc ?
### It's a powerful thing, and to be able to customize it open up a lot of possibilities for new users.

## Making Aliases
**What are aliases ?**
They are easier commands/phrases that you can give to virtually any shell commands to make you life easier.
They can condense common commands and save you the time and effort of typing out entire sentences and save you time and effort.
```
alias cls="clear"
alias bye="exit"
```
In the above example the keyword *'alias'* is followed by you choice of keyword that you want the command to be -

1. ***clear -*** the command to clear out your screen in the terminal, has been set to ***cls*** .
2. ***exit -*** the command to close the terminal, has been set to ***bye*** .


## Repository-Hopping
### Why do you need this?
If you do want to transition to working in just the terminal, quickly hopping to the desired repositories to update/cop/paste code is a necessity. To ease this process and save time on writing extensive *'cd'* commands.

### How do we solve this problem?
Install a distro-hopping script called 'z'
> For Linux or Mac users
```
wget https://raw.githubusercontent.com/rupa/z/master/z.sh
```
> For windows
```
Install-Module -Name z -Force
```
Post install you must add z to your path **only for bash/zsh users** *(if you are on windows, PowerShell takes care of it by itself. Kinda neat !)*
> Add these lines of code to your **.bashrc**
```
#The link to use 'z' a repository-hopper
[[-r "/usr/share/z/z.sh"]]  &&  source /usr/share/z/z.sh
```

# Oh-My-Bash and Oh-my-Zsh
### Some of the most popular shell aesthetics scripts written to to beautify you shell prompt

## Getting Started

### Prerequisites

__Disclaimer:__ _Oh My Bash works best on macOS and Linux._

* Unix-like operating system (macOS or Linux)
* `curl` or `wget` should be installed
* `git` should be installed
* Go to https://github.com/ohmybash/oh-my-bash.git for the entire documentation of Oh-my-bash. Saying it`s well documented is putting it lightly. 

### Basic Installation

Oh My Bash is installed by running one of the following commands in your terminal. You can install this via the command-line with either `curl` or `wget`.
> For installing either you may use your package manager and install curl/wget in your machine
```
# for wget
sudo pacman -S wget

#for curl
sudo pacman -S curl
```

#### via curl
```shell
bash -c "$(curl -fsSL https://raw.githubusercontent.com/ohmybash/oh-my-bash/master/tools/install.sh)"
```

#### via wget
```shell
bash -c "$(wget https://raw.githubusercontent.com/ohmybash/oh-my-bash/master/tools/install.sh -O -)"
```

This replaces `~/.bashrc` with the version provided by Oh My Bash. The original `.bashrc` is backed up with the name `~/.bashrc.omb-TIMESTAMP`. 

## Some food for thought
* The key is to make life easier and you terminal workflow more efficient, experiment and see what works best for you. Good Luck.
* NEVER, AND I MEAN NEVER SHY AWAY FROM SPENDING TIME ON DOCUMENTATION. It is a life saver, and any error that you will or might have are documented most of time. So spend time reading the manual.

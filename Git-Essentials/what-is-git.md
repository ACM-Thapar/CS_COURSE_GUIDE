# What is Git ?
### It's a version control software that lets you keep track of all changes made to your software code over the time that it takes to start coding it till the finish.

## What is Source Control ?
**Why do we need it ?**
Version control, also known as source control, is the practice of tracking and managing changes to software code. Version control systems are software tools that help software teams manage changes to source code over time. As development environments have accelerated, version control systems help software teams work faster and smarter. They are especially useful for [DevOps](https://www.atlassian.com/devops/what-is-devops) teams since they help them to reduce development time and increase successful deployments.

Version control software keeps track of every modification to the code in a special kind of database. If a mistake is made, developers can turn back the clock and compare earlier versions of the code to help fix the mistake while minimizing disruption to all team members.

## Installation
> For windows *(using **winget** package manager)*
```
winget install -e --id Git.Git
```
> For mac *(using **homebrew**)*
```
brew install git
```
> For Linux *(using system package managers)*
```
# for Arch
sudo pacman -S git

# for Ubuntu
sudo apt-get install git
```
==( ! ) Make sure to add git to your path during the install itself, or you will have to do it manually==

## Post-installation configuration
### connecting your GitHub account to git
>In your terminal type the following commands
```
#This will display the version of git on your system
git -version

#this links your username
git config --global user.name <your-github-id>

#this links your email-id
git config --global user.name <your-github-email>
```

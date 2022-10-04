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
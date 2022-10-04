# What is an SSH-Key and why should you have it ?
An SSH key is an access credential for the SSH (secure shell) network protocol. This authenticated and encrypted secure network protocol is used for remote communication between machines on an [unsecured open network](https://whatismyipaddress.com/unsecured-network). SSH is used for remote file transfer, network management, and remote operating system access. The SSH acronym is also used to describe a set of tools used to interact with the SSH protocol.

SSH uses a pair of keys to initiate a secure handshake between remote parties. The key pair contains a public and private key. The private vs public nomenclature can be confusing as they are both called keys. It is more helpful to think of the public key as a "lock" and the private key as the "key". You give the public 'lock' to remote parties to encrypt or 'lock' data. This data is then opened with the 'private' key which you hold in a secure place.


### How to generate and use an SSH-key for GitHub
>For Mac or Linux
1.  Execute the following to begin the key creation
	```bash
	ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
	```
	This command generates an ssh key using your GitHub email id as the label

2. You will then be prompted to "Enter a file in which to save the key."  
You can specify a file location or press “Enter” to accept the default file location.
	```bash
	> Enter a file in which to save the key (/Users/you/.ssh/id_rsa): [Press enter]
	```
3. The next prompt will ask for a secure passphrase.  
A passphrase will add an additional layer of security to the SSH and will be required anytime the SSH key is used. If someone gains access to the computer that private keys are stored on, they could also gain access to any system that uses that key. Adding a passphrase to keys will prevent this scenario.
	```bash
	 >Enter passphrase (empty for no passphrase): [Type a passphrase]
	 >Enter same passphrase again: [Type passphrase again]
	```
4. Add the new SSH key to the ssh-agent

	The ssh-agent is another program that is part of the SSH tool-suite. The ssh-agent is responsible for holding private keys. Think of it like a key-chain. In addition to holding private keys it also brokers requests to sign SSH requests with the private keys so that private keys are never passed around insecurely.

	Before adding the new SSH key to the ssh-agent first ensure the ssh-agent is running 	 by executing:
	```bash
	eval "$(ssh-agent -s)"
   > Agent pid 59566
	```
	Once the ssh-agent is running the following command will add the new SSH key to the local SSH agent.
	```bash
	ssh-add -K /Users/you/.ssh/id_rsa
	```
	 The new SSH key is now registered and ready to use!

> For Windows
> 
> *MUST NOTE: Since, Windows environments do not have a standard default UNIX shell. External shell programs will need to be installed for to have a complete keygen experience. The most straight forward option is to utilize [Git Bash](https://www.atlassian.com/git/tutorials/git-bash).*
> 1. Once Git Bash is installed the **same steps for Linux and Mac can be followed within the Git Bash shell.***
> 2. A second workaround is to set up **Windows Subsystem for Linux (WSL2)** The Windows Subsystem for Linux lets developers run a GNU/Linux environment -- including most command-line tools, utilities, and applications -- directly on Windows, unmodified, without the overhead of a traditional virtual machine or dualboot setup.
> 
> ## Why Windows Subsystem for Linux (WSL2) ?
> ### You get a near-native Linux experience without having to give up windows You can:
> -   Run common command-line tools such as `grep`, `sed`, `awk`, or other ELF-64 binaries.
> -   Run Bash shell scripts and GNU/Linux command-line applications including:
>     -   Tools: vim, emacs, tmux
>     -   Languages: [NodeJS](https://learn.microsoft.com/en-us/windows/nodejs/setup-on-wsl2),
> Javascript,
> [Python](https://learn.microsoft.com/en-us/windows/python/web-frameworks),
> Ruby, C/C++, C# & F#, Rust, Go, etc.
>     -   Services: SSHD, [MySQL](https://learn.microsoft.com/en-us/windows/wsl/tutorials/wsl-database),
> Apache, lighttpd,
> [MongoDB](https://learn.microsoft.com/en-us/windows/wsl/tutorials/wsl-database),
> [PostgreSQL](https://learn.microsoft.com/en-us/windows/wsl/tutorials/wsl-database).
> -   Install additional software using your own GNU/Linux distribution package manager.
> -   Invoke Windows applications using a Unix-like command-line shell.
> -   Invoke GNU/Linux applications on Windows.
> -   [Run GNU/Linux graphical applications](https://learn.microsoft.com/en-us/windows/wsl/tutorials/gui-apps)
> integrated directly to your Windows desktop
> -   [Use GPU acceleration](https://learn.microsoft.com/en-us/windows/wsl/tutorials/gpu-compute)
> for machine learning, data science scenarios and more

	

	


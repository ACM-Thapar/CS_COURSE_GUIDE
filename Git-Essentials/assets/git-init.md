# Initialize git in a local directory ( i.e. on your machine )

### When you setup a local directory and want to host it on GitHub.

-   [Create a new repository](https://docs.github.com/en/articles/creating-a-new-repository) on GitHub.com. To avoid errors, do not initialize the new repository with _README.md_, license, or `gitignore` files. You can add these files after your project has been pushed to GitHub. 
	
	![Create New Repository drop-down](https://docs.github.com/assets/cb-11427/images/help/repository/repo-create.png)
-   Open PowerShell, Bash etc.
    
-   Change the current working directory to your local project.
***Make sure that the name of local project and the repository on GitHub are exactly the same ( case-wise and spellings )***
	```
	cd <repo-name same in both>
	```
    
-   Use the `init` command to initialize the local directory as a Git repository. By default, the initial branch is called `master`.
    
    If you’re using Git 2.28.0 or a later version, you can set the name of the default branch using `-b`.
    
    ```shell
    $ git init -b main
    ```
    
    If you’re using Git 2.27.1 or an earlier version, you can set the name of the default branch using `&& git symbolic-ref HEAD refs/heads/main`.
    
    ```shell
    $ git init && git symbolic-ref HEAD refs/heads/main
    ```
    
- Now, let's add our README.md file, it's the file that will let everyone know the entire scope of our project- from software used to operating it.
	```shell
	echo "#README File" >> README.md
	```
-   Add the files in your new local repository. This stages them for the first commit.
    
    ```shell
    $ git add .
    # Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.
    ```
    
-   Commit the files that you've staged in your local repository.
***Make sure your commit messages are clear, concise and always meaningful. It should be understood that it eases documentation and looking back let's anyone know exactly what changed***
    
    ```shell
    $ git commit -m "First commit"
    # Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify the file, use 'git reset --soft HEAD~1' and commit and add the file again.
    ```
    
-   At the top of your repository on GitHub.com's Quick Setup page, click to copy the remote repository URL. ![Copy remote repository URL field](https://docs.github.com/assets/cb-25662/images/help/repository/copy-remote-repository-url-quick-setup.png)
-   In the Command prompt, [add the URL for the remote repository](https://docs.github.com/en/github/getting-started-with-github/managing-remote-repositories) where your local repository will be pushed.
    
    ```shell
    $ git remote add origin <REMOTE_URL>
    # Sets the new remote
    
    $ git remote -v
    # Verifies the new remote URL
    ```
    
-   [Push the changes](https://docs.github.com/en/github/getting-started-with-github/pushing-commits-to-a-remote-repository) in your local repository to GitHub.com.
    
    ```shell
    $ git push origin main
    # Pushes the changes in your local repository up to the remote repository you specified as 
    ```


	

	


# How to contribute to other's projects ?
### Contents-
- About Forking  
- Forking a repository
- Cloning a fork
- Making and pushing changes
- Making a pull request
- Managing feedback
- Finding projects

## About forking

After using GitHub by yourself for a while, you may find yourself wanting to contribute to someone else’s project. Or maybe you’d like to use someone’s project as the starting point for your own. This process is known as forking.

Creating a "fork" is producing a personal copy of someone else's project. Forks act as a sort of bridge between the original repository and your personal copy. You can submit pull requests to help make other people's projects better by offering your changes up to the original project. Forking is at the core of social coding at GitHub. For more information, see "[Fork a repo](https://docs.github.com/en/get-started/quickstart/fork-a-repo)."

## Forking a repository

This tutorial uses [the Spoon-Knife project](https://github.com/octocat/Spoon-Knife), a test repository that's hosted on GitHub.com that lets you test the fork and pull request workflow.

1.  Navigate to the `Spoon-Knife` project at [https://github.com/octocat/Spoon-Knife](https://github.com/octocat/Spoon-Knife).
2.  Click **Fork**. ![Fork button](https://docs.github.com/assets/cb-23088/images/help/repository/fork_button.png)
3.  Select an owner for the forked repository. ![Create a new fork page with owner dropdown emphasized](https://docs.github.com/assets/cb-151543/images/help/repository/fork-choose-owner.png)
4.  By default, forks are named the same as their parent repositories. You can change the name of the fork to distinguish it further. ![Create a new fork page with repository name field emphasized](https://docs.github.com/assets/cb-151542/images/help/repository/fork-choose-repo-name.png)
5.  Optionally, add a description of your fork. ![Create a new fork page with description field emphasized](https://docs.github.com/assets/cb-177452/images/help/repository/fork-description.png)
6.  Choose whether to copy only the default branch or all branches to the new fork. For many forking scenarios, such as contributing to open-source projects, you only need to copy the default branch. By default, only the default branch is copied. ![Option to copy only the default branch](https://docs.github.com/assets/cb-59189/images/help/repository/copy-default-branch-only.png)
7.  Click **Create fork**. ![Emphasized create fork button](https://docs.github.com/assets/cb-80721/images/help/repository/fork-create-button.png)

**Note:** If you want to copy additional branches from the parent repository, you can do so from the **Branches** page. For more information, see "[Creating and deleting branches within your repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-and-deleting-branches-within-your-repository)."

## Cloning a fork

You've successfully forked the Spoon-Knife repository, but so far, it only exists on GitHub. To be able to work on the project, you will need to clone it to your computer.

You can clone your fork with the command line, GitHub CLI, or GitHub Desktop.

1.  On GitHub, navigate to **your fork** of the Spoon-Knife repository.
    
2.  Above the list of files, click **Code**. 
 !["Code" button](https://docs.github.com/assets/cb-20363/images/help/repository/code-button.png)
3. Copy the URL for the repository.
    
    -   To clone the repository using HTTPS, under "HTTPS", click :clipboard:
	-   To clone the repository using an SSH key, including a certificate issued by your organization's SSH certificate authority, click **SSH**, then click 
	-   To clone a repository using GitHub CLI, click **GitHub CLI**, then click

![The clipboard icon for copying the URL to clone a repository with GitHub CLI](https://docs.github.com/assets/cb-33207/images/help/repository/https-url-clone-cli.png)

4. Open your terminal    
5.  Change the current working directory to the location where you want the cloned directory.
    
6.  Type `git clone`, and then paste the URL you copied earlier. It will look like this, with your GitHub username instead of `YOUR-USERNAME`:
    
    ```shell
    $ git clone https://github.com/YOUR-USERNAME/Spoon-Knife
    ```
    
5.  Press **Enter**. Your local clone will be created.
    
    ```shell
    $ git clone https://github.com/YOUR-USERNAME/Spoon-Knife
    > Cloning into `Spoon-Knife`...
    > remote: Counting objects: 10, done.
    > remote: Compressing objects: 100% (8/8), done.
    > remove: Total 10 (delta 1), reused 10 (delta 1)
    > Unpacking objects: 100% (10/10), done.
    ```
    

## Making and pushing changes

Go ahead and make a few changes to the project using your favorite text editor, like [Visual Studio Code](https://code.visualstudio.com). You could, for example, change the text in `index.html` to add your GitHub username.

When you're ready to submit your changes, stage and commit your changes. `git add .` tells Git that you want to include all of your changes in the next commit. `git commit` takes a snapshot of those changes.

```shell
git add .
git commit -m "a short description of the change"
```

When you stage and commit files, you essentially tell Git, "Okay, take a snapshot of my changes!" You can continue to make more changes, and take more commit snapshots.

Right now, your changes only exist locally. When you're ready to push your changes up to GitHub, push your changes to the remote.

```shell
git push
```

## Making a pull request

At last, you're ready to propose changes into the main project! This is the final step in producing a fork of someone else's project, and arguably the most important. If you've made a change that you feel would benefit the community as a whole, you should definitely consider contributing back.

To do so, head on over to the repository on GitHub where your project lives. For this example, it would be at `https://www.github.com/<your_username>/Spoon-Knife`. You'll see a banner indicating that your branch is one commit ahead of `octocat:main`. Click **Contribute** and then **Open a pull request**.

GitHub will bring you to a page that shows the differences between your fork and the `octocat/Spoon-Knife` repository. Click **Create pull request**.

GitHub will bring you to a page where you can enter a title and a description of your changes. It's important to provide as much useful information and a rationale for why you're making this pull request in the first place. The project owner needs to be able to determine whether your change is as useful to everyone as you think it is. Finally, click **Create pull request**.

## Managing feedback

Pull Requests are an area for discussion. In this case, the Octocat is very busy, and probably won't merge your changes. For other projects, don't be offended if the project owner rejects your pull request, or asks for more information on why it's been made. It may even be that the project owner chooses not to merge your pull request, and that's totally okay. Your copy will exist in infamy on the Internet. And who knows--maybe someone you've never met will find your changes much more valuable than the original project.

## Finding Projects

**Open source** is [source code](https://en.wikipedia.org/wiki/Source_code "Source code") that is made freely available for possible modification and redistribution. Products include permission to use the source code,[[1]](https://en.wikipedia.org/wiki/Open_source#cite_note-Open_Source_Org.,_2007-1) design documents,[[2]](https://en.wikipedia.org/wiki/Open_source#cite_note-Diffingo_Solutions_Inc.,_2008-2) or content of the product. The **open-source model** is a decentralized [software development](https://en.wikipedia.org/wiki/Software_development "Software development") model that encourages [open collaboration](https://en.wikipedia.org/wiki/Open_collaboration "Open collaboration").[[3]](https://en.wikipedia.org/wiki/Open_source#cite_note-LevinePrietula2013-3)[[4]](https://en.wikipedia.org/wiki/Open_source#cite_note-4) A main principle of [open-source software development](https://en.wikipedia.org/wiki/Open-source_software_development "Open-source software development") is [peer production](https://en.wikipedia.org/wiki/Peer_production "Peer production"), with products such as source code, [blueprints](https://en.wikipedia.org/wiki/Blueprint "Blueprint"), and documentation freely available to the public. The [open-source movement](https://en.wikipedia.org/wiki/Open-source_movement "Open-source movement") in software began as a response to the limitations of [proprietary code](https://en.wikipedia.org/wiki/Proprietary_software "Proprietary software").

### How to find what you want to contribute to ?
There are a lot of projects that you can contribute to, people are consistently brainstorming ideas and looking for help on GitHub.
Learn the language's syntax and get a general idea, from there on it's all about contributing and learning by gathering experience working with all sorts of people and software.

Find what interests you the most and just reach out, the open-source community is filled with people just like you who want to collaborate and grow together.

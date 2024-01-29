
<p align="center">
  <a href="https://github.com/kelloggcompany/Welcome">
    <img src="images/kelloggs.jpg"> <img src="images/ghec.png">
  </a>
</p>

                                                                         
[![](https://img.shields.io/badge/github-blue?style=for-the-badge)](https://github.com/hamzamohdzubair/redant)
# **$${\color{Indigo}Welcome \space to \space Kellogg's \space Github \space Enterprise \space Cloud!!}$$**                                                            

This repo gives a brief description about github and how to work with github.

### 💡 **What Is GitHub? A Beginner’s Introduction to GitHub**

At a high level, GitHub is a website and cloud-based service that helps developers store and manage their code, as well as track and control changes to their code. To understand exactly what GitHub is, you need to know two connected principles:

- Version control                   
- Git                         

<p align="center">
  <img src="https://github.com/kelloggcompany/Welcome/blob/latest-welcome/images/1centralized-vs-distributed.jpg" width=50% height=50%/>
</p>

### 💡 What Is Version Control?

Version control helps developers track and manage changes to a software project’s code. As a software project grows, version control becomes essential.This is a centralized way, there will be a single source or a central copy of your repository. You’ll have to grant permission to other team members/ add them as contributors to this central repositories(Central repositories are a matter of project organization), for them to start contributing to your central repo.version control lets developers safely work through branching and merging.

With branching, a developer duplicates part of the source code (called the repository). The developer can then safely make changes to that part of the code without affecting the rest of the project.Then, once the developer gets his or her part of the code working properly, he or she can merge that code back into the main source code to make it official.

All of these changes are then tracked and can be reverted if need be.

### 💡 What Is Git?

Git is a free and open-source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.Git is a distributed version control system, which means that the entire codebase and history is available on every developer’s computer, which allows for easy branching and merging.

<p align="center">
  <img src="https://github.com/kelloggcompany/Welcome/blob/latest-welcome/images/2%20distributed-1024x677.png" width=50% height=50%/>
</p>

 ***

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
      <a href="#Setting-up-Git-in-your-local">Setting up Git in your local</a>
      <ul>
        <li><a href="#To-configure-user-information-for-all-local-repositories">To configure user information for all local repositories</a></li>
        <li><a href="#Authenticating-with-GitHub-from-Git">Authenticating with GitHub from Git</a></li>
        <li><a href="#Creating-a-personal-access-token">Creating a personal access token</a></li>
        <li><a href="#Generating-a-new-SSH-key-and-adding-it-to-the-ssh-agent">Generating a new SSH key and adding it to the ssh-agent</a></li>
        <!-- <li><a href="#built-with">Built With</a></li> -->
      </ul>
    </li>
	<!-- <li><a href="#How-To-Use-Git-And-GitHub-At-Kellogg">How To Use Git And GitHub At Kellogg</a>
</li> -->
<!--    </ul>-->
      <li>
	<a href="#Get-Started-Learning-GitHub">Get Started Learning GitHub</a>
      <ul>
        <li><a href="#GitHub-Introduction">GitHub Introduction</a></li>
        <li><a href="#Merge-conflicts">Merge conflicts</a></li>
        <li><a href="#Git-Actions">Git Actions</a></li>
        <!-- <li><a href="#built-with">Built With</a></li> -->
      </ul>
    </li> 
	  <li>
		  <a href="#GitHub-best-practices">GitHub best practices</a>
      <ul>
          <ul><li><a href="#Who-this-guide-is-for">Who this guide is for</a></li></ul>
		  <ol type=1><li><a href="#Do-not-git-push-straight-to-master">Do not git push straight to master</a></li>
          <li><a href="#Do-not-commit-code-as-an-unrecognized author">Do not commit code as an unrecognized author</a></li>
          <li><a href="#Define-code-owners-for-faster-code-reviews">Define code owners for faster code reviews</a></li>
          <li><a href="#Do-not-leak-secrets-into-source-control">Do not leak secrets into source control</a></li>
          <li><a href="#Do-not-commit-dependencies-into-source-control">Do not commit dependencies into source control</a></li>
          <li><a href="#Do-not-commit-local-config-files-into-source-control">Do not commit local config files into source control</a></li>
          <li><a href="#Create-a-meaningful-git-ignore-file">Create a meaningful git ignore file</a></li>
          <li><a href="#Archive-dead-repositories">Archive dead repositories</a></li>
          <li><a href="#Lock-package-version">Lock package version</a></li>
          <li><a href="#Specify-standard-package-versions">Specify standard package versions</a></li>
          <li><a href="#Leverage-task-list">Leverage task list</a></li>
          <li><a href="#Use-a-branch-naming-convention">Use a branch naming convention</a></li>
          <li><a href="#Delete-stale-branches">Delete stale branches</a></li>
          <li><a href="#Keep-branches-up-to-date">Keep branches up to date</a></li>
          <li><a href="#Remove-inactive-GitHub-members">Remove-inactive-GitHub-members</a></li>
          <li><a href="#Enable-security-alerts">Enable security alerts</a></li>
      </ul>
    </li>   
 
 <li>
      <a href="#Issues">Issues</a>
  </li>
 
 <li>
      <a href="#Other-Git-and-GitHub-learning-resources">Other Git and GitHub learning resources</a>
    </li>
  <li>
      <a href="#Recommended-GitHub-Actions">Recommended GitHub Actions</a>
  </li>
    
   <li>
      <a href="#Glossary">Glossary</a>
  </li>
 </ol>
</details>
	
<br>	
	
## 🪁Setting up Git in your local

A new repository can either be created locally, or an existing repository can be cloned. When a repository was initialized locally and commited, you have to push it to GitHub afterwards.

### Getting started

To get started with Git, you need to download it to your machine. Head over to https://git-scm.com/ and download the version most compatible with your system.

During the installation of Git,select the git-bash option as well and make sure you choose to run Git on the normal console window, this will enable you to run Git on your command prompt. 

Run the below command to check git version in the command prompt

🖍️  **```git --version```**

<p align="center">
  <img src="https://github.com/kelloggcompany/Welcome/blob/latest-welcome/images/git--version.PNG" width=60% height=60%/>
</p>

Developers use Git in intergration with Visual Studio Code (VScode) by installing git plugins.

[//]: <### Initialize a git repository >

[//]: <Every change you make is tracked in a repository, so to use git this will be the first thing you’ll do. To initialize a git repository, use this command while inside the working folder.>

[//]: <🖍️ **```git init```**>

[//]: <git init is one way to start a new project with Git. To start a repository, use either git init or git clone - not both.>

[//]: <To initialize a repository, Git creates a hidden directory called .git. That directory stores all of the objects and refs that Git uses and creates as a part of your project's history. This hidden .git directory is what separates a regular directory from a Git repository.>

[//]: <![Alternative text](1_NyKNgA3E28bz20ptTTD2cg.png)>

### To Set/test your local git configuration 
 
Navigate to Windows -> GitBash

Run

🖍️ **```git config -l```**

Make sure Username/github username and Kellogg's email are updated in the git configuration.

if not, Run the below commands with (your)username & email-id to configure.

🖍️ **```git config --global user.name "Venu Cherukuri```"**

🖍️ **```git config --global user.email "venu.cherukuri@kellogg.com"```**

To set proxy, Run the below command:

🖍️ **```git config --global --add remote.origin.proxy "127.0.0.1:9000"```** 

To validate and ensure the proxy is listed in the config: 

Run the command as shown below in the screenshot:
  
🖍️ **```git config -l```**

<p align="center">
  <img src="https://github.com/kelloggcompany/Welcome/blob/latest-welcome/images/git-config-list.PNG" width=75% height=75%/>
</p>

Once the Configuration is set, Start with the below steps to test your access.

### Step 1: Create a working folder and clone the existing repo from Github.

Using Gitbash run **mkdir Kelloggs** to create a working folder named Kelloggs where you will clone the repository and run **cd kelloggs** to enter in to the folder.

You can clone the repository using https url which is highly recommended . While Cloning with https url, it may prompt for Github username and passcode (deprecated) or a PAT token.
 
To create a PAT token,Click the link 🔗[Creating Personel access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)

you can get url from the repository as shown in the screenshot:
 
<p align="center">
  <img src="https://github.com/kelloggcompany/Welcome/blob/latest-welcome/images/https%20clone.png" width=65% height=65%/>
</p>

To clone the repository run the below command as shown below:

🖍️ **```git clone [url]```**  

<p align="center">
  <img src="https://github.com/kelloggcompany/Welcome/blob/latest-welcome/images/git-clone.PNG" width=75% height=75%/>
</p>

### Step 2: List-out the branches in the repo and create a new branch

After cloning is finished,Change the directory to the cloned repository i.e., **cd welcome**

To list-out branchs,Run the below command

🖍️ **```git branch -a```** 

<p align="center">
  <img src="https://github.com/kelloggcompany/Welcome/blob/latest-welcome/images/git-list-branch.PNG" width=75% height=75%/>
</p>

A branch is a new/separate version of the main repository.Branches allow you to work on different parts of a project without impacting the main branch.

When the work is complete, a branch can be merged with the main project.You can even switch between branches and work without interfering with one another.By default you will be in main branch.

To create new branch and checkout to new branch, run the below commands

🖍️ **```git branch <new branch name>```**

🖍️ **```git checkout -b <branch name>```**

Here,the newly created branch is **Myfirst-repo**.

### Step 3: You can make changes to your code like adding an extra statement or function or adding a file.To keep track of your modifed files use **git add** command to stage them. Here is an example:

Use the following command  **echo "some text" >> filename.txt** to create a file.

Then list the files using **ls** command to ensure your .txt file is created.

check the file content using  **cat <file name>** command. Now add the file to the project directory/repo using the following command:

🖍️ **```git add <file name>```**

To add all the files use -A as an option i.e., **```git add -A```**

When you run git add, the files from your working directory are hashed and stored as objects in the index, leading them to be "staged changes"

### Step 4: When satisfied with adding a couple of changes to your index (Index is a staging area between the working directory and Repository), ensure you have the correct files on the stage, use this command to check what files are on the stage.

🖍️ **```git status```**

<p align="center">
  <img src="https://github.com/kelloggcompany/Welcome/blob/latest-welcome/images/git-add-status.PNG" width=75% height=75%/>
</p>

### Step 5: Committing changes create a snapshot of the staged changes along a timeline of a Git projects history, use the following command to commit changes

🖍️ **```git commit -m "This is the commit message"```**

The -m flag specifies that what follows is the commit message. This is a custom message intended to let your future self or other developers know what was added in that commit. You can use something like git commit -m “Successfully added a text file”, to keep track of the things you’ve added to the branch.

<p align="center">
  <img src="https://github.com/kelloggcompany/Welcome/blob/latest-welcome/images/git-commit.PNG" width=75% height=75%/>
</p>

### Step 6: Uploading your code to GitHub with Git push.

To link your remote git repository to your online repository on GitHub, you attach an origin to your remote git repo to specify the origin will be hosted online. You’ll use this command.. 

🖍️ **```git remote add origin {REMOTE_URL}```** 

Here,URL is the https url cloned from the repository shown in step 1 (url format: https:// github.com/kelloggcompany/{REPOSITORY_NAME}.git)

Above command will execute, but the system won't provide any feedback in the terminal. To verify that the remote repo was added to your configuration, use        **git remote –v** command. This command will show that GitHub is the fetch and push targets of the local repository.

Cloning a repository from a remote server downloads the project to your local computer and leaves you with a local Git repository. This local Git repository will already have a connection to the original remote set up, automatically. This is what the "origin" remote connection points to.

### To push the code to your repo, use the following command: 

🖍️ **```git push -u origin <branch name>```** 

Above command assumes that you already have a remote repository defined for default branch and pushs the commits from local repo to remote repo.

<p align="center">
  <img src="https://github.com/kelloggcompany/Welcome/blob/latest-welcome/images/git-push.PNG" width=75% height=75%/>
</p>

from the screenshot above, set-upstream means to set the remote repo for the new branch(Myfirst-repo is the newly created branch in my example).

Once the commits are pushed,you will get a notification message for a pull request in your repo in the github as shown in the screenshot below

<p align="center">
  <img src="https://github.com/kelloggcompany/Welcome/blob/latest-welcome/images/push-scrshot.PNG" width=60% height=60%/>
</p>

### Step 7: Going through your history (Optional)

Let’s say it’s been months since you worked on a particular project but used Git to keep track of it’s progress. You can successfully go through the history by using the command **git log** to view your commit history. 

### Here is a quick glance for Git setup:

<p align="center">
  <img src="https://github.com/kelloggcompany/Welcome/blob/latest-welcome/images/git%20setup%20edited.png" width=60% height=60%/>
</p>


<br>

## Authenticating with GitHub from Git

When you connect to a GitHub repository from Git, you will need to authenticate with GitHub using either HTTPS or SSH.

> 🚩 **Important: You can authenticate to GitHub using GitHub CLI, for either HTTP or SSH.**

### Connecting over HTTPS (recommended)
If you clone with HTTPS, you can cache your GitHub credentials in Git using a credential helper. For more information, see 🔗 "[Cloning with HTTPS urls](https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls)" and 🔗 "[Caching your GitHub credentials in Git](https://docs.github.com/en/get-started/getting-started-with-git/caching-your-github-credentials-in-git)."

Cloning with HTTPS URLs
The https:// clone URLs are available on all repositories, regardless of visibility. https:// clone URLs work even if you are behind a firewall or proxy.

When you git clone, git fetch, git pull, or git push to a remote repository using HTTPS URLs on the command line, Git will ask for your GitHub username and password. When Git prompts you for your password, enter your personal access token. Alternatively, you can use a credential helper like Git Credential Manager. Password-based authentication for Git has been removed in favor of more secure authentication methods. For more information, see "Creating a personal access token."

### Creating a personal access token

Personal access token are an alternative to using passwords for authentication to GitHub when using the GitHub API or the command line. It is recommanded to use PAT instead of using GitHub user defined password.
Please click the below link to create a personal access token (PAT) :

🔗 https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token


### Connecting over SSH
If you clone with SSH, you must generate SSH keys on each computer you use to push or pull from GitHub. For more information, see 🔗"[Cloning with SSH urls](https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories#cloning-with-ssh-urls)" and "Generating a new SSH key."

### Generating a new SSH key and adding it to the ssh agent

You can access and write data in repositories on GitHub.com using SSH (Secure Shell Protocol).
When you generate an SSH key, you can add a passphrase to further secure the key. Whenever you use the key, you must enter the passphrase. If your key has a passphrase and you don't want to enter the passphrase every time you use the key, you can add your key to the SSH agent. The SSH agent manages your SSH keys and remembers your passphrase.

Please click the below link to generating a new SSH key and adding it to the ssh-agent :

> 🚩 **Important: For any of the kellogg server's, if you would like to establish SSH connection then create SSH Keys to the server**

🔗 https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent?platform=windows

<br>

With this basic knowledge about Git, you can now use it to share code with a team of developers, keep track of their changes, commit changes to your project, authorize contributors, create experimental features with branches, merge code, pull code for templates.

<p align="center">
  <img src="https://github.com/kelloggcompany/Welcome/blob/latest-welcome/images/3github%20cycle.jpg" width=50% height=50%/>
</p>

***

## 🪁Get Started Learning GitHub 

> 🚩 **Important: It is recommended to complete the exercise given in the below course**
###  🚩🚩**Note: Use personal Github account for Training Modules instead of kellogg's organization***

### GitHub Introduction

GitHub is a development platform that enables you to host and review code, manage projects, and build software alongside 50 million developers.

Learn to use key GitHub features, including issues, notifications, branches, commits, and pull requests.

Please click the below link to start learning Github(Open the links in new tab).

🔗 https://learn.microsoft.com/en-us/training/modules/introduction-to-github/

### Merge conflicts
When Git cannot perform an auto-merge because changes are in the same region this causes merge conflicts. Many developers are confused about concepts like merging and resolving merge conflicts. Here, we will learn how to resolve merge conflicts. 

🔗 https://learn.microsoft.com/en-us/training/modules/resolve-merge-conflicts-github.

### Github Actions 
Automate, customize, and execute your software development workflows right in your repository with GitHub Actions. You can discover, create, and share actions to perform any job you'd like, including CI/CD, and combine actions in a completely customized workflow.Learn how to use GitHub Actions using below link. 

🔗 https://learn.microsoft.com/en-us/training/modules/introduction-to-github-actions/
	  
<br>

### 🛎️🚩**```Please use kellogg's template while you create a repository```** ,Here is the link to learn how to [create repository using template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)

<br>

***
		  
## 🪁GitHub best practices

This list of GitHub best practices is derived from the insights we gleamed from those experiences.These best practices are still applicable even if you use something other than GitHub for source control, because they’re all about improving code quality, security, and writing good code.

 <p align="center">
  <img src="https://github.com/kelloggcompany/Welcome/blob/latest-welcome/images/4og-git-best-practices-1024x538.png" width=100% height=30%/>
</p>


### 📰Who this guide is for
This guide is for anyone in the Application development Teams looking to improve developer workflow and productivity, as well as code quality and security.

Those responsible for putting together team-wide standard practices and policies would benefit greatly from this guide, but even if you’re a developer not “in charge” of driving such standards, you will find these practices applicable and useful to remember.

### 🔖Do not git push straight to master
Regardless if you use Gitflow or any other git branching model, it is always a good idea to turn on git branch protection to prevent direct commits and ensure your main branch code is deployable at all times. All commits should be pushed to master through pull requests.


### 🔖Do not commit code as an unrecognized author
Sometimes you commit code using the wrong email address, and as a result GitHub shows that your commit has an unrecognized author. Having commits with unrecognized authors makes it more difficult to track who wrote which part of the code.

Ensure your Git client is configured with the correct email address and linked to your GitHub user. Check your pull requests during code reviews for unrecognized commits.

### 🔖Define code owners for faster code reviews
When you’re dealing with dozens, hundreds, or more repositories and engineers, it’s nearly impossible to know who owns which parts of the codebase and need to review your changes.

Even in smaller teams you’d still have code owners – for example, front-end code changes should be reviewed by the Front-End Engineer.

Use Code Owners feature to define which teams and people are automatically selected as reviewers for the repository.
There is an option for projects where you want to keep more control. A protected branch option means that the code owner for each owned file has to leave a review before anyone can merge a pull request to that branch.

### 🔖Do not leak secrets into source control
Secrets, or secret keys or secret credentials, include things like account passwords, API keys, private tokens, and SSH keys. You should not check them into your source code.Instead, we recommend you inject secrets as environment variables externally from a secure store. You can use tools like Hashicorp Vault or AWS Secrets Manager to do this.

There are also tools for scanning secrets in repos and prevent them from getting into repos.

Git-secrets can help you to identify passwords in your code.Git hooks can be used to build a pre-commit hook and check every pull request for secrets.

### 🔖Do not commit dependencies into source control
Pushing dependencies into your remote origin will increase repository size. Remove any projects dependencies included in your repositories and let your package manager download them in each build. if you are afraid of “dependencies availability” you should consider using a binary repository manager solution like Jfrog or Nexus Repository. Or check out GitHub’s Git-Sizer.

### 🔖Do not commit local config files into source control
We strongly recommend against committing your local config files to version control. Usually, those are private configuration files you don’t want to push to remote because they are holding secrets, personal preferences, history or general information that should stay only in your local environment.

### 🔖Create a meaningful git ignore file
A .gitignore file is a must in each repository to ignore predefined files and directories. It will help you to prevent secret keys, dependencies and many other possible discrepancies in your code. You can choose a relevant template from Gitignore.io to get started quickly.

### 🔖Archive dead repositories
Over time, for various reasons, we find ourselves with unmaintained repositories. Sometimes developers create repos for an ad hoc use case, a POC, or some other reason. Sometimes they inherit repos with old and irrelevant code.

In any case, these repos were left intact. No one is doing any development work in those repos anymore, so you want to clean them up and avoid the risk of other people using them. The best practice is to archive them, i.e. make them “read-only” to everyone.

### 🔖Lock package version
Your manifest file contains information about all packages and dependencies in your project and their versions. The best practice is to specify a version or version range for every package and dependency listed in the manifest. Otherwise, you can’t be sure which version will get installed during the next build, and consequently your code may break.

### 🔖Specify standard package versions
Even when everyone on your team are using the same packages, reusing code and tests across different projects can still be difficult if the packages are of different versions.

If you have a package that is used in multiple projects, try at a minimum to use the same major version of the package.

### 🔖Leverage task list
Tasks lists provide a way for you to track to-dos directly within comments, issues, and even MarkDownfiles (*.MD) within your repository (users must have write access to the repository to make changes to MarkDownfiles).

Tasks lists provide an excellent way to capture a high-level overview of a task or issue, as well as keep others updated on its state. Make sure to take advantage of this powerful new feature!

### 🔖Use a branch naming convention
Adopting a consistent branch naming convention is essential to keeping your repository organized as your team grows in size. An efficient naming convention will allow you to keep merge conflicts at a minimum while ensuring your developers are as productive as possible.

While there are many branch naming conventions, one of the most popular ones is known as git flow:

![Alternative text](https://github.com/kelloggcompany/Welcome/blob/latest-welcome/images/6git%20flow.png)

### 🔖Delete stale branches
Every time one branch is merged into another, the branch that is merged in becomes stale, assuming further work isn’t being done in it.While it may seem useful or even necessary to keep the extra data on hand, the reality is that stale branches are abandoned 98% of the time and simply clutter up your project.

Even if you delete a branch when you shouldn’t have, you can restore it - and if you don’t trust GitHub’s restore feature,  chances are it’s safe on somebody’s computer, thanks to the magic of distributed versioning.

Don’t be a branch hoarder: delete your stale branches.

### 🔖Keep branches up to date
Let’s say you’ve finally completed some work on a long-outstanding branch and you’re ready to merge it into master. You pull from remote, hit merge, and suddenly you’re faced with a barrage of merge conflicts.

What happened?🤔

You failed to keep your branch up-to-date with the branch you’re attempting to merge into. Lots of commits went by and some conflicted with your changes... now you’re faced with spending time and energy resolving an unnecessary amount merge conflicts.

The best practice here is to ensure that you’re consistently merging your base branch into your current branch as you work, especially if it’s a long-outstanding branch.

### 🔖Remove inactive GitHub members
While it might seem obvious, it’s worth mentioning in a comprehensive list of best practices... Be sure to remove contributors from your organization that are no longer contributing to your codebase.

If you remove somebody from your organization for any reason, revoke their GitHub access immediately as well. Even in completely amicable situations, it’s better safe than sorry!

### 🔖Enable security alerts
Security alerts are another feature new to GitHub. You can read about them here, but the gist is that GitHub now tracks reported security vulnerabilities in some dependencies and will even suggest fixes for you.

This is turned on automatically for all public repositories, but if your repository is private, you’ll need to opt in manually.



***

## 🪁Issues

Issues can be used to keep track of bugs, enhancements, or other requests. For more information, see "🔗[About issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues)".

GitHub now also supports 🔗[multiple issue templates](https://help.github.com/articles/about-issue-and-pull-request-templates/). Feel free to log issues.

***
## 🪁Other Git and GitHub learning resources
		  
🔗  [ProGit book](http://git-scm.com/book) 

🔗  [Git docs](https://docs.github.com/en/get-started/using-git/about-git)

🔗  [Git command list](https://git-scm.com/docs)

🔗  [GitHub training & Guides in youtube](https://www.youtube.com/githubguides)
                                                                              		  
***

## 🪁Recommended GitHub Actions

Some starter [GitHub Actions workflows](https://docs.github.com/en/actions/learn-github-actions) included with this repo are:

🔗  [Stale issue](https://github.com/actions/stale) - labels and closes issues and pull requests with no activity for a set period of time

🔗  [LFS Warning](https://github.com/ActionsDesk/lfs-warning) - issues warnings when large files are added to the repository

🔗  [Release Drafter](https://github.com/marketplace/actions/release-drafter) - drafts release notes based on merged pull requests

🔗 [First Interaction](https://github.com/actions/first-interaction) - Greets new contributors to the repo

🔗 A [Dependabot config file](https://docs.github.com/en/github/administering-a-repository/configuration-options-for-dependency-updates) for alerting on dependency vulnerabilities

***
## 🪁Glossary

***git:*** an open source, distributed version-control system

***GitHub:*** a platform for hosting and collaborating on Git repositories

***commit:*** a Git object, a snapshot of your entire repository compressed into a SHA

***branch:*** a lightweight movable pointer to a commit

***clone:*** a local version of a repository, including all commits and branches

***remote:*** a common repository on GitHub that all team members use to exchange their changes

***fork:*** a copy of a repository on GitHub owned by a different user

***pull request:*** a place to compare and discuss the differences introduced on a branch with reviews, comments, integrated tests, and more



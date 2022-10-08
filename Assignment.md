
- [Introduction](#introduction)
- [What is GitHub](#what-is-github)
- [Why GitHub](#why-github)
- [Clone](#clone)
- [Commits in GitHub](#commits-in-github)
- [Pull Request (PR)](#pull-request-pr)
- [GitHub DeskTop Vs Github CLI](#github-desktop-vs-github-cli)
- [Conclusion](#conclusion)

 ## Introduction

 In our world today, things need to be kept in a secure easy to retrieve storage system, this ensures reusability and easy access to such resource, this span from things as simple as a basin of water to more complex ones such as the [blockchain]().

 As developers who write and maintain code or people in any tech stack, care is taken to ensure that this data _(mostly a codebase, but since software development is more than just writng lines codes and github allows for more than just storing code, we would stick with __data__ throughout this article)_ can be stored on a system for accessibility, reusablity and safety, such systems should have ease of you, afterall why add more complexity to the already complex life of a developer.


## What is GitHub
GitHub is a cloud based hosting service owned by MicroSoft for software development at any level, it aids developers and software companies in version control, access control, bug tracking, task management, [CI/CD]() aka Continuous integration, software feature request, social networking and many more, You can check this [Page]() for more about its history.

GitHub is simply a database on the cloud for software developers with functonalities that aid [software development lifecycle](). 


## Why GitHub
Since the turn of the decade, we have seen lots of improvement in cloud related softwares with most things previously done manually with difficulty and impossibility can now be automated and stored on the internet for easily accessiblity and safety, same applys to Github now most developers would most probably be in a team where there would be online collaboration, or they would need their data to be publicly available also known as [open source]() projects, having this data on thier local system won't suffice, and here is where GitHub shines with a very robust and trustworthy cloud storage that allows for online/realtime collaborations and storage every developer can effectively store and retrieve their work and also grant access to fellow collaborators to the same.

Github is also free to use for its most basic and important functions, you can keep tabs on what other developers or organisations are doing technical wise, fix and contribute to public Repositories (folder containing the data stored on GitHub), known as contributing to Open Source



GitHub is based on a previously created technology Git, which is an Open Source software used for managing and tracking files (mostly code files), its the most popular and widely used version control system [VCS]() (in simple terms a system that can track changes to a file or document over time), which is important in software development, as developers fix bugs and update previously written code to add features, as many collaborators could be on a single project, git allows each developer to have a copy of the main Repository on their local system, make modifications safely and then [push]() this copy back to the main repository for a possible [merge](), with steps known as commits each with well detailed explanations, git tracks this changes and stores them for reference in case anything breaks or there is need to revert to a previous state.

> Git is the tool that is used to interact with the repositories and allows developers to make changes and effectively track and manages the changes, it runs through the system's [command line]() .GitHub is the remote cloud storage facility for each of the repository, it provides a Graphical User Interface [(GUI)]() on top of Git, these makes it more user friendly and easy to use

**To SignUp to the GitHub service, simply go to [GitHub.com]()** 

**To also install Git, follow this [article's]() instructions**

## Clone
Cloning is very important when collaborating with other remote team members, as this is a advanced file sharing method, it would enable you to have a copy of that particular repository on your local system

Cloning from the Command Line from whatever operating system is easy, let's examine how to do so 

- make sure your internet connection is stable
- open your browser on your desktop 
- Open GitHUb and go to the Repository you want to clone
- click 'Code' and copy the resulting Url
  
![How to clone | 100](https://www.educative.io/cdn-cgi/image/f=auto,fit=contain,w=1800/api/edpresso/shot/4580530784305152/image/5062914986213376.png)

- open your command line or G
it Bash
- navigate to the directory you want to clone the repository to
  >*note: you would be downloading the Repos here, so make sure the folder is empty*
- type in *git clone "the copied Url"*
> In your Terminal type in
~~~ cmd
   git clone {the URL of the GitHub Repository}
 ~~~~

- press enter and voila
- wait a few seconds for the download to be complete

Now that you have cloned (downloaded) the repository, you can work on the project and effectively collaborate with others

## Commits in GitHub
To make commits in your local branch on your system, is to make small meaningful changes to the codebase, and letting git document it for you, this is important as it allows for the following
- saving the particular change made by the user
- decribing the change
- documenting who made the change

To make a commit to your local branch
- on your terminal navigate to the folder containing the folder or files you want to commit
- initialise git, this is to tell git that this folder is a git repository and git commands can be performed on it 
  
  > In your Terminal type in
~~~ cmd
   git init
 ~~~~
- next would be to add the files you want to commit (i.e add to the main remote branch) using the git [add]() commands
> adding a single file
~~~ cmd
   git add filename
 ~~~~
 > adding all the files where changes have been made
~~~ cmd
   git add .
 ~~~~
 > adding a group of files
~~~ cmd
   git add filename_1, filename_2, ...... , filename_n
 ~~~~
- now that you have added this changes, run git status on your terminal to verify your changes, it would show all tracked and untracked files
> on your terminal
~~~ cmd
   git status
 ~~~~

- to commit run on you terminal the following command
> on your terminal
~~~ cmd
   git commit -m 'your commit message'
 ~~~~
Your commit message should be very intuitive and short, check this [link]() on how to write good commit messages
Now you have made a commit.
> note
>- You can make numerous commits
>- check the list of all commits from the terminal

 >  on your terminal
~~~ cmd
   git log
 ~~~~
  
## Pull Request (PR)
Now that you are familiar with git and github, how to commit and cloning a repository, you can create a pr to effectively collaborate, this shows that you are done with your changes locally and need to merge with the Main branch (or master), which is usually done by the developer in charge of the project, or whoever is assigned to merging duties,

So in this order, **you ought to have** 
  
- committed any changes on your local system to a local branch
- push this local branch to the remote repository

> note:
> To create a PR you must have [Write access]() to the repository in question.

- Create a new branch reflecting the change you want to make using the git checkout command
 > In your terminal
 ~~~ cmd
   git checkout -b [Branch Name]
 ~~~~
- make,[commit](#commits-in-github) and add your changes 
- push these changes to github by using the git [push]() commands
- On GitHub navigate to the branch you want to create a PR for
- look for 'Compare and pull request' button and click it
  ![compare and pull button](https://www.freecodecamp.org/news/content/images/2020/01/compare.png)
- provide necessary details on what you have done, add reviewers etc
  ![PR Image](https://www.freecodecamp.org/news/content/images/2020/01/pullRequest-1.png)
- congratulations you have created a pull request
- an email notification would be sent to this effect, and when your PR is merged 


## GitHub DeskTop Vs Github CLI
## Conclusion
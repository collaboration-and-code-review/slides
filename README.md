# Get a Jumpstart on Collaboration and Code Review in GitHub

<!--
https://2017.djangocon.us/speaking/speaker-resources/#slide-guidelines
https://docs.google.com/presentation/d/16LvCzF1mywdEvhXwUyJCdEuyiw05q-ITGiJEgFT6L-Y/edit#slide=id.g20735b3908_0_0
-->

This is a transcript of a talk Katherine "Kati" Michel ([Twitter](https://twitter.com/KatiMichel), [GitHub](https://github.com/KatherineMichel)) will give at [DjangoCon](https://2017.djangocon.us), [PyLadies Remote](http://remote.pyladies.com), and other events.

<!--
* [Original slide deck]()
* [Video recording]()
-->

## Attribution

The style of this transcript is heavily inspired by:

* Ana Balica's ([Twitter](https://twitter.com/anabalica), [GitHub](https://github.com/ana-balica)) transcript of her [Humanizing among coders](https://ana-balica.github.io/2017/05/28/humanizing-among-coders/) keynote for [PyCon CZ 2016](https://cz.pycon.org/2016). 
* Honza Javorek's ([Twitter](https://twitter.com/honzajavorek), [GitHub](https://github.com/honzajavorek)) transcript of Anna Ossowski's ([Twitter](https://twitter.com/OssAnna16), [GitHub](https://github.com/OssAnna16)) keynote [Be(Come) A Mentor! Help Others Succeed!](https://github.com/honzajavorek/become-mentor) for [PyCon CZ 2017](https://cz.pycon.org/2017/). 

Thank you!

## Table of Contents

- [Get a Jumpstart on Collaboration and Code Review in GitHub](#get-a-jumpstart-on-collaboration-and-code-review-in-github)
- [Welcome](#welcome)
- [About Me](#about-me)
- [About You](#about-you)
- [Announcing TacoFancy on Twitter](#tacofancy)
- [The One Sentence that Motivated Me to Start Using GitHub](#the-one-sentence-that-motivated-me-to-start-using-github)
- [My First Pull Request](#my-first-pull-request)
- [DjangoCon US Website as Example Project](#djangocon-us-website-as-example-project)
- [Prerequisites for Getting Started](#prerequisites-for-getting-started)
- [What are Git and GitHub?](#what-are-git-and-github)
- [GitHub: Social Network](#github-social-network)
- [GitHub: Repositories](#github-repositories)
- [Local Development Environment](#local-development-environment)
- [What I Would Do Differently](#what-i-would-do-differently)
- [Collaboration and Code Review Best Practice Workflow](#collaboration-and-code-review-best-practice-workflow)
- [Working on a File in GitHub](#working-on-a-file-in-github)
- [Branches](#branches)
- [How to Create a Branch](#how-to-create-a-branch)
- [Overview](#overview)
- [Section 1](#section-1)
- [The Two Types of Accounts](#the-two-types-of-accounts)
- [The Two Collaborative Development Models](#the-two-collaborative-development-models)
- [The Two Types of Accounts and Models](#the-two-types-of-accounts-and-models)
- [Write Permission](#write-permission)
- [Why We Need Write Permission](#why-we-need-write-permission)
- ["Shared Repository"](#shared-repository)
- ["Fork and Pull" Model](#fork-and-pull-model)
- [Write Permission and Collaboration Examples](#write-permission-and-collaboration-examples)
- [How to Fork a Repo](#how-to-fork-a-repo)
- [Forked Repo](#forked-repo)
- [About Forks](#about-forks)
- [Section 2](#section-2)

- [Fork and Pull Diagram](#fork-and-pull-diagram)
- [Shared Repository Diagram](#shared-repository-diagram)

- [Another Workflow](#another-workflow)
- [Learn More About Workflow](#learn-more-about-workflow)

- [Getting Help](#getting-help)
- [Thank You](#thank-you)

<!--
- [Local Branch Process](#local-branch-process)

### Pushing and Pulling to Keeping Your Local Clone and GitHub Repo in Sync
### Submit a Pull Request

### Perspective: Checking Out Remote Branches
### Pull Request Review Process

### The Difference Between a Feature Branch and a Pull Request Branch
### Fetching from Origin Versus Pulling from a Fork
### Remote, Remote Branch, Remote Tracking Branch, and Local Branches
### Shared Repo Model Feature Branch or Pull Request Branch
### Forked Repo Model Feature Branch or Pull Request Branch

### Merge Pull Request Locally and Push to Master Branch
### Alternatively, Fetch Individual Pull Request
### How to Deal With Merge Conflicts
### Tidy Up
### Syncing Changes
### Adding an Upstream Remote and Syncing a Fork

- [Organization and Team Setup](#organization-and-team-setup)
- [Safeguards Checklist](#safeguards-checklist)
- [Community and Communication Strategy](#community-and-communication-strategy)
- [Documentation](#documentation)
- [Issue Templates](#issue-templates)
- [Pull Request Templates](#pull-request-templates)
- [Forum](#forum)
- [Productivity Tips](#productivity-tips)
- [Tips for Getting Started](#tips-for-getting-started)

### Debunking Myths

- [The Other Way Around](#the-other-way-around)
-->

## Script

<table>


<tr><td width="30%">

![Slide 1]()

</td><td>

### Get a Jumpstart on Collaboration and Code Review in GitHub 

By Katherine "Kati" Michel

</td></tr>


<tr><td width="30%">

![Slide 2]()

</td><td>

### Welcome 

Thank you for being here. I'm thrilled to have the opportunity to teach you what I've learned you about collaboration and code review in GitHub. 

</td></tr>


<tr><td width="30%">

![Slide 3]()

</td><td>

### About Me 

A lot of what I'm going to talk to you about, I learned as the DjangoCon US Website Chair

* DjangoCon Website Chair
* DjangoCon Europe Website Committee Member
* DEFNA (Django Events Foundation North America) Board Member
* Project Manager
* Web Designer and Developer

</td></tr>


<tr><td width="30%">

![Slide 4]()

</td><td>

### Goal

I want to teach you a process that will get you up and running doing collaboration and code review as quickly as possible. 

I'm going to be showing you a lot of screenshots and diagrams, because I think one of the difficulties of learning Git and GitHub is that it can be difficult to now what the process looks like. I want you to understand what it should look like. 

At the end of my talk, there will be a slide with a link to Useful Resources where you will find documentation and all of the commands I will be showing you today. You will also be able to look at my slides and the video of this online. 

<!--
I want to teach you the essential process and underlying logic so that you can get started collaborating and doing code review as quickly as possible. 

When it comes to Git commands, there are variations of how you can do things. I'm not going to be going into detail about that. 

At the end of this talk, there will be a slide with a link to a list of resources which will include the official Git and GitHub documentation. You can learn about all of the variations there. 
-->

</td></tr>


<tr><td width="30%">

![Slide 5]()

</td><td>

### Announcing TacoFancy on Twitter

I want to tell you how I got started witih open-source contribution, which is a bit unconventional and might show you that there are many ways to get involved. 

I first signed up for GitHub on April 18, 2013. But my account sat unused for months. I didn't know how to get started.  

7 months later, I happened to be looking at Twitter. I saw a tweet from a man named Dan Sinker who works in journalism and web development. He had made a really delicious Mexican meal and he and a few other people had decided to start a project on GitHub to share Mexican recipes. 

So I clicked on the link and went to the project to take a look. 

</td></tr>


<tr><td width="30%">

![Slide 6]()

</td><td>

### The One Sentence that Motivated Me to Start Using GitHub

One sentence in the project information that had a huge impact on me: "Are You New to Github But Want to Contribute?" 

That was me. I had been wanting to contribute for months, but wasn't sure how, and now was my chance. I felt it was my destiny to contribute now. 

</td></tr>


<tr><td width="30%">

![Slide 7]()

</td><td>

### My First Pull Request

I struggled through, but I was extremely motivated and submitted my first pull request. I had a huge adrenaline rush. 

</td></tr>


<tr><td width="30%">

![Slide 8]()

</td><td>

### DjangoCon US Website as Example Project

I kept using Git and GitHub and getting better at it. Eventually, I came across the DjangoCon US Website Repo and became a contributor in 2016, then became the Website Chair and maintainer for 2017. 

I am going to use DjangoCon US website as an example throughout this talk. 

<!--
I asked to do code review for the DjangoCon US website and started doing it. 
* I hope that providing concrete examples will reinforce your understanding

DjangoCon US Website Homepage
DjangoCon US Website Repo
-->

</td></tr>


<tr><td width="30%">

![Slide 9]()

</td><td>

### Prerequisites for Getting Started

* Create a free [GitHub](https://github.com) account online
* Install Git on your computer and set your email and username
* Find and open your computer terminal (a.k.a. command line) on your computer
* The ability to navigate via terminal would be helpful (example: know how to change directory, I will give a few helpful commands later and see bash commands resource in Useful Resources section)
* You might also want to have a text editor of your choice installed, to use to edit files

There are a ton of tutorials out there for getting started. I am going to be focused on workflow because there are fewer tutorials out there for what I am going to explain. 

<!--
* Some tasks vary by operating system- check tabs at the top of GitHub Help pages for special OS instructions
* <variable> is a placeholder for the real thing
By the way, some operating systems do not use dollar signs $ as command line prompts. Just be aware of that.
-->

</td></tr>


<tr><td width="30%">

![Slide 10]()

</td><td>

### What are Git and GitHub?

GitHub is a website built on the version control software Git. Git can be installed used in the command line of your computer. 

<!--
GitHub Website Landing Page
Git command line- verifying Git is installed and the version
-->

</td></tr>


<tr><td width="30%">

![Slide 11]()

</td><td>

### GitHub: Social Network

GitHub is a social network. You can:
* Make a user account and profile
* Follow people
* Follow their activity in your newsfeed
* Find interesting projects

<!--
You have a profile where you store your code in repos
-->

</td></tr>


<tr><td width="30%">

![Slide 12]()

</td><td>

### GitHub: Repositories

GitHub users can store and work on code together in repositories

<!--
DjangoCon US Organization Account List of Repositories
DjangoCon US Website Repo
-->

</td></tr>


<tr><td width="30%">

![Slide 13]()

</td><td>

### Local Development Environment

<!--
You can't do everything in the browser
Using url and git command git clone <url> to clone (make a copy of) the repo, which will then appear
.git folder
now a copy online and a copy in your local development environment
pushing and pulling
-->

</td></tr>


<!--
### What I Would Do Differently

There is a way of doing things that involves the best practices of collaboration and code review and there is a way of doing things that doesn't. In this talk, I will be teaching you the best practices. 
-->


<tr><td width="30%">

![Slide 14]()

</td><td>

### Collaboration and Code Review Best Practice Workflow

In order to be able to increase your level of responsibility, we need to have the freedom to switch between multiple tasks. 
* You keep your main code branch (master) up-to-date
* Create one or more features
* Do code review

</td></tr>


<tr><td width="30%">

![Slide 15]()

</td><td>

### Working on a File in GitHub

</td></tr>


<tr><td width="30%">

![Slide 16]()

</td><td>

### Branches

</td></tr>

<!--
### Branch Diagram

To do this, we need to learn how to use branches

Branches
* Can be used by any GitHub user
* You can have an unlimited number of branches

Two different types
* Feature branches (a.k.a. topic branches)
* Pull requests branches

When the repo is created, by default, there will be a branch named master that contains the initial files. When you want to create a new feature, you can make a copy of the master branch and give the new branch a different name. Now there are two branches, in the same repo, the master branch and a feature branch. If there is more than one branch in the repo, you make a copy of the branch you intend your new feature to be merged into (in this case, the master branch). After you are done working on the feature branch, you submit a pull request for the changes to be merged. The feature branch is now a pull request branch. If the changes are accepted, they will be merged into the intended branch. The master branch will be like before, except with the changes from the branch. 

You will want to keep the master and feature branches up-to-date by merging in updates. If you want to start working on another feature, you can make another new branch off of the branch it's intended to be merged into.  

You can toggle back and forth between the branches by clicking on the branches in the branches tab. You can also create and work on branches in your local development environment, which we will demonstrate later. 

Both feature branches and pull request branches are examples of remote branches. We can work on them in much the same way. 

They are a best practice. 
-->

<tr><td width="30%">

![Slide 17]()

</td><td>

### How to Create a Branch

</td></tr>


<tr><td width="30%">

![Slide 18]()

</td><td>

### Overview

* Determine which collaboration approach to use (there are two)
* Clone the repo that we have write permission to into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo
* Review the two different types of pull requests as a DjangoCon US website repo maintainer

</td><td>


<tr><td width="30%">

![Slide 19]()

</td><td>

### Section 1

* Determine which collaboration approach to use (there are two)

</td></tr>


<tr><td width="30%">

![Slide 20]()

</td><td>

### The Two Collaborative Development Models

There are two different ways to contribute and they have a fancy name. 

The two Collaborative Development Models
* "Shared Repository" Model
* "Fork and Pull" Model

The two different collaborative development models typically correspond to the two different account types

<!--
A Collaborative Development Model is a fancy term for the process users go through to contribute to a repo.
-->

</td></tr>


<tr><td width="30%">

![Slide 21]()

</td><td>

### The Two Types of Accounts and Models

User account (example: my user account), Shared Repository Model
* A user account is a personal account that a user owns

Organization account (example: DjangoCon organization account), Fork and Pull Model
* An account where teams of people are working together

</td></tr>


<tr><td width="30%">

![Slide 22]()

</td><td>

### Write Permission

We are not talking about "write" permission in the context of English. When a user has write permission to a repo, it means they can make changes directly inside of the repo, probably in a feature branch.

The way that you contribute to a repo depends on whether you have write permission to it. 

<!--
Some examples of what I can do within the repo now:
* Push work (a branch) directly to the repo (instead of via fork)
* Edit a file
* Submit pull requests
* Review pull requests

See write permissions chart for info
-->

</td></tr>


<tr><td width="30%">

![Slide 23]()

</td><td>

### Why We Need Write Permission

Example: DjangoCon US website is a deployed live and has a fairly high volume of traffic. We wouldn't want just anyone to be able to go into the DjangoCon repo and directly make changes. Occassionally, a DjangoCon organization account owner may give certain users write permission to be maintainers. There is often a level of trust involved in having write permission.

</td></tr>


<tr><td width="30%">

![Slide 24]()

</td><td>

### "Shared Repository"

Think about the word "shared". A shared repository is typically found in an organization account where there are teams of maintainers who have write permission to the repos working on them together. 

</td></tr>


<tr><td width="30%">

![Slide 25]()

</td><td>

### "Fork and Pull" Model

The “Fork and Pull” Model is typically used in user account repos, because users come across repos they want to contribute to but don’t have write permission to it and need to fork it to contribute 

<!--
Going to need to go into the repo and make the proposed change. You can only do that if you have write permission to the repo
-->

</td></tr>


<tr><td width="30%">

![Slide 26]()

</td><td>

### Write Permission and Collaboration Examples

Example: DjangoCon US Website Repo as a "Shared Repository"

This year I became a maintainer of the DjangoCon US website, so I was given write permission to the DjangoCon US website repo. Along with the other maintainers, I can make changes directly within the DjangoCon US website repo (usually using a feature branch). I no longer need a fork. This is called the "Shared Repository" Model. 

Example: DjangoCon US Website Repo "Fork and Pull" Model

Wen I first wanted to contribute to the DangoCon US website, I was not a maintainer, so I did not have write permission to the repo. So I made a copy (fork0 of the DjangoCon US website repo in my user account, created a feature branch, made a change, and submitted a pull request to the Django US website repo. When a maintainer approved the pull request, the changes were pulled from the fork into the DjangoCon US website repo (that's why it's called a pull request. 

This is the "Fork and Pull" Model. 

In addition to using a fork to propose a change to the original repo, you can also use a fork for the starting point of a new idea of your own (depending on the license). 

</td></tr>


<tr><td width="30%">

![Slide 27]()

</td><td>

### How to Fork a Repo

DjangoCon US website repo is a shared repo

* Click the "Fork" button
* Try to edit a file in a repository that you do not have write permission to. GitHub will automatically fork the repo to your user (or organizational) account, and notify you that it is forking it. 

<!--
Forking graphic
-->

</td></tr>


<tr><td width="30%">

![Slide 28]()

</td><td>

### Forked Repo

This is a copy of the DjangoCon US Website repo in my user account under my user account URL. 

</td></tr>


<tr><td width="30%">

![Slide 29]()

</td><td>

### About Forks

You own all of the repos in your user account, including ones you have created and forks. I am the only user with write permission to it unless I give permission to someone else, such as a maintainer, when I am submitting a pull request. The fork is an exact copy of the original repo at the time it was forked. I could make any changes I wanted to the fork, and the original rep will not be affected, including deleting the fork.

<!--
When you create a user account, you own all of your repos and have write permission to all of them.  

Unless you make a pull request and it is accepted
-->

</td></tr>


<tr><td width="30%">

![Slide 30]()

</td><td>

### Section 2

* Determine which collaboration approach to use (there are two)
* Clone the repo that we have write permission to into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo

</td></tr>


<tr><td width="30%">

![Slide 31]()

</td><td>

### Fork and Pull Model

If you cloned from a fork, when you push to "origin", you will be pushing to the fork.

</td></tr>


<tr><td width="30%">

![Slide 32]()

</td><td>

### Shared Repository Model

If you cloned from a shared repo, when you push to "origin", you will be pushing to the shared repo. 

</td></tr>


<tr><td width="30%">

![Slide 33]()

</td><td>

### Local Development Environment

The process will be almost the same regardless of whether we are working from a shared repository or fork and pull.

 The two main differences are that if you are using the "Fork and Pull" Model:
* If you do not have write permission to the source repo, you need to fork the repo before you use the URL to clone it
* When you submit the pull request, a box will be checked by default giving (upstream) maintainers the ability to edit the pull request (like I said, maintainers do not automatically have write permission to a fork). 

</td></tr>

<!--
### Local Branch Process

Git Magic
When we are working on code, we can’t do everything in the GitHub website. We sometimes need to make a copy of our code in our local development environment. When we are working on code, we can't do everything in the GitHub website. There is where Git is very useful. 

For example, the code in the DjangoCon US website repo is for a website. We cannot run it on GitHub. We sometimes need to make a copy of the code in the local development environment of our computer, install any necessary software, run the code in a local browser on a local server. 

This could be so that we can add a feature to it, or it could be so that we can look at a change proposed by a pull request and decide how to proceed.  
This could be because we want to create a new feature. Or it could be because someone has proposed a change and we want to test change before accepting it.

Git is installed in our local development environment and we use it by tying commands in the command line. When we have Git initialized in a project, there is a hidden folder named .git that contains the Git configuration information that helps Git track certain things, such as which repo the code was cloned from. 

* I work in my home directory, which you can see from the command prompt. 
* The GitHub repo has been cloned using its URL
* There is now a folder on the computer in my home directory by the same name as the GitHub repo I just cloned and filled with the contents of the repo and a .git folder
* I now have a copy of the codebase on my computer and a copy online in a GitHub repo
* When I stage any changes I make, Git will record the changes to the files
* I can push and pull changes between the local development environment and the GitHub repo
* Meanwhile other users can work on the code on their computer and push the changes back to GitHub 
* Our changes are all merged into the GitHub repo we are working on
* Git will tell us if there is a conflict.

You can see the corresponding folders and files
The format may be a bit different because on your local computer, you are going to be working on raw files

### Remotes

When you clone a repo to your local development environment, Git will know where you cloned your code from and will name this remote repo "origin". When you make a change to a GitHub repo, or in your local clone, the code elsewhere does not automatically update with the change. You can refer to the origin on the command line to push and pull code back and forth between your local development environment and GitHub repo, to keep them in sync.

You can add other remote repos to your local clone and give them a name in order to push and pull from them. We will see an example of this later when we are keeping a fork up-to-date. 

clone: local copy of a repo
push: transfer changes from local clone to online repo
pull: transfer changes from online repo to local clone

When you a change is made to the DjangoCon US website repo, the fork does not automatically update. When you make a change to an origin, your local code does not automatically update. When you make a change to your local code, your origin does not automatically update. 
-->

<tr><td width="30%">

![Slide 34]()

</td><td>

### GitHub Repo Versus Local Directory

</td></tr>


<tr><td width="30%">

![Slide 35]()

</td><td>

### Working on a File Locally

</td></tr>


<tr><td width="30%">

![Slide 36]()

</td><td>

### Local Development Environment

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Commands

Clone (or download) the repo you have write permission to using the repo URL (this repo will be your origin)

```bash
$ git clone <repo-url>
```

Example: clone (or download) an organizational repo (organizational repo will be "origin")

```bash
$ git clone https://github.com/<organization-name>/<repo-name>
```

Example: clone (or download) a user account repo (repo needs to have already been forked to user account, forked repo will be "origin")

```bash
$ git clone https://github.com/<user-name>/<repo-name>
```

Change directory into the folder of the repo you cloned. Folder name will be the repo name.

```bash
$ cd <repo-name>
```

Verify which branch you are checked out on (important if more than one branch); you will be checkout out on the default branch initially (in this case master, which is the norm)

```bash
$ git branch
```

Create and checkout (switch) to a feature branch, branching off of the branch you intend your changes to be merged into (note how the local files switch to the files of the branch you are checked out on, exactly the same at first, but if you make a change in a branch and then switch back and forth between branches, you can see the difference)

```bash
$ git checkout -b <branch-name>
```

Make your change, then add, commit, create a message (if you don't use -m, a Vim editor will open and you will need to know how to exit)

```bash
$ git add .
$ git commit -m "Your note"
```

Push the new branch to GitHub to your origin (by default, the origin is the repo you cloned from that you have write permission to); This can also be used to push additional commits

```bash
$ git push origin <branch-name>
```

There will now be a new branch in the repo that is your origin. The branch will not be affecting anything else. If you never did anything else with it, it would just exist there.

<!--
DjangoCon and fork as examples

Folder/files/text editor
-->

</td></tr>


<tr><td width="30%">

![Slide 37]()

</td><td>

### New Branch

</td></tr>


<tr><td width="30%">

![Slide 38]()

</td><td>

### Submit a Pull Request

In the browser, go to the repo you want your pull request to be merged into, in this case, the DjangoCon US website repo. 

There should be a message prompting you to submit a pull request because GitHub will detect your branch and suggest for you to submit a pull request, even if your branch is in a fork. Be forewarned, that if you forked the repo and you go to your fork instead, you can accidentally submit a pull request to yourself. 

* Make sure base corresponds to the repo and branch you want to contribute to
* Make sure compare corresponds to your branch
* Create a pull request title and perhaps a description
* If the pull request is via a forked repo, a box will be checked by default giving (upstream) maintainers the ability to edit the pull request 
* Click "Create pull request"

If you are submitting the pull request from within the repo:
* base: master compare:<branch-name>

If you are submitting the pull request a forked repo:
* base fork: django/2017.djangocon.us base: master head fork: katherinemichel/2017.djangocon.us base: <branch-name>

</td></tr>


<tr><td width="30%">

![Slide 39]()

</td><td>

### Section 3

* Determine which collaboration approach to use (there are two)
* Clone the repo that we have write permission to into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo
* Review the two different types of pull requests as a DjangoCon US website repo maintainer

</td></tr>

<!--
Perspective: Reviewing Pull Requests
Point of view: organizational maintainer
Organizational repo is your “origin”
Forked repos branches are remotes
Pull requests are branches
-->

<tr><td width="30%">

![Slide 40]()

</td><td>

### Pull Request Review Process

* If you are a repo maintainer, you will receive a message (by browser or email, based on your notification preferences) to let you know there is a pull request
* Follow the link to the pull request in the repo pull request tab in the browser
* Look over the information about the pull request provided by the contributor

* There will a set of command line instructions for reviewing the pull request locally. The set of instructions will be slightly different depending on whether the pull request was submitted from within the organization as "Shared Repository" Model or from the forked repo (remote branch) as "Fork and Pull" Model.  

</td></tr>




<tr><td width="30%">

![Slide 43]()

</td><td>

### Remote Branches

</td></tr>


<tr><td width="30%">

![Slide 44]()

</td><td>

### Remote Tracking Branches

</td></tr>









<tr><td width="30%">

![Slide 00]()

</td><td>

### Perspective: Checking Out Remote Branches

We are DjangoCon US website maintainer with write permission to the DjangoCon repo. The DjangoCon US website repo is our origin. 

The forked repo is not an origin for us and we do not have write permission to it, unless we given permission, for example to edit the pull request as a DjangoCon US website maintainer. 

</td></tr>


<!--
Why are the Instructions Different?

When we are working from within the origin, we can temporarily fetch all of the updates from the origin into the hidden .git folder that contains all of the Git configuration information. When we fetch these updates, they will include branches and commits made directly to the DjangoCon US website, but they will not include branches created through a fork or a pull request branch from a fork, because they come from outside of the origin. 

There are three types of branches:
* remote branch (in a remote repo)
* remote-tracking branch (inside of the hidden .git folder, which stores info)
* local branch

```bash
$ git fetch --prune
$ git branch -a
$ git branch -r
```

<!--
Fetching from Origin Versus Pulling from a Fork
These instructions work for any remote branch. 
etch or pull a remote branch (feature branch or pull request branch) into your local folder and work on it 
We've already talked about the concept of remotes when we talked about origin. 
-->


</td></tr>



<tr><td width="30%">

![Slide 00]()

</td><td>

### Checking Out Remote Branches

Feature branches and pull request branches are both remote branches. 

The feature branch will become a pull request branch when a pull request is submitted. And eventually a maintainer will decide whether to merge the branch into the branch it is intended to be merged with. 

Any person with write permission to a remote branch can fetch it to their local development environment and add commits to it, even if a pull request has already been made. If a pull request has already been made, the additional commits will be automatically added to the pull request when you push the additional commits to the branch, up to the point that the pull request is merged. 

</td></tr>



<tr><td width="30%">

![Slide 00]()

</td><td>

### Pull Request Review Options

There are two ways to merge a pull request
* Via browser (click merge button- options are regular, squash, or rebase merge)
* Via command line locally

Simplest scenario
* When you look at the pull request in the browser, you can tell it can be accepted and click merge (for example, if the pull request is fixing a typo) 

Second simplest scenario
* You look at the pull request in the browser. You need to change something, but you can change it in the browser. You edit the file in the browser and click merge (for example, if you fix a typo in the pull request) 

Less simple
* You can't always accept the pull request based on just looking at the code in the browser
* You sometimes need to run the code in the pull request locally to evalute it

After you run the code locally, if you decide a change does need to be made
* You can go back to the browser and click merge

After you run the code locally, if you decide a change needs to be made, there are a few options
* As the contributor to make a change to the pull request
* Push additional commits yourself to the pull request branch
* You can make the change locally, merge the branch with the branch it is intended to be merged with locally, and push to the branch on GitHub


<!--
https://help.github.com/articles/committing-changes-to-a-pull-request-branch-created-from-a-fork
* push to origin (follow instructions, live branch/deployed?)
An example would be if the code for a website has been updated and submitted as a pull request. You can fetch the pull request branch to your computer. 
Checkout a pull request locally

Merge pull request in browser
Merge pull request locally and push to branch
Ask pull request contributor to update pull request
Update the pull request yourself

Flow chart of possibilities:
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Shared Repo Model Feature Branch or Pull Request Branch

Fetch updates to your local .git folder. Create a local branch and insert the contents of the remote branch into it. Merge the master branch into it to keep it up to date. (If the repo was cloned before the pull request)

```bash
$ git fetch origin
$ git checkout -b <local-branch-name> origin/<branch-name>
$ git merge master
```

Push additional commits to organizational feature branch or pull request branch

```bash
$ git push origin <branch-name> 
```

Push additional commits to organizational feature branch or pull request branch, if local branch name is different than pull request branch name
 
```bash
$ git push origin <local-branch-name>:<remote-branch-name>
```

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Forked Repo Model Feature Branch or Pull Request Branch

Because it is outside of the origin, it is not fetched in updates. We need to fetch it by its URL. 

Create and checkout a new branch (in this case off of the master branch, but could be another). Pull the contents of the remote forked repo branch into it (could be as a feature branch or a pull request branch).

```bash
$ git checkout -b <local-branch-name> master
$ git pull https://github.com/<user-name>/<repo-name> <branch-name>
```

Push additional commits to forked repo feature branch or pull request branch (contributor needs to have given permission, and local branch name and remote branch name need to match)

```bash
$ git push https://github.com/<user-name>/<repo-name> <branch-name>
```

Push additional commits to forked repo feature branch or pull request branch, if local branch name is different than pull request branch name

```bash
$ git push https://github.com/<user-name>/<repo-name> <local-branch-name>:<remote-branch-name>
```

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Merge Pull Request Locally and Push to Master Branch

Step 2: Merge the changes and update on GitHub. (Same process no matter where the pull request originated), (merge into the appropriate branch)

```bash
$ git checkout master
$ git merge --no-ff <local-branch-name>
$ git push origin master
```

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Alternatively, Fetch Individual Pull Request

Pull updates to the individual pull request into your local branch

```bash
$ git pull origin pull/<pull-request-number>/head:<branch-name>
```

Alternatively, fetch the individual pull request into your folder

```bash
$ git fetch origin pull/<pull-request-number>/head:<branch-name>
```

Example

```bash
$ git fetch origin pull/1/head:patch-1
```

<!--
See also, pull request shortcuts
-->

</td></tr>


<tr><td width="30%">

![Slide 39]()

</td><td>

### How to Deal With Merge Conflicts

Two ways to resolve a merge conflict
* In the browser
* In the local development environment by command line

<!--
Addressing merge conflicts- "competing changes", resolving on GitHub/through command line/text editor
About merge conflicts- Resolve conflicts buttons, can't push until resolved
Resolving a merge conflict on GitHub- only "competing line changes", otherwise do locally
"Delete the conflict markers <<<<<<<, =======, >>>>>>> and make the changes you want in the final merge."
Resolving a merge conflict using the command line- varies by OS, revisit
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>


### Tidy Up

When the pull request is accepted, delete the branch. It's good practice to delete merged or stale branches.  

* Close pull request
* Revert pull request (hopefully not needed)
* Delete local and remote (in browser) feature branch

Delete a branch

```bash
$ git branch -d  <branch-name>
```

Force delete branch

```bash
$ git branch -D  <branch-name>
```

Delete remote branch

```bash
$ git push <remote-name> :<branch-name>
```

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Syncing Changes

Keep master branch up-to-date

Fetch new branches and commits from the remote repository to local .git folder (add a remote first, if needed), without merging them locally. The branches stored here are called remote-tracking branches.  

```bash
$ git fetch <remote-name>
```

Checkout the branch you will be merging updates into (presumably the branch already exists)

```bash
$ git checkout <branch-name>
```

Merge remote-tracking branch updates with branch you are currently checked out on

```bash
$ git merge <remote-name>/<branch-name>
```

The remote name is often origin or upstream.

Origin example

```bash
$ git fetch origin
$ git checkout master
$ git merge origin/master
```

Upstream example (syncing a fork)

```bash
$ git fetch upstream
$ git checkout master
$ git merge upstream/master
```

Push the changes to your corresponding branch in the forked repository in GitHub

```bash
$ git push origin master
```

Keep feature branch up-to-date (often merging master into feature branch)

```bash
$ git checkout <feature-branch-name>
$ git merge <branch-name>
```



Do not pull remote tracking branch updates (defeats the purpose because you already did $ git fetch (updated remote tracking branch with remote changes), which is $ git fetch + $ git merge in one command)

```bash
$ git pull <remote-name>/<branch-name>
```

If pull remote tracking branch updates, and have a problem

```bash
$ git merge --abort
```



Instead, pull directly from the remote repository branch ($ git fetch + $ git merge in one command)

<!--
Pushing and pulling via <remote-name>
-->

```bash
$ git pull <remote-name> <branch-name>
$ git push <remote-name> <branch-name>
```

Pushing and pulling via remote URL (will come in handy later when we are working with pull request from a fork)

```bash
git pull https://github.com/<user-name>/<repo-name> <branch-name>
git push https://github.com/<user-name>/<repo-name> <branch-name>
```

<!--
Here are the generic commands you can use to push and pull

If you are pushing, you need to have write permission to the branch. The remote can be represented by a <remote-name> or a remote URL
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Adding an Upstream Remote and Syncing a Fork

The git remote add command takes two arguments:
* A remote name, for example, upstream (you will be using this name in commands to refer to the remote)
* A remote URL, for example, https://github.com/upstream-username/original-repository

Add a remote

```bash
$ git remote add <remote-name> <remote-url>
```

Verify existing remote repository

```bash
$ git remote -v
origin  https://github.com/your-username/your-fork (fetch)
origin  https://github.com/your-username/your-fork (push)
```

Add upstream remote repository that will be synced with the fork

```bash
$ git remote add upstream https://github.com/upstream-username/original-repository.git
```

Verify new upstream remote (can only push to upstream if have write permission)

```bash
$ git remote -v
origin  https://github.com/your-username/your-fork (fetch)
origin  https://github.com/your-username/your-fork (push)
upstream  https://github.com/upstream-username/original-repository (fetch)
upstream  https://github.com/upstream-username/original-repository (push)
```

<!--
If you clone from the “Shared Repository”, you can just fetch changes directly to your local repo because there is no fork 
If you forked the “Shared Repository”, you need to update the fork without deleting it. You do this by adding the “Shared Repository” as an upstream, fetching changes, and pushing them to your origin , which is the the fork
-->

</td></tr>




<tr><td width="30%">

![Slide 00]()

</td><td>

### Another Workflow

</td></tr>

<!--
* The process is based on GitHub Flow, which is a simple, agile process

Which Workflow Should I Use?

Use the workflow that is right for the projects
They all have pros and cons
A mission critical project with a high volume of users is likely to use a develop branch and staging to gate-keep updates before going live
-->

<tr><td width="30%">

![Slide 00]()

</td><td>

### Learn More About Workflow

* Git Flow (basically, the workflow we've been using)
* A Successful Git Branching Model (more advanced)
* A Successful Git Branching Model Considered Harmful (alternative view)
* SemVer
* See also: Atlassian and GitLab docs (you can also find insights in the docs of other software built on top of Git)

<!--
* Tags
* Releases
-->

</td></tr>

<!--
### Workflow Decisions

Some project will have a master branch and a develop branch. The development branch will be done in the develop branch. The develop branch will be merged with the master branch when the work is production ready. 

If you choose to use a develop branch:
* In addition to the master branch, create the develop branch
* Choose a default branch (the default branch will be the first branch you see when you look at a repo, it will be the branch you are checked into when you cd into a folder after cloning, and it will be the default base for a pull request)
* Default branch is usually master branch

For example, a mission critical project with a high volume of users is likely to use a develop branch and stage updates before going live. 

Which workflow is "best"? Depends on what you are trying to accomplish. Use the workflow that is right for the projects. They all have pros and cons. Some developers have passionate views about this topic (see comment threads in some posts). 
-->



<tr><td width="30%">

![Slide 00]()

</td><td>

### Organization and Team Setup

</td></tr>


<tr><td width="30%">

![Slide 39]()

</td><td>

### Safeguards Checklist

Setting Up Repo Fail Safes
* Back up the repo (third-party software)
* Protect main branch(es) 
* Enable required reviews of pull requests
* Decide whether to use status checks (external)
* Worst case scenario: How to recover deleted branch
* Sensitive data warning (if made public, consider compromised, immediately remove and change)

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Community and Communication Strategy

* What impression you want to give people about your project? Hopefully welcoming, user-friendly. 
* How can you make contributor experience easier/faster/enjoyable (for example, tell people how to contribute)
* Draft community guidelines

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Documentation

<!--
* README.md
* LICENSE (auto-generate, legality of contributions, attribution)
* CODE_OF_CONDUCT.md (auto-generate, choosing from two different Codes of Conduct)
* CONTRIBUTING.md (look at examples for ideas, will generate a message "Please review the guidelines for...")
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Issue and Pull Request Templates

* ISSUE_TEMPLATE
* PULL_REQUEST_TEMPLATE

<!--
* Issues Tab
* Pull Requests Tab
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Forums

* Wikis
* GitHub Pages/Jekyll
* Gists

</td></tr>


<tr><td width="30%">

![Slide 39]()

</td><td>

### Productivity Tips

* Cache your password
* Set up special configs (example: line endings)
* Create saved replies
* Link to specific line number on GitHub

<!--
* Request a review from a specific person
* Close an issue via commit message by using keyword

# Notifications

- [ ] Find the Notifications Overview Page
- [ ] Decide which notifications to receive, whether by browser or email, and which email to receive at

# Conversations

Where They Happen
* Issues
* Pull Requests

Helpers
* GitHub Flavored Markdown 
* @mentions (of people and teams)
* Issue and PR references
* Emojis

Writing and Formatting
* Get to know GitHub Flavored Markdown
-->

</td></tr>



<tr><td width="30%">

![Slide 00]()

</td><td>

### Tips for getting started

* “Help Wanted” tags, topics/First-timers initiatives
* Look for community-oriented projects and other welcoming projects
* Cherry pick problems or issues that fit your skill level
* Look for triaging (example: node.js website issues)
* Practice your skills and workflow (don't be afraid to delete/start over)
* You can create your own sandbox by making pull requests on your own account or setting up an organization to learn more about options for maintainers

</td></tr>



<tr><td width="30%">

![Slide 00]()

</td><td>

### Getting Help

* Help via Git, GitHub Help and Guides (links in Useful Resources Section)
* Help via GitHub Keyboard Shortcuts (type "?")
* Help via command line (exit by typing "q")

```bash
$ git help <verb>
$ git <verb> --help
$ man git-<verb>
```

```bash
$ git help clone
$ git clone --help
$ man git-clone
```

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Thank You

You can also contact me by email or on Twitter.

Useful Links: 
https://git.io/v7LGr

* Twitter handle: @KatiMichel
* GitHub username: KatherineMichel

<!--
Talk slides and other resources online
-->

</td></tr>


</table>

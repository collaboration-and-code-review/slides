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

* Ana Balica's ([Twitter](https://twitter.com/anabalica), [GitHub](https://github.com/ana-balica)) transcript of her [Humanizing among coders](https://ana-balica.github.io/2017/05/28/humanizing-among-coders/) keynote for [PyCon CZ 2016](https://cz.pycon.org/2016/). 
* Honza Javorek's ([Twitter](https://twitter.com/honzajavorek), [GitHub](https://github.com/honzajavorek)) transcript of Anna Ossowski's ([Twitter](https://twitter.com/OssAnna16), [GitHub](https://github.com/OssAnna16)) keynote [Be(Come) A Mentor! Help Others Succeed!](https://github.com/honzajavorek/become-mentor) for [PyCon CZ 2017](https://cz.pycon.org/2017/). 

Thank you!

## Transcript

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

Thank you for being here. I'm thrilled to have the opportunity to talk to you about getting a jumpstart on collaboration and code review in GitHub

</td></tr>


<tr><td width="30%">

![Slide 3]()

</td><td>

### About Me 

* DjangoCon Website Chair (where I learned a lot of what I"m going to be teaching you)
* DEFNA (Django Events Foundation North America) Board Member
* Project Manager
* Web Designer and Developer

I hope you've had a chance to take a good look at the DjangoCon website. I'm so proud of what the team has accomplished. It's truly a beautiful website.

</td></tr>


<tr><td width="30%">

![Slide 4]()

</td><td>

### The Journey

Let’s pretend we’re going on a journey. The journey is to learn collaboration and code review. I've made this Journey Before. When you are making a journey, often you are engrossed in each step. When you complete the journey, looking back, perhaps you see the larger picture and have learned something. If I were to start my journey of learning collaboration and code review over again, knowing what I know now, I would do things differently from the beginning. 

I want to impart some of my knowledge to you, to save you the time and frustration of learning by trial and error the way that I did, because I want all of you to get started more quickly than me.

</td></tr>


<tr><td width="30%">

![Slide 5]()

</td><td>

### What is the Destination?

Do you remember a time before you were interested in building things with code? There is a lot of power and value in the ability to make things. You can apply collaboration and code review skills in an unlimited number of situations. GitHub is a very popular place to work on open-source code. Check out GitHub Showcases and Trending to see some of the awesome projects.  

Some benefits of learning collaboration and code review
* If you are a student: being prepared for your studies and career
* If a developer: perhaps you can get a promotion
* In general: you can make cool stuff, make choices that influence product

</td></tr>

<!--
### GitHub Audiences

Organizations
* For-profit (business)
* Not-for-profit

People
* Professional developers
* Hobbyists
* Students

Types of Projects
* Cutting edge
* Novelty
-->

<tr><td width="30%">

![Slide 6]()

</td><td>

### How My Own Journey Began

I want to do a bit of a flashback now. 

I first signed up for GitHub on April 18, 2013. I knew using GitHub was a good idea. But my account sat unused for months. I felt a bit intimidated. I wasn't sure if I fit in and I didn't know how to get started. Later on in this talk, I will debunk some of the myths that I believed at the time. 

</td></tr>


<tr><td width="30%">

![Slide 7]()

</td><td>

### TacoFancy

7 months later, I happened to be looking at Twitter. I saw a tweet from a man named Dan Sinker who works in journalism and web development. He had made a really delicious Mexican meal and he and a few other people had decided to start a project on GitHub to share Mexican recipes. 

So I clicked on the link to the repo (definition?) to take a look. 

</td></tr>


<tr><td width="30%">

![Slide 8]()

</td><td>

### The One Sentence that Motivated Me to Start Using GitHub

One sentence in the project README (definition?) made a big impact on me: "Are You New to Github But Want to Contribute?" 

I had been wanting to contribute for months, but wasn't sure how, and now was my chance. I felt it was my destiny to contribute now. 

</td></tr>


<tr><td width="30%">

![Slide 9]()

</td><td>

### My First Pull Request

I didn't quite feel like I knew what I was doing, but I was extremely motivated. I struggled through and submitted my first pull request. As is often characteristic of moments of achievement like this, there was a huge adrenaline rush. 

</td></tr>


<tr><td width="30%">

![Slide 10]()

</td><td>

### It Would Take Almost 3 More Years for Me to Do Code Review

Unfortunately, it would take almost 3 more years for me to begin doing code review. Now that I do it, I wonder, why did it take so long?! It didn't have to be that way.

<!--
This doesn't make sense in terms of the number of maintainers.
Bus Factor
-->

</td></tr>


<tr><td width="30%">

![Slide 11]()

</td><td>

### What This Talk Is and Isn’t

<!--
There is a saying, "Don't miss the forest for the trees". It means, don't focus so much on the details that you don't see the larger picture. I think quite often, when people are using Git and GitHub, they are focusing on the details and missing the larger picture. This talk is about the larger picture. 
-->

This talk is about teaching you the essential process and the underlying common thread between collaboration and code review, so that you can get started as quickly as possible. 

There are many variations to how things can be done in GitHub. This talk is not about teaching you all of those variations. At the end of this talk, you will find links to the official documentation of Git and GitHub where you can find info about variations. 

</td></tr>


<tr><td width="30%">

![Slide 12]()

</td><td>

### A Few Notes

* This talk uses GitHub examples, but similar features and workflows could be found in Bitbucket or other services (which some people prefer)
* We will focus on command line, not browser or GUI (such as GitHub Desktop). Can only make full use of git functionality by using command line. 
* The examples I will be using will focus on public, organizational repos and “Shared Repository Model”, because that is where most of the collaboration and code review are done
* The process is based on GitHub Flow, which is a simple, agile process
* I will identify best practices any time possible
* Some tasks vary by operating system- check tabs at the top of GitHub Help pages for special OS instructions

<!--
You will use terminal/command line often with code review.

(<> symbol denotes a placeholder/variable)
Using HTTPS examples
Example- some operating systems do not use dollar signs $ as command line prompts.
-->

</td></tr>


<tr><td width="30%">

![Slide 13]()

</td><td>

### Getting Started

* Install Git on your computer and set your email and username
* Create a free [GitHub](https://github.com) account online
* Find and open your computer terminal (a.k.a. command line)
* The ability to navigate via terminal would be helpful (example: know how to change directory)
* You might also want to have a text editor of your choice installed, to use to edit files

There are a ton of tutorials out there for getting started. I am going to be focused on workflow because there are fewer tutorials out there for what I am going to explain. 

<!--
Bash command list, text editor recommendations
-->

</td></tr>


<tr><td width="30%">

![Slide 14]()

</td><td>

### Getting Help

* Help via Git, GitHub Help and Guides (links in Useful Resources Section)
* Help via command line

```bash
$ git help <verb>
$ git <verb> --help
$ man git-<verb>
```

There will also be some Keyboard Shortcuts in the Productivity Tips part of my talk

</td></tr>




<tr><td width="30%">

![Slide 15]()

</td><td>

### Git and GitHub Tour

<!--
What are open-source, Git and GitHub?
-->

High level explanation: Git is a version control system that you install on your computer and use via your terminal. Some people came along and decided to create a web-based dashboard that you can use in connection with Git. I kind of think of GitHub as being like Facebook for developers. You have a profile where you store your code in repositories (a.k.a repos) and you have a newsfeed where you can see the activity of developers you follow. Organizations can have accounts too. If you want to work on code, you can clone or download a repo onto your personal computer, make your changes, then push the changes back to the repo on GitHub. Meanwhile, other users can add their own changes. Git and GitHub will record every change to a file and will tell you if there is a conflict between the changes of two different people. 

GitHub Vocab and Tour

* source!!!!! (the original code base, probably an organizational repo that is being used as a "Shared Repository" that people without write access fork

* repo (a place where a code base is stored)
* fork (copy of an entire repo)
* branch (a copy of a code base within a repo, often a "feature branch")

<!--
Some things can be done by browser or command line; some things can only be done by command line
Can create, add, rename, move file in browser or from command line (images are an exception)
Can make a branch by command line or in the browser
Images can be drag and drop/upload, but can't rename or move in browser

Called a pull request because the changes are "pulled into the source repository by the project maintainer."

About forks
"Original repository, also known as the "upstream" repository"
"synchronizing your fork with the upstream repository"
Configuring a remote for a fork- different depending on OS
"You must configure a remote that points to the upstream repository in Git to sync changes you make in a fork with the original repository."
Syncing a fork- see process, varies by OS
"Syncing your fork only updates your local copy of the repository. To update your fork on GitHub, you must push your changes."
Merging an upstream repository into your fork- revisit, varies by OS

Creating and deleting branches within your repository- branch selector menu, click  NUMBER branches to delete
Viewing branches in your repository- branches tab, can delete, change default
Create a branch by command line or in the browser below the commit message field. 

When you try to edit a repository that you do not have read/write access to, GitHub will automatically fork the repo to your user account. After you commit the change, you can submit a pull request.
Or, you can click the "Fork" button. 

Editing files in another user's repository
"When you edit a file in another user's repository, we'll automatically fork the repository and open a pull request for you." "Above the new content, click Preview changes."

"Deleting a fork does not delete the original upstream repository. In fact, you can make any changes you want to your fork--add collaborators, rename files, generate GitHub Pages--with no effect on the original."

A fork is a copy of the repo in your user account that you can make your proposed changed to. The fork will be an exact copy at the time that it was forked, in your account, with your username in the URL. You will be the only person with read/write access to it unless you give read/write access to someone else. If you make changes to it, the repo you want to contribute to will not be affected unless you submit a pull request and it is accepted. 
-->

* local development environment (your computer environment)
* clone (a local copy of a repo)

* remote (the default name for the remote you cloned from)
* origin
* upstream

<!--
### A Note About Remotes

What is origin? The place where your code originates from.

When you clone a repo locally, the remote will automatically assigned the remote name "origin". That means that when you push changed files to origin, you are pushing the files to the repo that you cloned from. For example, if you cloned from a fork, you will be pushing to the fork. If you cloned from an organizational repo, you will be pushing to the organizational repo. Then, you will submit a pull request from there.

* Understand difference between origin (the default remote, and where you clone from), upstream (where you pull from), and fork (user account copy)
* If you cloned from an organization, the origin is the organization account, if you cloned from a fork, the origin is your user account
-->

* git fetch (obtain code locally, without merging)
* git merge (merge code)
* git pull (fetch and merge, all in one action)

* pull request

* Some things can be done in both browser or command line, some things only by command line locally.

Examples of How to Do Important Things in Browser versus Locally

Action |Browser | Command Line
:---: | --- | ---
Fork a repo | Can only do in browser | N/A
Create a branch | Open a file and choose "Create a branch new..." | ```$ git checkout -b <branch-name>```
Delete a branch | Branch tab | ```$ git branch -d  <branch-name>```
Create a file | Click "Create new file" button | ```$ touch <file-name>```
Add a file | Click "Upload files" button | ```$ git push origin <remote>```
Commit | Click "Commit changes" button in an open, altered file | ```$ git commit -m  "Your note"```
Open an issue | Can only do in browser | N/A
Open a pull request | Can only do in browser | N/A

<!--
Browser and Local Graphic 

# Organization and User Accounts

- [ ] Create a user account repo
- [ ] Create an organization
- [ ] Take a user account tour and understand the parts
- [ ] Take an organizational account tour and understand the parts
- [ ] Understand how to create teams with permissions
- [ ] Access your organizational account and dashboard
- [ ] Create an organizational repo
-->

</td></tr>


<tr><td width="30%">

![Slide 16]()

</td><td>

### Write Permission and Why It Matters

Write Permission is an important concept in GitHub collaboration

* Regardless of what repo you are contributing to, whether or not you have write permission to the repo determines how you contribute to it
* If you have write permission to a repo, you can make changes directly within the repo

<!--
What Does Write Permission Allow You to Do?

Write permission is special access.

See write permissions chart for info
Write permission allows you to do things like push a branch directly to the repo (not by fork), change a file, review pull request, etc.
You have to have read/write access to do tasks
Look at "Shared Repository" permissions

Definition of write
We're talking about "write" in the context of...
-->

</td></tr>


<tr><td width="30%">

![Slide 17]()

</td><td>

### Two Collaborative Development Models

The question of write permission leads us to collaborative development models. Collaborative development model is just a fancy term for how people contribute to repos. The two collaborative development models correspond to whether you have write permission.

The two collaborative development models: 
* If you do not have write permission to the repo, you need to make a copy of the repo in your user account or an organization (the copy is called a fork), make your changes, and submit a request for the changes to be accepted to the source repo (this is called a pull request). This is the “Fork and Pull” Model
* If you have write permission to a repo (user account or organizational), you can make changes directly within the repo along with other users, this is called the “Shared Repository” Model

</td></tr>


<tr><td width="30%">

![Slide 18]()

</td><td>

### "Shared Repository" Model Etiquette

Even if you have write permission to a "Shared Repository", it is still common to submit a pull request, but you can do it from within the repo. There is often a level of trust involved, for instance, if you are added to an organization as a maintainer of a critical project. If you make a change to the repo without submitting a pull request first, you may be changing code in a live branch. Whether or not you want to do that depends on your level of comfort with the project. It's often still best to have another maintainer review your work through a pull request.

</td></tr>


<tr><td width="30%">

![Slide 19]()

</td><td>

### User Account

Example: 

* One owner with full control over sources and forks (this is an example of "Fork and Pull" Model)
* Owner can give other users write permission to a repo (this is an example of "Shared Repository" Model)

<!--
An organization can also fork and pull
-->

</td></tr>


<tr><td width="30%">

![Slide 20]()

</td><td>

### Organization Account

Example: 

* One or more owners who have full control over the organization
* Owners can give other users write permission to "Shared Repositories" (this is an example of "Shared Repository" Model)
 
</td></tr>


<tr><td width="30%">

![Slide 21]()

</td><td>

### Shared Repository Model: User Account Versus Organization

Using an organizational account "Shared Repository" rather than a user account "Shared Repository" for collaboration has some advantages:
* With a user account "Shared Repository", there is one owner and the collaborators have access to an individual repo
* The advantage of an organizational account, is that an owner can create teams and permissions across multiple repos
* Otherwise, the repo "Shared Repository" settings are almost exactly the same

</td></tr>


<tr><td width="30%">

![Slide 22]()

</td><td>

### Collaboration and Code Review Best Practice Workflow

There is an overall theme to this talk. In order to be able to increase your level of responsibility, you need to be able to switch between multiple tasks. 
* Keep your code up-to-date
* Create one or more features
* Do code review

</td></tr>


<tr><td width="30%">

![Slide 23]()

</td><td>

### Example of a Not-Scalable Workflow

* Fork a repo, make changes directly into the branch you want to change, then submit a pull request. You are then stuck waiting until the pull request is resolved. If you delete the fork and refork the repo, the pull request can still be accepted, but the process becomes more complicated because it's now considered an inactive pull request and it will be more difficult for you to add additional commits to if you are asked to, and for the reviewer to accept.

<!--
Positives
* Enable follow on commits to be pushed to a pull request (contributor needs to give repo maintainers permission if via fork)
* Prevent inactive pull requests
-->

</td></tr>


<tr><td width="30%">

![Slide 24]()

</td><td>

### How Do We Switch Between Multiple Tasks

Feature Branches (a.k.a. Topic Branches)
* Feature branches are a best practice
* Can be used by any GitHub user
* Give you more freedom

<!--
Pull request branches
-->

If you learn to use branches, you will have the fundamentals skills and freedom that will help you to do both collaboration and code review. 

</td></tr>


<tr><td width="30%">

![Slide 25]()

</td><td>

### What is a Branch?

<!--
A branch is a copy of code inside of your repo.

Within your a repo is a codebase. You can make a copy of the codebase within the repo. The copy is called a branch. When you are finished making changes to a branch, you can submit a pull request and if the pull request is accepted, your changes will be merged into the codebase. Git will replace the old part of the codebase with your changes, and keep everything else the same. Meanwhile, you can keep your codebase up to date and make unlimited new branches. When you review pull requests, the pull requests will also be in the form of branches. 
-->

</td></tr>


<tr><td width="30%">

![Slide 26]()

</td><td>

### Perspective

Our perspective is of a person who has cloned a repo (either the organizational repo or a fork) that he or she has write permission to, is going to create a feature branch, make changes to the feature branch, push the branch back to the origin, and submit a pull request for the changes to be merged into the source.

</td></tr>


<tr><td width="30%">

![Slide 27]()

</td><td>

### Branch Process Overview

The process for working with branch is very similar for anyone, regardless of which collaborative development model you are using ("Shared Repository" or "Fork and Pull"). Parts of this process can be reused, for instance, during code review. 

<!--
* Checkout to a feature branch)

The user will make a change in the browser, or clone the repo locally, and make change and push back to user account (which is the origin). User will submit pull request via own account. 

* Fork an organizational/user account repo

Typical "fork and pull" situation/process: a user forks a repo within GitHub. New repo will appear in user account, with username in repo URL. Go to the fork, which will be in your user account. 

Best practice "Shared Repository Model" workflow
Typical situation/process: User clones the repo locally using the organizational repo URL (the organizational repo is the origin). 

# Clone/Download and Push Feature Branch to Repo (Almost Same Process for Forked Repo or Organizational Repo)

The two main differences are that if you are using the "Fork and Pull" Model:
* If you do not have write permission to the source repo, you need to fork the repo before you clone it
* When you submit the pull request, a box will be checked by default giving maintainers the ability to change the pull request

* Perhaps clone or download the forked repo/organizational repo (this is the place you have write permission to and will be your origin)
* Change directory
* Verify which branch you are checked out on

* Create a new feature branch, branching off the branch your changed is intended to be merged into
* Switch to the new feature branch (note how the local files will have switched to the files of the branch you are checked out on)
* Make change, add, commit, create a message
* Push the branch back to GitHub to your origin
* There will now be a new branch in the origin repo
* Create pull request title, description, make sure base and compare are correct
* If from a forked repo- give repo maintainers permission to amend pull request
* Submit the pull request
* Push follow-on commits to the pull request
* When the pull request is accepted, delete the branch

* Give upstream repository maintainers permission to push follow on commits to a pull request (forked)
-->

</td></tr>


<tr><td width="30%">

![Slide 28]()

</td><td>

### Commands

Clone (or download) an organizational repo (organizational repo will be "origin")

```bash
$ git clone https://github.com/<organization-name>/<repo-name>
```

Clone (or download) a user account repo (repo needs to have already been forked to user account, forked repo will be "origin")

```bash
$ git clone https://github.com/<user-name>/<repo-name>
```

Change directory (folder name will be the repo name)

```bash
$ cd <repo-name>
```

Verify which branch you are checked out on (important if more than one branch)

```bash
$ git branch
```

Create and switch to a branch (note how local files switch to the files of the branch you switch to)

```bash
$ git checkout -b <branch-name>
```

If not working from within the branch you are branching off of, need to specify which branch branching off of

```bash
$ git checkout -b <branch-name> <branch-branching-off-of>
```

If the branch already exists, just switch to a branch

```bash
$ git checkout <branch-name>
```

Make your change to the files, then add, commit, create a message (if you don't use -m, a Vim editor will open and you will need to know how to exit)

```bash
$ git add .
$ git commit -m "Your note"
```

Push branch to GitHub (by default, the origin is the repo you cloned from); This can also be used to push additional commits

```bash
$ git push origin <branch-name>
```

There will now be a new branch in the repo that is your origin. The branch will not be affecting anything else. If you never did anything else with it, it would just exist there.

</td></tr>



<!--
* URL of the repo you have write permission to

* Clone or download the organizational or forked repo (whatever your origin is)

* Push branch to organizational or forked repo (whatever your origin is)
-->

<!--
```bash
$ git clone <repo-url>
```
-->

<!--
# Reusable Commands

-->



<tr><td width="30%">

![Slide 26]()

</td><td>

### How to Add Additional Commits

Anyone who has write permission to a repo the branch is in, or just the branch itself, can continue to make changes to the branch. If a pull request has already been made, the additional commit(s) will be automatically added to the pull request when you push to the branch, up to the point that the pull request is merged.

<!--
can also fetch it, make a change, and push to the branch too. The process is the same as earlier. 
-->

</td></tr>




<tr><td width="30%">

![Slide 27]()

</td><td>

### Submit a Pull Request

<!--
base fork, base, head fork, compare
base, compare

branch-name ... "Compare & pull request"
base: master ... compare: branch-name
Click "Create pull request"
-->

In the browser, go to the repo you want your pull request to be merged into. There should be a message prompting you to submit a pull request because GitHub will detect your branch. Be forewarned, that if you go to your fork instead, you can accidentally submit a pull request to yourself. 

* Make sure that base corresponds to the repo and branch you want to contribute to
* Make sure compare corresponds to your branch
* Create a pull request title and perhaps a description
* If the pull request is via a forked repo, you might want to leave the box checked to give repo maintainers permission to amend the pull request. This gives them read/write access to the branch and later I'll explain how to amend it.
* Create the pull request

</td></tr>



<tr><td width="30%">

![Slide 26]()

</td><td>

### Perspective

We are switching our perspective now. We are now a maintainer working from within an organizational repo, with write permission to the organizational repo, but without write permission to a forked repo, unless permission has been given to edit a pull request. The organizational repo is our origin, but any forked repo is not. 

</td></tr>


<tr><td width="30%">

![Slide 28]()

</td><td>

### What Are You Doing When You Review a Pull Request?

* If you are a repo maintainer, you will receive a message (by browser or email, based on your notification preferences) to let you know there is a pull request . 
* You go to the pull request in the browser and look at it
* In the simplest scenario, you can merge the pull request without making a change, or by making a change in the browser. 

<!--
In the less simple scenario, you will need to fetch the pull request branch to your computer to run the code so that you can evaluate the proposed change. An example would be if the code for a website has been updated and submitted as a pull request. You can fetch the pull request branch to your computer, checkout the branch, complete any installation process, look at the website in your browser as you run in on a local server, and literally see the change proposed by the pull request. Then decide how to proceed. 
-->

</td></tr>


<tr><td width="30%">

![Slide 29]()

</td><td>

### Code Review Options

* When you look at the pull request in the browser, you can tell it can be accepted (for example a typo) and click merge
* You run the code locally, but you do not need to make a change; you go back to the browser and click merge
* You run the code locally, and you think a change needs to be made; you ask the contributor to update the pull request
* You run the code locally, and you think a change needs to be made; you update the pull request branch locally (add, commit, create a message), merge the branch locally via command with the branch it is intended to change, and push to GitHub
* You run the code locally, and you think a change needs to be made; you push additional commits to the pull request

<!--
Two Ways to Merge
* Via browser
* Via command line

Merge Options
* Regular merge
* Squash
* Rebase

Flow chart

Check out pull request, run it like normal, for instance, a website

- [ ] Fetch an organizational pull request
- [ ] Checkout a pull request locally
- [ ] Merge pull request via browser- regular, squash, or rebase
- [ ] Merge pull request via command line
- [ ] Ask contributor to make a change to pull request
- [ ] Request a review from a specific person
- [ ] Add, commit, create a message, merge pull request via command line and push to live branch
- [ ] Push follow-on commits to organizational pull request
- [ ] Push follow-on commits to forked repo pull request via HTTP/HTTPS or SSH
- [ ] Close pull request via browser
- [ ] Close an issue via commit message by using keyword

Ways to Deal with a Pull Request
* Checkout a pull request via GitHub and merge
* Checkout a pull request locally and merge
* Checkout a pull request locally and ask contributor to make changes to pull request
* Checkout a pull request locally, edit, merge with branch, and push to live branch to GitHub
* Checkout a pull request locally and push a follow on commit to pull request from fork
* Checkout a pull request locally and push a follow on commit to pull request from organizational branch

Flow chart of possibilities:
Small change, can merge in browser without running locally (example: typo)
Need to run locally, but don't need to make a change- go back to browser and merge
Need to run locally, need to make a change: 
* ask PR author to make change (person's commits automatically go to PR)
* you make change and push to PR
https://help.github.com/articles/committing-changes-to-a-pull-request-branch-created-from-a-fork/
* you make change, merge with intended branch and push to origin (follow instructions)
Need to run locally, need to resolve merge conflict:
* resolve in browser
* resolve locally
Delete remote and local branches

Code Review Process (PR gives link to instructions)
- Process is slightly different for "fork and pull" pull request versus "shared repository model" pull request
- If no change needed locally- merge button (merge options)
- General process for making a local change, committing, merging and
pushing back to GitHub
- How to keep local code up to date
-->

</td></tr>


<tr><td width="30%">

![Slide 30]()

</td><td>

### Pull Request Review Process

When you go to the pull request in the browser, there will a set of command line instructions for reviewing the pull request locally (on your own computer). The set of instructions will be slightly different depending on whether the pull request was submitted via "Fork and Pull" Model (remote branch) or "Shared Repository" Model.  

<!--
(whether organization branch or fork branch)
-->

I actually want to show you a slightly different way to do it that I think is easier to understand. 

</td></tr>


<tr><td width="30%">

![Slide 31]()

</td><td>

### Simple Code Review Process

<!--
Step 1: From your project repository, bring in the changes and test.

git fetch origin
git checkout -b instructions-pr origin/instructions-pr
git merge master

git pull origin <branch-name>

Step 1: From your project repository, check out a new branch and test the changes.

git checkout -b <branch-name> master
git pull https://github.com/<user-name>/<repo-name> <branch-name>

Step 2: Merge the changes and update on GitHub. (Same)

git checkout master
git merge --no-ff <branch-name>
git push origin master


Pull or push additional changes to pull request
git pull https://github.com/<user-name>/<repo-name> <branch-name>
git push https://github.com/<user-name>/<repo-name> <branch-name>

Push additional changes if local branch name and pull request branch name are different
git push https://github.com/<user-name>/<repo-name> <local-branch-name>:<remote-branch-name>
-->



Push additional commits to forked repo pull request (contributor needs to have given permission, and local branch name and remote branch name need to match)

```bash
$ git push https://github.com/<user-name>/<repo-name> <branch-name>
```

Push additional commits to forked repo pull request if local branch name is different than pull request branch name

```bash
$ git push https://github.com/<user-name>/<repo-name> <local-branch-name>:<remote-branch-name>
```

Pull updates to the individual pull request into your local branch

```bash
$ git pull origin pull/<pull-request-number>/head:<branch-name>
```

Alternatively, fetch the individual pull request into your folder

```bash
$ git fetch origin pull/<pull-request-number>/head:<branch-name>
```

<!--
git fetch origin pull/8/head:Mariatta-patch-1
git push https://github.com/Mariatta/practice Mariatta-patch-1
git push https://github.com/Mariatta/practice Mariatta-patch-1-test:Mariatta-patch-1
git pull origin pull/8/head:Mariatta-patch-1

git pull https://github.com/Mariatta/practice.git Mariatta-patch-1
git push https://github.com/Mariatta/practice.git Mariatta-patch-1
-->

</td></tr>


<tr><td width="30%">

![Slide 32]()

</td><td>

### Forked Repo Model Pull Request

<!--
Committing Changes to a Pull Request Branch Created from a Fork
-->

</td></tr>

<tr><td width="30%">

![Slide 33]()

</td><td>

### Shared Repo Model Pull Request

</td></tr>


<tr><td width="30%">

![Slide 34]()

</td><td>

### Tidy Up

<!--
Deleting branch in browser will not delete it in your local repo, like other things need to update
-->

* Close pull request
* Revert pull request (hopefully not needed)
* Delete feature branch (locally and remote/browser)

Delete a branch

```bash
$ git branch -d  <branch-name>
```

Force delete branch

```bash
$ git branch -D  <branch-name>
```

<!--
Delete remote branch
-->

</td></tr>




<!--
### Keep Main Branch(es) Up-to-Date
### Keep Feature Branch(es) Up-to-Date
-->



<tr><td width="30%">

![Slide 35]()

</td><td>

### Should Your Project Use a Develop Branch?

<!--
# Making Workflow Decisions

- [ ] Look at an example of master only versus master/develop, production/staging
- [ ] Decide a workflow
- [ ] If will have both master and develop branch, choose default branch

### Workflow Decisions

* Are you going to have both master and development branches? (master only or master/develop as production/staging)
* If you have both, which will be your default branch? (base against which future pull requests and commits will be made)
* Default branch can be changed
-->

Some projects will involve both a master and develop branch. For example, a mission critical project with a high volume of users is likely to use a develop branch and staging to gate-keep updates before going live. Use the workflow that is right for the projects. They all have pros and cons. 

If you choose to use a develop branch:
* In addition to the master branch, create the develop branch
* Choose a default branch

If you want to know much more about this, see: A Successful Git Branching Model.

</td></tr>


<tr><td width="30%">

![Slide 36]()

</td><td>

### Go Further with Advanced Workflow

* Git Flow (basically, the workflow we've been using)
* A Successful Git Branching Model (more advanced)
* A Successful Git Branching Model Considered Harmful (alternative view)
* SemVer

</td></tr>

<!--
# Advanced Workflow

- [ ] Look at advanced workflows and understand different choices
- [ ] Create a tag
- [ ] Create a release

Advanced
* Resolve a merge conflict in the browser
* Resolve a merge conflict by command line
* Understand rebasing
* Understand update "strategies": fast forward, recursive
-->

<tr><td width="30%">

![Slide 37]()

</td><td>

### 10X Developers

<!--
Important Non-Coding Leadership Skills (see 10x results article)
* Communication
* People management/mentoring
* Keeping docs up to date
-->

</td></tr>


<tr><td width="30%">

![Slide 38]()

</td><td>

### Documentation

<!--
### Communication Strategy

* What impression you want to give people about your project? Hopefully welcoming, user-friendly. 
* How can you make contributor experience easier/faster/enjoyable (for example, tell people how to contribute)
* Draft community guidelines

Community

# Setting Up Repo Documentation

- [ ] Get to know GitHub Flavored Markdown

### Documentation- Forums

* wikis
* GitHub pages/Jekyll
* gists

### Documentation- Files

* README.md
* LICENSE (auto-generate)
* CODE_OF_CONDUCT.md (auto-generate, choosing from two different Codes of Conduct)
* CONTRIBUTING.md
* PITCHME.md

<!--
Documentation and Community
* LICENSE (legality of contributions)
* CONTRIBUTING.md (look at examples for ideas, will generate a message "Please review the guidelines for...")
-->

# Issue and Pull Request Documentation

* ISSUE_TEMPLATE
* PULL_REQUEST_TEMPLATE

* Issues Tab
* Pull Requests Tab
-->

</td></tr>


<tr><td width="30%">

![Slide 39]()

</td><td>

### Productivity Tips

<!--
* Cache your password
* Set up special configs (example: line endings)
* Create saved replies
* Link to specific line number on GitHub

Productivity
* Help via GitHub Keyboard Shortcuts (type "?")

Writing and Formatting

# Notifications

- [ ] Find the Notifications Overview Page
- [ ] Decide which notifications to receive, whether by browser or email, and which email to receive at

* [Emails (need to be logged in)](https://github.com/settings/emails)
* [Notifications center (need to be logged in)](https://github.com/settings/notifications)

Two Types of Notifications
* Watching
* Participating

Delivery Methods
* Browser (Web)
* Email

# Conversations

Where They Happen
* Issues
* Pull Requests

Helpers
* GitHub Flavored Markdown 
* @mentions (of people and teams)
* Issue and PR references
* Emojis
-->

</td></tr>




<tr><td width="30%">

![Slide 38]()

</td><td>

### What Could Go Wrong?

</td></tr>


<tr><td width="30%">

![Slide 39]()

</td><td>

### Safety Checklist

Setting Up Repo Fail Safes
* Back up the repo (third-party software)
* Protect main branch(es) 
* Enable required reviews of pull requests
* Decide whether to use status checks (external)
* Worst case scenario: How to recover deleted branch

</td></tr>

<!--
# Sensitive Data Warning

Any sensitive information made public, should be immediately considered compromised, removed from GitHub, and changed in development/production (famous companies have done it too!)
-->

<tr><td width="30%">

![Slide 40]()

</td><td>

### Go For It!

</td></tr>


<tr><td width="30%">

![Slide 41]()

</td><td>

### Tips for getting started:

* “Help Wanted” tags, topics/First-timers initiatives
* Look for community-oriented projects
* Cherry pick problems or issues that fit your skill level (look for triaging)
* Practice your workflow (don't be afraid to delete/start over)
* You can create your own sandbox by making pull requests on your own account or setting up an organization to learn more about options for maintainers

</td></tr>



<!--
# What If?

* What if contributors were encouraged to learn code contribution and review at the same time, instead of code review as an end result? More people could take on more responsibility. 

### Learn skills

Advice of how to get started making pull requests and doing code review

* Start where you feel welcome and supported (can evaluate projects using GitHub Open Source Project checklist)

### Finding Open Source Projects to Contribute To

Projects that have reputation
* Search (including advanced search) repositories, code, commits, issues, users, wikis, topics
* Use search syntax "help wanted", "first-timers-only", etc.

* Do a GitHub search such as ["pull requests welcome"](https://github.com/search?utf8=%E2%9C%93&q=pull+requests+welcome)
* [First Timers Only](https://medium.com/@kentcdodds/first-timers-only-78281ea47455#.barzl7cwa)

Look at Issue Triaging Example
* node.js website issues
-->


<tr><td width="30%">

![Slide 41]()

</td><td>

### Debunking Myths

</td></tr>


<tr><td width="30%">

![Slide 42]()

</td><td>

### Thank You :)

Useful Resources: Bitly Link

* Twitter handle: @KatiMichel
* GitHub username: KatherineMichel

</td></tr>


</table>


## Useful Resources

<!--
* [Using Keyboard Shortcuts](https://help.github.com/articles/using-keyboard-shortcuts)
-->

GitHub and Bitbucket
* [GitHub](https://github.com)
* [Bitbucket](https://bitbucket.org)

Getting Set Up
* [Set Up Git](https://help.github.com/articles/set-up-git)
* [Getting Started Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
* [Homebrew Git Formula](http://braumeister.org/formula/git)

Git Official 
* [Git Homepage](https://git-scm.com)
* [Git Doc (Docs and Pro Git Book](https://git-scm.com/doc)
* [Git Documentation](https://git-scm.com/documentation)
* [Git Pro Git Book](https://git-scm.com/book/en/v2)

Glossaries and Cheatsheets
* [GitHub Glossary](https://help.github.com/articles/github-glossary)
* [Git Cheatsheet](https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf)
* [GitHub Git Cheatsheet](https://help.github.com/articles/git-cheatsheet)

GitHub Help and Training
* [GitHub Help](https://help.github.com)
* [GitHub Guides](https://guides.github.com)
* [GitHub Training Guides YouTube](https://www.youtube.com/githubguides)

GitHub Try
* [Try Git](https://try.github.io)
* [GitHub Bootcamp](https://help.github.com/categories/bootcamp) 
* [GitHub Hello World Tutorial](https://guides.github.com/activities/hello-world)

GitHub Learning Resources
* [Git and GitHub Learning Resources](https://help.github.com/articles/git-and-github-learning-resources)

GitHub Open Source Guides
* [Open Source Guides](https://opensource.guide)

Writing and Formatting
* [Getting Started with Writing and Formatting on GitHub](https://help.github.com/articles/getting-started-with-writing-and-formatting-on-github)
* [Working with Advanced Formatting](https://help.github.com/articles/working-with-advanced-formatting)

Setting Up and Maintaining Teams
* [Setting Up Teams](https://help.github.com/articles/setting-up-teams)
* [Maintaining Teams](https://help.github.com/articles/maintaining-teams)

Collaborative Development Models and Permission Levels
* [About Collaborative Development Models](https://help.github.com/articles/about-collaborative-development-models)
* [Types of Collaborative Development Models](https://help.github.com/enterprise/2.7/user/articles/types-of-collaborative-development-models)
* [Permission Levels for an Organization](https://help.github.com/articles/permission-levels-for-an-organization)
* [Repository Permission Levels for an Organization](https://help.github.com/articles/repository-permission-levels-for-an-organization)
* [Permission Levels for a User Account Repository](https://help.github.com/articles/permission-levels-for-a-user-account-repository)

<!--
Gitflow 
http://scottchacon.com/2011/08/31/github-flow.html
https://help.github.com/articles/what-is-a-good-git-workflow
https://guides.github.com/introduction/flow
https://help.github.com/articles/about-collaborative-development-models
https://help.github.com/articles/github-flow

Section: releases, working with tags
https://help.github.com/categories/releases
-->

Pull Request Branches Created from a Fork
* [Allowing Changes to a Pull Request Branch Created from a Fork](https://help.github.com/articles/allowing-changes-to-a-pull-request-branch-created-from-a-fork)
* [Committing Changes to a Pull Request Branch Created from a Fork](https://help.github.com/articles/committing-changes-to-a-pull-request-branch-created-from-a-fork)

Advanced Collaborative Development Workflow Examples
* Git Flow
* [A Successful Git Branching Model](http://nvie.com/posts/a-successful-git-branching-model) (more advanced)
* [A Successful Git Branching Model Considered Harmful](https://barro.github.io/2016/02/a-succesful-git-branching-model-considered-harmful)
* [SemVer](http://semver.org) (subtopic)

* [Can I Recover Branch After its Deletion in Git?](https://stackoverflow.com/questions/3640764/can-i-recover-branch-after-its-deletion-in-git)

<!--
* Browser
* [Desktop App](https://desktop.github.com) (Mac or Windows GUI)
* Command line (recommended, because can do everything with Git)
* [Hub](https://hub.github.com) (makes command line simpler to use)

Pros and Cons
* Some people find GUI (Graphical User Interfaces) such as the Browser or Desktop App to be easier to use

Permission Levels
https://help.github.com/articles/access-permissions-on-github
Owners, members, billing managers, outside collaborators
https://help.github.com/articles/permission-levels-for-an-organization
https://help.github.com/articles/repository-permission-levels-for-an-organization
https://help.github.com/articles/inviting-collaborators-to-a-personal-repository
https://help.github.com/articles/permission-levels-for-a-user-account-repository
https://help.github.com/articles/differences-between-user-and-organization-accounts

* What is [open-source software](https://en.wikipedia.org/wiki/Open-source_software)?

* [A Checklist Before You Contribute](https://opensource.guide/how-to-contribute/#a-checklist-before-you-contribute)

* [Getting to 10x (Results): What Any Developer Can Learn from the Best](https://medium.com/javascript-scene/getting-to-10x-results-what-any-developer-can-learn-from-the-best-54b6c296a5ef)

* [GitHub Pages Basics](https://help.github.com/categories/github-pages-basics)
* [Customizing GitHub Pages](https://help.github.com/categories/customizing-github-pages)
* [Wikis](https://help.github.com/categories/wiki)
* [Gists](https://help.github.com/categories/gists)
* [About READMEs](https://help.github.com/articles/about-readmes)
* [Licensing a Repository](https://help.github.com/articles/licensing-a-repository)
* [Adding a License to a Repository](https://help.github.com/articles/adding-a-license-to-a-repository)
* [Adding a Code of Conduct to Your Project](https://help.github.com/articles/adding-a-code-of-conduct-to-your-project)
-->

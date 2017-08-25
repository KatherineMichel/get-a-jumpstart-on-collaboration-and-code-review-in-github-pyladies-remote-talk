# Get a Jumpstart on Collaboration and Code Review in GitHub- PyLadies Remote

# Table of Contents

- [About](#about)
- [Important Webcast Links](#important-webcast-links)
- [Additional PyLadies Resources](#additional-pyladies-resources)
- [Slides and Script Table of Contents](#slides-and-script-table-of-contents)
- [Slides and Script](#slides-and-script)
- [Useful Resources](#useful-resources)
    - [Links](#links)    
    - [Bash Commands](#bash-commands)
    - [Local Development](#local-development)
    - [Review Shared Repo Pull Request](#review-shared-repo-pull-request)
    - [Review Forked Repo Pull Request](#review-forked-repo-pull-request)
    - [Merge Pull Request Locally and Push to Master Branch](#merge-pull-request-locally-and-push-to-master-branch)
- [Attribution](#attribution)
- [Copyright](#copyright)

<!--
### Alternatively, Fetch Individual Pull Request
-->

<hr>

## About

Slides and script for a talk Katherine "Kati" Michel ([Twitter](https://twitter.com/KatiMichel), [GitHub](https://github.com/KatherineMichel)) will give for [PyLadies Remote](https://2017.djangocon.us).

* Original slide deck: Coming soon!
* Video recording: Coming soon!

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Important Webcast Links

* ["Get a Jumpstart on Collaboration and Code Review" Webcast Link](https://www.youtube.com/watch?v=eBTLPYbVvQY)
* [PyLadies Remote tlk.io Chat Forum](https://tlk.io/pyladiesremote)
* [DjangoCon GitHub Repo](https://github.com/djangocon)
* [DjangoCon U.S. 2017 Website Repo GitHub](https://github.com/djangocon/2017.djangocon.us)
* [Collaboration and Code Review Classroom GitHub](https://github.com/collaboration-and-code-review-classroom)

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Additional PyLadies Resources

PyLadies and PyLadies Remote
* [PyLadies](http://www.pyladies.com), [PyLadies GitHub](https://github.com/pyladies), and [PyLadies Slack](http://slackin.pyladies.com)
* [PyLadies Remote Twitter](https://twitter.com/pyladiesremote)
* [PyLadies Remote Website GitHub](https://github.com/pyladies-remote/website)
* [PyLadies Remote YouTube Webcasts](https://www.youtube.com/channel/UCyVogtilYlp1B1ZeFdnmDxQ)

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Slides and Script Table of Contents

- [Get a Jumpstart on Collaboration and Code Review in GitHub](#get-a-jumpstart-on-collaboration-and-code-review-in-github)
- [Welcome](#welcome)
- [About Me](#about-me)
- [Goal](#goal)
- [Hands On Practice](#hands-on-practice)
- [Announcing TacoFancy](#announcing-tacofancy)
- [The One Sentence that Motivated Me to Start Using GitHub](#the-one-sentence-that-motivated-me-to-start-using-github)
- [My First Pull Request](#my-first-pull-request)
- [DjangoCon US Website as Example Project](#djangocon-us-website-as-example-project)
- [What are Git and GitHub?](#what-are-git-and-github)
- [Social Network](#social-network)
- [Repositories](#repositories)
- [Local Development Environment](#local-development-environment)
- [Collaboration and Code Review Best Practice Workflow](#collaboration-and-code-review-best-practice-workflow)
- [Working on a File in GitHub](#working-on-a-file-in-github)
- [Branches](#branches)
- [How to Create a Branch](#how-to-create-a-branch)
- [Overview](#overview)
- [Section 1](#section-1)
- [The Two Collaborative Development Models](#the-two-collaborative-development-models)
- [The Two Types of Accounts](#the-two-types-of-accounts)
- [Write Permission](#write-permission)
- [Examples of What Write Permission Will Allow You to Do](#examples-of-what-write-permission-will-allow-you-to-do)
- [Why We Need Write Permission](#why-we-need-write-permission)
- [Write Permission and Collaboration Examples](#write-permission-and-collaboration-examples)
- [How to Fork a Repo](#how-to-fork-a-repo)
- [Forked Repo](#forked-repo)
- [Interesting Thing #1: Opposites](#interesting-thing-1-opposites)
- [Interesting Thing #2: User Account Shared Repo Disadvantage](#interesting-thing-2-user-account-shared-repo-disadvantage)
- [Interesting Thing #3: Write Permission Examples](#interesting-thing-3-write-permission-examples)
- [Interesting Thing #4: Inactive Pull Requests](#interesting-thing-4-inactive-pull-requests)
- [Section 2](#section-2)
- [Fork and Pull Model](#fork-and-pull-model)
- [Shared Repository Model](#shared-repository-model)
- [Bash Commands](#bash-commands)
- [Local Dev Environment](#local-dev-environment)
- [Cloning](#cloning)
- [Changing Directory](#changing-directory)
- [GitHub Repo Versus Local Directory](#github-repo-versus-local-directory)
- [Verifying Branch](#verifying-branch)
- [Creating a New Branch](#creating-a-new-branch)
- [Working on a File Locally](#working-on-a-file-locally)
- [Adding and Committing](#adding-and-committing)
- [Pushing](#pushing)
- [New Branch](#new-branch)
- [Submit a Pull Request](#submit-a-pull-request)
- [Section 3](#section-3)
- [Pull Request Review Process](#pull-request-review-process)
- [Pull Request Command Line](#pull-request-command-line)
- [Pull Request Review Options](#pull-request-review-options)
- [Pull Request Branches](#pull-request-branches)
- [Pull Request Review](#pull-request-review)
- [Merging](#merging)
- [Merge Conflict](#merge-conflict)
- [Tidy Up](#tidy-up)
- [Advanced Topics](#advanced-topics)
- [Section 4](#section-4)
- [Common Branch Commands](#common-branch-commands)
- [Common Add and Commit Commands](#common-add-and-commit-commands)
- [Common Push and Pull Commands](#common-push-and-pull-commands)
- [Fetch and Merge Versus Pull](#fetch-and-merge-versus-pull)
- [Keeping Branches Up-to-Date](#keeping-branches-up-to-date)
- [Adding a Remote Upstream and Syncing a Fork](#adding-a-remote-upstream-and-syncing-a-fork)
- [GitHub Flow](#github-flow)
- [Another Workflow](#another-workflow)
- [Workflow Decisions](#workflow-decisions)
- [Learn More About Workflow](#learn-more-about-workflow)
- [Section 5](#section-5)
- [Getting to 10x Results](#getting-to-10x-results)
- [Communication Strategy](#communication-strategy)
- [Documentation](#documentation)
- [Templates](#templates)
- [Communication Forums](#communication-forums)
- [Section 6](#section-6)
- [Code Safety](#code-safety)
- [Additional Safety Considerations](#code-safety-considerations)
- [Productivity Helpers](#productivity-helpers)
- [Triaging](#triaging)
- [Sandboxing](#sandboxing)
- [Go For It!](#go-for-it)
- [Section 7](#section-7)
- [Debunking Myths](#debunking-myths)
- [Section 8](#section-8)
- [Prerequisites for Getting Started](#prerequisites-for-getting-started)
- [Browser, Desktop, Command Line](#browser-desktop-command-line)
- [Getting Help](#getting-help)
- [Organization and Repo Tour](#organization-and-repo-tour)
- [Thank You](#thank-you)

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Slides and Script

<table>

<tr><td width="30%">

![Slide 1](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_0.jpg)

</td><td>

### Get a Jumpstart on Collaboration and Code Review in GitHub 

By Katherine "Kati" Michel

</td></tr>


<tr><td width="30%">

![Slide 2](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_1.jpg)

</td><td>

### Welcome 

Welcome, everyone. I'm Kati Michel. I'm thrilled to have the opportunity to teach you what I've learned as the DjangoCon US Website Chair.

</td></tr>


<tr><td width="30%">

![Slide 3]()

</td><td>

### About Me

* DjangoCon Website Chair
* DEFNA (Django Events Foundation North America) Board Member
* DjangoCon Europe Website Committee Member
* Project Manager
* Web Designer and Developer

</td></tr>


<tr><td width="30%">

![Slide 4](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_2.jpg)

</td><td>

### Goal

* I want to teach you a process that will get you started collaborating and doing code review as quickly as possible. 
* For one thing, there is more male participation than female. I want to see female participation increase. More women should be maintainers.

</td></tr>


<tr><td width="30%">

![Slide 5]()

</td><td>

### I Don’t Want You to Be Like Me!

* I wish I had taken on more responsibility sooner
* For example, I thought that being a repo maintainer was for other people, and how it is done was a mystery to me
* Once I became a maintainer, I learned as I went along. I made mistakes in front of people. I sometimes had to ask senior developers to explain things to me or spend time researching online. 
* Fortunately, I have been a maintainer in an extremely supportive environment. 
* I want all of you to benefit from my trial and error.

</td></tr>


<tr><td width="30%">

![Slide 6]()

</td><td>

### Understanding the Process and Hands On Practice

* This is a real process that you can learn and use.
* I'm going to be showing you a lot of screenshots and diagrams, because I want you to understand what the process looks like.
* At the end of my presentation, there will be an opportunity to practice reviewing a pull request in a no-pressure environment. 
* I think this highly valuable, because if you learn the process first, you can be more confident to seek opportunities to collaborate and maintain. 

</td></tr>


<tr><td width="30%">

![Slide 7]()

</td><td>

### Resources
* If you miss anything during my talk, my slides and a replay of my talk will be online later
* On my last slide, there will be a link to Useful Resources where you will find documentation and all of the commands I will be showing you today. 
* If you choose to take part in the simulation exercise, your repo will remain there indefinitely so that you can practice and experiment in the future. 
* You are welcome to contact me if you have any questions

</td></tr>



<tr><td width="30%">

![Slide 6](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_3.jpg)

</td><td>

### Announcing TacoFancy

* I want to tell you how I got started with open-source contribution, which I think will show you there are many ways to get involved. 
* I first signed up for GitHub in April 2013. But my account sat unused for 7 months. I didn't know how to get started.  
* I happened to be looking at Twitter. I saw a tweet from a man named Dan Sinker. He had made a really delicious taco meal and decided to start a project on GitHub to share taco recipes. 
* So I clicked on the link and went to the project to take a look. 

</td></tr>


<tr><td width="30%">

![Slide 7](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_4.jpg)

</td><td>

### The One Sentence that Motivated Me to Start Using GitHub

One sentence in the project information that had a huge impact on me: "Are You New to Github But Want to Contribute?" 

</td></tr>


<tr><td width="30%">

![Slide 8](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_5.jpg)

</td><td>

### My First Pull Request

That was me. I became very determined to contribute and submitted my first pull request there.

</td></tr>


<tr><td width="30%">

![Slide 9](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_6.jpg)

</td><td>

### DjangoCon US Website as Example Project

I kept using Git and GitHub and getting better at it. I eventually became a DjangoCon US website contributor in 2016, then became the Website Chair and maintainer in 2017. 
* I am going to use DjangoCon US website as an example throughout this talk. 

</td></tr>


<tr><td width="30%">

![Slide 10](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_7.jpg)

</td><td>

### What are Git and GitHub?

GitHub is a website built on the version control software Git.  

</td></tr>


<tr><td width="30%">

![Slide 11](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_8.jpg)

</td><td>

### Social Network

GitHub is a social network. You can:
* Make a user profile
* Follow people
* Follow their activity in your newsfeed
* Find interesting projects

</td></tr>


<tr><td width="30%">

![Slide 12](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_9.jpg)

</td><td>

### Repositories

But the really important part of GitHub is that users can store and work on code together in repositories

</td></tr>


<tr><td width="30%">

![Slide 13](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_10.jpg)

</td><td>

### Repositories

(Animation)

For example, if you go to the DjangoCon US organization account you will see a list of repos and at the top is the DjangoCon US website repo. 

</td></tr>


<tr><td width="30%">

![Slide 14](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_11.jpg)

</td><td>

### Repositories

(Animation)

If you click on the hyperlink, it will open up the repo and you will see the folders and files filled with the website code and you can look through. 

</td></tr>


<tr><td width="30%">

![Slide 15](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_12.jpg)

</td><td>

### Local Dev Environment

When we are working on code, we can't do everything in the GitHub website. 
* For example, we might want to make a copy of the DjangoCon US website code in the local development environment of our computer, install the necessary software, and run the code in a local browser so that you can add a feature to it, or test a pull request branch.
* There is where Git is very useful. Git is installed in our local development environment and used in the command line of your computer. You can use Git to make a snapshot of your project at any point in time and revert back if needed.
* Here is a screenshot of my local development environment.
* In the background I have GitHub open in the browser
* In front of that, I have my local folder window and my command line

</td></tr>


<tr><td width="30%">

![Slide 16](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_13.jpg)

</td><td>

### Local Dev Environment

(Animation)

* I can use the web address (URL) from the GitHub repo in the command line to create a copy of the repo in my local development environment. Making a copy of a repo locally is called cloning.

</td></tr>


<tr><td width="30%">

![Slide 17](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_14.jpg)

</td><td>

### Local Dev Environment

(Animation)

* I can make changes and push the changes back to GitHub. 
* Meanwhile, other users can do the same thing on their computers.

I will elaborate on this process later.

</td></tr>


<tr><td width="30%">

![Slide 18](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_15.jpg)

</td><td>

### Collaboration and Code Review Best Practice Workflow

There is a concept that I think is very important.

In order to be able to increase your level of responsibility, we need to have the freedom to switch between multiple tasks. 
* You keep your main code branch (master) up-to-date
* Create one or more features
* Do code review

</td></tr>


<tr><td width="30%">

![Slide 19](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_16.jpg)

</td><td>

### Working on a File in GitHub

When I first started using GitHub, I would go into my own GitHub repo, click on a file, click on the pencil icon to open the file, make a change, and save it. 
This is fine, but imagine if there were multiple people all working on a repo and all of them were going into files and making changes and saving them. It wouldn't be very practical. For instance, how would you give feedback? 
* There is a way to make changes that enables you to switch between multiple tasks the way that you need to to collaborate and do code review.

</td></tr>


<tr><td width="30%">

![Slide 20](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_17.jpg)

</td><td>

### Branches

We need to use branches instead. 

Branches
* They are a best practice
* Can be used by any GitHub user

When you create a repo, by default you are working within a branch named master. 

</td></tr>


<tr><td width="30%">

![Slide 21](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_18.jpg)

</td><td>

### Branches

(Animation)

Say for instance that you want to make a change in the branch, you can make a copy of the entire master branch and give it a different name. Now there are two branches, in the same repo, the master branch and a feature branch (GitHub will also refer to a feature branch as a topic branch). 

</td></tr>


<tr><td width="30%">

![Slide 22](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_19.jpg)

</td><td>

### Branches

(Animation)

You can create an unlimited number of branches and you can switch in between them to work on them.

</td></tr>


<tr><td width="30%">

![Slide 23](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_20.jpg)

</td><td>

### Branches

(Animation)

At some point, when the feature branch author thinks it's done, a pull request will be submitted and the feature branch will become a pull request branch. 

</td></tr>


<tr><td width="30%">

![Slide 24](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_21.jpg)

</td><td>

### Branches

(Animation)

If the changes are accepted, they will be merged into the master branch. The master branch will be like before, except with the changes from the branch.  

* But both feature branches (a.k.a. topic branches) and pull request branches are examples of branches. We can work on them in much the same way. 

</td></tr>


<tr><td width="30%">

![Slide 25](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_22.jpg)

</td><td>

### How to Create a Branch

Let's go back to the screenshot of editing a file in GitHub. 

</td></tr>


<tr><td width="30%">

![Slide 26](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_23.jpg)

</td><td>

### How to Create a Branch

(Animation)

There is a radial button you can choose to indicate you want to create a new branch. There is also a place to give the branch a new name. When you click to save the changes, they will not save in the current file. Instead, a new branch will be created. 

You can also create and work on branches through the command line in your local development environment, which I will show you later. 

</td></tr>


<tr><td width="30%">

![Slide 27](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_24.jpg)

</td><td>

### Overview
* Determine which collaboration approach to use (there are two)
* Clone a repo into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo
* Review the two different types of pull requests as a DjangoCon US website repo maintainer
* Additional workflow and command info
* People, communication, documentation
* Recommendations
* Don’t Be Me
* Simulation Exercise

</td><td>


<tr><td width="30%">

![Slide 28](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_25.jpg)

</td><td>

### Section 1

* Determine which collaboration approach to use (there are two)

</td></tr>


<tr><td width="30%">

![Slide 29](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_26.jpg)

</td><td>

### The Two Collaborative Development Models

A Collaborative Development Model is a fancy term for how users contribute to a repo. There are two different models. 
* "Shared Repository" Model
* "Fork and Pull" Model
The two different models typically correspond to the two different account types and which model you uses depends on whether you have write permission to the repo.

</td></tr>


<tr><td width="30%">

![Slide 30](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_27.jpg)

</td><td>

### The Two Types of Accounts

There are two types of accounts
* Organization accounts such as the DjangoCon organization
* User accounts, such as my own personal account

</td></tr>


<tr><td width="30%">

![Slide 31](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_28.jpg)

</td><td>

### Write Permission

We are not talking about "write" permission in the context of English.
When a user has write permission to a repo, it means they can make changes directly inside of the repo.

</td></tr>


<tr><td width="30%">

![Slide 32]()

</td><td>

### Examples of What Write Permission Will Allow You to Do

* Edit files
* Push branches directly to the repo (instead of via fork)
* Merge and close pull requests

https://help.github.com/articles/repository-permission-levels-for-an-organization

</td></tr>


<tr><td width="30%">

![Slide 33]()

</td><td>

### Why We Need Write Permission

Example: DjangoCon US website is a deployed live from the master branch and has a fairly high volume of traffic. We wouldn't want just anyone to be able to go into the DjangoCon repo and directly make changes. There is often a level of trust involved in having write permission.

</td></tr>


<tr><td width="30%">

![Slide 34](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_29.jpg)

</td><td>

### Write Permission and Collaboration Examples

First, we’ll look at the “Shared Repository” Model. A shared repository is typically found in an organization account, which makes sense when you think about the word shared.
* For example, this year I became a maintainer of the DjangoCon US website, so I was given write permission to the DjangoCon US website repo, which is a “Shared Repository”. Along with the other maintainers I work with who have write permission, I can make changes directly within the DjangoCon US website repo.

</td></tr>


<tr><td width="30%">

![Slide 35](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_30.jpg)

</td><td>

### Write Permission and Collaboration Examples

(Animation)

The “Fork and Pull” Model is typically used in user account repos. For example, when I first came across the DjangoCon US website repo, I wanted to contribute, but I was not a maintainer, so I didn't have write permission. So I made a copy (a.k.a. fork) of the DjangoCon US website repo in my user account, which I have write permission to, made a change, and submitted a pull request to the Django US website repo. 

</td></tr>


<tr><td width="30%">

![Slide 36](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_31.jpg)

</td><td>

### How to Fork a Repo

We've gone to the DjangoCon US website repo. 
* Click the "Fork" button
* Try to edit a file in a repository that you do not have write permission to. GitHub will automatically fork the repo to your user account. 

</td></tr>


<tr><td width="30%">

![Slide 37](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_32.jpg)

</td><td>

### How to Fork a Repo

(Animation)

There will be a message notifying you that it is being forked.

</td></tr>


<tr><td width="30%">

![Slide 38](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_33.jpg)

</td><td>

### Forked Repo

* The forking message will lead you back to your user account. 

</td></tr>


<tr><td width="30%">

![Slide 39](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_34.jpg)

</td><td>

### Forked Repo

(Animation)

* In the list of repos in your account, you will now see an entry for the fork, which will also tell where it was forked from

</td></tr>


<tr><td width="30%">

![Slide 40](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_35.jpg)

</td><td>

### Forked Repo

(Animation)

* Click on the hyperlink and it will open the repo
* The repo URL will have my user account name in it
* The fork is an exact copy of the original repo at the time it was forked. I could make any changes I wanted to the fork, including deleting it, and the original repo will not be affected. 
* In addition to using a fork to propose a change to the original repo, you can also use a fork for the starting point of a new idea of your own (depending on the license). 

</td></tr>





<tr><td width="30%">

![Slide 41]()

</td><td>

### Interesting Thing #1: Opposites

It’s typical that a shared repository will be found in an organization and a fork will be found in a user account. However, it can be the other way around, it’s just not nearly as common. I think it’s interesting to know that a repo can be forked into an organization account and a user account can have a shared repository. 

</td></tr>


<!--
### Shared Repository Model: User Account Versus Organization

A user account repo can be a shared repository. A user account owner can invite other users to collaborate on a repo that he or she owns. But there are a few advantages to using a organizational repo as a shared repository instead of an user account repo. 
-->


<tr><td width="30%">

![Slide 42]()

</td><td>

### Interesting Thing #2: User Account Shared Repo Disadvantage

* Organization account owners can create teams and permissions across multiple repos
* Otherwise, the repo “Shared Repository” settings are almost exactly the same. Teams and permissions are at an organization level.

</td></tr>


<tr><td width="30%">

![Slide 43]()

</td><td>

### Interesting Thing #3: Write Permission Examples

* Organization account maintainer (an organizational account owner can give you write permission to one or more repos)
* User account owner (sources and forks, which is why you fork if you do not have write permission to shared repo)
* User account collaborator (a user account owner has given you write permission to one of their personal repos)

</td></tr>


<tr><td width="30%">

![Slide 44]()

</td><td>

### Interesting Thing #4: Inactive Pull Requests

A few minutes ago, I talked about how it’s impractical to go into a file and make changes directly if you are working with multiple people and that it’s better to use branches. If you fork a repo, you also want to use branches. Say for instance, you make a change in the file and submit a pull request (without using a branch), you’re stuck waiting for the pull request to be resolved. Normally, you want your main branch to stay up-to-date so that you create new feature branches, but you’ve made a change in your main branch. If you delete the fork and refork to make it up to date, the pull request remains, but is inactive. It will be harder for the maintainer and you to work on. Instead, you want to keep the main branch up-to-date and use branches, just like we talked about a few minutes ago. 

</td></tr>


<tr><td width="30%">

![Slide 45](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_36.jpg)

</td><td>

### Section 2

* Determine which collaboration approach to use (there are two)
* Clone a repo into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo

</td></tr>


<tr><td width="30%">

![Slide 46](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_37.jpg)

</td><td>

### Fork and Pull Model

I've made a couple of diagrams that I hope will give you an idea of what the process is for working locally for each collaborative development model. 

</td></tr>


<tr><td width="30%">

![Slide 47](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_38.jpg)

</td><td>

### Fork and Pull Model

(Animation)

* Fork the repo

</td></tr>


<tr><td width="30%">

![Slide 48](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_39.jpg)

</td><td>

### Fork and Pull Model

(Animation)

* Clone the fork. 

Git will track some details about the project, for instance, where we cloned our code from. In relation to the clone, the GitHub repo we cloned from is now a remote repo and Git will assign the name "origin" to it. We can use the name origin in the command line to refer to the repo so we can push and pull changes back and forth between the local development environment and the GitHub repo.

</td></tr>


<tr><td width="30%">

![Slide 49](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_40.jpg)

</td><td>

### Fork and Pull Model

(Animation)

* Make our changes, push the changes back to the fork

</td></tr>


<tr><td width="30%">

![Slide 50](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_41.jpg)

</td><td>

### Fork and Pull Model

(Animation)

* Submit the pull request

</td></tr>


<tr><td width="30%">

![Slide 51](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_42.jpg)

</td><td>

### Shared Repository Model

Here's what it looks like when we use the "Shared Repository" Model

</td></tr>


<tr><td width="30%">

![Slide 52](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_43.jpg)

</td><td>

### Shared Repository Model

(Animation)

* The fork is not needed, because we have write permission
* Clone the shared repository. The shared repository will now be the remote "origin"

</td></tr>


<tr><td width="30%">

![Slide 53](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_44.jpg)

</td><td>

### Shared Repository Model

(Animation)

* Make our changes, push the changes back to the shared repository
* Submit the pull request

</td></tr>




<tr><td width="30%">

![Slide 54]()

</td><td>

### Bash Commands

Bash commands are commands that you use in the command line to communicate directly with your computer operating system. These commands are enough to be able to use git. In the Useful Resources section, I’ve included a link to more bash commands. The other commands we are going to use are git commands.

A couple useful things to know
* Some tasks vary by operating system- check tabs at the top of GitHub articles for special OS instructions; For instance, not all command lines use a $
* <variable> is a placeholder for the real thing

Go to the home directory
$ cd

Change directory
$ cd <directory-name>

List the folders and files in a directory
$ ls

Move back a directory
$ cd ..

</td></tr>


<tr><td width="30%">

![Slide 54](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_45.jpg)

</td><td>

### Local Development Environment

What I'm going to show you now is a generic process that you can use for a shared repository or a fork. You will clone the repo you have write permission to.

Let's go back to the screenshot of my local development environment. 
* I am working in my home directory. The name of home directory is at the top of the command line, and in front of the prompt. The reason why this matters is because the repo will be cloned into the directory we are working in.

</td></tr>


<tr><td width="30%">

![Slide 55](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_46.jpg)

</td><td>

### Cloning

(Animation)

* I am going to type the command $ git clone into the command line and copy and paste the URL from the browser of either the shared repo or fork, then hit enter. 

</td></tr>


<tr><td width="30%">

![Slide 56](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_47.jpg)

</td><td>

### Cloning

(Animation)

* A folder will appear in my home directory by the same name as the GitHub repo (2017.djangocon.us) and filled with the contents of the repo. 
* I now have a copy of the code online in the GitHub repo and a copy in my local development environment. 

</td></tr>


<tr><td width="30%">

![Slide 57](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_48.jpg)

</td><td>

### Changing Directory

(Animation)

* I will now change directory into the folder so that I can work there by typing cd 2017.djangocon.us, which is the folder name.

</td></tr>


<tr><td width="30%">

![Slide 58](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_49.jpg)

</td><td>

### Changing Directory

(Animation)

* I've clicked on the folder in the folder window so that I can see the contents visually. But I can also see I am working from within the folder in my command line because the name of the folder is at the top of the command line and in front of the prompt. 

</td></tr>


<tr><td width="30%">

![Slide 59](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_50.jpg)

</td><td>

### GitHub Repo Versus Local Directory

(Animation)

* You can pull up your GitHub repo and your local folder and compare the files. You can see the corresponding files. The format will be slightly different between one set is being rendered in the browser, and another set are raw files. 

</td></tr>


<tr><td width="30%">

![Slide 60](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_51.jpg)

</td><td>

### Verifying Branch

(Animation)

* Use the command $ git branch to verify which branch you are checked out on; initially, you will be checkout out on the default branch (in this case master)

</td></tr>


<tr><td width="30%">

![Slide 61](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_52.jpg)

</td><td>

### Creating a New Branch

(Animation)

* Create and checkout (switch) to a feature branch. We are calling this feature branch example-branch. We want to branch off of the branch we intend our changes to be merged into (note how the local files switch to the files of the branch you are checked out on, exactly the same at first, because a copy, but if you make a change in a branch and then switch back and forth between branches, you can see the difference)

</td></tr>


<tr><td width="30%">

![Slide 62](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_53.jpg)

</td><td>

### Working on a File Locally

(Animation)

* Open a file in the text editor. Make your change and save it.

</td></tr>


<tr><td width="30%">

![Slide 63](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_54.jpg)

</td><td>

### Adding and Committing

(Animation)

* Add and commit our change to git version control, create a message "Creating branch and updating"

</td></tr>


<tr><td width="30%">

![Slide 64](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_55.jpg)

</td><td>

### Pushing

(Animation)

* Push the new branch named example-branch to GitHub to your origin (the repo you cloned from that you have write permission to)

</td></tr>


<tr><td width="30%">

![Slide 65](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_56.jpg)

</td><td>

### New Branch

There will now be a new branch in the repo that is your origin and a message telling you it's there. The branch will not be affecting anything else. It's just there. If you click on the branch tab you can choose the name of the branch to switch to the new branch. 

</td></tr>


<tr><td width="30%">

![Slide 66](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_57.jpg)

</td><td>

### New Branch

(Animation)

You can toggle back and forth between the branches by clicking on the branches in the branches tab. 

</td></tr>


<tr><td width="30%">

![Slide 67](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_58.jpg)

</td><td>

### Submit a Pull Request

Go to the repo you want your pull request to be merged into, in this case, the DjangoCon US website repo. The reason why I saw this is because you can accidentally submit a pull request to yourself in your fork. In the DjangoCon US website repo, there will also be a message here telling you about the branch and suggesting that you submit a pull request, even if the branch is in a fork, because GitHub will detect it. Click on the "Compare & pull request" button. 

</td></tr>


<tr><td width="30%">

![Slide 68](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_59.jpg)

</td><td>

### Submit a Pull Request

(Animation)

* Make sure that the base branch is the branch you want your change to be merged into
* Make sure compare branch is your branch
* Create a pull request title and perhaps a description
* If the pull request is via a forked repo, a box will be checked by default giving maintainers the ability to edit the pull request 
* Double check your changes
* Click "Create pull request"

</td></tr>


<tr><td width="30%">

![Slide 69](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_60.jpg)

</td><td>

### Section 3

* Determine which collaboration approach to use (there are two)
* Clone a repo into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo
* Review the two different types of pull requests as a DjangoCon US website repo maintainer

</td></tr>


<tr><td width="30%">

![Slide 70](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_61.jpg)

</td><td>

### Pull Request Review Process

* When a pull request is submitted repo maintainers will receive a notification by browser or email to let them know there is a pull request
* Follow the link to the pull request tab in the browser
* Look over the information about the pull request. You can see the title and description and click on the “Files changed” link to see all of the changes that were made. 

</td></tr>


<tr><td width="30%">

![Slide 71](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_62.jpg)

</td><td>

### Pull Request Review Process

(Animation)

Underneath that will be info about how to merge the pull request. 
* There will be a merge button that you can click to merge in the browser
* Or there will be a link that says “command line instructions” 

</td></tr>


<tr><td width="30%">

![Slide 72](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_63.jpg)

</td><td>

### Pull Request Command Line

When you click on that link, it will open up a set of instructions for how to review and merge the pull request in your local development environment. The instructions will be different depending on whether the pull request was submitted from within the shared repository or from a forked repo.   

I will go over that in a minute. 

</td></tr>


<tr><td width="30%">

![Slide 73](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_64.jpg)

</td><td>

### Pull Request Review Options

But first, let's go over the options for what you can do when you review a pull request.

The first two options involve clicking the merge button in GitHub without running the code locally
* You look at the pull request changes, you can tell they can be accepted and click merge  
* You look at the pull request changes. Something needs to be changed, but you can change it in GitHub. So you edit the pull request file in the browser, similarly to how we edited a file earlier, and click merge.

</td></tr>


<tr><td width="30%">

![Slide 74](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_65.jpg)

</td><td>

### Pull Request Review Options

The other options involve fetching the pull request into your locally development environment and running the code there. 

If a change does not need to be made, you can
* Go back to the browser and click merge

If a change needs to be made, you can
* Ask the pull request author to make a change to the pull request
* Make the change locally yourself and push additional commits to the pull request branch on GitHub
* Make the change locally yourself, merge the branch with the branch it is intended to be merged with locally, and push to the branch on GitHub

</td></tr>


<tr><td width="30%">

![Slide 75](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_66.jpg)

</td><td>

### Pull Request Branches

This is why the pull request instructions are different.
* As a DjangoCon US website maintainer, we are able to fetch updates made to the DjangoCon US website repo into a hidden folder named .git in our local development environment. These updates will include branches made directly to the DjangoCon US website repo, but they will not include branches made through a fork, because they come from outside of the origin. 
* Branches made through a fork need to be pulled individually into our local development environment.
* The branches in the .git folder will be remote-tracking branches and can be referred to aas <remote>/<branch>

</td></tr>


<tr><td width="30%">

![Slide 76](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_67.jpg)

</td><td>

### Pull Request Review

* The instructions on this slide can actually be used by any maintainer to work on any branch they have write permission to.  
* If a pull request has already been made, the additional commits will be automatically added to the pull request, up to the point that the pull request is merged.
* For a shared repository pull request, we use the command $ git fetch origin to fetch the updates into the .git folder. We create and checkout to a new local branch, which we give a name to, and we insert the pull request branch contents from the .git folder into the new local branch by referring to the branch as origin/<branch-name>. We can merge master to make sure the branch is up-to-date. If we make a change, we can push additional commits to the branch on GitHub. 

```bash
$ git fetch origin
$ git checkout -b <local-branch-name> origin/<branch-name>
$ git merge master
```

```bash
$ git push origin <branch-name> 
```

* For a pull request submitted through a fork, we create a new branch off master and pull in the contents of the pull request branch from the fork. If we make a change, we can also push additional commits if we have been given permission to edit the pull request. 

```bash
$ git checkout -b <local-branch-name> master
$ git pull https://github.com/<user-name>/<repo-name> <branch-name>
```

```bash
$ git push https://github.com/<user-name>/<repo-name> <branch-name>
```

</td></tr>


<tr><td width="30%">

![Slide 77](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_68.jpg)

</td><td>

### Merging

This piece of code is for merging a pull request locally and pushing to the master branch.  

You are checking out to the master branch, merging the feature branch into the master branch, then pushing the change to the live master branch on GitHub. 

```bash
$ git checkout master
$ git merge --no-ff <local-branch-name>
$ git push origin master
```

</td></tr>




<tr><td width="30%">

![Slide 78]()

</td><td>

### Merge Conflict

</td></tr>


<tr><td width="30%">

![Slide 79]()

</td><td>

### Tidy Up

After a pull request is closed, it’s good practice to delete the feature branch in the browser and locally. There will be a button on the pull request page that you can use to delete the feature branch in the browser, or you can delete it in the branches tab. Or, you can use the third command. The first two commands are to delete the branch locally. 

$ git branch -d <branch-name>
$ git branch -D <branch-name>
$ git push <remote-name> :<branch-name>

</td></tr>



<!--
* Delete local and remote (in browser) feature branch
-->


<tr><td width="30%">

![Slide 80]()

</td><td>

### Advanced Topics

</td></tr>


<tr><td width="30%">

![Slide 81](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_69.jpg)

</td><td>

### Section 4

* Determine which collaboration approach to use (there are two)
* Clone a repo into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo
* Review the two different types of pull requests as a DjangoCon US website repo maintainer
* Additional workflow and command info 

</td><td>


<tr><td width="30%">

![Slide 82]()

</td><td>

### Common Branch Commands

</td><td>


<tr><td width="30%">

![Slide 83]()

</td><td>

### Common Add and Commit Commands

</td><td>


<tr><td width="30%">

![Slide 84]()

</td><td>

### Common Push and Pull Commands

</td><td>


<tr><td width="30%">

![Slide 85]()

</td><td>

### Fetch and Merge Versus Pull

</td><td>


<tr><td width="30%">

![Slide 86]()

</td><td>

### Keeping Branches Up-to-Date

</td><td>


<tr><td width="30%">

![Slide 87]()

</td><td>

### Adding a Remote Upstream and Syncing a Fork

</td><td>



<tr><td width="30%">

![Slide 88]()

</td><td>

### GitHub Flow

The workflow we have been using is basically GitHub Flow. It consists of merging pull requests into a master branch, which, in the cast of DjangoCon US website, deploys directly to the live site. 

</td><td>


<tr><td width="30%">

![Slide 89]()

</td><td>

### Another Workflow

Some projects use both a master and develop branch. For example, in a mission critical project with a high volume of users, pull requests might be merged into the develop branch, where the development is done. The develop branch might deploy to a staging site where the changes can be tested. The develop branch will be merged into the master branch when the recent changes are ready to deploy live. 

</td><td>


<tr><td width="30%">

![Slide 90]()

</td><td>

### Workflow Decisions

</td><td>




<tr><td width="30%">

![Slide 91]()

</td><td>

### Learn More About Workflow

Some developers have passionate views about workflow (see comment threads in some posts). Sometimes people ask, “Which is the best workflow?” There is not really a “best” workflow. You should use the workflow that fits what you are trying to accomplish. They all have pros and cons. 
* Git Flow (basically, what we’ve been using)
* A Successful Git Branching Model (more advanced)
* A Successful Git Branching Model Considered Harmful (alternative view)
* SemVer
* See also: Atlassian and GitLab docs  (you can also find insights in the docs of other software built on top of Git)

</td><td>


<tr><td width="30%">

![Slide 92]()

</td><td>

### Section 5

* Determine which collaboration approach to use (there are two)
* Clone a repo into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo
* Review the two different types of pull requests as a DjangoCon US website repo maintainer
* Additional workflow and command info
* People, communication, documentation

</td><td>




<tr><td width="30%">

![Slide 93]()

</td><td>

### Getting to 10x Results

</td><td>


<tr><td width="30%">

![Slide 94]()

</td><td>

### Communication Strategy

</td><td>


<tr><td width="30%">

![Slide 95]()

</td><td>

### Documentation

My first recommendation is that you go to the Useful Resources Section, follow the links to the DjangoCon US website repo documentation, read it, and make the documentations in your own projects equally welcoming and positive. 

</td></tr>


<tr><td width="30%">

![Slide 96]()

</td><td>

### Templates

</td></tr>


<tr><td width="30%">

![Slide 97]()

</td><td>

### Communication Forums

* Wikis
* GitHub Pages/Jekyll
* Gists

</td></tr>




<tr><td width="30%">

![Slide 98]()

</td><td>

### Section 6

* Determine which collaboration approach to use (there are two)
* Clone a repo into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo
* Review the two different types of pull requests as a DjangoCon US website repo maintainer
* Additional workflow and command info
* People, communication, documentation
* Recommendations

</td></tr>


<tr><td width="30%">

![Slide 99](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_71.jpg)

</td><td>

### Code Safety

My first recommendation is that if you have the authority, go into a repo’s Settings, click the Branches tab
* Protect the main branch so it can’t be deleted (for example, your master branch)

</td></tr>


<tr><td width="30%">

![Slide 100]()

</td><td>

### Additional Safety Considerations

Here are a few things you might want to do to keep your code safe
* Back up the repo (third-party software)
* Enable required reviews of pull requests, for example, a review has to be done before a pull request can be merged
* Use status checks (external)
* Revert pull requests, if needed
* Worst case scenario: How to recover deleted branch (link in Useful Resources section)
* Sensitive data warning (if made public, consider compromised, immediately remove and change)

</td></tr>


<tr><td width="30%">

![Slide 101]()

</td><td>

### Productivity Helpers

My second recommendation is to use productivity helpers
* Password caching
* Closing issues via commit messages by using keywords
* Saved replies
* Link to specific line numbers on GitHub

</td></tr>


<tr><td width="30%">

![Slide 102](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_72.jpg)

</td><td>

### Triaging

My third recommendation is that when you are looking for a project to contribute to
* Search by tag to find projects that use triaging. Triaging is where issues are sorted by difficulty level
* As a collaborator or code reviewer, you can cherry-pick issues and pull requests that fit your skill level

</td></tr>


<tr><td width="30%">

![Slide 103](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_73.jpg)

</td><td>

### Sandboxing

My fourth recommendation is that you 
* Practice your skills and workflow. Don't be afraid to delete and start over
* You can use your own user account as a sandbox. You can submit pull requests to yourself to practice.

</td></tr>


<tr><td width="30%">

![Slide 104](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_74.jpg)

</td><td>

### Go For It!

My last but not least recommendation is that you become a contributor to the DjangoCon US website next year 
* We have a diverse group of contributors of all skill levels and we are always looking for more contributors. Let us know if you are interested.  

</td></tr>


<tr><td width="30%">

![Slide 105]()

</td><td>

### Section 7
* Determine which collaboration approach to use (there are two)
* Clone a repo into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo
* Review the two different types of pull requests as a DjangoCon US website repo maintainer
* Additional workflow and command info
* People, communication, documentation
* Recommendations
* Don’t Be Me

</td></tr>




<tr><td width="30%">

![Slide 106]()

</td><td>

### Debunking Myths

</td></tr>



<tr><td width="30%">

![Slide 107]()

</td><td>

### Section 8

* Determine which collaboration approach to use (there are two)
* Clone a repo into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo
* Review the two different types of pull requests as a DjangoCon US website repo maintainer
* Additional workflow and command info
* People, communication, documentation
* Recommendations
* Don’t Be Me
* Simulation Exercise

</td></tr>


<tr><td width="30%">

![Slide 108]()

</td><td>

### Prerequisites for Getting Started

* Create a free [GitHub](https://github.com) account online
* Install Git on your computer and set your email and username
* Find and open your command line (a.k.a. terminal) on your computer
* Be able to navigate via command line (See Bash commands)
* You might also want to have a text editor of your choice installed, to use to edit files
You will find documentation for all of these things in the Useful Resources section.

</td></tr>




<tr><td width="30%">

![Slide 109]()

</td><td>

### Browser, Desktop, Command Line

</td></tr>


<tr><td width="30%">

![Slide 110]()

</td><td>

### Getting Help

* Help via Git, GitHub Help and Guides  (links in Useful Resources Section)
* Help via command line (exit by typing “q”)
* Help via GitHub Keyboard Shortcuts (type "?")

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

![Slide 111]()

</td><td>

### Organization and Repo Tour

</td></tr>


<tr><td width="30%">

![Slide 112](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_75.jpg)

</td><td>

### Thank You

Feel free to contact me.

Useful Resources: 
https://git.io/v5kpy

* Twitter handle: @KatiMichel
* GitHub username: KatherineMichel

</td></tr>

</table>

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>


<!--
See write permissions chart for info
Advanced workflow

* [A Checklist Before You Contribute](https://opensource.guide/how-to-contribute/#a-checklist-before-you-contribute)

* [Getting to 10x (Results): What Any Developer Can Learn from the Best](https://medium.com/javascript-scene/getting-to-10x-results-what-any-developer-can-learn-from-the-best-54b6c296a5ef)

http://opensourcesurvey.org/2017/#insights
-->


## Useful Resources

### Links

GitHub and Bitbucket
* [GitHub](https://github.com)

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
* [A Checklist Before You Contribute](https://opensource.guide/how-to-contribute/#a-checklist-before-you-contribute)

<!--
Insights, 
Eric Survey
http://opensourcesurvey.org/2017/#insights
-->

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

Pull Request Branches Created from a Fork
* [Allowing Changes to a Pull Request Branch Created from a Fork](https://help.github.com/articles/allowing-changes-to-a-pull-request-branch-created-from-a-fork)
* [Committing Changes to a Pull Request Branch Created from a Fork](https://help.github.com/articles/committing-changes-to-a-pull-request-branch-created-from-a-fork)

Advanced Collaborative Development Workflow Examples
* Git Flow
* [A Successful Git Branching Model](http://nvie.com/posts/a-successful-git-branching-model) (more advanced)
* [A Successful Git Branching Model Considered Harmful](https://barro.github.io/2016/02/a-succesful-git-branching-model-considered-harmful)
* [SemVer](http://semver.org) (subtopic)

* [Can I Recover Branch After its Deletion in Git?](https://stackoverflow.com/questions/3640764/can-i-recover-branch-after-its-deletion-in-git)

Documentation
* [DjangoCon US Website README.md](https://github.com/djangocon/2017.djangocon.us/blob/master/README.md)
* [DjangoCon US Website LICENSE](https://github.com/djangocon/2017.djangocon.us/blob/master/LICENSE)
* [DjangoCon US Website CODE_OF_CONDUCT.md](https://github.com/djangocon/2017.djangocon.us/blob/master/CODE_OF_CONDUCT.md)
* [DjangoCon US Website CONTRIBUTING.md](https://github.com/djangocon/2017.djangocon.us/blob/master/CONTRIBUTING.md)

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

### Bash Commands

Go to the home directory

```bash
$ cd
```

Change directory

```bash
$ cd <folder-name>
```

List the folders and files in a directory

```bash
$ ls
```

Move back a directory

```bash
$ cd ..
```

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

### Local Development

```bash
$ git clone <repo-url>
$ cd <repo-name>
$ git branch
$ git checkout -b <branch-name>
$ git add .
$ git commit -m "Your note"
$ git push origin <branch-name>
```

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

### Review Shared Repo Pull Request

```bash
$ git fetch origin
$ git checkout -b <branch-name> origin/<branch-name>
$ git merge master
```



Push Follow-On Commit to Shared Repo Pull Request



```bash
$ git push origin <branch-name> 
```

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

### Review Forked Repo Pull Request

```bash
$ git checkout -b <branch-name> master
$ git pull https://github.com/<user-name>/<repo-name> <branch-name>
```

Push additional commits to forked repo feature branch or pull request branch (contributor needs to have given permission, and local branch name and remote branch name need to match)


```bash
$ git push https://github.com/<user-name>/<repo-name> <branch-name>
```

Push additional commits to forked repo feature branch or pull request branch, if local branch name is different than pull request branch name (contributor needs to have given permission)


```bash
$ git push https://github.com/<user-name>/<repo-name> <local-branch-name>:<remote-branch-name>
```

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

### Merge Pull Request Locally and Push to Master Branch

```bash
$ git checkout master
$ git merge --no-ff <branch-name>
$ git push origin master
```

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

### Alternatively, Fetch Individual Pull Request

This will only work for pull request branches, not feature branches. 

Fetch the individual pull request, checkout the branch, add and commit changes, push changes to the branch

```bash
$ git fetch origin pull/<pull-request-number>/head:<branch-name>
$ git checkout <branch-name>
$ git push <remote-name> <branch-name>
```

Example

```bash
$ git fetch origin pull/1/head:patch-1
$ git checkout patch-1
$ git push origin patch-1
```

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

### Delete a Branch

Delete local branch

```bash
$ git branch -d  <branch-name>
```

Force delete local branch

```bash
$ git branch -D  <branch-name>
```

Delete remote branch

```bash
$ git push <remote-name> :<branch-name>
```

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Branch Commands

Switching to a branch that already exists (-b is not needed, because is used to create branch)

```bash
$ git checkout <branch-name>
```

Create and checkout (switch) to a branch (you are in the branch you are branching off of, or there is only one branch, so you do not need to specify which branch you are branching off of)

```bash
$ git checkout -b <branch-name>
```

Create and checkout (switch) to a branch (you are not in the branch you are branching off of)

```bash
$ git checkout -b <branch-name> <branch-branching-off-of>
```

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

### Add, Commit, Create a Message

After you have checked out (switched) to a branch

```bash
$ git add .
$ git commit -m "Your note"
```

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

### Push and Pull Commands

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

### Fetching and Merging Versus Pulling


<!--
There are two ways to fetch a pull request branch to your local development environment to run.  

* You can fetch and merge (two separate commands)
* Or you can pull, which combines fetching and merging into one command



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



Instead, pull directly from the remote repository branch ($ git fetch + $ git merge in one command)

```bash
$ git pull <remote-name> <branch-name>
$ git push <remote-name> <branch-name>
```



Pushing and pulling via remote URL (will come in handy later when we are working with pull request from a fork)

```bash
git pull https://github.com/<user-name>/<repo-name> <branch-name>
git push https://github.com/<user-name>/<repo-name> <branch-name>
```
-->

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Adding Upstream Remote and Syncing a Fork

Add a remote

```bash
$ git remote add <remote-name> <remote-url>
```

<!--
Does not update automatically
Upstream is the name commonly used for adding a shared repository as a remote for a fork.
-->

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

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

<!--
Merging a remote branch into a local branch

### Syncing Branches to Keep Them Up-to-Date

Whichever collaborative development model you are using, you can fetch updates from the shared repository and merge them into your local development environment. 

If you are working from the "Shared Repository" Model, you are fetching from the origin. 
If you are working from the "Fork and Pull" Model, you are fetching from the upstream.
-->

Common origin example

```bash
$ git fetch origin
$ git checkout master
$ git merge origin/master
```

Common pull and push example

```bash
$ git pull origin master
$ git push origin master
```

Common upstream example (including pushing changes to corresponding branch in forked repository in GitHub)

```bash
$ git fetch upstream
$ git checkout master
$ git merge upstream/master
$ git push origin master
```

Keep feature branch up-to-date (often merging master into feature branch)

```bash
$ git checkout <feature-branch-name>
$ git merge <branch-name>
```

Example

```bash
$ git checkout example-branch
$ git merge master
```

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Attribution

The style of this transcript is heavily inspired by:

* Ana Balica's ([Twitter](https://twitter.com/anabalica), [GitHub](https://github.com/ana-balica)) transcript of her [Humanizing among coders](https://ana-balica.github.io/2017/05/28/humanizing-among-coders/) keynote for [PyCon CZ 2016](https://cz.pycon.org/2016). 
* Honza Javorek's ([Twitter](https://twitter.com/honzajavorek), [GitHub](https://github.com/honzajavorek)) transcript of Anna Ossowski's ([Twitter](https://twitter.com/OssAnna16), [GitHub](https://github.com/OssAnna16)) keynote [Be(Come) A Mentor! Help Others Succeed!](https://github.com/honzajavorek/become-mentor) for [PyCon CZ 2017](https://cz.pycon.org/2017/). 

Thank you!

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Copyright

© 2017 Katherine Michel. All Rights Reserved.

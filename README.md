# Get a Jumpstart on Collaboration and Code Review in GitHub- PyLadies Remote

# Table of Contents

- [About](#about)
- [Attribution](#attribution)
- [Slides and Script Table of Contents](#slides-and-script-table-of-contents)
- [Slides and Script](#slides-and-script)
- [Useful Resources](#useful-resources)
    - [Links](#links)    
    - [Bash Commands](#bash-commands)
    - [Local Development](#local-development)
    - [Review Shared Repo Pull Request](#review-shared-repo-pull-request)
    - [Review Forked Repo Pull Request](#review-forked-repo-pull-request)
    - [Merge Pull Request Locally and Push to Master Branch](#merge-pull-request-locally-and-push-to-master-branch)
    
<hr>

## About

Slides and script for a talk Katherine "Kati" Michel ([Twitter](https://twitter.com/KatiMichel), [GitHub](https://github.com/KatherineMichel)) will give for [PyLadies Remote](https://2017.djangocon.us).

* Original slide deck: Coming soon!
* Video recording: Coming soon!

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Attribution

The style of this transcript is heavily inspired by:

* Ana Balica's ([Twitter](https://twitter.com/anabalica), [GitHub](https://github.com/ana-balica)) transcript of her [Humanizing among coders](https://ana-balica.github.io/2017/05/28/humanizing-among-coders/) keynote for [PyCon CZ 2016](https://cz.pycon.org/2016). 
* Honza Javorek's ([Twitter](https://twitter.com/honzajavorek), [GitHub](https://github.com/honzajavorek)) transcript of Anna Ossowski's ([Twitter](https://twitter.com/OssAnna16), [GitHub](https://github.com/OssAnna16)) keynote [Be(Come) A Mentor! Help Others Succeed!](https://github.com/honzajavorek/become-mentor) for [PyCon CZ 2017](https://cz.pycon.org/2017/). 

Thank you!

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Slides and Script Table of Contents

- [Get a Jumpstart on Collaboration and Code Review in GitHub](#get-a-jumpstart-on-collaboration-and-code-review-in-github)
- [Welcome](#welcome)
- [Goal](#goal)

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Slides and Script

<table>

<tr><td width="30%">

![Slide 0](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_0.jpg)

</td><td>

### Get a Jumpstart on Collaboration and Code Review in GitHub 

By Katherine "Kati" Michel

</td></tr>


<tr><td width="30%">

![Slide 1](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_1.jpg)

</td><td>

### Welcome 

Welcome, everyone. I'm Kati Michel. I'm thrilled to have the opportunity to teach you what I've learned as the DjangoCon US Website Chair.

</td></tr>


<tr><td width="30%">

![Slide 2](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_2.jpg)

</td><td>

### Goal

* I want to teach you a process that will get you started collaborating and doing code review as quickly as possible. 
* I'm going to be showing you a lot of screenshots and diagrams, because I want you to understand what the process looks like.
* But don’t worry if you miss anything, because at the end of my talk, there will be a slide with a link to Useful Resources where you will find documentation and all of the commands I will be showing you today. 
* My slides and a video of my talk will also be online later.

</td></tr>


<tr><td width="30%">

![Slide 00](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_74.jpg)

</td><td>

### Go For It!

My last but not least recommendation is that you become a contributor to the DjangoCon US website next year 
* We have a diverse group of contributors of all skill levels and we are always looking for more contributors. Let us know if you are interested.  

</td></tr>


<tr><td width="30%">

![Slide 00](https://speakerd.s3.amazonaws.com/presentations/9c443e1c285345d6a370956f3852ae18/slide_75.jpg)

</td><td>

### Thank You

Feel free to contact me.

Useful Resources: 
https://git.io/v5fRh

* Twitter handle: @KatiMichel
* GitHub username: KatherineMichel

</td></tr>

</table>

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Useful Resources

### Links

GitHub
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

Collaborative Development Models and Permission Levels
* [About Collaborative Development Models](https://help.github.com/articles/about-collaborative-development-models)
* [Types of Collaborative Development Models](https://help.github.com/enterprise/2.7/user/articles/types-of-collaborative-development-models)
* [Permission Levels for an Organization](https://help.github.com/articles/permission-levels-for-an-organization)
* [Repository Permission Levels for an Organization](https://help.github.com/articles/repository-permission-levels-for-an-organization)

Documentation
* [DjangoCon US Website README.md](https://github.com/djangocon/2017.djangocon.us/blob/master/README.md)
* [DjangoCon US Website LICENSE](https://github.com/djangocon/2017.djangocon.us/blob/master/LICENSE)
* [DjangoCon US Website CODE_OF_CONDUCT.md](https://github.com/djangocon/2017.djangocon.us/blob/master/CODE_OF_CONDUCT.md)
* [DjangoCon US Website CONTRIBUTING.md](https://github.com/djangocon/2017.djangocon.us/blob/master/CONTRIBUTING.md)

Recovering a Deleted Branch
* [Can I Recover Branch After its Deletion in Git?](https://stackoverflow.com/questions/3640764/can-i-recover-branch-after-its-deletion-in-git)

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

```bash
$ git push https://github.com/<user-name>/<repo-name> <branch-name>
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

© 2017 Katherine Michel. All Rights Reserved.

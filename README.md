# A quick guide

[![forthebadge](https://forthebadge.com/images/badges/made-with-crayons.svg)](https://forthebadge.com)

## Table of Contents
* [tl;dr](#tl-dr)
* [Fork the project](#fork-the-project)
* [Clone the files](#clone-the-files)
* [Add upstream](#add-upstream)
* [Branch](#branch)
* [Do the actual work](#do-the-actual-work)
* [Push your changes](#push-your-changes)
* [Create the Pull Request](#create-the-pull-request)


## tl;dr
|&nbps;| action       | hint                                                      |
|------|--------------|-----------------------------------------------------------|
| 1.   | fork         | click <kbd>Fork</kbd>                                     |
| 2.   | clone        | `git clone git@github.com:name/project.git`               |
| 3.   | add upstream | `git remote add upstream git@github.com:name/project.git` |
| 4.   | branch       | `git checkout -b new-branch`                              |
| 5.   | work         | _finally_                                                 |
| 6.   | push         | `git push -u origin new-branch`                           |
| 7.   | create PR    | click <kbd>Compare & pull request</kbd>                   |


## Fork the project

Create a fork into your github by clicking the respective button inside the original project.

## Clone

Create a local copy of the project files and `cd` into it.

```bash
git clone git@github.com:name/project.git`
cd project
```

git clone https://github.com/pastparty/github-collaboration-instructions.git && cd !$:t

## Add upstream

Add the _upstream_ to the original project.

_origin_ points to your fork of the project (read + write)
_upstream_ points to the original project (read)

```bash
git remote add upstream git@github.com:name/project.git
```

## Branch 

Check for the project's right branching model (e.g. [git-flow](https://nvie.com/posts/a-successful-git-branching-model/)) and `git checkout branchname` 

```bash
git checkout master
git pull upstream master && git push origin master
git checkout -b new-branch
```
reads as

_Switch into `master` branch, have a look into the original project's master branch and update your local `master` branch and send these updates to your fork's master branch. Afterwards create and switch to `new-branch` locally._

## Work

Now you work on the actual files you want to. 
Add, commit as usual.

## Push

After you finished your work you want to create the Pull Request in the original's project repository.

```bash
git push -u origin new-branch
```

reads as

_Push my `new-branch` containing my work to my github fork and link the changes to the original project._

## Pull Request

Checkout your fork on Github and click the shiny buttonto create a pull request.
Create a matching description and don't forget to read the projects contribution guidelines.


With the help of [The beginner's guide to contributing to a GitHub project](https://akrabat.com/the-beginners-guide-to-contributing-to-a-github-project/) by Rob Allen.
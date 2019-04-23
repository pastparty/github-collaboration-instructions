# A quick guide
[![forthebadge](https://forthebadge.com/images/badges/made-with-crayons.svg)](https://forthebadge.com)

## tl;dr
|&nbsp;| action         | hint                                                      |
|------|:---------------|:----------------------------------------------------------|
| 1.   | _fork_         | click <kbd>Fork</kbd>                                     |
| 2.   | _clone_        | `git clone git@github.com:name/project.git`               |
| 3.   | _add upstream_ | `git remote add upstream git@github.com:name/project.git` |
| 4.   | _branch_       | `git checkout -b new-branch`                              |
| 5.   | _work_         | finally :gem:                                             |
| 6.   | _push_         | `git push -u origin new-branch`                           |
| 7.   | _create PR_    | click <kbd>Compare & pull request</kbd>                   |

---


## Table of Contents
* [tl;dr](#tldr)
* [Fork the project](#fork-the-project)
* [Clone the files](#clone-the-files)
* [Add upstream](#add-upstream)
* [Branching](#branching)
* [Do the actual work](#do-the-actual-work)
* [Push your changes](#push-your-changes)
* [Create the Pull Request](#create-the-pull-request)



## Fork the project

Create a fork into your github by clicking the respective button inside the original project.


## Clone the files

Create a local copy of the project files and `cd` into it.

```bash
git clone git@github.com:name/project.git`
cd project
```


## Add upstream

Add the _upstream_ to the original project.

:arrow_upper_right: _origin_ points to your fork of the project (read + write)

:arrow_upper_right: _upstream_ points to the original project (read)

```bash
git remote add upstream git@github.com:name/project.git
```


## Branching

Check for the project's right branching model (e.g. [git-flow](https://nvie.com/posts/a-successful-git-branching-model/)) and `git checkout branchname` 

```bash
git checkout master
git pull upstream master && git push origin master
git checkout -b new-branch
```
reads as:

_Switch into `master` branch, have a look into the original project's master branch and update your local `master` branch and send these updates to your fork's master branch. Afterwards create and switch to `new-branch` locally._


## Do the actual work

Now you work on the actual files you want to. 
Add, commit, business as usual.


## Push your changes

After you finished your work you want to create the Pull Request in the original's project repository.

```bash
git push -u origin new-branch
```
reads as:

_Push my `new-branch` containing my work to my github fork and link the changes to the original project._


## Create the Pull Request

Checkout your fork on Github and click the shiny button to create a pull request.
Create a matching description and don't forget to read the projects contribution guidelines.

---

With the help of [The beginner's guide to contributing to a GitHub project](https://akrabat.com/the-beginners-guide-to-contributing-to-a-github-project/) by Rob Allen. Thanks.

<!--
  <<< Author notes: Step 2 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
  TBD-step-2-notes.
-->

# Week 2: Introduction to branches and remotes

In the second week of the course:
- you will practice creating new branches and merging them
- you will practice resolving conflicts
- you will learn about Git remotes
- you will learn how to create a Pull Request to various branches

## 1. :book: Week 1 review
Review the content from the previous week reading more from Software Carpentry:
- [Creating a Repository](https://swcarpentry.github.io/git-novice/03-create.html)
- [Tracking Changes](https://swcarpentry.github.io/git-novice/04-changes.html)

## 2 :book: :eyes: What are the branches in this Git repository?

#### :eyes: **Video** :eyes: 
Watch another 10min of my presentation from [ABCD/RerproNim course](https://www.abcd-repronim.org/week2.html) 
for [introduction to Git branches and Git remotes](https://youtu.be/SyKmry47SsY?si=mUW-LOSmKsgnJZVK&t=2763) 
(the video should open at timestamp 46m03s, and you should watch till 55m40s).
Note that `master` used to be a default name of the main branch, but it has been changed to `main`.


> Questions:
> - Why would you use branches in Git?
> - Do you know how to check the current branch you are on?

## 3 :book: Git Parable
I highly recommend reading the [Git Parable](https://practical-neuroimaging.github.io/git_parable.html#the-git-parable) 
to understand the philosophy behind Git.

## 4 :keyboard: :white_check_mark: Exercise 1: Creating a new branch
In the new branch that was created for this week `week2` you will find a new directory `week2` that will be used as a working directory for this week. 

Your exercise is to create a new branch `week2_new1` and add a new file `week2/new_file_1.txt`, commit the content, 
and merge it to the `week2` branch. 

> [!TIP]
> If you don't remember how to open Codespace, create a new file and add to the repository, you can review instruction from the previous week [here](./week1/Readme.md)

## 5 :keyboard: :white_check_mark: Exercise 2: Resolving conflicts
In this exercise you will create two new branches `week2_new2` and `week2_new3` from the `week2` branch.
Change the file `week2/file_1.txt` in both branches and try to merge them back to the `week2` branch. 
You should see a conflict that you will need to resolve.

## 6 :keyboard: :white_check_mark: Exercise 3: Creating a Pull Request to the week2 branch

In the previous exercises you were merging branches to the `week2` branch directly using the `git` commands.
When working on the course, you were also practicing creating Pull Requests using GitHub interface to the `mian` branch.
In this exercise, I want you to create a new branch `week2_new4` from the `week2` branch, add a new file `week2/new_file_2.txt`,
and create a Pull Request using GitHub interface to the `week2` branch.

##

> [!IMPORTANT]
> Update the repository in order to move to the next week/part of the course:
>  - After finishing all the exercises, create a Pull Request from the `week2` branch to the `main` branch
>  - Check the status of tests
>  - If all tests pass, merge the Pull Request, this should update a new `README.md` on the main page of the repository 
> (you can reload the page after 30-60s if you don't see the new content)

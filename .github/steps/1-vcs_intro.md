<!--
  <<< Author notes: Step 1 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
  TBD-step-1-notes.
-->

# Week 1: Version Control Systems overview and Introduction to Git

In the first part of the course:
- you will learn basic information about Version Control Systems (VCS)
- you will learn what is Git and how to use it
- you will practice using Git in the GitHub codespace

## 1 :book: :eyes: What is Version Control System and Git

Version Control Systems help you track versions of digital artifacts, such as code (scripts, source files), 
configuration files, images, documents, and data. 
With proper annotation of changes, a VCS becomes the lab notebook for changing content in the digital world. 
Since all versions are stored, VCS makes it possible to provide any previous version at a later point in time. 
You can see how this is critical for reproducing previous results – if your work’s history is stored in a VCS, 
you just need to get a previous version of your materials to reproduce an earlier work. 
You can also recover a file which you mistakenly removed since a previous version would be contained within your VCS. 
These features alone make it worthwhile to place any materials you produce and care about under an appropriate VCS.

Besides tracking changes, another main function of a VCS is collaboration. 
Any modern VCS supports transfer and aggregation of changes to your work among collaborators. 
Public versioning and collaboration services (such as GitHub) allow you to integrate 
other online services, e.g., Codespace we will be using in this course.

#### :eyes: **Video** :eyes: 
Watch 10min of my presentation from [ABCD/RerproNim course](https://www.abcd-repronim.org/week2.html) 
for [introduction to VCS and Git](https://youtu.be/SyKmry47SsY?si=10_UXbh5fuEU8za6&t=2139) 
(the video should open at timestamp 35m39s, and you should watch till 46m)


#### More about VCS and Git from Software Carpentry
Software Carpentry provides an excellent introduction to VCS and Git, I recommend reading these parts:
- [Summary and Setup](https://swcarpentry.github.io/git-novice/index.html) (in this course we will be using GitHub Codespace, but I highly recommend following the instruction for installing Git on your local machine)
- [Another overview of VCS](https://swcarpentry.github.io/git-novice/01-basics.html)
- [All about setting up Git](https://swcarpentry.github.io/git-novice/02-setup.html)


> Questions:
> - Do you know how to add a new file to the repository?
> - Do you know how to check the status of the repository?
> - Do you know how to create a new snapshot of the repository?


## 2 :keyboard: Practicing using Git in Codespace

> [!TIP]
> - I recommend opening another browser tab with this repository, so you can keep these instructions open for reference all the time.
> - In case you haven't used Codespace before, I will provide very detailed steps for this first exercise.

1. Opening Codespace with terminal
  - Start from the landing page of your repository opened in new tab.
  - Change the branch to "week1" (you should see a new content that was not in the `main` branch)
  - Click the green "Code" button located in the middle of the page.
  - Select the Codespaces tab in the box that pops up and then click the "Create codespace on week1" button.
  - Verify your codespace is running. The browser should contain a VS Code web-based editor and a terminal.
  - In the terminal, move to the `week1` directory that is the working directory for this week.
    (if you don't see this directory, you're likely in a wrong branch).

2. Practice using the command you learn about from the video:
  -  `git add`
  -  `git commit`
  -  `git push`
  - `git log`
  - `git status`
  - `git diff`
  -  try using `man` to learn more about the commands, e.g. `man git status`

## 3 :keyboard: :white_check_mark: Exercise 1: Modify the content of the files and update the repository

> [!TIP]
> - This exercise has :keyboard: and :white_check_mark:, that means you will have a specific task and the output will be checked by automatic tests I wrote for this course, and the repository will move to **Part 2** after the task is completed.
> - This is our first exercise of this type, so I will provide very detailed steps to guide you.


1. Go to terminal in Codespace (you can use the one that you opened in part 2, or follow the instruction from part 2 to open again)
2. Update content of a file:
  - Go to `week1` directory
  - Check the content of `file1.txt` file and update it to "Hello, World!"
  - Add the changes to the repository and commit them
3. Create a new file:
  - Create a new file `file.txt` with a content "It's a beutiful day" (you can use `touch` or/and `echo` command)
  - Add a new file to the repository and commit the changes
4. Change the name of your new file:
   - change the name of the file `file.txt` to `file2.txt` in a way that you keep 
   the file history (use `man` to check `git mv` command)
   - Add the changes to the repository and commit them
   - Run `git log` to check the history of the `file2.txt` file
5. Create a Pull Request to the `main` branch
   - Use GitHub interface to create a Pull Request
   - Check the status of tests
   - If all tests pass, merge the Pull Request, this should update a new `README.md` on the main page of the repository (you can reload the page after 30-60s if you don't see the new content)

> [!IMPORTANT]
> Following all the steps from part 3, including creating and merging the Pull Request, is necessary to move to the next parts of the course.

# Contributing to RISC OS Community Projects and repositories
This is a relatively short guide about how to contribute to the ROS Community projects.

You can contribute by:
1) Adding new projects and ideas
2) Improving/fixing code in existing repositories
3) Reviewing/Improving requirements and documentation
4) Helping us with the graphics/sound that certain projects and repositories may require
5) Helping us testing the code on as many RISC OS platforms and OS versions as possible (within the supported range)
6) Providing us constructive feedback on the work/projects/repositories/requirements/designs

Next chapters will help who is completely new to this process, introduce a common dictionary of technical terms to make sure we are all on the same page and finally provide instructions on how to submit back your contribution.

Thanks for considering helping us and we hope you'll have fun!

## Is this your first contribution ever?
If this is your first ever contribution to an Open Source project then don't be afraid, here there is a free course for you to follow that will give you a lot of good information: [How to contribute to an Open Source project on GitHub](https://app.egghead.io/playlists/how-to-contribute-to-an-open-source-project-on-github)

## Submitting code
To submit your changes we use Pull Requests (if you used GitLab instead they are called there Merge Requests). Any code change should be submitted as a pull request, no other ways are allowed, sorry. Read below for the details and the guidelines.

## Common dictionary
Table of technical terms and meaning in this context:
```
+------------------------------+------------------------------------------------+
|         Terms                |                Description                     |
+------------------------------+------------------------------------------------+
| Divergent Development        | Development that may end up generating two or  |
|                              | more projects as a split from an original one. |
|                              | A typical example of this are Forks, they may  |
|                              | not converge back into the original project    |
|                              | and originate a new one or a split from the    |
|                              | original one.                                  |
+------------------------------+------------------------------------------------+
| Convergent Development       | Development that is always going to converge   |
|                              | back into the original project. A good example |
|                              | of this are Branches that are ALWAYS meant to  |
|                              | converge back to the original project.         |
+------------------------------+------------------------------------------------+
| Versioning System            | Is a tool or a framework that allows a team of |
|                              | developers to manage their shared source code  |
|                              | in both way Divergent and Convergent Dev.      |
|                              | Git is an example of this and github too.      |
+------------------------------+------------------------------------------------+
| Fork                         | In git a fork is a complete copy of an entire  |
|                              | repository which includes its history till     |
|                              | that moment a user forked the repo.            |
|                              | Forks are recommended when the new code may or |
|                              | may NOT converge back to the original codebase |
+------------------------------+------------------------------------------------+
| Branch                       | Branches are more like "construction zones" in |
|                              | a codebase and so they are meant to rejoin the |
|                              | original codebase when done.                   |
|                              | Branches should be intended as a short living  |
|                              | entity use to work to improve/change a specific|
|                              | feature in the original codebase.              |
+------------------------------+------------------------------------------------+
| diff                         | Its a tool or an automatic procedure meant to  |
|                              | detect all the changes between the codebase    |
|                              | and the fork or the branch we are comparing.   |
+------------------------------+------------------------------------------------+ 
```
**Please note:** 

Forks are more expensive than branches as they creates a full copy of a project and when merged back to the codebase git has to run a full diff of everything while with a Branch git runs a diff only of the portion we have worked/modified. Forks also take up more space generally.

## Pre-requisites (before you start)
Please make sure you have a github account before you start. Also we recommend to add your RSA Public key to your github account. If you do not know how to do that please follow the instructions here:

- [Create a github account](https://github.com/join)
- [Add an RSA key to your github account](https://docs.github.com/en/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account)
- [It's a good practice to protect your accoutn by adding 2 factors authentication](https://docs.github.com/en/github/authenticating-to-github/configuring-two-factor-authentication)
- [Join RISC OS Community, by filling up this form and give us your github account name and what type of contribution you would like to purse](https://paolozaino.wordpress.com/contact/)

## Contributing to this project/repository
To contribute is fairly easy:

Until a proper RISC OS git tool is being released, we encourage you to use for your "local git" either a Windows computer or a Linux computer or Virtual Machine.

There are some very useful tips [here at the ROOL Forum](https://www.riscosopen.org/content/documents/git-cheatsheet)

## Contributing General Guidelines
In general you'd want to:
* Clone a repo from here to your local git using: `git clone repo-url`
* Get into the repo using: `cd repo-name`
* Create your branch using: `git branch -b branch-name`
  - we suggest that you name your branches following this pattern: `your_nick-what_type_of_changes_you_are_applying` with no spaces, you can use either dash or underscore to your preference
* Start adding your changes
  - Where applicable stick to RISC OS Style guide
  - Make sure you keep the documentation and code comments up-to-date with your changes
* When done with your changes add them to your local git using: `git add ./what-you-chaged`
* Commit your changes using: `git commit -m "commit message"`
  - Make sure your commit messages are clear and meaningful to help reviewers to understand what you were trying to achieve
  - When possible try to make small commits and Pull Requests so that the review process can be quicker
* Push your local branch into github using: `git push -u origin your_nick-what_type_of_changes_you_are_applying`
* Submit your branch for review when it is done, do this by making a Pull Request and requesting a review from the Code Reviews Team
  - Make sure you've tested your changes before submitting a Pull Request


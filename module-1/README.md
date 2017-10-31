# Introduction to Source Control
## Module 1

### Introduction

Welcome to the Aggie MakerSpace course on source control for software development!
This course is designed to introduce university students to the power of collaborative, distributed
source control through git and GitHub. The purpose of this module is to prepare your machine to
use git and familiarize you with git and GitHub terminology.

### Course Content

This module can be experienced in one of two ways:
  1. YouTube video available [here](http://www.youtube.com/watch?v=Crp40qvuRSE).
  2. Full text of the video is available below.

### Course Transcript

#### What is Source Control?

Source control is a technology that allows developers and other professionals to track
changes to a project over time, and manage releases of data. Basically, this allows
you to have a `master`, or `release` copy of your project, and multiple working copies
called _branches_ that individual team members can contribute to, and submit these changes for review.

#### Git Source Control Management

Specifically, this course will use git to control our projects. Git is a _distributed source control system_,
meaning that each developer's computer has a full copy of the project, which allows developers to
work when offline and unable to connect to a central server. Multiple full copies also helps prevent
data loss.

##### Branching

Git uses a model called _branching_ to help control code. Each branch is a separate set
of changes over time. The `master` branch is the main, default set of the refined project.
For a software organization, the `master` branch would be the code currently deployed to
customers and available on app stores. Making a new branch takes all the history from
the current branch and makes a new copy of it. For example, making `branch-1` from the `master`
branch makes a copy of all of the changes in the master branch and saves it under the `branch-1`.
Now, while `branch-1` is the active branch, any changes that are saved, or _committed_ in git terminology,
are added to the `branch-1` history **but not the `master` branch history**.
This separation allows developers to implement new features, troubleshoot and fix bugs,
and enhance the user experience **without** affecting the code shipping to customers.

Branches should be address one specific task or change. They should target only one bug
or add only one feature. This allows the changes for that specific feature to be reviewed
separately from any other changes. Speaking of code review, let's discuss pull requests.

##### Pull Requests

Once a developer has completed all changes for his or her specific branch, it is time to request a review!
Code review is an important step of the software development process. In a collaborative
project, no changes should be merged to the `master` branch without being checked by another
team member. Even in a two person team, Developer A should always have Developer B review his or her
changes before merging. Likewise, Developer B will always ask Developer A to check his or her
changes before merging to `master`. This process can be quickly handled in a _pull request_.

Remember that each developer is working on a separate _working branch_ that contains only the
changes for their specific task. A _pull request_ is a request by the developer to _pull_ those
changes from the _working branch_ into the `master` branch. In a pull request, reviewers can view
the changes made and make comments, ask for clarification, or suggest changes. This ensures that the
only changes to make it to the `master` branch are the **best possible work of the whole team**, not
just a single developer. The largest benefit of the pull request model is that these comments are
made within the context of the changes themselves. Reviewers can comment on the **exact** line
that they are referring to, which makes it easier to communicate between team members without
being in the same place or even working at the same time.

Once a _pull request_ is approved, it can be merged into the `master` branch, which adds all
changes made since the creation of the branch to the `master` branch.

### Exercise

Your exercise for this module is to submit a pull request introducing yourself to the
NC A&T Makerspace community. From the [main repository page](https://github.com/aggiemakerspace/github-training), open the `submissions` directory
and create a new file called `about.md` in `submissions/[your-github-username]/`.
Your `about.md` file is a [Markdown](https://guides.github.com/features/mastering-markdown/)
document that can be formatted using Markdown syntax. Your document should answer the following questions:
* Who are you? What is your name and what do you do on campus?
* What do you do outside of school? What are your hobbies and passions?
* What do _you_ have experience in? What can others ask you about for assistance? This community can only thrive with the cumulative skills and experience of all of us. **Those skills and collaborations** are what we are using GitHub to enhance.

Once you have completed your `about.md`, select "Create a new branch for this commit and start a pull request". Follow the _pull request template_ provided when you click "Commit new file".

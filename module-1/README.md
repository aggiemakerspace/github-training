# Introduction to Source Control
## Module 1

### Introduction

Welcome to the Aggie Makerspace course on source control for software development!
This course is designed to introduce university students to the power of collaborative, distributed
source control through git and GitHub. The purpose of this module is to prepare your machine to
use git and familiarize you with git and GitHub terminology.

### Course Content

This module can be experienced in one of two ways:
  1. YouTube video available here
  2. Full text of the video is available below

### Course Transcript

#### What is Source Control?

Source control is a technology that allows developers and other professionals to track
changes to a project over time, and manage releases of data. Basically, this allows
you to have a `master`, or `release` copy of your project, and multiple working copies
called `branches` that individual team members can contribute to, and submit these changes for review.

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

Once a developer

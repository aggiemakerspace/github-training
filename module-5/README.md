# Project Management in GitHub

## Module 5

### Introduction

Collaboration is a powerful force, and to harness that force, the open source community, as well as project teams in academia, public service, and private enterprise need skilled project managers. Project managers need equally powerful tools to guide the combined power of a project team towards their objectives, and GitHub has tools that can help!

### Course Content

This module is currently only available in text form. Video coming soon!

### Course Transcript

#### People First

In any project, the most important thing is the PEOPLE who are working with you! This can be a few close friends or an interdisciplinary team of professional developers, designers, QA engineers, and more. Therefore, it is important to keep track of people, our most vital resource.

##### Organizations

Organizations are the highest level grouping of people. An organization should be a group of people working together on one or more projects with common purpose. These can reflect campus organizations, project teams, or many other social groups. Just at A&T, there are GitHub organizations for the Makerspace, Robotics Club, AutoDrive Challenge team, COMP 167 Classroom, and countless student projects. The first step to managing any project is building your organization.

##### Teams

Larger organizations can use teams to organize people. Teams can serve any purpose, and are especially helpful for setting permissions levels. For example, let's say I am trying to organize a team to develop an app that connects students to their Aggie Access and Blackboard accounts in a native interface, rather than the poorly formatted webviews we currently deal with on mobile. This is a complex undertaking that could be divided into several tasks:
    - iOS Application Development
    - Android Application Development
    - Server integration with Aggie Access and Blackboard (back-end)
    - Test and Quality Control

Each of these subtasks requires a unique set of skills, as well as coordination with the larger effort, sounds like a great job for teams! I can create the teams for the individual tasks and assign developers as needed.

#### Communication

Once the organization is created and teams are organized, it's time to open line of communication! One of the most important needs of complicated, technical communication is _context_. It's absolutely vital that conversation about code, designs, or technical documentation be able to reference the _exact_ item being discussed. Additionally, the closer important discussions are kept to the project, the more they can influence future development.

Additionally, it is essential that managers be able to assign tasks quickly to the developers, engineers, and others working on the project. Tasks should be organized, searchable, and have an opportunity to have questions answered and objective clarified.

The solution to **both** of the above needs is GitHub Issues! Issues can be used for conversations, task tracking, bug reporting, and anything else the project manager can imagine. Labels are fully customizable so they can be organized any way the project requires. For our example project, we may add a _task_ label and a _discussion_ label. Issues can be assigned to up to 10 people, and when the task is complete or the conversation has reached a conclusion, they can be closed.

You can also create and [issue template](https://help.github.com/articles/creating-an-issue-template-for-your-repository/) that will prompt users for specific information your organization needs in an issue. This can also be customized for each individual repository as each one has unique needs.

#### Organizing Work

Now that we have some issues related to our project, we should assign due dates and organize them visually. Due dates can be assigned by creating _milestones_ and adding issues to them. Milestones are a tool from the scrum framework of agile development. Scrum depends on set-length iterations that repeat, with set tasks to be completed each iteration. For example, on a set interval, say a week or a month, the team will decide which tasks should be addressed, and add them to the _sprint_. At the conclusion of the sprint, the team can see what was planned versus what was accomplished, and factor that into place for the following sprint! This method of rolling, iterative deadlines is a great way to build software over time, but its only one way that we can use milestones to make GitHub issues time-bound.

In addition to organizing through milestones, we can organize tasks and discussions visually using GitHub _project boards_. Project boards organize issues and cards into columns of the managers design, and can be used to track overall issue progress, individual sprints, or really anything you need to see to manage. Common columns are things like _backlog_, open tasks or bugs that have not been scheduled to be completed. _In progress_ is another common column that holds issues an individual developer or team is actively working on. _Under review_ indicates an open pull request has been submitted for a particular issue and it should be closing soon. Project boards can be hosted at _either_ the Organization or the Repository level, but issues can _only_ be made at the repository level.

Automation is your friend as a project manager, and GitHub recently released some basic automations for project boards. These can aid you as the project manager by automatically moving certain issues around the board, and will be expanding in capability in the future.

#### Controlled Collaboration

The final thing the project manager must be aware of is the protection of organization data. Collaboration is _great_, and it is the source of GitHub's collective strength. However, collaboration without process and review is _not_ conducive to an engineering environment. Our organization has worked **hard** on our fictional iOS and Android application, and we don't want just _any_ code to make it into our production branch.

Therefore, managers must use GitHub permissions to control who can access repositories. It is advised that only the individuals and/or teams who work in a specific repository should be given _write_ access to that repository. Additionally, protecting branches keeps unreviewed code from being merged with the production branch. Code review is an absolutely essential part of the collaborative process. On GitHub, we use PULL REQUESTS to review code before merging it with our branches, and protecting our production branch can require a pull request before code is added.

[CODEOWNERS](https://help.github.com/articles/about-codeowners/) is a useful tool for larger repositories or projects. The CODEOWNERS file can say, for example, that if a C# source file is changed, our C# expert must review it. Or, if a source file in a specific package is changed, the architect of that particular package must review it. This empowers technical experts on your team to contribute where they are most qualified in code review.

To facilitate these requests, you can provide a template for a pull request by creating a [PULL_REQUEST_TEMPLATE](https://help.github.com/articles/creating-a-pull-request-template-for-your-repository/) document that outlines the information you need from developers who want to merge code into production branches, this can speed up the review process because all necessary information is requested up front.

#### Management Conclusion

Now you are familiar with all of GitHub's tools to manage the individuals, tasks, discussions, and deadlines for your project. Remember that ethical managers practice servant leadership, placing the needs of your people first and providing them the resources they need to succeed. Use these tools to provide constant, constructive feedback to your team members, and also use them as a way to _listen_ to what your team has to say with empathy and grace. Communication tools are only as strong as the **two-way** flow of information, which requires active listening on the part of the project manager.

Finally, project managers should actively work to make their open source community, project team, or student group as inclusive an welcoming as possible. Tools like the [code of conduct](https://help.github.com/articles/adding-a-code-of-conduct-to-your-project/) for your project or organization set expectations up front for the respect and courtesy that you as the manager expect for all contributors. Strong, healthy development communities are also welcoming, inclusive communities for all.

#### Bonus Points

For your information, the following resources may also be useful to project teams:
- [Summary of project management features by GitHub](https://github.com/features/project-management)
- [Atom Teletype - Real Time Collaborative Coding](https://teletype.atom.io)

### Exercise

For this exercise, practice making an organization on GitHub. This can be for an actual organization or project you are involved with, or just for practice. Create a project and add some cards to the project board. In your `submission/[user-name]` directory, create a `module-5.md` document that provides a link to your organization and a couple of sentences on how GitHub Project Management features can improve your organizations productivity.

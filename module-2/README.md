# Using Git with GitHub
## Module 2

### Introduction

GitHub is only as powerful as our ability to harness git! Remember, git is the underlying technology that _actually_ tracks our changes, saves our commits, and stores our branches. GitHub, on the other hand, is an incredibly powerful web interface and cloud-hosting platform that allows us to store our git repositories remotely and collaborate with a community of over _3.5 million_ developers worldwide with additional tools and views.

In this module, there are two ways to complete it. You can either complete it using the [GitHub Desktop Application](https://desktop.github.com) or the [terminal/gitbash](https://git-scm.com). It is recommended that those without command line experience _start_ with the GitHub Desktop version. Experienced developers or those looking for a challenge are encouraged to try working with git on the command line.

### Course Content

As always, this module can be experienced in two ways:
  1. Youtube video available using GitHub Desktop here.
  2. Youtube video available using the terminal/git bash here.
  2. Full text of the course is available below.

### Course Transcript

#### Creating a Repository

If you do not already have a repository, or you are not using a repository that already exists, you must create one! For the purposes of this course, we are not creating a repository, but we will go over the steps. Repositories are a great way to keep code together for classes or projects, so you'll definitely be creating some on your own as you work GitHub into your personal workflow.

To create a new repository, go to your [GitHub homepage](https://github.com) and select "New Repository". The only thing you need to create your repository is a name. Remember, much like branch names, repository names do not have spaces. You may choose to add a description, but this is not necessary. You can also select whether your repository should be public or private on this page. This determines whether or not people can view your repository without your express permission. If you have signed up for the [GitHub Student Developer Pack](https://education.github.com/pack) in [Module 0](../module-0), then you have unlimited private repositories, so feel free to use them when you feel it necessary.

Finally, you have the option to add a README, a license, and a .gitignore file to your repostiory:
- A README is a markdown file that renders automatically on GitHub. You will notice that assignments in this repository use READMEs to display instructions without you having to manually open a file. READMEs are great for installation instructions, announcements, or any other information any visitor to your repository may need.
- A .gitignore file contains files, directories, and file types that exist in your project repository but should _not_ be committed. A great candidate for a .gitignore is any generated file, like .class and .jar files in Java applications. These files are recreated every single time NetBeans compiles a project, and committing them just takes up more room and can potentially cause merge conflicts. GitHub has several template .gitignore files to choose from for many popular languages and frameworks, including Java.
- A license file describes what users are and are not allowed to do with your repository. Technically, a project on GitHub is not [open source](https://github.com/open-source) unless the license specifically gives permission for users to view, fork, and modify said code. There are several great license templates available on GitHub, and GitHub created [this useful guide](https://choosealicense.com) to help you choose the one right for you. For something like basic code written for a class, consider the [Unlicense Academic](https://github.com/ccannon94/UnlicenseAcademic), which releases your code completely into the public domain but has specific language disallowing users from using your code to cheat.

Once you've made your selection, choose "Create repository" and you are good to go!

#### Cloning a Repo

Now that you have a repository, in this case, the github-traning repository, you should clone it to your local machine so that you can work on it! It is important to remember two key concepts with your cloned repository, remote and local.
- Remote: an internet-accessible copy of your repository that is treated as an authoritative source of that repository. In this case, your remote is GitHub!
- Local: a full copy of your repository cloned to a personal computer to be worked on.

GitHub Desktop automatically creates a subdirectory of "Documents" called "GitHub", where it clones all of your repositories, we will follow the same convention with both GitHub Desktop and the command line.

##### GitHub Desktop

From your repository homepage, click "Clone or download" and choose "Open in Desktop".

##### Command Line

- From your repository homepage, click "Clone or download", copy the link to your clipboard.
- Open terminal or Git Bash. If you do not already have a "~/Documents/GitHub" directory, run `mkdir ~/Documents/GitHub`
- Now, run `cd ~/Documents/GitHub` to change your active directory to your GitHub directory.
- Run `git clone [paste-link here]` to clone your repository inside your GitHub directory.
- **IMPORTANT** you MUST run `cd [github-repository-name]` after cloning before you can run any git commands!

#### Creating a Working Branch

Remember, our "master" branch is a clean, "release-worthy" branch of our highest-quality code. Now, when you are working on your own repository where you are the sole contributor and you are just working on a simple homework assignment, it may not be necessary to use individual branches. For working in this repository, as well as any other well-maintained public repository, you _cannot_ commit directly to the master branch, and therefore **must** make a working branch. For this module, we will name your working branch "[GitHub Username]-module2".

##### GitHub Desktop

##### Command Line

#### Making, Saving, and Tracking changes

Now, when it's time to make changes, you simply open the files you cloned in your text editor of choice! Make changes and save them just like you'd usually work on code. If you are creating a new project in an IDE, make sure you place this project _inside_ your repository, **not** the default save location for that IDE. For example, NetBeans will try to save all new projects in "~/Documents/NetBeansProjects/", but if you are using git in COMP163 or COMP167, you will want to set your project location to "~/Documents/GitHub/[Repository-Name]". Finally, once changes have been made, you must tell git to track these changes and add them to your staging area for a commit.

##### GitHub Desktop

##### Command Line

#### Committing

Once your changes have been saved, you wrap up these changes in a "commit" so that git can add them to the project history. You should commit often enough that you can describe what each commit does in a single concise sentence. For example "Override toString method", "Implement getters/setters", "Create UIViewController class". Notice that these commit messages are given in the _imperative voice_, which means they explain what the commit _will do_, they don't talk about what they've _done_. The reason for this is quite simple: when working on git, you should be committing changes to a working branch, not the "master" branch. Given that the "master" branch is considered the shipping version of your code, any code not in master isn't technically _done_ just yet, so saying "Overrode toString method" or "Implemented getters/setters" isn't actually accurate yet! Writing in the imperative voice gives a concise summary of changes in a commit message that clearly tells the reviewer what a pull request WILL DO if merged.

##### GitHub Desktop

##### Command Line

#### Pushing/Pulling

The more often you push, the better. One rule is certain, before you close your laptop or sign off of a desktop, you should _definitely_ push your changes to your remote. This adds any changes you made on a given branch locally to the remote version of that branch. You should do this whenever you are getting ready to leave a computer in case you need to continue work on another computer, or if something physically happens to the computer you were working on previously.

You should also pull at the start of each development session, and any time you check out a new branch, to make sure you are working on the most up to date version of that branch. A _pull_ operation consists of two parts: _fetching_ the remote version of your current branch and _merging_ it in to your local verison. This is generally handled behind the scenes without the user needing to add more control.

##### GitHub Desktop

##### Command Line

#### Updating Branches from Master

Often, especially on projects including two or more developers, the "master" branch may be updated since you created your working branch. If you remember from [Module 1](../module-1), we must merge those changes into our working branch in order to make sure we are continually working on the most up to date version of our code.

##### GitHub Desktop

##### Command Line

### Exercise

Using your chosen git client (command line or GitHub Desktop), clone this repository, create a new working branch, and create a file called "git-quiz.md" in "submissions/[Your-username]/module-2". Answer the following questions in your file:
1. How often should you commit, when working in git?
2. How often should you push, when working in git?
3. Did you decide to use GitHub Desktop or the command line to complete this exercise?
4. How will you commit and push these changes using your chosen method?

Push these changes and open a pull request in the [github-training repo](https://github.com/aggiemakerspace/github-training).

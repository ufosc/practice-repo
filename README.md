# Git-Intro

This repository is meant to let people learn how git and GitHub work, without messing with a project. Feel free to change files (aside from this README) and upload new ones.

## General Guideline
\* _These are general rules to follow, not set in stone_

1. Fetch often
2. Commit often and in appropriate chunks
3. Test before commit
4. Concise commit messages (No more than 80 characters)
5. Good Workflow (see below)


## Getting Started

### Terms

**Git** - An open source distributed version control software. Allows for multiple people to easily work on the same project.

**Repository** - A place where the project and it's history is stored.

**Branch** - Is the source from a repository taken at certain point in time. Usually done to apply your own changes to it.

**GitHub** - A web based Git repository hosting service. It's where we will be hosting our projects.

**Commit** - A commit is an update to the code. It can do things like add files or modify sections of code.

**Issues** - A bug or feature request you want to let the team know about.

### What you need

Install Git here https://www.git-scm.com/downloads

GitHub account here https://github.com/

#### Setting up Git

On Linux or OSX open up a terminal. On Windows open up the Git Bash application.

Set up your name and the email you used for your GitHub account.

```
git config --global user.name "Your Name Here"

git config --global user.email "your_email@youremail.com"
```

### Create local repository

Navigate to where you want the projects to be on your computer.

```
cd path/to/where/you/want/the/code
```

#### New Project

Make a folder with the name of the Project

```
mkdir Project-Name
```

**git init** - This will create a new git repository in the current directory.
```
git init
```

#### Project from GitHub

Copy the url from the repository you want on your computer.

**git clone** - This will create a copy of the designated repository on your computer.

```
git clone https://github.com/UFOSC/Git-Intro.git
```

### Updating

**git fetch** - Checks if there are updates from a specific branch. Usually check the original branch. It doesn't change anything on your local branch.

```
git fetch origin/master
```

**git merge** - This merges changes from the branch specified to your current brach.

```
git merge origin/master
```

Always update before trying to commit code

### Committing

**git add** - This tells git you want to add specific files to a branch, this does not actually change anything.

```
git add helloWorld.txt
```

**git commit** - This wraps the added files with a message ready to push up to the branch. It will open up a text editor in the terminal where you can type the message.

```
git commit
```

Update again!

**git push** - This pushes your committed changes to the branch indicated.

```
git push origin/master
```

### Switching Branches

Check for any updates

```
git fetch
```

**git checkout** - This switches the branch your working on to a different one. Usually it will be to a development branch or a bug fix branch.

```
git checkout dev
```

### Creating Issues

On the GitHub page for the repository clcik on the issues tab. Then clcik the green `New Issue` button.

Give an appropriate title and detailed description so people can recreate the issue.

Click Submit New Issue when you're done. A number will be assigned to the issue.

### Closing Issues

In a commit message to that branch include:

```
Fix #X
```

or

```
Close #X
```

### Workflow

Usually there are several branches on the main repository.

Master, which is usually a stable version of the software, Normally you don't directly update this.

Development or dev branch is where you pull and push most the development. You typically don't edit code directly here.

Other branches are made for a variety of reasons. For example, if there is a feature being worked on, create a new branch from development. Once that feature is working, push it back into the devleopment branch.

Name the new branch in a way that is short and descriptive, such as Contact-Database.

Once a feature branch is working, make a pull request to the development branch. Administrators will check it, and confirm the merge. When the development branch is stable enough, it will be mergred into the master branch.

### TODO

- Section on handling conflicts

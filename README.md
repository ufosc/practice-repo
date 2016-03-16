# Test-Repository

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
git clone https://github.com/UFOSC/Test-Repository.git
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

### Workflow

Usually there are several branches on the main repository.

Master, which is usually a stable version of the software, Normally you don't directly update this.

Development or dev branch is where most development occurs. New features and bug fixes often are added here.

Other branches are made as necessary for a variety of reasons. Often if a feature is big enough or something is experimental, it will get it's own branch.

### TODO

- Section on handling conflicts
- Section on creating issues
- Section on fixing issues 

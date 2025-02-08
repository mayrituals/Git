# git

In this repository I would like to provide some commands that I use to work with Git console and local/remote repositories.

For example, we can see how I created my GitHub portfolio step by step.

## Navigation

- [Creating repository](#creating-repository)
 - [Cloning our repository](#cloning-our-repository)
 - [Checking repository status](#checking-repository-status)
 - [Opening VSC with console](#opening-vsc-with-console)
 - [Adding changes](#adding-changes)
 - [Commit changes](#commit-changes)
 - [Uploading commits](#uploading-our-local-commits-to-a-remote-repository)
 - [Updating the local repository](#updating-the-local-repository)
 - [Updating the local repository](#updating-the-local-repository)
 - [Resetting changes](#resetting-changes)
- [Working with branches](#working-with-branches)
  - [Creating a new branch](#creating-a-new-branch)
  - [Listing all branches](#listing-all-branches)
  - [Switching to another branch](#switching-to-another-branch)
  - [Creating and switching to a new branch](#creating-and-switching-to-a-new-branch-in-one-command)
  - [Merging branches](#merging-branches)

## Working with Repository

#### Creating repository

```git
git init mayrituals                        
```

If using a username the same as in GitHub, we can get a special README file that we can turn into our portfolio.

#### Cloning our repository

```git
git clone https://github.com/mayrituals/mayrituals.git
```

We need to copy our link on GitHub to our repository to clone it on our computer.

#### Checking repository status

```git
git status
```

Just to check if our file is in its right place.

#### Opening VSC with console

```git
code mayrituals
```

VSC opened, and we can edit our README file. Save file (CTRL + S) after you did changes or added new things.

#### Adding changes

```git
git add . or (file_name)
```

We're using this command to stage our changes before committing them.

#### Commit changes

```git
git commit -m "Portfolio Description Update"
```

#### Uploading our local commits to a remote repository

```git
git push
```

#### Updating the local repository with remote changes

```git
git pull
```
In case if the changes was made on remote repository by somebody and we need to have it on our computer.

#### Viewing commit history

```git
git log
```
#### Resetting changes

```git
git reset --hard HEAD~1
```
used to reset the repository's state and move the branch pointer to the previous commit.

## Working with branches


#### Creating a new branch

```git
git branch feature-branch
```

#### Listing all branches

```git
git branch
```

#### Switching to another branch

```git
git checkout feature-branch
```

```git
git switch feature-branch
```

#### Creating and switching to a new branch in one command

```git
git checkout -b new-branch
```

```git
git switch -c new-branch
```

#### Merging branches

```git
git checkout main
git merge feature-branch
```

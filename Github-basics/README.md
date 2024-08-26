### Github Basics

## Configure Git

<p>Set name and email</p>

```sh
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

## Initialize a Git Repository

```sh
git init
git add .
git commit -m "Initial commit"
git remote add origin git@github.com:username/new_repo
git push -u origin master
```

## Git Branch

<p>List All Remote Branches</p>

```sh
git branch
```

<p>List All Remote Branches</p>

```sh
git branch -r
```

<p>List All local and Remote Branches</p>

```sh
git branch -a
```

<h3>Create a New Branch</h3>

```sh
git branch <branch-name>
```

<p>Create and Switch to a New Branch</p>

```sh
git checkout -b <branch-name>
```


<h3>Rename a Branch</h3>

<p>Create and Switch to a New Branch</p>

```sh
git branch -m <new-branch-name>
```

<p>Rename a Specific Branch</p>

```sh
git branch -m <old-branch-name> <new-branch-name>
```

<h3>Delete a Branch</h3>

<p>Delete a Local Branch</p>

```sh
git branch -d <branch-name>
```

<p>Delete a Remote Branch</p>

```sh
git push origin --delete <branch-name>
```

## Git Pull

<h3>Pull from a Specific Remote Repository</h3>

```sh
git pull <remote-name>
```

<p>Pulls changes from the specified remote repository. For example, if your remote is named upstream instead of the default origin, you would use git pull upstream.</p>

<h3>Pull from a Specific Branch</h3>

```sh
git pull origin <remote-name>
```

<p>Pulls changes from the specified branch in the remote repository. For example, git pull origin main will pull changes from the main branch on the remote named origin.</p>

## Git Last Commits

```sh
git log
git log branch_name
```
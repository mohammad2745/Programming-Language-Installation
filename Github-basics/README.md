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

## Clone a Repository
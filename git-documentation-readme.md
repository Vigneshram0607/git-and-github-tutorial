# Git & Github
    Git is a version control system, helps you keep track of code changes, used to collaborate on code.

### Git Alternatives:
- BitBucket
- GitBucket

### Git Configuration:
Add username and mail id to git configuration

```bash 
$ git config --global user.name "YourUsername"
$ git config --global user.email "YourEmail@gmail.com"
```

## Commands
> *plan* [insert->add->commit->push]

Clone the Git repo 
> here linke-to-the-github-repo is said to be **ORIGIN**
```bash
$ git clone link-to-the-github-repo
```
To Initialize the git repo
```bash
$ git init
```

Check the `git status` to check whether the file is a part of our repo
```bash
$ git status
```

Add the newly created file to the **Staging Environment**

> *Staged files* are files that are ready to be committed to the repository you are working on.

```bash
$ git add file-to-be-committed.txt
```

To add all files (Files under same folder)
```bash
$ git add --all 
```
or
```bash
$ git add -A
```

Move the file from `stage` to `commit` for our repo

>Adding *commits* keep track of our progress and changes as we work. Git considers each commit change point or "save point". It is a point in the project you can go back to if you find a bug, or want to make a change.

>[!IMPORTANT] : When we `commit`, we should **always** include a **message**
```bash
$ git commit -m "Your one-line message!"
```

Commit files directly to `commit stage` instead of `staging environment`
```bash
$ git commit -a -m "Your one-line message!"
```

To view the history of commits for a repository
```bash
$ git log
```

To upload local git-copy folder to github folder we use **PUSH**
- Here, origin is "link-to-the-github-repo"
- We are asking them to push our local git-copy folder to ORIGIN's main folder
```bash
$ git push origin main
```
To update the local git-copy folder to present version
```bash
$ git pull
```
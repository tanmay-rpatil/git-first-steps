# Getting Started!

## Local Setup

1. Install and verify git from [Git - Downloads](https://git-scm.com/downloads)

2. Create a remote repository, and get its URL 

3. Config - open terminal (or git bash on Windows)
   
   ```bash
   # The config is a one-time setup for git
   $ git conﬁg --global user.name "tanmay-rpatil" #your username
   $ git conﬁg --global user.email tanmaypatil@example.com #your mail
   
    # the following is a one-time setup for each repo
    # make a dir and initialize a repo
   $ mkdir new-repo
   $ cd ./new-repo
   $ git init
   $ git remote add origin https://your-url-here
    # there! now a remote is linked. Let's add a file and push it
   ```

## First changes - and Repeated Steps

Open a terminal in your new-repo directory. These are the steps you'll repeat for any further changes to add-commit-push!

```bash
$ touch file.txt
$ git add .
$ git commit -m "first commit" 
# include useful commit messsages here next time!
$ git push -u origin main # maybe master, depending on config
# after this, "git push" would siffice for pushing to main!
```

## Branching off

```bash
$ git branch test-branch
$ git checkout test-branch

# now that we've swwitched branch, we repeat the add-commit-push steps here, with a slight change
$ git add .
$ git commit -m "first commit on test-branch" 
$ git push -u origin test-branch
```

```
git help
```
List to all the git command
```
git help -a
```
To Access the git guide
```
git help -g
```
git blame

## Table of Content

##### Introduction  
1. What is git ?
2. What is version Control System ?
3. What is centralised and distributed system ?
4. Benefits of the VCS ?

#### Installation
1. How to install the git ?
2. How to configuration the git ?

##### The Basic
1. What is a Repository ?
2. How to Create a git Repository ?  
3. How to track the history of the git ?


what is Merging ?  
How to resolve merging ?

What is conflict ?  
How to resolve conflict ?

- Usage of git help
- Local repository and remote repository
- Push and Pull
- Branching and Merging
- Loging and showng
- Undo/revert/reset
- gitignore


What is cherry-pick


git log --stat

git log -p

git branch -v   




# 3 ways of creating a repository
1. Empty repository.
2. Adding exists working directory to the git.
3. Cloning the central repository.

- A fun metaphor is to think of Git as timeline management utility.



- Introduction
    - What is Version Control System VCS
    - What is distributed and centralised VCS
    - What is git ?
    - Advantages of using git ?
- Getting Started
    - create a git repository
        - git init
        - git clone
        - git config
    - Save files to a repository
        - git add
        - git commit
        - git stash
        - .gitignore
    - Inspecting a repository Reviewing Changes
        - git status
        - git log
    - Undoing the commit and changes
        - git checkout
        - git clean
        - git revert
        - git reset
    - Rewriting history
- Advanced git
    - Branches and merging
        - git branch
        - git checkout
        - git merge
    - Resolving conflict
    - Creating Tags
    - Configuring Text Editor
    - Configuring a Diff and Merge tool
- Misdss
    - deleting a files
    - Renaming a files
    - Moving a files
    - Copying a files
- Working with Remote repository
    - Synch with remote repository
        - git clone
        - git remote
        - git fetch
        - git pull
        - git push


git branch -d deletes a local branch. Use -D instead of -d to force delete a local branch without checking its merge status.

Fixing the Commit Message Before git push

I often notice a typo or a mistake in my commit message after I commit. Luckily, Git has a way to fix this problem.

$ git commit --amend -m 'New commit message'
To bring up the message editor, don’t provide the -m parameter:

$ git commit --amend
Keep in mind that it will not just modify the commit message but also commit any new changes that you might have. This will not work if you have pushed the commit to remote repository.

git merge --abort

git stash - To save changes made when they're not in a state to commit  them to  a repository.

git rebase - Takes a set of commits, copies them and store them outside the repository.

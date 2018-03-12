## Git Branch

Syntax:
```
git branch [options][<BranchName>][<StartPoint>]
```

local > Creating > merging > deleting  
remote > creating > fetching > merging > deleting

Options:

##### Listing Existing Branch
>List all local branches:
```
$ git branch
```
List all remote branches
```
$ git branch -r
```
List all local and remote branches:
```
$ git branch -a
```

##### Creating Branches

>Create a new branch starting at the some point in history as the current branch:
```
$ git branch <branch_name>
```

##### Switching the Branches

> Switch from the current branch to the indicated branch:
```
$ git checkout <branch_name>
```
Create a new branch and switch to it from the current branch:
```
$ git checkout –b NewBranchName StartPoint
```
Note that StartPoint refers to a revision number (or the first 6 characters of such) or an appropriate tag.

#### Deleting the branches

> Delete the feature branch:
```
git branch -d <branch_name>
```

#### Fetching the remote Branches
>

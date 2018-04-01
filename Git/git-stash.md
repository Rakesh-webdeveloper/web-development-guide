#### Stash

What is stash ?
  - Stash the changes in a dirty working directory away.
  - To save changes made when they're not in a state to commit  them to a repository.
  -  Stashing is handy if you need to quickly switch context and work on something else, but you're mid-way through a code change and aren't quite ready to commit.

What is the use of the Stash ?  
 Stashing takes the dirty state of your working directory — that is, your modified tracked files and staged changes — and saves it on a stack of unfinished changes that you can reapply at any time.

When to use the Status ?  
Often, when you’ve been working on part of your project, things are in a messy state and you want to switch branches for a bit to work on something else. The problem is, you don’t want to do a commit of half-done work just so you can get back to this point later. The answer to this issue is the git stash command.

**Note**
- Stash is local to your Git repository; stashes are not transferred to the server when you push.
- By default Git won't stash changes made to untracked or ignored files.

_Save the changes temp and makes working dir clean_
```
git stash
```



#### Re-applying your stashed changes
_Reapply previously stashed changes_  
_Popping your stash removes the changes from your stash and reapplies them to your working copy._
```
git stash pop
```
_Reapply the changes to your working copy and keep them in your stash_  
_This is useful if you want to apply the same stashed changes to multiple branches._
_To apply the recent stash_
```
git stash apply
```
_To apply the older stash_
```
git stash apply stash@{2}
```

#### Stashing untracked or ignored files
By default, running git stash will stash:

- Changes that have been added to your index (staged changes)
- Changes made to files that are currently tracked by Git (unstaged changes)

But it will not stash:

- New files in your working copy that have not yet been staged
files that have been ignored

_Stashing the untracked files_
```
git stash -u
git --include-untracked
```

#### Managing multiple stashes
_To view multiple stash list_
```
git stash list
```
_To annotate your stashes with a description_
```
git stash save "<message>";
```
_Reapply the stash_
```
git stash pop stash@{2}
```

#### Viewing stash diffs
_To view a summary of a stash_
```
git stash show
```
_To view the full diff of a stash_
```
git stash show -p
git stat show --patch
```
#### Partial stashes
You can also choose to stash just a single file, a collection of files, or individual changes from within files. If you pass the -p option (or --patch) to git stash, it will iterate through each changed "hunk" in your working copy and ask whether you wish to stash it.
```
git stash -p
```
You can hit ? for a full list of hunk commands. Commonly useful ones are:

|Command|Description|
|:------------------|
| /	| search for a hunk by regex |
| ? | help |
| n | don't stash this hunk |
| q | quit (any hunks that have already been selected will be stashed) |
| s | split this hunk into smaller hunks |
| y | stash this hunk |
>There is no explicit "abort" command, but hitting CTRL-C(SIGINT) will abort the stash process.

#### Creating a branch from your stash
_To create a branch from a stash_  
```
git stash branch <branch_name>
```
_To create a new branch to apply your stashed perticular changes_
```
git stash branch <branch_name> stash@{<index>}
git stash branch add-stylesheet stash@{1}
```

#### Cleaning up your stash
_To delete all of your stashes_
```
git stash clear
```
_To delete a particular stash_
```
git stash drop stash@{1}
```
_To log the git stash_
```
 git log --oneline --graph stash@{0}
```

#### Un-applying a Stash
_To unapply the older version of the stash_
```
git stash show -p stash@{0} | git apply -R
```
_To unapply the recent version of the stash_
```
git stash show -p | git apply -R
```
Others
git stash apply --index

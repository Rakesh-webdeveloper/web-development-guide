## Git Undo changes

- git checkout
  >    
  - Checking out a specific commit will put the repo in a "detached HEAD" state.
  - This means you are no longer working on any
  - In a detached state, any new commits you make will be orphaned when you change branches back to an established branch.
  - Orphaned commits are up for deletion by Git's garbage collector.
  - The garbage collector runs on a configured interval and permanently destroys orphaned commits.
  - To prevent orphaned commits from being garbage collected, we need to ensure we are on a branch.

- git clean
- git revert
- git reset


#### Undo uncommitted Changes
> _undo an uncommitted changes with git checkout_  
_To  discard changes in the working directory_
```
git checkout -- <file_name/sha-1>
```
_Undo unchanges all the files_
```
git checkout -- .
```
#### Undo Commited Changes
>_Undo using the git reset_
_Commit history is reset to that specified commit_
```
git reset --hard a1e8fb5
```
_Undoing a committed snapshot_
```
git checkout -- <sha-1>
```


_undo a public commit with git revert_

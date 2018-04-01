## Viewing Your Staged and Unstaged Changes
#### git diff
- `git diff` shows you the exact lines added and removed — the patch, as it were.


_To see what you’ve changed but not yet staged, type git diff with no other arguments_
_That command compares what is in your working directory with what is in your staging area. The result tells you the changes you’ve made that you haven’t yet staged._
_only changes that are still unstaged_
```
git diff
```
_To check the stage diff_
_This command compares your staged changes to your last commit_
```
git diff --staged
git diff --cached 
```

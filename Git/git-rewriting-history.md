#### Changing the Last Commit

- `git commit --amend` command is a convenient way to modify the most recent commit.
- It combine staged changes with the previous commit instead of creating an entirely new commit.
- It can also be used to simply edit the previous commit message without changing its snapshot.
- It will be a new entity with its own ref.
- Amended commits are actually entirely new commits and the previous commit will no longer be on your current branch.

#### Change most recent Git commit message
```
git commit --amend
```
_Edit the previous commit’s message without altering its snapshot_
```
git commit --amend -m "<new message"
```
#### Changing committed files
```
git commit --amend --no-edit
```
>The --no-edit flag will allow you to make the amendment to your commit without changing its commit message. The resulting commit will replace the incomplete one, and it will look like we committed the changes to hello.py and main.py in a single snapshot.

#### Changing older or multiple commits



git rebase
git rebase -i
git rebase --continue
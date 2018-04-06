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


#### git reflog
- Reflogs track when Git refs were updated in the local repository.
- By default, git reflog will output the reflog of the HEAD ref
- "ref", which is a pointer to a commit.
- Reflogs are stored in directories under the local repository's .git directory.
- git reflog directories can be found at .git/logs/refs/heads/., .git/logs/HEAD
- .git/logs/refs/stash if the git stash has been used on the repo.
- A special reflog is maintained for the Git stash

```
git reflog
git reflog show HEAD # equivalent to above command
```

git rebase
git rebase -i
git rebase --continue
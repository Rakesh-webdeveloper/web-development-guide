## Remote Repository

##### Showing Your Remotes
_To see which remote servers you have configured_
```
git remote
```
_To see the remote urls that git has stored_
```
git remote -v
```

##### Adding Remote Repositories


##### Delete the remote branches
```
$ git push origin --delete <branch_name>
```


git pull
>git pull does this by doing a git fetch to bring the local copy of the
remote repository up to date, and then merging the changes into your own
code repository and possibly your working copy.
`git pull` pulls down from a remote and instantly merges.
`git pull` will download latest changes from the remote repository and automatically merge those changes in the local repository
`git pull` will merge only into the current working branch


git fetch
>It will just fetch all the changes in the remote repository
It does not merge them with your current branch.

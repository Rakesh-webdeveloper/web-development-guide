# Git Commit (Creating HEAD)

##### Adding to the project history
- The ```git commit``` command commits the staged snapshot to the project history.
- Committed snapshots can be thought of as “safe” versions of a project—Git will never change them unless you explicitly ask it to.

#### Committing Your Changes
_Committing the message inline_
```
git commit -m "<Message>" <file_name>
```
_committing the message on the external Editor_
```
git config --global core.editor <editor_name>
```
#### Skipping the Staging Area
```
git commit -a -m "<Message>" <file_name>
```

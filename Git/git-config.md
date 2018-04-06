#### Git Configuration

- Configuration names are dot delimited strings composed of a 'section' and a 'key' based on their hierarchy.
For example :
```
git config user.email
```
_To set the user name and email address_
```
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

_config the core editor_
```
git config --global core.editor nano
```
_Setting the diff tool_
```
git config --global merge.tool vimdiff
```
_To check the git config value_
```
git config user.name
```

### Git config levels
- --local
- --global
- --system

_Set the config value_

_Delete a config_
```
git config --unset diff.renames
```
_To get the git config value_
```
git config --get core.filemode
git config core.filemode
```

### Aliases
- Aliases save you the time and energy cost of typing frequently used commands.
- Git aliases are stored in Git configuration files.

Examples :
_This example creates a ci alias for the git commit command._
```
git config --global alias.ci commit
```
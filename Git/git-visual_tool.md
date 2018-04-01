## Visual git tool
___

#### Setup git diff tool
`git-difftool` - Show changes using common diff tools

_Copy the modified files to a temporary location and perform a directory diff on them. This mode never prompts before launching the diff tool._
```
git difftool -d/--dir-diff
```
_Do not prompt before launching a diff too_
```
git difftool -y/--no-prompt
```
_List of valid tool_
```
git difftool --tool-help
```
_Set the path for the tool_
```
git config --local mergetool.meld.path "C:\Program Files (x86)\Meld\Meld.exe"
```

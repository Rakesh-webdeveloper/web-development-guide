## Ignoring a files

_ignore all .a files_
```
*.a
```

_but do track lib.a, even though you're ignoring .a files above_
```
!lib.a
```
some example
only ignore the TODO file in the current directory, not subdir/TODO /TODO
# ignore all files in the build/ directory build/
# ignore doc/notes.txt, but not doc/server/arch.txt doc/*.txt
# ignore all .pdf files in the doc/ directory and any of its subdirectories doc/**/*.pdf

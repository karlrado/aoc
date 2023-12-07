Notes

1. Files showing up as modified in VSCode (git extension) when they are not.
   Reference: https://stackoverflow.com/questions/62724723/git-in-visual-studio-code-says-file-is-modified-even-when-there-is-no-change
   Solution is to run `git config --global core.filemode false`.  It seems that this must be done at the global (just in the container)
   level in order for VSCode to see it.  This means that the config change needs to be reapplied whenever the container is rebuilt.

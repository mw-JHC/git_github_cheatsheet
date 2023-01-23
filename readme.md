# This is git and github cheatsheet for me
## If gitignore doesn't work
gitignore sometimes doesn't work because of git cache.  
you can remove git cache with this command  
**git rm -r --cached .**
```console
git rm -r --cached .
git add .
git commit -m "fixed untracked files and git ignore"
git push
```
---
## how to use submodule
Git submodules are used when using Git resources created by other developers  
**git submodule add \<git URL> \<file Path>**

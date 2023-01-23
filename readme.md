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
```console
git submodule add https://github.com/mw-JHC/git_github_cheatsheet catkin_ws/src
```
if you add a some new submodule, git create a file named as .gitsubmodule. you shouldn't modify this file directly.  

### Submodule initiation and update
Even if you add a new Git submodule, the folder will probably be empty. To download submodules, the following command is required.  
```console
git submodule init
git submodule update
```
### Delete Submodule
If you download an unwanted submodule or the download location of a submodule is wrong, you should delete the submodule with the following command instead of just deleting it.  
**git submodule deinit -f \<submodule name>**  
delete the local file of submodule  
**rm -rf .git/module/\<submodule name>**  
delete the file in git  
**git rm -f move_base**  
```console
git submodule deinit -f move_base
rm -rf .git/modules/move_base
git rm -f move_base
```


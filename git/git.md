<h1 style="font-family: Roboto" align="center">
GIT CHEAT SHEET
</h1>

```bash
git init 
```
<p style="font-family: Roboto">
Initiates git in the current directory. 
</p>

```bash
git remote add origin https://github.com/repo_name.git 
```

<p style="font-family: Roboto">
Add remote reposiory. 
</p>

```bash
git clone <address> 
```

<p style="font-family: Roboto">
Creates a git repo from given address (get the address from your git-server). 
</p>

```bash
git clone <address> -b <branch_name> <path/to/directory> 
```

<p style="font-family: Roboto">
Clones a git repo from the address into the given directory and checkout's the given branch. 
</p>

```bash
git clone <address> -b <branch_name> --single-branch 
```

<p style="font-family: Roboto">
Clones a single branch. 
</p>

```bash
git add <file_name> 
```

<p style="font-family: Roboto">
Adds(stages) file.txt to the git. 
</p>

```bash
git add * 
```

<p style="font-family: Roboto">
Adds(stages) all new modifications, deletions, creations to the git. 
</p>

```bash
git reset file.txt 
```

<p style="font-family: Roboto">
Removes file.txt from the stage. 
</p>

```bash
git reset --hard 
```

<p style="font-family: Roboto">
Throws away all your uncommitted changes, hard reset files to HEAD. 
</p>

```bash
git reset --soft <commit_id> 
```

<p style="font-family: Roboto">
Moves the head pointer. 
</p>

```bash
git reset --mixed <commit_id> 
```

<p style="font-family: Roboto">
Moves the head pointer and then copies the files from the commit it is now pointing to the staging area,
 the default when no argument is provided. 
</p>

```bash
git reset -hard <commit_id> 
```

<p style="font-family: Roboto">
Moves the head pointer and then copies the files from the commit it is now pointing to the staging area 
 and working directory thus, throw away all uncommitted changes. 
</p>

```bash
git rm file.txt 
```

<p style="font-family: Roboto">
Removes file.txt both from git and file system. 
</p>

```bash
git rm --cached file.txt 
```

<p style="font-family: Roboto">
Only removes file.txt both from git index. 
</p>

```bash
git status 
```

<p style="font-family: Roboto">
Shows the modifications and stuff that are not staged yet. 
</p>

```bash
git branch 
```

<p style="font-family: Roboto">
Shows all the branches (current branch is shown with a star). 
</p>

```bash
git branch -a 
```

<p style="font-family: Roboto">
Shows all the branches local and remote. 
</p>

```bash
git branch my-branch 
```

<p style="font-family: Roboto">
Creates my-branch. 
</p>

```bash
git branch -d my-branch 
```

<p style="font-family: Roboto">
Deletes my-branch. 
</p>

```bash
git checkout my-branch 
```

<p style="font-family: Roboto">
Switches to my-branch. 
</p>

```bash
git merge my-branch 
```

<p style="font-family: Roboto">
Merges my-branch to current branch. 
</p>

```bash
git push origin --delete my-branch 
```

<p style="font-family: Roboto">
Delete remote branch. 
</p>

```bash
git branch -m <new-branch-name> 
```

<p style="font-family: Roboto">
Rename the branch. 
</p>

```bash
git checkout --orphan <branch_name> 
```

<p style="font-family: Roboto">
Checkout a branch with no commit history. 
</p>

```bash
git branch -vv 
```

<p style="font-family: Roboto">
List all branches and their upstreams, as well as last commit on branch.
</p>

```bash
git branch -a 
```

<p style="font-family: Roboto">
List all local and remote branches. 
</p>

```bash
git cherry-pick <commit_id> 
```

<p style="font-family: Roboto">
Merge the specified commit. 
</p>

```bash
git cherry-pick <commit_id_A>^..<commit_id_B> 
```

<p style="font-family: Roboto">
Pick the entire range of commits where A is older than B ( the ^ is for including A as well ). 
</p>

```bash
git remote 
```

<p style="font-family: Roboto">
Shows the remotes. 
</p>

```bash
git remote -v 
```

<p style="font-family: Roboto">
Shows the remote for pull and push. 
</p>

```bash
git remote add my-remote <address> 
```

<p style="font-family: Roboto">
Creates a remote (get the address from your git-server). 
</p>

```bash
git remote rm my-remote 
```

<p style="font-family: Roboto">
Remove a remote. 
</p>

```bash
git log 
```

<p style="font-family: Roboto">
Shows the log of commits. 
</p>

```bash
git log --no-pager 
```

<p style="font-family: Roboto">
Shows the log of commits without less command. 
</p>

```bash
git log --oneline 
```

<p style="font-family: Roboto">
Shows the log of commits, each commit in a single line. 
</p>

```bash
git log --oneline --graph --decorate 
```

<p style="font-family: Roboto">
Shows the log of commits, each commit in a single line with graph. 
</p>

```bash
git log --since=<time> 
```

<p style="font-family: Roboto">
Shows the log of commits since given time. 
</p>

```bash
git log -n <x> 
```

<p style="font-family: Roboto">
Lists the last x commits. 
</p>

```bash
git log -n <x> --oneline 
```

<p style="font-family: Roboto">
Lists the last x commits, each commit in single line. 
</p>

```bash
git reflog 
```

<p style="font-family: Roboto">
Record when the tips of branches and other references were updated in the local repository. 
</p>

```bash
git ls-files 
```

<p style="font-family: Roboto">
Show information about files in the index and the working tree. 
</p>

```bash
git commit -m "msg"
```

<p style="font-family: Roboto">
Commit changes with a msg. 
</p>

```bash
git commit -m "title" -m "description" 
```

<p style="font-family: Roboto">
Commit changes with a title and description. 
</p>

```bash
git commit --amend           
```

<p style="font-family: Roboto">
Combine staged changes with the previous commit, or edit the previous commit message without changing its snapshot. 
</p>

```bash
git commit --amend --no-edit 
```

<p style="font-family: Roboto">
Amends a commit without changing its commit message. 
</p>

```bash
git commit --amend --author='Author Name <email@address.com>'    
```

<p style="font-family: Roboto">
Amend the author of a commit. 
</p>

```bash
git push my-remote my-branch 
```

<p style="font-family: Roboto">
Pushes the commits to the my-remote in my-branch (does not push the tags).
</p>

```bash
git revert <commit-id>       
```

<p style="font-family: Roboto">
Undo a commit by creating a new commit. 
</p>

```bash
git show                    
```

<p style="font-family: Roboto">
Shows one or more objects (blobs, trees, tags and commits).
</p>

```bash
git diff                     
```

<p style="font-family: Roboto">
Show changes between commits, commit and working tree. 
</p>

```bash
git diff HEAD               
```

<p style="font-family: Roboto">
Show changes between working directory vs last commit. 
</p>

```bash
git diff --staged HEAD    
```

<p style="font-family: Roboto">
Show changes between stage area vs last commit. 
</p>

```bash
it diff --color             
```

<p style="font-family: Roboto">
Show colored diff. 
</p>

```bash
git diff --staged            
```

<p style="font-family: Roboto">
Shows changes staged for commit. 
</p>

```bash
git stash                            
```

<p style="font-family: Roboto">
Stashes the staged and unstaged changes (git status will be clean after it). 
</p>

```bash
git stash -u                         
```

<p style="font-family: Roboto">
Stash everything including new untracked files (but not .gitignore). 
</p>

```bash
git stash save "msg"                 
```

<p style="font-family: Roboto">
Stash with a msg. 
</p>

```bash
git stash list    
```                   

<p style="font-family: Roboto">
List all stashes.
</p>

```bash
git stash pop                        
```

<p style="font-family: Roboto">
Delete the recent stash and applies it. 
</p>

```bash
git stash pop stash@{2}              
```

<p style="font-family: Roboto">
Delete the {2} stash and applies it. 
</p>

```bash
git stash show                       
```

<p style="font-family: Roboto">
Shows the description of stash. 
</p>

```bash
git stash apply      
```                

<p style="font-family: Roboto">
Keep the stash and applies it to the git. 
</p>

```bash
git stash branch my-branch stash@{1} 
```

<p style="font-family: Roboto">
Creates a branch from your stash. 
</p>

```bash
git stash drop stash@{1}             
```

<p style="font-family: Roboto">
Deletes the {1} stash. 
</p>

```bash
git stash clear                      
```

<p style="font-family: Roboto">
Clears all the stash. 
</p>

```bash
git rebase -i <commit_id>         
```

<p style="font-family: Roboto">
Rebase commits from a commit ID. 
</p>

```bash
git rebase --abort            
```

<p style="font-family: Roboto">
Abort a running rebase. 
</p>

```bash
git rebase --continue      
```

<p style="font-family: Roboto">
Continue rebasing after fixing all conflicts.
</p>

```bash
git clean -f             
```

<p style="font-family: Roboto">
Clean untracked files permanently. 
</p>

```bash
git clean -f -d/git clean -fd    
``` 

<p style="font-family: Roboto">
To remove directories permanently. 
</p>

```bash
git clean -f -X/git clean -fX   
```

<p style="font-family: Roboto">
To remove ignored files permanently. 
</p>

```bash
git clean -f -x/git clean -fx     
```

<p style="font-family: Roboto">
To remove ignored and non-ignored files permanently. 
</p>

```bash
git clean -d --dry-run          
```

<p style="font-family: Roboto">
Shows what would be deleted.
</p>

```bash
git config --global --list                   
```

<p style="font-family: Roboto">
Lists the git configuration for all repos. 
</p>

```bash
git config --global --edit                   
```

<p style="font-family: Roboto">
Opens an editor to edit the git config file. 
</p>

```bash
git config --global alias.<handle> <command> 
```

<p style="font-family: Roboto">
Add git aliases to speed up workflow , eg. 
</p>

```bash
git config --global core.editor <editor_name>   
```

<p style="font-family: Roboto">
Config default editor. 
</p>
git branch -M main => because master is no longer preffered  
git commit -am "update" => adds and commits (works after first commit)  
git config --global alias.up "commit -m "update"" => setting alias  
git config --global --edit => opens config file  
git commit --amend -m "amended" => changes message of commit  
git revert HEAD^ - reverts last commit  
git revert 2213bf43 - revert specific commit  
git stash  
git stash pop  
git stash list  
git stash save "alias for stash"  
git stash apply 1 => applies second stash (can apply only one, for applying second, it is needed to commit or stash)  
git reset --soft HEAD^ => uncommits (locally) commited files
git reset HEAD^ => uncommits (localy) **pushed** files and stage them again  
git reset --hard HEAD^ => uncommits (localy) **pushed** files and unstaged them  
git push --force => if there is no commits, just deletes last commit from remote (also from history)  
git rebase => with rebase you say to use another branch as the new base for your work. moves changes from a branch to another but alters the history by moving. using when someone made changes in e.g. main and you want to update (rebase) your base 
the origin branch's starting point. it does not create a merge commit  
git merge [branch-name]  => merges two branches. it also adds all commits to the branch history. history is preserved  
git merge --abort => aborts merge conflict  
git restore . => disacard changes  
git clean -fd => deletes untracked files and directories   
git clean -fx => deletes all untracked (also ignored) files and directories  
for rebase purposes  
git fetch origin fetch data only from origin  
git fetch --all fetch data from all remotes (origin is one of them)  
trying fetch and fetch2
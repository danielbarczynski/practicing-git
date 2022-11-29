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
git merge --abort => aborts merge conflict  
git restore . => disacard changes  
git clean -fd => deletes untracked files from directory  
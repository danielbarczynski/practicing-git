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
git merge [branch-name]  => merges two branches, push needed after this (no changes in history)  
git merge --abort => aborts merge conflict  
git rebase => don't know yet   
git restore . => disacard changes  
git clean -fd => deletes untracked files and directories   
git clean -fx => deletes all untracked (also ignored) files and directories   
some merge  
# Hi!

This is just some stuff... and few notes on what I learnt, following the course.

## Commands etc.

* **`git add <path>`**  
 adds the contents of current path to the index  
 `-v` for verbose

* **`git branch`**
 shows current branches  
 `--color` : show with colors  
 * **`git branch -d <b1>`**  
  deletes a branch b1

* **`git checkout <branchname>`**  
 change aka checkout to that branch

* **`git commit`**  
 commits changes in current index  
 `-a` for interactive [opens vim]  
 `-m` like "`git commit -m 'commit message here'`"

* **`gitk --all`**  
 the git repositiory browser  
 shows a visualization of branches etc

* **`git rebase <branchname>`**  
 basically goes back to the branch specified in branchname and replays all edits made in current (checked out) branch to it and this all happens in the current branch. the old "branchname" branch is unchanged.

* **`git diff <b1> <b2>`**  
 will show diff b/w the two

* **`git merge <b1>`**  
 merges current branch with b1

* **`git reset --hard ORIG_HEAD`**  
 pulls back changes and reverts to the point before last merge

* **`git checkout -b <bname>`**  
 creates a new branch bname and then checks out to it (shorthand)

* **`git stash`**  
 its like a half-a$$ed commit.  
 when you don't want to commit half-done work, just **stash** it. The changes to tracked files get added to a "**stash stack**".  
 this stack can be reapplied later using:-
 * `git stash apply`  
  once stashed you can checkout to other branches and come back and apply as required
 * `git stash list`  
  shows all stashes

* **`git clone <repository:https>`**  
 clone a repository. will ask for username & password.

* **`git push [branch]`**  
 push current commits to the origin/master

* **`git pull [branch]`**  
 pull from the origin/master to current branch
 does a fetch+merge

* **`git fetch [branch]`**  
 gets all the stuff from the branch specified, and makes the changes in your local rep. but does not commit these changes.
 finally, you should merge these two branches.

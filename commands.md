# Hi!

This is just some stuff... and few notes on what I learnt, following the course.

## Commands etc.

* git  add <path>
	adds the contents of current path to the index
	-v for verbose

git branch
	shows current branches
	--color : show with colors
	### git branch -d <b1>
		deletes a branch b1

git checkout <branchname>
	change to that branch

git commit 
	commits changes from current index
	-a for interactive [opens vim]
	-m like "git commit -m 'commit message here'"

gitk --all
	the git repositiory browser
	shows a visualization of branches etc

git rebase <branchname>
	this basically goes back to the branch specified in branchname and replays all edits made in current (checked out) branch
	to it and this all happens in the current branch. the old "branchname" branch is unchanged 

git diff <b1> <b2>
	will show diff b/w the two

git merge <b1>
	merges current branch with b1

git reset --hard ORIG_HEAD
	pulls back changes and reverts to the point before last merge


git checkout -b <bname>
	creates a new branch bname and then checks out to it (shorthand)

git stash
	its like a half-assed commit.
	when you don't want to commit half-done work, just stash it. the changes to tracked files get added to a stash stack.
	this stack can be reapplied later using
		### git stash apply
	once stashed you can checkout to other branches and come back and apply as required
		### git stash list
			shows all stashed
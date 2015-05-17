HI! This is just some stuff and notes on what I learnt from git

This line of text only appears in master branch as of now
## Learnt Stuff:-

git  add <path>
	adds the contents of current path to the index
	-v for verbose

git branch
	shows current branches
	--color : show with colors

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
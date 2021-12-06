Usefull list of commands for git:

| Command  | Description |
|---|---|
| git log master..development | show what commits are in development but not in master |
| git push -u origin newBranch | push a new local branch to remote, similar with --set-upstream |
| git show --pretty="format:" --name-only COMMIT_ID | show changes from a specific commit |
| git branch -a | show all branches, including remote |
| git branch &#124; grep "pattern" &#124; xargs git branch -D | delete all branches that match a pattern |
| git branch -vv  &#124; grep ': gone]'  &#124; awk '{print $1}'  &#124; xargs git branch -D | delete all branches that got removed from remote
| git log --pretty=format:"%ad:%an:%d:%B" --date=short --reverse --all --since=1.month.ago --author=Adrian | what I did last month
| git rebase --whitespace=fix -f <last_good_commit> | undo line ending changes

## Task instructions

1) Create a new GitHub repository.
2) Create a local repository.
3) Add READMD.md.
4) Connect local and remote repositories.
5) Make changes locally and push to remote.
6) Make changes on the remote repository.
7) Make additional changes locally and push.
8) Solve merge conflict.
9) Update the README.md to include steps to resolve merge conflicts.

## Steps to resolve merge conflict

1) Pull changes from remote repository:
`git pull origin <your-branch>`

2) Choose one of the following options:
- Merge (default): Combines the remote changes with your local changes:
`git pull --no-rebase origin <your-branch>`
- Rebase (rewrite history): Applies your local changes on top of the remote ones, keeping the history cleaner but rewriting commits:
`git pull --rebase origin <your-branch>`
- Fast-Forward (no merge or rebase): Only allows a fast-forward if there are no local changes that conflict with the remote branch:
`git pull --ff-only origin <your-branch>`

3) After resolving conflicts, push the changes back to the remote repository:
`git push origin <your-branch>`

## Branch task

1) Create a new branch, do checkout, select created branch
`git checkout -b <new_branch_name>`
2) Make changes and push to the remote:
`git push origin <new_branch_name>`
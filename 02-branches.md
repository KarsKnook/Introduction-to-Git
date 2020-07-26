# Workshop 2
This workshop is intended to familiarise you with branches and remotes in Git.

# branches

1. A branch is an independent line of development in Git (preferably one for each member of a project).
2. Let's start by showing all the branches , in the existing repo ( which oyou should already have if you completed workshop 1).

```git branch -v ```

git branch <username> (create branch)
git log --oneline --decorate (to show SHA-256 commits for branches)
git checkout <username> (switch to branch)

shorthand is git checkout -b <username>

nano username.py
print("<Your GitHub Username>")

python username.py

git cp username.py sandbox/username.py
git rm username.py
git add sandbox/username.py
git commit -m "second commit"
git push origin <username>

git merge master <username>
git add sandbox/username.py
git commit -m "second commit"
git push

git -diff to check conflicts
delete it one and push it (master branch) and modify it in <username> branch

git checkout <username>
git rebase master

-- remotes

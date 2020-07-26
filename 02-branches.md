# Workshop 2
This workshop is intended to familiarise you with branches and remotes in Git.

# branches

1. A branch is an independent line of development in Git (preferably one for each member of a project).
2. Let's start by showing all the branches , in the existing repo ( which you should already have if you completed workshop 1).

```git branch -v ```

3. To create a branch with your username:
```git branch <username> (create branch)```
The following command lists all your SHA-256 commits for a repository:
```git log --oneline --decorate (to show SHA-256 commits for branches)```
In order to switch to the new branch ( the one with your username you just created):
```git checkout <username> (switch to branch)```

This can actually be done in one command as:
```git checkout -b <username>```

4. Create a python file named ```username.py``` (I am using nano , you may wish to use some other IDE like VSCode/PyCharm/Notepad etc.):
```
nano username.py
print("<Your GitHub Username>")
```
You can run it using ```python username.py```. ( It should output your GitHub username).

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

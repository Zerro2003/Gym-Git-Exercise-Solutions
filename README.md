# Git Exercises

# Bundle 1

## Exercise 1

```bash
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git init
Initialized empty Git repository in C:/Users/user/Downloads/Gym-Git-Exercise-Solutions/.git/
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git add README.md
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git commit -m "creating a readme"
[master (root-commit) 3d4d93c] creating a readme
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git remote add origin https://github.com/Zerro2003/Gym-Git-Exercise-Solutions.git
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git branch --show-current
master
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git branch -m main
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 234 bytes | 78.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Zerro2003/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git checkout -b dev
Switched to a new branch 'dev'
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git checkout -b test
Switched to a new branch 'test'
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git checkout dev
Switched to branch 'dev'
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git branch -d test
Deleted branch test (was 3d4d93c).
```

## Exercise 2

```bash
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git add home.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git stash
Saved working directory and index state WIP on dev: f28deca add steps of git commands in README
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git add about.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git stash
Saved working directory and index state WIP on dev: f28deca add steps of git commands in README
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git add team.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git stash
Saved working directory and index state WIP on dev: f28deca add steps of git commands in README
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git stash list
stash@{0}: WIP on dev: f28deca add steps of git commands in README
stash@{1}: WIP on dev: f28deca add steps of git commands in README
stash@{2}: WIP on dev: f28deca add steps of git commands in README
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git stash pop 'stash@{1}'
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (11c27ed41930d360812a34858a7e650cf33f35bf)
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git stash pop 'stash@{1}'
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (cc8cc3a1996fb73ac72b9c1c76052ed7f90d1d4c)
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git commit -m "create new about and home page"
[dev 6054d46] create new about and home page
 2 files changed, 20 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git push origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 505 bytes | 252.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Zerro2003/Gym-Git-Exercise-Solutions.git
   f28deca..6054d46  dev -> dev
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git stash pop 'stash@{0}'
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped stash@{0} (0ba6c2fe3bcc9b938b395e61b0d02283461da526)
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git reset
```

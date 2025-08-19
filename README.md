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

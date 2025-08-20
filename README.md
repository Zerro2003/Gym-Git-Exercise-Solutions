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

# Bundle 2

## Exercise 1

```bash
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git branch ft/bundle-2
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git checkout ft/bundle-2
Switched to branch 'ft/bundle-2'
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git add services.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git commit -m "add services page"
[ft/bundle-2 6eb5d26] add services page
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 services.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git push origin ft/bundle-2
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 16 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (7/7), 819 bytes | 204.00 KiB/s, done.
Total 7 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To https://github.com/Zerro2003/Gym-Git-Exercise-Solutions.git
   2e019f4..6eb5d26  ft/bundle-2 -> ft/bundle-2
```

```bash
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git pull origin main
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 889 bytes | 68.00 KiB/s, done.
From https://github.com/Zerro2003/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
   3d4d93c..0474631  main       -> origin/main
Updating 3d4d93c..0474631
Fast-forward
 README.md     | 120 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 about.html    |  10 +++++
 home.html     |  10 +++++
 services.html |   0
 team.html     |  10 +++++
 5 files changed, 150 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 services.html
 create mode 100644 team.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git add services.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git commit -m "new feature in services page"
[ft/service-redesign 67bd2a4] new feature in services page
 1 file changed, 10 insertions(+)
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git push origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 428 bytes | 428.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Zerro2003/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/Zerro2003/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git add services.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git commit -m "edit the services page"
[main a599d58] edit the services page
 1 file changed, 10 insertions(+)
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 422 bytes | 422.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Zerro2003/Gym-Git-Exercise-Solutions.git
   0474631..a599d58  main -> main
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git diff main..ft/service-redesign
diff --git a/services.html b/services.html
index 44978dd..cc45107 100644
--- a/services.html
+++ b/services.html
@@ -5,6 +5,6 @@
     <title>Document</title>
   </head>
   <body>
-    <p>new changes in main</p>
...skipping...

                   SUMMARY OF LESS COMMANDS

      Commands marked with * may be preceded by a number, N.
      Notes in parentheses indicate the behavior if N is given.
      A key preceded by a caret indicates the Ctrl key; thus ^K is ctrl-K.

  h  H                 Display this help.
  q  :q  Q  :Q  ZZ     Exit.
HELP -- Press RETURN for more, or q when done...skipping...
diff --git a/services.html b/services.html
index 44978dd..cc45107 100644
--- a/services.html
+++ b/services.html
@@ -5,6 +5,6 @@
     <title>Document</title>
   </head>
   <body>
-    <p>new changes in main</p>
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git add services.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git commit -m "resolve conflict in marge and ft/service-redesign"
[ft/service-redesign 2cf512b] resolve conflict in marge and ft/service-redesign
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git push origin ft/service-redesign
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 240 bytes | 240.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Zerro2003/Gym-Git-Exercise-Solutions.git
   67bd2a4..2cf512b  ft/service-redesign -> ft/service-redesign
```

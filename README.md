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

# Bundle 3

## Exercise 1

```bash
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git add team.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git commit -m "add team page"
[ft/team-page 65f818f] add team page
 1 file changed, 14 insertions(+)
 create mode 100644 team.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git push origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 452 bytes | 150.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Zerro2003/Gym-Git-Exercise-Solutions/pull/new/ft/team-pag
remote:
To https://github.com/Zerro2003/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
65f818f (HEAD -> ft/team-page, origin/ft/team-page) add team page
13073f0 (origin/main, main, ft/contact-page) delete team
a599d58 edit the services page
0474631 Merge pull request #2 from Zerro2003/ft/bundle-2
1d47264 (origin/ft/bundle-2, ft/bundle-2) updating README
:
65f818f (HEAD -> ft/team-page, origin/ft/team-page) add team page
13073f0 (origin/main, main, ft/contact-page) delete team
a599d58 edit the services page
0474631 Merge pull request #2 from Zerro2003/ft/bundle-2
1d47264 (origin/ft/bundle-2, ft/bundle-2) updating README
~
~
~
~
(END)
65f818f (HEAD -> ft/team-page, origin/ft/team-page) add team page
13073f0 (origin/main, main, ft/contact-page) delete team
a599d58 edit the services page
0474631 Merge pull request #2 from Zerro2003/ft/bundle-2
1d47264 (origin/ft/bundle-2, ft/bundle-2) updating README
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git chekout ft/contact-page
git: 'chekout' is not a git command. See 'git --help'.

The most similar command is
        checkout
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git checkout ft/contact-page
Switched to branch 'ft/contact-page'
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git cherry-pick 65f818f (HEAD -> ft/team-page, origin/ft/team-page) add team page
HEAD : The term 'HEAD' is not recognized as
the name of a cmdlet, function, script
file, or operable program. Check the
spelling of the name, or if a path was
included, verify that the path is correct
and try again.
At line:1 char:26
+ git cherry-pick 65f818f (HEAD ->
ft/team-page, origin/ft/team-page) a ...
+                          ~~~~
    + CategoryInfo          : ObjectNotFoun
   d: (HEAD:String) [], CommandNotFoundExc
  eption
   ndException
   ndException

PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git cherry-pick 65f818f
[ft/contact-page ad1dc15] add team page
 Date: Thu Aug 21 10:49:49 2025 +0200
 1 file changed, 14 insertions(+)
 create mode 100644 team.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git add contact.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git commit -m "Add contact page"
[ft/contact-page 555cae2] Add contact page
 1 file changed, 10 insertions(+)
 create mode 100644 contact.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git push origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 16 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 826 bytes | 826.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote:
To https://github.com/Zerro2003/Gym-Git-Exercise-Solutions.git
remote:
To https://github.com/Zerro2003/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git add faq.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git commit -m "Add faq page for Q&A"
[ft/faq-page 0560ec5] Add faq page for Q&A
 1 file changed, 10 insertions(+)
 create mode 100644 faq.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 439 bytes | 439.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Zerro2003/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/Zerro2003/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git revert 65f818f --no-edit
[ft/faq-page 0672d99] Revert "add team page"
 Date: Thu Aug 21 11:25:07 2025 +0200
 1 file changed, 14 deletions(-)
 delete mode 100644 team.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git push origin ft/faq-page
Enumerating objects: 3, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Zerro2003/Gym-Git-Exercise-Solutions.git
   0560ec5..0672d99  ft/faq-page -> ft/faq-page
```

# Bundle 4

## Exercise 1

```bash
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git remote add git-copy https://github.com/Zerro2003/before-delete.git
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git add home.html
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git commit -m "changed few things in home page"
[main f7d7026] changed few things in home page
 1 file changed, 1 insertion(+)
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 345 bytes | 345.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Zerro2003/Gym-Git-Exercise-Solutions.git
   7a4cadb..f7d7026  main -> main
PS C:\Users\user\Downloads\Gym-Git-Exercise-Solutions> git push git-copy main
Enumerating objects: 39, done.
Counting objects: 100% (39/39), done.
Delta compression using up to 16 threads
Compressing objects: 100% (35/35), done.
Writing objects: 100% (39/39), 5.37 KiB | 917.00 KiB/s, done.
Total 39 (delta 17), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (17/17), done.
To https://github.com/Zerro2003/before-delete.git
 * [new branch]      main -> main
```

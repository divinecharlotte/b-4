# g-exercesises

### BUNDLE1

## EXERCESISE1

```

admin-MacBook-Pro:~ $ cd Desktop/
admin-MacBook-Pro:Desktop $ cd gym/
admin-MacBook-Pro:gym $ git clone https://github.com/divinecharlotte/g-exercesises.git
Cloning into 'g-exercesises'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
admin-MacBook-Pro:gym $ cd g-exercesises/
admin-MacBook-Pro:g-exercesises $ code .
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "Bundle1 exercesise1"
[main 5c9a1c9] Bundle1 exercesise1
 1 file changed, 11 insertions(+)
 create mode 100644 index.html
admin-MacBook-Pro:g-exercesises $ git checkout -b dev
Switched to a new branch 'dev'
admin-MacBook-Pro:g-exercesises $ git checkout -b test
Switched to a new branch 'test'
admin-MacBook-Pro:g-exercesises $ git checkout dev
Switched to branch 'dev'
admin-MacBook-Pro:g-exercesises $ git branch -d test
Deleted branch test (was 5c9a1c9).
admin-MacBook-Pro:g-exercesises $
```

### EXERCESISE2

```
admin-MacBook-Pro:g-exercesises $ git stash list
stash@{0}: On dev: stash team.html
stash@{1}: On dev: stash about.html
stash@{2}: On dev: stash home.html
admin-MacBook-Pro:g-exercesises $ git stash pop stash@{X}
stash@{X} is not a valid reference
admin-MacBook-Pro:g-exercesises $ git stash pop stash@{2}
Already up to date!
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        home.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped stash@{2} (44272dc236832190701eb24c48b7ad6a64579f7d)
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "bundle1 exercesise2"
[dev 66edfd6] bundle1 exercesise2
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 home.html
admin-MacBook-Pro:g-exercesises $ git push origin dev
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 313 bytes | 313.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/divinecharlotte/g-exercesises.git
   0114d68..66edfd6  dev -> dev
admin-MacBook-Pro:g-exercesises $ git stash pop stash@{0}
Already up to date!
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        team.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped stash@{0} (bdbf0abe2037ba99466530d7025997c01088f1e2)
admin-MacBook-Pro:g-exercesises $ git log --oneline
66edfd6 (HEAD -> dev, origin/dev) bundle1 exercesise2
0114d68 bundle1 exercesise1
5c9a1c9 (main) Bundle1 exercesise1
ed3be8e (origin/main, origin/HEAD) Initial commit
admin-MacBook-Pro:g-exercesises $ git reset --hard 66edfd6
HEAD is now at 66edfd6 bundle1 exercesise2
admin-MacBook-Pro:g-exercesises $
```

## BUNDLE2

### EXERCESISE1

```
admin-MacBook-Pro:g-exercesises $ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "bundle2 exercesise1"
[ft/bundle-2 48a1791] bundle2 exercesise1
 1 file changed, 11 insertions(+)
 create mode 100644 services.html
admin-MacBook-Pro:g-exercesises $ git push origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 423 bytes | 423.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/divinecharlotte/g-exercesises/pull/new/ft/bundle-2
remote:
To https://github.com/divinecharlotte/g-exercesises.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
admin-MacBook-Pro:g-exercesises $
```

### EXERCESISE2

````
admin-MacBook-Pro:g-exercesises $ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
admin-MacBook-Pro:g-exercesises $ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "bundle2 exercesise2"
[ft/service-redesign f746b2b] bundle2 exercesise2
 1 file changed, 11 insertions(+)
 create mode 100644 service.html
admin-MacBook-Pro:g-exercesises $ git push
admin-MacBook-Pro:g-exercesises $ git push origin ft/service-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 468 bytes | 468.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/divinecharlotte/g-exercesises/pull/new/ft/service-redesign
remote:
To https://github.com/divinecharlotte/g-exercesises.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
admin-MacBook-Pro:g-exercesises $ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "bundle2 exercesise2 on main"
[main 9c9271b] bundle2 exercesise2 on main
 1 file changed, 11 insertions(+)
 create mode 100644 service.html
admin-MacBook-Pro:g-exercesises $ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), done.
From https://github.com/divinecharlotte/g-exercesises
   ed3be8e..4eac444  main       -> origin/main
Merge made by the 'recursive' strategy.
 README.md | 87 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-
 home.html |  0
 team.html |  0
 3 files changed, 86 insertions(+), 1 deletion(-)
 create mode 100644 home.html
 create mode 100644 team.html
admin-MacBook-Pro:g-exercesises $ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 770 bytes | 770.00 KiB/s, done.
Total 5 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/divinecharlotte/g-exercesises.git
   4eac444..06b7aea  main -> main
admin-MacBook-Pro:g-exercesises $ ft/service-redesign
bash: ft/service-redesign: No such file or directory
admin-MacBook-Pro:g-exercesises $ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
admin-MacBook-Pro:g-exercesises $ git diff main
diff --git a/README.md b/README.md
index 12ccf78..640de47 100644
--- a/README.md
+++ b/README.md
@@ -1,86 +1 @@
-# g-exercesises
-
-### BUNDLE1
-
-## EXERCESISE1
-
-```
-
-admin-MacBook-Pro:~ $ cd Desktop/
-admin-MacBook-Pro:Desktop $ cd gym/
-admin-MacBook-Pro:gym $ git clone https://github.com/divinecharlotte/g-exercesises.git
-Cloning into 'g-exercesises'...
-remote: Enumerating objects: 3, done.
-remote: Counting objects: 100% (3/3), done.
-remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
-Unpacking objects: 100% (3/3), done.
-admin-MacBook-Pro:gym $ cd g-exercesises/
-admin-MacBook-Pro:g-exercesises $ code .
-admin-MacBook-Pro:g-exercesises $ git add .
-admin-MacBook-Pro:g-exercesises $ git commit -m "Bundle1 exercesise1"
-[main 5c9a1c9] Bundle1 exercesise1
- 1 file changed, 11 insertions(+)
- create mode 100644 index.html
-admin-MacBook-Pro:g-exercesises $ git checkout -b dev
-Switched to a new branch 'dev'
-admin-MacBook-Pro:g-exercesises $ git checkout -b test
-Switched to a new branch 'test'
-admin-MacBook-Pro:g-exercesises $ git checkout dev
-Switched to branch 'dev'
-admin-MacBook-Pro:g-exercesises $ git branch -d test
-Deleted branch test (was 5c9a1c9).
-admin-MacBook-Pro:g-exercesises $
-```
-
-### EXERCESISE2
-
-```
-admin-MacBook-Pro:g-exercesises $ git stash list
-stash@{0}: On dev: stash team.html
-stash@{1}: On dev: stash about.html
-stash@{2}: On dev: stash home.html
-admin-MacBook-Pro:g-exercesises $ git stash pop stash@{X}
-stash@{X} is not a valid reference
-admin-MacBook-Pro:g-exercesises $ git stash pop stash@{2}
-Already up to date!
-On branch dev
-Untracked files:
-  (use "git add <file>..." to include in what will be committed)
-
-        home.html
-
-nothing added to commit but untracked files present (use "git add" to track)
-Dropped stash@{2} (44272dc236832190701eb24c48b7ad6a64579f7d)
-admin-MacBook-Pro:g-exercesises $ git add .
-admin-MacBook-Pro:g-exercesises $ git commit -m "bundle1 exercesise2"
-[dev 66edfd6] bundle1 exercesise2
- 1 file changed, 0 insertions(+), 0 deletions(-)
- create mode 100644 home.html
-admin-MacBook-Pro:g-exercesises $ git push origin dev
-Enumerating objects: 4, done.
-Counting objects: 100% (4/4), done.
-Delta compression using up to 4 threads
-Compressing objects: 100% (2/2), done.
-Writing objects: 100% (3/3), 313 bytes | 313.00 KiB/s, done.
-Total 3 (delta 0), reused 0 (delta 0)
-To https://github.com/divinecharlotte/g-exercesises.git
-   0114d68..66edfd6  dev -> dev
-admin-MacBook-Pro:g-exercesises $ git stash pop stash@{0}
-Already up to date!
-On branch dev
-Untracked files:
-  (use "git add <file>..." to include in what will be committed)
-
-        team.html
-
-nothing added to commit but untracked files present (use "git add" to track)
-Dropped stash@{0} (bdbf0abe2037ba99466530d7025997c01088f1e2)
-admin-MacBook-Pro:g-exercesises $ git log --oneline
-66edfd6 (HEAD -> dev, origin/dev) bundle1 exercesise2
-0114d68 bundle1 exercesise1
:
Your branch is up to date with 'origin/main'.
admin-MacBook-Pro:g-exercesises $ git merge ft/service-redesign
Auto-merging service.html
CONFLICT (add/add): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git checkout git merge ft/service-redesign
error: pathspec 'git' did not match any file(s) known to git
error: pathspec 'merge' did not match any file(s) known to git
error: pathspec 'ft/service-redesign' did not match any file(s) known to git
admin-MacBook-Pro:g-exercesises $ git checkout ft/service-re
design
Switched to branch 'ft/service-redesign'
admin-MacBook-Pro:g-exercesises $ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
admin-MacBook-Pro:g-exercesises $ git pull main
fatal: 'main' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
admin-MacBook-Pro:g-exercesises $ git pull
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (2/2), done.
From https://github.com/divinecharlotte/g-exercesises
   06b7aea..c05af45  main       -> origin/main
Updating 06b7aea..c05af45
Fast-forward
 services.html | 11 +++++++++++
 1 file changed, 11 insertions(+)
 create mode 100644 services.html
admin-MacBook-Pro:g-exercesises $ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
admin-MacBook-Pro:g-exercesises $ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
admin-MacBook-Pro:g-exercesises $ git checkout ft/bundle-2
Switched to branch 'ft/bundle-2'
admin-MacBook-Pro:g-exercesises $
````

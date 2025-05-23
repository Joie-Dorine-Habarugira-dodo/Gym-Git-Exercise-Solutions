# GIT Exercises

## Bundle 1

### Exercise 1

```bash
hp@Dorine MINGW64 /c/users/hp/git-exercises (master)
$ git init
Reinitialized existing Git repository in C:/Users/hp/git-exercises/.git/

hp@Dorine MINGW64 /c/users/hp/git-exercises (master)
$ git branch -M main

hp@Dorine MINGW64 /c/users/hp/git-exercises (main)
$ git add .

hp@Dorine MINGW64 /c/users/hp/git-exercises (main)
$ git commit -m "added files"
[main (root-commit) 026a696] added files
 1 file changed, 18 insertions(+)
 create mode 100644 index.html

hp@Dorine MINGW64 /c/users/hp/git-exercises (main)
$ git remote add origin git@github.com:Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions.git

hp@Dorine MINGW64 /c/users/hp/git-exercises (main)
$ git status
On branch main
nothing to commit, working tree clean

hp@Dorine MINGW64 /c/users/hp/git-exercises (main)
$ git push origin main
The authenticity of host 'github.com (20.87.245.0)' can't be established.
ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
This key is not known by any other names.     
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository. 

Please make sure you have the correct access rights
and the repository exists.

hp@Dorine MINGW64 /c/users/hp/git-exercises (main)
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main       

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


hp@Dorine MINGW64 /c/users/hp/git-exercises (main)
$  git push --set-upstream origin main
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository. 

Please make sure you have the correct access rights
and the repository exists.

hp@Dorine MINGW64 /c/users/hp/git-exercises (main)
$ git config user.name
Joie-Dorine-Habarugira-dodo

hp@Dorine MINGW64 /c/users/hp/git-exercises (main)
$  git push origin main
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository. 

Please make sure you have the correct access rights
and the repository exists.

hp@Dorine MINGW64 /c/users/hp/git-exercises (main)
$ git remote
origin

hp@Dorine MINGW64 /c/users/hp/git-exercises (main)
$ git remote rm origin

hp@Dorine MINGW64 /c/users/hp/git-exercises (main)
$ git remote add origin https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions.git

hp@Dorine MINGW64 /c/users/hp/git-exercises (main)
$ git push origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 12 threads      
Compressing objects: 100% (2/2), done.        
Writing objects: 100% (3/3), 535 bytes | 178.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main

hp@Dorine MINGW64 /c/users/hp/git-exercises (main)
$ git branch -b dev
error: unknown switch `b'
usage: git branch [<options>] [-r | -a] [--merged] [--no-merged]
   or: git branch [<options>] [-f] [--recurse-submodules] <branch-name> [<start-point>]     
   or: git branch [<options>] [-l] [<pattern>...]
   or: git branch [<options>] [-r] (-d | -D) <branch-name>...
   or: git branch [<options>] (-m | -M) [<old-branch>] <new-branch>
   or: git branch [<options>] (-c | -C) [<old-branch>] <new-branch>
   or: git branch [<options>] [-r | -a] [--points-at]
   or: git branch [<options>] [-r | -a] [--format]

Generic options
    -v, --[no-]verbose    show hash and subject, give twice for upstream branch
    -q, --[no-]quiet      suppress informational messages
    -t, --[no-]track[=(direct|inherit)]       
                          set branch tracking configuration
    -u, --[no-]set-upstream-to <upstream>     
                          change the upstream info
    --[no-]unset-upstream unset the upstream info
    --[no-]color[=<when>] use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --[no-]abbrev[=<n>]   use <n> digits to display object names

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --[no-]delete     delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --[no-]move       move/rename a branch and its reflog
    -M                    move/rename a branch, even if target exists
    --[no-]omit-empty     do not output a newline after empty formatted refs
    -c, --[no-]copy       copy a branch and its reflog
    -C                    copy a branch, even if target exists
    -l, --[no-]list       list branch names   
    --[no-]show-current   show current branch name
    --[no-]create-reflog  create the branch's reflog
    --[no-]edit-description
                          edit the description for the branch
    -f, --[no-]force      force creation, move/rename, deletion
    --merged <commit>     print only branches that are merged
    --no-merged <commit>  print only branches that are not merged
    --[no-]column[=<style>]
                          list branches in columns
    --[no-]sort <key>     field name to sort on
    --[no-]points-at <object>
                          print only branches of the object
    -i, --[no-]ignore-case
                          sorting and filtering are case insensitive
    --[no-]recurse-submodules
                          recurse through submodules
    --[no-]format <format>
                          format to use for the output


hp@Dorine MINGW64 /c/users/hp/git-exercises (main)
$ git checkout -b dev
Switched to a new branch 'dev'

hp@Dorine MINGW64 /c/users/hp/git-exercises (dev)
$ git status
On branch dev
nothing to commit, working tree clean

hp@Dorine MINGW64 /c/users/hp/git-exercises (dev)
$ git push origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev

hp@Dorine MINGW64 /c/users/hp/git-exercises (dev)
$ git checkout -b test
Switched to a new branch 'test'

hp@Dorine MINGW64 /c/users/hp/git-exercises (test)
$ git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions/pull/new/test
remote:
To https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions.git
 * [new branch]      test -> test

hp@Dorine MINGW64 /c/users/hp/git-exercises (test)
$ git checkout dev
Switched to branch 'dev'

hp@Dorine MINGW64 /c/users/hp/git-exercises (dev)
$ git branch -
fatal: '-' is not a valid branch name
hint: See `man git check-ref-format`
hint: Disable this message with "git config advice.refSyntax false"

hp@Dorine MINGW64 /c/users/hp/git-exercises (dev)
$ git branch -D test
Deleted branch test (was 026a696).

hp@Dorine MINGW64 /c/users/hp/git-exercises (dev)
$ git push origin --delete test
To https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions.git
 - [deleted]         test
```

### Exercise 2
```bash
hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git add home.html

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git stash list

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git stash
Saved working directory and index state WIP on dev: 8e539de added README file

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ touch about.html

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git add about.html

hp@Dorine MINGW64 ~/git-exercises (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html


hp@Dorine MINGW64 ~/git-exercises (dev)
$ git stash
Saved working directory and index state WIP on dev: 8e539de added README file

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git stash list
stash@{0}: WIP on dev: 8e539de added README file
stash@{1}: WIP on dev: 8e539de added README file

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ touch team.html

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git add team.html

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html


hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git stash
Saved working directory and index state WIP on dev: 8e539de added README file

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git stash list
stash@{0}: WIP on dev: 8e539de added README file
stash@{1}: WIP on dev: 8e539de added README file
stash@{2}: WIP on dev: 8e539de added README file

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (87dc6e98885fe944e5c294857cdc206555e3112b)

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git stash list
stash@{0}: WIP on dev: 8e539de added README file
stash@{1}: WIP on dev: 8e539de added README file

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (00bde07de7cf4e9a340715d091acdd7a1a4ee004)

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git stash list
stash@{0}: WIP on dev: 8e539de added README file

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html


hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git commit -m "restored about and home file"
[dev 5f1e1ec] restored about and home file
 2 files changed, 22 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev        

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git push origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads      
Compressing objects: 100% (4/4), done.        
Writing objects: 100% (4/4), 614 bytes | 614.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.   
To https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions.git
   8e539de..5f1e1ec  dev -> dev

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git stash list
stash@{0}: WIP on dev: 8e539de added README file

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git stash pop stash@{0}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (146886f099f2908daa4ad109fd1d97e1358d4a07)

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git reset --hard
HEAD is now at 5f1e1ec restored about and home file

hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git status
On branch dev
nothing to commit, working tree clean
```

## Bundle 2

### Exercise 1

```bash
hp@Dorine MINGW64 ~/git-exercises (dev)       
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

hp@Dorine MINGW64 ~/git-exercises (ft/bundle-2)
$ touch services.html

hp@Dorine MINGW64 ~/git-exercises (ft/bundle-2)
$ git add service.html
fatal: pathspec 'service.html' did not match any files

hp@Dorine MINGW64 ~/git-exercises (ft/bundle-2)
$ git add services.html

hp@Dorine MINGW64 ~/git-exercises (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   services.html


hp@Dorine MINGW64 ~/git-exercises (ft/bundle-2)
$ git commit -m "created a services file"
[ft/bundle-2 6e0fb8c] created a services file
 1 file changed, 11 insertions(+)
 create mode 100644 services.html

hp@Dorine MINGW64 ~/git-exercises (ft/bundle-2)
$ git push origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads      
Compressing objects: 100% (3/3), done.        
Writing objects: 100% (3/3), 475 bytes | 475.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
```

### Exercise 2
 
```bash
hp@Dorine MINGW64 ~/git-exercises (ft/bundle-2)
$ git checkout main
Switched to branch 'main'

hp@Dorine MINGW64 ~/git-exercises (main)      
$ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.   
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 922 bytes | 153.00 KiB/s, done.
From https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions
   026a696..40c8358  main       -> origin/main
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> main


hp@Dorine MINGW64 ~/git-exercises (main)
$ git pull
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 1 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 1.80 KiB | 367.00 KiB/s, done.
From https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions
   40c8358..7afc28b  main                 -> origin/main
 * [new branch]      revert-2-ft/bundle-2 -> origin/revert-2-ft/bundle-2
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> main


hp@Dorine MINGW64 ~/git-exercises (main)
$ $ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 922 bytes | 153.00 KiB/s, done.
From https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions
   026a696..40c8358  main       -> origin/main
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

    git branch --set-upstream-to=origin/<branch> mainch you can do so with:
bash: $: command not found
bash: remote:: command not found
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `('
bash: From: command not found
bash: origin/main: No such file or directory
bash: There: command not found
bash: Please: command not found
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `<'
bash: If: command not found
bash: branch: No such file or directory       

hp@Dorine MINGW64 ~/git-exercises (main)      
$ git pull origin main
From https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD 
Updating 026a696..7afc28b
Fast-forward

hp@Dorine MINGW64 ~/git-exercises (main)      
$ git pull origin ft/bundle-2
From https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions
 * branch            ft/bundle-2 -> FETCH_HEAD
Already up to date.

hp@Dorine MINGW64 ~/git-exercises (main)      
$ git branch
  dev
  ft/bundle-2
* main

hp@Dorine MINGW64 ~/git-exercises (main)      
$ git log --oneline --graph --all
*   7afc28b (HEAD -> main, origin/main) Merge pull request #3 from Joie-Dorine-Habarugira-dodo/revert-2-ft/bundle-2
|\  
| * 7132d41 (origin/revert-2-ft/bundle-2) Revert "Added a service page for the project"     
|/  
*   40c8358 Merge pull request #2 from Joie-Dorine-Habarugira-dodo/ft/bundle-2
|\
| | * 249fd5c (ft/bundle-2) Updated the README file
| |/
| * 6e0fb8c (origin/ft/bundle-2) created a services file
| * 62a21af (origin/dev, dev) finished exercise 2
| * 5f1e1ec restored about and home file      
| * 8e539de added README file
|/
* 026a696 added files
(END)
|\
| | * 249fd5c (ft/bundle-2) Updated the README file
| |/
| * 6e0fb8c (origin/ft/bundle-2) created a services file
| * 62a21af (origin/dev, dev) finished exercise 2
| * 5f1e1ec restored about and home file      
| * 8e539de added README file
|/
* 026a696 added files
(END)
*   7afc28b (HEAD -> main, origin/main) Merge pull request #3 from Joie-Dorine-Habarugira-dodo/revert-2-ft/bundle-2
|\
| * 7132d41 (origin/revert-2-ft/bundle-2) Revert "Added a service page for the project"     
|/
*   40c8358 Merge pull request #2 from Joie-Dorine-Habarugira-dodo/ft/bundle-2
*   7afc28b (HEAD -> main, origin/main) Merge pull request #3 from Joie-Dorine-Habarugira-dodo/revert-2-ft/bundle-2
|\
| * 7132d41 (origin/revert-2-ft/bundle-2) Revert "Added a service page for the project"     
|/
*   40c8358 Merge pull request #2 from Joie-Dorine-Habarugira-dodo/ft/bundle-2
*   7afc28b (HEAD -> main, origin/main) Merge pull request #3 from Joie-Dorine-Habarugira-dodo/revert-2-ft/bundle-2
|\
| * 7132d41 (origin/revert-2-ft/bundle-2) Revert "Added a service page for the project"     
|/
*   40c8358 Merge pull request #2 from Joie-Dorine-Habarugira-dodo/ft/bundle-2
|\
| | * 249fd5c (ft/bundle-2) Updated the README file
| |/
| * 6e0fb8c (origin/ft/bundle-2) created a services file
| * 62a21af (origin/dev, dev) finished exercise 2
| * 5f1e1ec restored about and home file      
| * 8e539de added README file
|/
* 026a696 added files
(END)
|\
| | * 249fd5c (ft/bundle-2) Updated the README file
| |/
| * 6e0fb8c (origin/ft/bundle-2) created a services file
| * 62a21af (origin/dev, dev) finished exercise 2
| * 5f1e1ec restored about and home file      
| * 8e539de added README file
|/
* 026a696 added files

hp@Dorine MINGW64 ~/git-exercises (main)      
$ git checkout 249fd5c -- .

hp@Dorine MINGW64 ~/git-exercises (main)      
$ git add .

hp@Dorine MINGW64 ~/git-exercises (main)      
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

hp@Dorine MINGW64 ~/git-exercises (ft/service-redesign)
$ git add .

hp@Dorine MINGW64 ~/git-exercises (ft/service-redesign)
$ git commit -m "added changes to the service page"
[ft/service-redesign 22b2544] added changes to the service page
 4 files changed, 438 insertions(+)
 create mode 100644 README.md
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 services.html

hp@Dorine MINGW64 ~/git-exercises (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads      
Compressing objects: 100% (6/6), done.        
Writing objects: 100% (6/6), 3.83 KiB | 784.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.   
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign

hp@Dorine MINGW64 ~/git-exercises (ft/service-redesign)
$ git checkout main
Switched to branch 'main'

hp@Dorine MINGW64 ~/git-exercises (main)      
$ git add .

hp@Dorine MINGW64 ~/git-exercises (main)      
$ git commit -m "retrieving files"
[main 278a7c9] retrieving files
 5 files changed, 448 insertions(+)
 create mode 100644 README.md
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 services.html
 create mode 100644 team.html

hp@Dorine MINGW64 ~/git-exercises (main)      
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main       

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


hp@Dorine MINGW64 ~/git-exercises (main)      
$ git push --set-upstream origin main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 12 threads      
Compressing objects: 100% (7/7), done.        
Writing objects: 100% (7/7), 3.64 KiB | 466.00 KiB/s, done.
Total 7 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), done.   
To https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions.git
   7afc28b..278a7c9  main -> main
branch 'main' set up to track 'origin/main'.  

hp@Dorine MINGW64 ~/git-exercises (main)      
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

$ git merge main
Auto-merging about.html
$ git merge main
Auto-merging about.html
$ git merge main
Auto-merging about.html
CONFLICT (add/add): Merge conflict in about.html
Auto-merging services.html
Auto-merging services.html
CONFLICT (add/add): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

hp@Dorine MINGW64 ~/git-exercises (ft/service-redesign|MERGING)
$ git add .

hp@Dorine MINGW64 ~/git-exercises (ft/service-redesign|MERGING)
$ git commit -m "merged to main"
[ft/service-redesign 5be0044] merged to main

hp@Dorine MINGW64 ~/git-exercises (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads      
Compressing objects: 100% (3/3), done.        
Writing objects: 100% (3/3), 350 bytes | 175.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions.git
   22b2544..5be0044  ft/service-redesign -> ft/service-redesign
```

## Bundle 3

### Exercise 1

```bash
hp@Dorine MINGW64 ~/git-exercises (ft/service-redesign)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

hp@Dorine MINGW64 ~/git-exercises (ft/team-page)
$ touch team.html

hp@Dorine MINGW64 ~/git-exercises (ft/team-page)
$ git add team.html

hp@Dorine MINGW64 ~/git-exercises (ft/team-page)
$ git commit -m "added a paragraph to the team page"
[ft/team-page 3d9b384] added a paragraph to the team page
 1 file changed, 6 insertions(+)

hp@Dorine MINGW64 ~/git-exercises (ft/team-page)
$ git push origin ft/team-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads      
Compressing objects: 100% (3/3), done.        
Writing objects: 100% (3/3), 1.07 KiB | 1.07 MiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page

hp@Dorine MINGW64 ~/git-exercises (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'. 

hp@Dorine MINGW64 ~/git-exercises (main)      
$ git chekcout -b ft/contact-page
git: 'chekcout' is not a git command. See 'git --help'.

The most similar command is
        checkout

hp@Dorine MINGW64 ~/git-exercises (main)      
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

hp@Dorine MINGW64 ~/git-exercises (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'

hp@Dorine MINGW64 ~/git-exercises (ft/team-page)
$ git log
commit 3d9b384f2f1b6cda3dd3b3464e7ce3cb84c86593 (HEAD -> ft/team-page, origin/ft/team-page) 
Author: Joie-Dorine-Habarugira-dodo <joiedorine.habarugira22a@kepler.org>
Date:   Thu May 22 11:24:59 2025 +0200        

    added a paragraph to the team page        

commit dfeddc543372604e2caa0058e23af233a09cc7d1 (origin/ft/service-redesign, ft/service-redesign)
Author: Joie-Dorine-Habarugira-dodo <joiedorine.habarugira22a@kepler.org>
Date:   Thu May 22 11:19:08 2025 +0200        

    updated README file

commit 5be004414d47acd9bbc2b3b2b428a35661422120
Merge: 22b2544 278a7c9
Author: Joie-Dorine-Habarugira-dodo <joiedorine.habarugira22a@kepler.org>
Date:   Thu May 22 11:13:42 2025 +0200        

    merged to main

commit 278a7c9b9c434f6b293092046ec30d714caddf2e (origin/main, main, ft/contact-page)        
Author: Joie-Dorine-Habarugira-dodo <joiedorine.habarugira22a@kepler.org>
Date:   Thu May 22 10:02:27 2025 +0200        

    retrieving files

commit 22b2544d30e87add0795e0f6c02d53d5ea93c73f
Author: Joie-Dorine-Habarugira-dodo <joiedorine.habarugira22a@kepler.org>
Date:   Thu May 22 09:58:06 2025 +0200        

    added changes to the service page

commit 7afc28b02f8459cb3c889d38f2f272463e8bf262
Merge: 40c8358 7132d41
Author: Joie-Dorine-Habarugira-dodo <hjoydoreen08@gmail.com>
Date:   Wed May 21 12:09:22 2025 +0200        

    Merge pull request #3 from Joie-Dorine-Habarugira-dodo/revert-2-ft/bundle-2

    Revert "Added a service page for the project"

commit 7132d412ebb96b89db2372cf616f72d9b9dcb92a (origin/revert-2-ft/bundle-2)
Author: Joie-Dorine-Habarugira-dodo <hjoydoreen08@gmail.com>
Date:   Wed May 21 12:08:45 2025 +0200        

    Revert "Added a service page for the project"

commit 40c835819d59224ec07b535bda9537ec3adea73d
Merge: 026a696 6e0fb8c
Author: Joie-Dorine-Habarugira-dodo <hjoydoreen08@gmail.com>
Date:   Wed May 21 12:00:00 2025 +0200        

    Merge pull request #2 from Joie-Dorine-Habarugira-dodo/ft/bundle-2

    Added a service page for the project      

commit 6e0fb8c8a69d87ae2ddb77332bb6cf0d22d7a204 (origin/ft/bundle-2)
Author: Joie-Dorine-Habarugira-dodo <joiedorine.habarugira22a@kepler.org>
Date:   Wed May 21 11:31:11 2025 +0200        

    created a services file

commit 62a21afd24d45b900e1096b60216f55a7f7d2d01 (origin/dev, dev)
Author: Joie-Dorine-Habarugira-dodo <joiedorine.habarugira22a@kepler.org>
Date:   Wed May 21 10:55:21 2025 +0200        

    finished exercise 2
:
e.habarugira22a@kepler.org>
Date:   Wed May 21 11:31:11 2025 +0200        

    created a services file

commit 62a21afd24d45b900e1096b60216f55a7f7d2d01 (origin/dev, dev)
Author: Joie-Dorine-Habarugira-dodo <joiedorine.habarugira22a@kepler.org>
Date:   Wed May 21 10:55:21 2025 +0200        

    finished exercise 2

hp@Dorine MINGW64 ~/git-exercises (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

hp@Dorine MINGW64 ~/git-exercises (ft/contact-page)
$ git cherry-pick 3d9b384f2f1b6cda3dd3b3464e7ce3cb84c86593
[ft/contact-page 8ae5eb1] added a paragraph to the team page
 Date: Thu May 22 11:24:59 2025 +0200
 1 file changed, 6 insertions(+)

hp@Dorine MINGW64 ~/git-exercises (ft/contact-page)
$ touch contact.html

hp@Dorine MINGW64 ~/git-exercises (ft/contact-page)
$ git add .

hp@Dorine MINGW64 ~/git-exercises (ft/contact-page)
$ git commit -m "feat: add contact page"
[ft/contact-page f3d501d] feat: add contact page
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html

hp@Dorine MINGW64 ~/git-exercises (ft/contact-page)
$ git push origin ft/contact-page
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 12 threads      
Compressing objects: 100% (6/6), done.        
Writing objects: 100% (6/6), 1.52 KiB | 389.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page

hp@Dorine MINGW64 ~/git-exercises (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$ touch faq.html

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$ git add .

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$ git commit -m "feat: add faq page"
[ft/faq-page 123f5bd] feat: add faq page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$ git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads      
Compressing objects: 100% (3/3), done.        
Writing objects: 100% (3/3), 474 bytes | 118.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
new/ft/faq-page
remote:
To https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$ git revert 3d9b384f2f1b6cda3dd3b3464e7ce3cb84c86593
hint: Waiting for your editor to close the file...
[ft/faq-page 764cc58] Revert "added a paragraph to the team page"
 1 file changed, 6 deletions(-)

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$ 

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$ git add .

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$ git commit -m "reverted the changes"
[ft/faq-page dc5dd06] reverted the changes
 1 file changed, 275 insertions(+), 1 deletion(-)

hp@Dorine MINGW64 ~/git-exercises (ft/faq-page)
$ git push origin ft/faq-page
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 12 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 2.34 KiB | 799.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (4/4), completed with 3 local objects.
To https://github.com/Joie-Dorine-Habarugira-dodo/Gym-Git-Exercise-Solutions.git
   123f5bd..dc5dd06  ft/faq-page -> ft/faq-page
   ```

   



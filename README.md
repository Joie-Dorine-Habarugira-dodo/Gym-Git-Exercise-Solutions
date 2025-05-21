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
#Git-Cheat-Sheet

Initialize `init` to the first git-repo with:
```
$ git init "REPO-NAME"
$ cd REPO-Name/.git
$ code README.md
```

**NOTE** To Add VSC as Code editor type:

``` 
$ git config --global core.editor "code --wait"
$ git config --global -e
```
Now, just edit the config in VSC.

**NOTE** Directories are not tracked, just add a `.keep` file

To ignore files add them to `.gitignore`:

```
log/*.log
```

To just add parts to the index, we can use `git add -p`(`-p` File-Name).

##Disaster Recovery

In case of deleted commits use `git reflog` and `git cherry-pick` to recover those commits:

```
$ git cherry-pick LOST-COMMIT-SHA1
```

**NOTE** Will be cleaned once `git gc` was executed.

##Check Log for a file or repo
```
$ git log --oneline --graph
$ git blame FILE-NAME.xoxo
$ git log -S<what you are looking for>
```

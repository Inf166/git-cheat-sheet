#Git-Cheat-Sheet

Initialize `init` to the first git-repo with:
```
$ git init "REPO-NAME"
$ cd REPO-Name/.git
$ code README.md
```

**NOTE** Directories are not tracked, just add a `.keep` file

To ignore files add them to `.gitignore`:

```
log/*.log
```

**NOTE** To Add VSC as Code editor type:

``` 
$ git config --global core.editor "code --wait"
$ git config --global -e
```
Now, just edit the config in VSC.
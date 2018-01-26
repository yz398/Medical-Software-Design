# GitFundamentals
## Lecture 02
\*.md files indicate markdown formatting on render of content: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

## Completing Tasks with Git
* How do I clone a repository created / existing on GitHub on my local computer?
```
git clone git@github.com/$USERNAME/$REPONAME.git [$LOCALREPONAME]
```
This command will clone the most recent files and complete history of the
repository to a local directory (can specify a name different than the
repository name with `$LOCALREPONAME`.

* How do I figure out what files in my local repository have changed or their status in the git commit process?
```
git status
```
This will show files that are untracked (not under git version control),
modified (changed since last committed version), and files that are queued for
commit.
* How do I see what has changed in a file since it was last committed?
```
git diff
```
* How do I queue files to be added / removed in the next commit?
```
git add $FILENAME
git rm $FILENAME
```
* How do I commit changes to the repository version history on my local computer?
```
git commit
'''
* How do I send or get committed changes from GitHub (your default remote `origin`)?
```
git push
git pull
```
* How do I figure out what remote version of my repository are linked to my local repository?
```
git remote
'''
You can add, remove and modify remote URLs with this same command.

`.gitignore`: patterns in file or directory names that we want git to ignore by default in version history management

vim workflow:
  + vim filename
  + Type `i` to go into Insert mode
  + Type amazing code
  + Type `Esc` to exit Insert mode and go into Command mode
  + Type `:w` - write file
  + Type `:q` - quit
  + OR combine with `:wq`

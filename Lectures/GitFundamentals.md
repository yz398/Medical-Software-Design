# GitFundamentals
## Markdown Formatting
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
```
* How do I send or get committed changes from GitHub (your default remote `origin`)?
```
git push
git pull
```
* How do I figure out what remote version of my repository are linked to my local repository?
```
git remote
```
You can add, remove and modify remote URLs with this same command.


## Ignoring local files from git control
Text editors and IDEs can create a lot of temporary files in your repository
that you do not want to share with collaborators.  Additionally, you may have
test data and scripts that you also don't want to share.  Instead of having
these files constantly show up in your `git status` output, you can tell git to
ignore these files by creating a `.gitignore` files that contains file and
directory name patterns that you want to ignore.  If there are files that you
very commonly need to ignore in your repositories, you can add them to a file
in your home directory: `$HOME/.gitignore_global`.

## VIM Workflow:
* `vim filename`
* Type `i` to go into Insert mode (how you can edit your file)
* Type `ESC` to exit Insert mode and go into Command mode
* Type `:w` - write file
* Type `:q` - quit
* :sparkles: Shortcut - combine write and quit in one command: `:wq`

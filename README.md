#Getting and Creating Projects

| Command                                                           | Description                                                                                                                                                                                                                                                                                                 |
| ----------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `git init`                                                        | To initialize a local Git repository. (Running git init in an existing repository is safe. It will not overwrite things that are already there. The primary reason for rerunning git init is to pick up newly added templates (or to move the repository to another place if --separate-git-dir is given).) |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | To clone a repository into a new directory.                                                                                                                                                                                                                                                                 |

#Basic Snapshotting

| Command                            | Description                                               |
| ---------------------------------- | --------------------------------------------------------- |
| `git add [file-name.txt]`          | To add file contents to the index.                        |
| `git add -A`                       | Add all new and changed files to the staging area.        |
| `git status`                       | Show the working tree status.                             |
| `git commit -m "[commit message]"` | To record changes to the repository.                      |
| `git rm -r [file-name.txt]`        | To remove files from the working tree and from the index. |

#Branching and Merging

| Command                                              | Description                                 |
| ---------------------------------------------------- | ------------------------------------------- |
| `git branch`                                         | To list, create, or delete branches.        |
| `git branch -a`                                      | List all branches (local and remote).       |
| `git branch [branch name]`                           | Create a new branch.                        |
| `git branch -d [branch name]`                        | Delete a branch.                            |
| `git push origin --delete [branch name]`             | Delete a remote branch.                     |
| `git checkout -b [branch name]`                      | Create a new branch and switch to it.       |
| `git checkout -b [branch name] origin/[branch name]` | Clone a remote branch and switch to it.     |
| `git branch -m [old branch name] [new branch name]`  | Rename a local branch.                      |
| `git checkout [branch name]`                         | Switch to a branch.                         |
| `git checkout -`                                     | Switch to the branch last checked out.      |
| `git checkout -- [file-name.txt]`                    | Discard changes to a file.                  |
| `git merge [branch name]`                            | Merge a branch into the active branch.      |
| `git merge [source branch] [target branch]`          | Merge a branch into a target branch.        |
| `git stash`                                          | Stash changes in a dirty working directory. |
| `git stash clear`                                    | Remove all stashed entries.                 |

#Sharing and Updating Projects

| Command                                                                           | Description                                                  |
| --------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| `git push origin [branch name]`                                                   | Push a branch to your remote repository.                     |
| `git push -u origin [branch name]`                                                | Push changes to remote repository (and remember the branch). |
| `git push`                                                                        | Push changes to remote repository (remembered branch).       |
| `git push origin --delete [branch name]`                                          | Delete a remote branch.                                      |
| `git pull`                                                                        | Update local repository to the newest commit.                |
| `git pull origin [branch name]`                                                   | Pull changes from remote repository.                         |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git`     | Add a remote repository.                                     |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH.                     |

#Inspection & Comparison

| Command                                    | Description                     |
| ------------------------------------------ | ------------------------------- |
| `git log`                                  | Show commit logs.               |
| `git log --summary`                        | View changes (detailed).        |
| `git log --oneline`                        | View changes (briefly).         |
| `git diff [source branch] [target branch]` | Preview changes before merging. |

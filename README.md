# Git Cheatsheet
![git_cheatsheet](git_cheatsheet.png)


# Basic git command
---

<details><summary> <code>git clone</code></summary>
This command is used for downloading the latest version of a remote project and copying it to the selected location on the local machine. It looks like this:

```
git clone <repository url>
```

To clone a specific branch, you can use
```
git clone <repository url> -b <branch name>
```
</details>

<details><summary> <code>git fetch</code></summary>
This git command will get all the updates from the remote repository, including new branches.
</details>

<details><summary> <code>git checkout</code></summary>
You can use the <strong>checkout</strong> command to switch the branch that you are currently working on.

```
git checkout <branch name>
```
If you want to create a new branch and switch to it, you can do it by using this command:

```
git checkout -b <branch name>
```
</details>

<details><summary> <code>git init</code></summary>
This is the command you need to use if you want to start a new empty repository or to reinitialize an existing one in the project root. It will create a .git directory with its subdirectories. It should look like this:

```
git init <repository name>
```
</details>
<details><summary> <code>git commit</code></summary>
This one is probably the most used Git command. After changes are done locally, you can save them by “committing” them. A commit is like local a snapshot of the current state of the branch, to which you can always come back. To create a new commit, type this command in Git Bash:

```
git commit -m "<commit message>"
```
</details>

<details><summary> <code>git push</code></summary>
Git push will push the locally committed changes to the remote branch. If the branch is already remotely tracked, simply use it like this (with no parameters):

```
git push
```

If the branch is not yet tracked, and only resides on the local machine, you need to run the command like this:

```
git push --set-upstream <remote branch> <branch name>
```
</details>

<details><summary> <code>git diff</code></summary>
You can use this command to see the unstaged changes on the current branch. Here’s an example of a branch with an edited feature file. <br>

If you want to see the staged changes, run the diff command like this:

```
git diff --staged
```

Or you can compare two branches:

```
gif diff <branch1> <branch2>
```
</details>

<details><summary> <code>git pull</code></summary>
Using git pull will fetch all the changes from the remote repository and merge any remote changes in the current local branch.
</details>

<details><summary> <code>git add</code></summary>
This is the command you need to use to stage changed files. You can stage individual files:

```
git add <file path>
```

Or all files:
```
git add .
```
</details>

<details><summary> <code>git branch</code></summary>
Using git branch will list all the branches of the repository. Or you can use it to create a new branch, without checking it out:

```
git branch <new branch>
```

To delete a branch, run it like this:

```
git branch -d <branch name>
```
</details>

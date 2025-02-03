<< [Main](./README.md)  <<

# Git Advanced

<details>
<summary>Branching and Merging</summary>

### Creating a New Branch
```sh
git checkout -b new-branch
```
This command creates and switches to a new branch.

### Merging Branches
```sh
git checkout main
git merge new-branch
```
This command merges `new-branch` into `main`.

</details>

<details>
<summary>Rebasing</summary>

### Rebasing a Branch
```sh
git checkout feature-branch
git rebase main
```
This command rebases `feature-branch` onto `main`.

</details>

<details>
<summary>Stashing Changes</summary>

### Stashing Uncommitted Changes
```sh
git stash
```
This command stashes your uncommitted changes.

### Applying Stashed Changes
```sh
git stash apply
```
This command applies the stashed changes.

</details>

<details>
<summary>Resetting Changes</summary>

### Soft Reset
```sh
git reset --soft HEAD~1
```
This command undoes the last commit but keeps the changes staged.

### Hard Reset
```sh
git reset --hard HEAD~1
```
This command undoes the last commit and discards all changes.

</details>

<< [Main](./README.md)  <<

<< [Main](./README.md)  <<

# Git Advanced

<details>
<summary>Creating a New Branch</summary>
This command creates and switches to a new branch.
```sh
git checkout -b new-branch
```
</details>

<details>
<summary>Merging Branches</summary>
This command merges `new-branch` into `main`.
```sh
git checkout main
git merge new-branch
```
</details>

<details>
<summary>Rebasing a Branch</summary>
This command rebases `feature-branch` onto `main`.
```sh
git checkout feature-branch
git rebase main
```
</details>

<details>
<summary>Stashing Uncommitted Changes</summary>
This command stashes your uncommitted changes.
```sh
git stash
```
</details>

<details>
<summary>Applying Stashed Changes</summary>
This command applies the stashed changes.
```sh
git stash apply
```
</details>

<details>
<summary>Soft Reset</summary>
This command undoes the last commit but keeps the changes staged.
```sh
git reset --soft HEAD~1
```
</details>

<details>
<summary>Hard Reset</summary>
This command undoes the last commit and discards all changes.
```sh
git reset --hard HEAD~1
```
</details>

<< [Main](./README.md)  <<

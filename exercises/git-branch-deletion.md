# Delete a Git Branch

Deleting a Git branch can be done either locally or remotely. Follow these steps to delete a branch safely.

## Deleting a Local Branch

**Step 1** : List All Branches

Before deleting a branch, it’s a good practice to list all the branches to ensure you are deleting the correct one.
```sh
git branch
```
**Step 2**: Switch to a Different Branch

You cannot delete the branch you are currently on. Switch to another branch first.
```sh
git checkout main
```
**or**
```sh
git switch main
```
**Step 3**: Delete the Local Branch

Use the following command to delete the local branch.

```sh
git branch -d branch_name
```

Replace branch_name with the name of the branch you want to delete.

The -d option will delete the branch only if it has been fully merged. 

If you want to force delete the branch, use:
```sh
git branch -D branch_name
```
## Deleting a Remote Branch

**Step 1**: List All Remote Branches

To confirm the existence of the branch on the remote repository.

```sh
git branch -r
```

**Step 2**: Delete the Remote Branch

Use the following command to delete the branch from the remote repository.
```sh
git push origin --delete branch_name
```
Replace branch_name with the name of the branch you want to delete.

**Step 3** : Fetch Updates

To ensure your local repository reflects the deletion, fetch the updates from the remote.

```sh
git fetch -p
```
The -p option (or --prune) will remove any remote-tracking references that no longer exist on the remote.

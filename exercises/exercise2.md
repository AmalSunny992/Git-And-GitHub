# Exercise 2: Branching and Merging

In this exercise, you'll learn how to create branches, switch between them, and merge changes.

## Steps

1. **Create a New Branch**
   - Create a new branch called `feature-branch`:
     ```sh
     git branch feature-branch
     ```

2. **Switch to the New Branch**
   - Switch to `feature-branch`:
     ```sh
     git checkout feature-branch
     ```

3. **Make Changes in the New Branch**
   - Create a new file called `feature.txt` and add some content:
     ```sh
     echo "This is a new feature." > feature.txt
     ```
   - Add and commit the new file:
     ```sh
     git add feature.txt
     git commit -m "Add feature.txt with feature description"
     ```

4. **Switch Back to the Main Branch**
   - Switch back to the `main` branch:
     ```sh
     git checkout main
     ```

5. **Merge the Feature Branch into Main**
   - Merge the changes from `feature-branch` into `main`:
     ```sh
     git merge feature-branch
     ```

6. **Check the Status and Log**
   - Check the status:
     ```sh
     git status
     ```
   - View the commit history:
     ```sh
     git log
     ```

You've successfully created a new branch, made changes, and merged those changes back into the main branch.

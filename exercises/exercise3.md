# Exercise 3: Working with Remote Repositories

In this exercise, you'll learn how to connect to a remote repository on GitHub, push your changes, and pull updates.

## Steps

1. **Create a Remote Repository**
   - Go to [GitHub](https://github.com/) and create a new repository called `my-remote-repo`.

2. **Add the Remote Repository**
   - Add the remote repository to your local repository:
     ```sh
     git remote add origin <your-repository-url>
     ```

3. **Push Changes to the Remote Repository**
   - Push your changes to the remote repository:
     ```sh
     git push -u origin main
     ```

4. **Make a Change Locally**
   - Create a new file called `update.txt`:
     ```sh
     echo "This is an update." > update.txt
     ```
   - Add and commit the file:
     ```sh
     git add update.txt
     git commit -m "Add update.txt with update message"
     ```

5. **Push the Change to the Remote Repository**
   - Push the changes to the remote repository:
     ```sh
     git push
     ```

6. **Pull Changes from the Remote Repository**
   - Simulate another user making a change by editing the repository on GitHub.
   - Pull the latest changes from the remote repository:
     ```sh
     git pull
     ```

You've learned how to connect to a remote repository, push your changes, and pull updates from GitHub.

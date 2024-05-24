# Exercise 1: Initializing a Repository and Making Your First Commit

In this exercise, you'll learn how to initialize a Git repository, add files, and make your first commit.

## Steps

1. **Initialize a Git Repository**
   - Create a new directory for your project:
     ```sh
     mkdir my-first-repo
     cd my-first-repo
     ```
   - Initialize a Git repository:
     ```sh
     git init
     ```

2. **Create a New File**
   - Create a new file called `hello.txt`:
     ```sh
     echo "Hello, Git!" > hello.txt
     ```

3. **Check the Status of Your Repository**
   - Check the status of your repository:
     ```sh
     git status
     ```

4. **Add the File to the Staging Area**
   - Add `hello.txt` to the staging area:
     ```sh
     git add hello.txt
     ```

5. **Make Your First Commit**
   - Commit the file with a message:
     ```sh
     git commit -m "Add hello.txt with a greeting message"
     ```

6. **Check the Log**
   - View the commit history:
     ```sh
     git log
     ```

Congratulations! You've initialized a Git repository and made your first commit.

# How to Get a Single File from Another Branch using `git checkout`

If you need to retrieve just one file from a different branch in your Git repository, you can use the `git checkout` command. Follow these steps:

1. **Navigate to your repository**: Open your terminal or command prompt and change to your repository's directory:

   ```sh
   cd /path/to/your/repository
   ```

2. **List all branches**: Ensure you know the branch name from which you want to retrieve the file. List all branches with:

   ```sh
   git branch
   ```

3. **Checkout the specific file**: Use the `git checkout` command to get the file from the desired branch. Replace `branch_name` with the branch you want to get the file from, and `path/to/file` with the relative path to the file in your repository:

   ```sh
   git checkout branch_name -- path/to/file
   ```

4. **Stage the file**: After checking out the file, you need to stage it for commit:

   ```sh
   git add path/to/file
   ```

5. **Commit the change**: Commit the file to your current branch:
   ```sh
   git commit -m "Add file from branch_name"
   ```

### Example

If you have a branch named `feature-branch` and you want to retrieve a file located at `src/components/Button.js`, you would run:

```sh
git checkout feature-branch -- src/components/Button.js
git add src/components/Button.js
git commit -m "Add Button.js from feature-branch"
```

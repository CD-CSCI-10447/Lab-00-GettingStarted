## Lab Exercise: Working with Git, GitHub, and Resolving Merge Conflicts

### Objective:
This lab will give you hands-on experience with Git and GitHub, especially in the areas of branching and resolving merge conflicts.

### Requirements:
1. A GitHub account.
2. Git installed on your local machine.
3. Access to the terminal or command prompt.

### Instructions:

#### 1. **Cloning the Repository**:
- Open your terminal or command prompt.
- Navigate to a directory where you'd like to store the project.
- Clone the `student-info` repository using the command:
```bash
git clone [URL-of-student-info-repository]
```
Replace `[URL-of-student-info-repository]` with the actual URL.

#### 2. **Creating Your Own Branch**:
- Navigate into the cloned repository:
```bash
cd student-info
```
- Make sure you are on the main branch:
```bash
git checkout main
```
- Pull the latest changes:
```bash
git pull
```
- Create and switch to a new branch with your name (replace "john-doe" with your name):
```bash
git checkout -b [your-name]
```

#### 3. **Adding Your Information**:
- Using any text editor, open the file `info.txt` located in the repository directory.
- Add the following details, each on a separate line:
  - Your full name
  - Your email
  - Your GitHub username
- Save and close the file.

#### 4. **Committing and Pushing Your Changes**:
- Commit the changes you made:
```bash
git commit -am "Added my details"
```
- Push your branch and changes to the GitHub repository:
```bash
git push origin [your-name]
```
Replace `[your-name]` with the branch name you created earlier.

#### 5. **Resolving Potential Merge Conflicts**:
If informed by the instructor, you may have to resolve a merge conflict. Here's how:

- Switch back to the main branch:
```bash
git checkout main
```
- Pull the latest changes:
```bash
git pull
```
If there's a merge conflict, Git will notify you.

- Open the conflicting file (`info.txt`) in your text editor. You'll see sections marked with `<<<<<<<`, `=======`, and `>>>>>>>`, which indicate the conflicting areas.
- Decide whether to keep your changes, the other changes, or a combination of both. Edit the file accordingly.
- Make sure to remove the conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`) after making your changes.
- Save and close the file.
- Commit and push the resolved changes:
```bash
git commit -am "Resolved merge conflict"
git push origin main
```

#### 6. **Creating a Pull Request (PR)**:
- Go to the GitHub page of the `student-info` repository.
- Click on the "Pull requests" tab.
- Click the "New pull request" button.
- Set the "base" branch as `main` and the "compare" branch as the one you created.
- Fill out any required information and click "Create pull request".

### Congratulations! 🎉
You've just navigated the essentials of Git and GitHub. Merge conflicts might seem daunting initially, but with practice, you'll get more comfortable resolving them. Remember, effective communication with your team can often prevent many merge conflicts. Happy coding!
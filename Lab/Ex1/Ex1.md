<table style="width: 100%; border-collapse: collapse; padding:0;">
  <tr>
    <td style="width: 20%; border: 1px solid black; padding: 0;">
      <table style="width: 100%; border-collapse: collapse; border: none;">
        <tr>
          <td style="padding-top: 0; border-bottom: 1px solid black; text-align: center; font-weight: bold; border-left: none; border-top: none; vertical-align: middle;">Ex. No. 1</td>
        </tr>
        <tr>
          <td style="padding-bottom:0; text-align: center; border-bottom: none; border-right: none; vertical-align: middle;">12/07/2024</td>
        </tr>
      </table>
    </td>
    <td style="width: 80%; border: 1px solid black; text-align: center; font-weight: bold; vertical-align: middle;">Git & GitHub</td>
  </tr>
</table>

#### AIM

Algorithm for Git and GitHub Operations

#### Algorithm

1. **Create a Repository**:
   - Initialize a new Git repository named "Master".
   - Verify repository initialization.

2. **Add and Commit Changes**:
   - Create a new text file named `README.md`.
   - Add content to the `README.md` file.
   - Add the file to the staging area.
   - Commit the changes with a message.

3. **Exploring History**:
   - Modify or add content to the text file.
   - Add and commit the changes.

4. **Branching and Merging**:
   - Create a new branch named `Updated_ReadMe`.
   - Commit changes in the new branch.
   - Merge changes from `Updated_ReadMe` branch into `Master` branch.

5. **Collaborating with Remote Repositories**:
   - Link the local repository to a remote repository.

6. **Push Changes**:
   - Push local commits to the remote repository.

7. **Cloning a Repository**:
   - Clone the repository from GitHub.

8. **Making Changes and Creating a Branch**:
   - Navigate into the cloned repository.
   - Make necessary changes.
   - Check the status of the repository.

9. **Pushing Changes to GitHub**:
   - Add the changes to the staging area.
   - Commit the changes.
   - Push the local branch to the remote repository.

10. **Collaborating through Pull Requests**:
    - Create a pull request on GitHub.
    - Choose base branch and compare with the new branch.
    - Review and merge the pull request.
    - Add title, description, and assign reviewers.
    - Reviewers approve and merge the pull request into the base branch.

11. **Syncing Changes**:
    - Update local repository after the pull request is merged.

#### Input

```sh
# Task 1
## a. Create a Repository
git init

## b. Add and Commit Changes
touch README.md
echo "# This is the readme file for devops" > README.md
git add README.md
git commit -m "Added README.md"

## c. Exploring History
echo "# This is the README file for DevOps" > README.md
git add README.md
git commit -m "Corrected content of README.md"

## d. Branching and Merging
git checkout -b Updated_ReadMe
echo "# This is the updated README file for DevOps" > README.md
git add README.md
git commit -m "Updated README.md"
git checkout main
git merge Updated_ReadMe

## e. Collaborating with Remote Repositories
git remote add origin https://github.com/NakshathraP/DevOps.git

## f. Push Changes
git branch -M main
git push -u origin main

# Task 2
## a. Cloning a Repository
git clone https://github.com/NakshathraP/DevOps.git

## b. Making Changes and Creating a Branch
cd WebTechLab
touch README.md
echo "# This is the README file for WebTechLab" > README.md
git status

## c. Pushing Changes to GitHub
git add .
git commit -m "Added README.md"
git push -u origin main

## d. Collaborating through Pull Requests
# Performed on GitHub:
# 1. Create a pull request.
# 2. Choose base branch and compare with new branch.
# 3. Review and merge the pull request.
# 4. Add title and description.
# 5. Assign reviewers.
# 6. Reviewers approve and merge the pull request.

## e. Syncing Changes
git pull origin main
```

#### Output

1. **Repository Creation**:
   - A new Git repository named "Master" is created.
   - Confirmation message displayed.

2. **Add and Commit Changes**:
   - `README.md` file is created.
   - File contents are added.
   - File is added to the staging area and committed.

3. **Exploring History**:
   - `README.md` file is modified and changes committed.

4. **Branching and Merging**:
   - New branch `Updated_ReadMe` is created and changes committed.
   - Changes are merged into the `main` branch.

5. **Collaborating with Remote Repositories**:
   - Local repository is linked to the remote repository.

6. **Push Changes**:
   - Local commits are pushed to the remote repository.

7. **Cloning a Repository**:
   - Repository is cloned from GitHub.

8. **Making Changes and Creating a Branch**:
   - Changes are made and the status of the repository is checked.

9. **Pushing Changes to GitHub**:
   - Changes are pushed to the remote repository.

10. **Collaborating through Pull Requests**:
    - Pull request is created, reviewed, and merged on GitHub.

11. **Syncing Changes**:
    - Local repository is updated with the latest changes from the remote repository.

    ![1a](../photos/Ex1/1a.png?raw=true)
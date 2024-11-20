<table style="width: 100%; border-collapse: collapse; padding:0;">
  <tr>
    <td style="width: 20%; border: 1px solid black; padding: 0;">
      <table style="width: 100%; border-collapse: collapse; border: none;">
        <tr>
          <td style="padding-top: 0; border-bottom: 1px solid black; text-align: center; font-weight: bold; border-left: none; border-top: none; vertical-align: middle;">Ex. No. 3</td>
        </tr>
        <tr>
          <td style="padding-bottom:0; text-align: center; border-bottom: none; border-right: none; vertical-align: middle;">07/08/2024</td>
        </tr>
      </table>
    </td>
    <td style="width: 80%; border: 1px solid black; text-align: center; font-weight: bold; vertical-align: middle;">Git & BitBucket</td>
  </tr>
</table>

#### AIM

Algorithm for Implementing Bitbucket Operations using Git

#### Algorithm

1. **Creating a Repository**:
   - Log into your Bitbucket account.
   - Click on the `Repositories` tab in the sidebar.
   - Click on the `Create repository` button.
   - Fill in the repository details and set the access level.
   - Click on the `Create repository` button.

2. **Cloning a Repository**:
   - Copy the repository URL from Bitbucket.
   - Open the terminal.
   - Clone the repository using the URL.

3. **Making Changes and Creating a Branch**:
   - Navigate into the cloned repository.
   - Create a new text file named `test.txt`.
   - Add content to the `test.txt` file.
   - Check the repository status.
   - Stage the changes for commit.
   - Commit the changes with a message.
   - Create a new branch named `feature`.
   - Switch to the `feature` branch.

4. **Pushing Changes to Bitbucket**:
   - Add the repository URL to a variable.
   - Push the `feature` branch to Bitbucket.
   - Confirm the new branch is available in the Bitbucket repository.

5. **Collaborating through Pull Requests**:
   - Go to the repository on Bitbucket.
   - Click on `Create pull request`.
   - Choose the source branch (`feature`) and the target branch (`main`).
   - Review the changes and create the pull request.
   - Review and merge the pull request.

6. **Syncing Changes**:
   - After merging, update the local repository with the latest changes from the remote repository.

#### Input

```sh
# Task 1: Creating a Repository
# 1. Log into your Bitbucket account.
# 2. Click on the `Repositories` tab in the sidebar.
# 3. Click on the `Create repository` button.
# 4. Fill in the repository details:
#    - Repository name: `example-repo`
#    - Access level: Choose between Private or Public.
# 5. Click on the `Create repository` button.

# Task 2: Cloning a Repository
# 1. Copy the repository URL.
# 2. Open terminal.
git clone https://nakshathragreeneem@bitbucket.org/devops-example-72/devops-ex3.git

# Task 3: Making Changes and Creating a Branch
cd devops-ex3
echo "This is a test file." > test.txt
git status
git add test.txt
git commit -m "Edited test.txt"
git branch feature
git checkout feature

# Task 4: Pushing Changes to Bitbucket
git push -u origin feature

# Task 5: Collaborating through Pull Requests
# 1. Go to the Bitbucket repository.
# 2. Click on `Create pull request`.
# 3. Choose the source branch (`feature`) and the target branch (`main`).
# 4. Review the changes and create the pull request.
# 5. Add a title and description for the pull request.
# 6. Assign reviewers if needed.
# 7. Once the pull request is approved, merge it into the target branch.

# Task 6: Syncing Changes
git checkout main
git pull origin main
```

#### Output

1. **Creating a Repository**:
   - A new Bitbucket repository named `devops-ex3` is created with the specified details.
   ![1-1](../photos/Ex3/3-1.png?raw=true)

2. **Cloning a Repository**:
   - The repository is successfully cloned to the local machine.
   ![2-1](../photos/Ex3/3-2.png?raw=true)

3. **Making Changes and Creating a Branch**:
   - Navigated into the cloned repository.
   - `test.txt` file created and modified.
   - Changes staged and committed.
   - New branch `feature` created and switched to.
   ![3-1](../photos/Ex3/3-3.png?raw=true)
   ![3-1](../photos/Ex3/3-4.png?raw=true)

4. **Pushing Changes to Bitbucket**:
   - `feature` branch pushed to Bitbucket.
   - Verified the new branch `feature` is available in the Bitbucket repository.

5. **Collaborating through Pull Requests**:
   - Pull request created, reviewed, and merged on Bitbucket.
   ![5-1](../photos/Ex3/3-5.png?raw=true)
   ![5-2](../photos/Ex3/3-6.png?raw=true)

6. **Syncing Changes**:
   - Local repository updated with the latest changes from the remote repository.
   ![6-1](../photos/Ex3/3-7.png?raw=true)

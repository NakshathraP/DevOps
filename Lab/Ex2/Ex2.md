<div style="page-break-after: always;"></div>

<table style="width: 100%; border-collapse: collapse; padding:0;">
  <tr>
    <td style="width: 20%; border: 1px solid black; padding: 0;">
      <table style="width: 100%; border-collapse: collapse; border: none;">
        <tr>
          <td style="padding-top: 0; border-bottom: 1px solid black; text-align: center; font-weight: bold; border-left: none; border-top: none; vertical-align: middle;">Ex. No. 2</td>
        </tr>
        <tr>
          <td style="padding-bottom:0; text-align: center; border-bottom: none; border-right: none; vertical-align: middle;">07/08/2024</td>
        </tr>
      </table>
    </td>
    <td style="width: 80%; border: 1px solid black; text-align: center; font-weight: bold; vertical-align: middle;">Git & GitLab</td>
  </tr>
</table>

#### AIM

Algorithm for Implementing GitLab Operations using Git

#### Algorithm

1. **Creating a Repository**:
   - Log into your GitLab account.
   - Click on the `New project` button.
   - Select `Create blank project`.
   - Fill in the project details and set the visibility level.
   - Click on the `Create project` button.

2. **Cloning a Repository**:
   - Copy the repository URL from GitLab.
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

4. **Pushing Changes to GitLab**:
   - Add the repository URL to a variable.
   - Push the `feature` branch to GitLab.
   - Confirm the new branch is available in the GitLab repository.

5. **Collaborating through Merge Requests**:
   - Go to the `Merge Requests` tab in the GitLab repository.
   - Click on the `New merge request` button.
   - Select the `source branch` as `feature` and the `target branch` as `main`.
   - Click on the `Compare branches and continue` button.
   - Fill in the merge request details and create the merge request.
   - Review and merge the request.

6. **Syncing Changes**:
   - After merging, update the local repository with the latest changes from the remote repository.

#### Input

```sh
# Task 1: Creating a Repository
# 1. Log into your GitLab account.
# 2. Click on the `New project` button.
# 3. Select `Create blank project`.
# 4. Fill in the project details:
#    - Project name: `DevOpsLab`
#    - Project slug: `devopslab` (auto-filled)
#    - Visibility level: Choose between Private, Internal, or Public.
# 5. Click on the `Create project` button.

# Task 2: Cloning a Repository
# 1. Copy the repository URL.
# 2. Open terminal.
git clone https://gitlab.com/NakshathraP/devops-ex2.git

# Task 3: Making Changes and Creating a Branch
cd devops-ex2
touch test.txt
echo "This is a test file." > test.txt
git status
git add test.txt
git commit -m "Added test.txt"
git branch feature
git checkout feature

# Task 4: Pushing Changes to GitLab
git push -u origin feature

# Task 5: Collaborating through Merge Requests
# 1. Go to the GitLab repository.
# 2. Click on the `Merge Requests` tab.
# 3. Click on the `New merge request` button.
# 4. Select `source branch` as `feature` and `target branch` as `main`.
# 5. Click on the `Compare branches and continue` button.
# 6. Fill in the merge request details and click `Create merge request`.
# 7. Review and click `Merge` to merge the request.

# Task 6: Syncing Changes
git checkout main
git pull origin main
```

#### Output

1. **Creating a Repository**:
   - A new GitLab repository named `DevOpsLab` is created with the specified details.
   ![1-1](../photos/Ex2/2-1.png?raw=true)

2. **Cloning a Repository**:
   - The repository is successfully cloned to the local machine.
   ![2-2](../photos/Ex2/2-2.png?raw=true)
   ![2-3](../photos/Ex2/2-3.png?raw=true)

3. **Making Changes and Creating a Branch**:
   - Navigated into the cloned repository.
   - `test.txt` file created and modified.
   - Changes staged and committed.
   - New branch `feature` created and switched to.

4. **Pushing Changes to GitLab**:
   - `feature` branch pushed to GitLab.
   - Verified the new branch `feature` is available in the GitLab repository.
   ![3-1](../photos/Ex2/2-4.png?raw=true)

5. **Collaborating through Merge Requests**:
   - Merge request created, reviewed, and merged on GitLab.
   ![5-5](../photos/Ex2/2-5.png?raw=true)
   ![5-6](../photos/Ex2/2-6.png?raw=true)
   ![5-7](../photos/Ex2/2-7.png?raw=true)
   ![5-8](../photos/Ex2/2-8.png?raw=true)

6. **Syncing Changes**:
   - Local repository updated with the latest changes from the remote repository.
   ![6-1](../photos/Ex2/2-9.png?raw=true)

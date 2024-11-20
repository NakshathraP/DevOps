<table style="width: 100%; border-collapse: collapse; padding:0;">
  <tr>
    <td style="width: 20%; border: 1px solid black; padding: 0;">
      <table style="width: 100%; border-collapse: collapse; border: none;">
        <tr>
          <td style="padding-top: 0; border-bottom: 1px solid black; text-align: center; font-weight: bold; border-left: none; border-top: none; vertical-align: middle;">Ex. No. 4</td>
        </tr>
        <tr>
          <td style="padding-bottom:0; text-align: center; border-bottom: none; border-right: none; vertical-align: middle;">28/08/2024</td>
        </tr>
      </table>
    </td>
    <td style="width: 80%; border: 1px solid black; text-align: center; font-weight: bold; vertical-align: middle;">Advanced Git Commands</td>
  </tr>
</table>

#### **AIM**

Algorithm for Advanced Git Commands

#### **Algorithm**

1. **Interactive Rebase**:
   - Review the commit history using `git log --oneline`.
   - Enter interactive rebase mode with `git rebase -i HEAD~N` (where N is the number of commits).
   - Modify, edit, or squash commits as necessary to clean up the history.
   - Rebase your branch onto another branch if needed using `git rebase <branch>`.

2. **Stashing Changes**:
   - Make changes in your working directory.
   - Stash changes using `git stash`.
   - Apply the stashed changes when required using `git stash apply`.

3. **Reverting and Resetting**:
   - Create a new commit and revert it using `git revert <commit_hash>`.
   - Experiment with `git reset --soft`, `--mixed`, and `--hard` to understand the differences in resetting commit history.

4. **Cherry-Picking a Commit**:
   - Select a commit from another branch and apply it using `git cherry-pick <commit_hash>`.
   - Resolve any conflicts that arise and continue the cherry-pick process.

5. **Working with Submodules**:
   - Add a submodule to your repository using `git submodule add <repository_url> <path>`.
   - Clone a repository with submodules using `git clone --recurse-submodules <repository_url>`.
   - Update submodules using `git submodule update --remote --merge`.

6. **Implementing Git Hooks**:
   - Create a pre-commit hook in the `.git/hooks` directory to prevent commits with "TODO" comments.
   - Make the script executable and test it by attempting to commit a file with a "TODO" comment.

#### **Input**

```sh
# Task 1: Interactive Rebase
git log --oneline
git rebase -i HEAD~N
# Task 2: Stashing Changes
git stash
git stash apply
# Task 3: Reverting and Resetting
git revert <commit_hash>
git reset --soft <commit_hash>
git reset --mixed <commit_hash>
git reset --hard <commit_hash>
# Task 4: Cherry-Picking a Commit
git cherry-pick <commit_hash>
# Task 5: Working with Submodules
git submodule add <repository_url> <path>
git clone --recurse-submodules <repository_url>
git submodule update --remote --merge
# Task 6: Implementing Git Hooks
echo "#!/bin/sh
if grep -r \"TODO\" .; then
    echo \"Commit rejected: please remove TODO comments.\"
    exit 1
fi" > .git/hooks/pre-commit
chmod +x .git/hooks/pre-commit
```

#### **Output**

1. **Interactive Rebase**:
   - Successfully rebased the commit history to clean up and combine multiple commits.
   ![a-1](../photos/Ex4/1-1.png?raw=true)

2. **Stashing Changes**:
   - Successfully stashed and reapplied changes.
   ![b-1](../photos/Ex4/2-1.png?raw=true)

3. **Reverting and Resetting**:
   - Successfully reverted a commit and experimented with different reset options.
   ![c-1](../photos/Ex4/3-1.png?raw=true)
   ![c-2](../photos/Ex4/3-2.png?raw=true)

4. **Cherry-Picking a Commit**:
   - Successfully cherry-picked a commit from another branch and resolved any conflicts.
   ![d-1](../photos/Ex4/4-1.png?raw=true)

5. **Working with Submodules**:
   - Successfully added, cloned, and updated submodules in the repository.

6. **Implementing Git Hooks**:
   - Successfully created a pre-commit hook that prevents commits with "TODO" comments.

#### **Result**

By following this AIM Algorithm, you have successfully mastered advanced Git operations, including interactive rebase, stashing, reverting, resetting, cherry-picking, managing submodules, and implementing Git hooks. This exercise enhances your ability to manage commit histories effectively, collaborate efficiently, and enforce coding standards within your projects.

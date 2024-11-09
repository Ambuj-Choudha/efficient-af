# Git Workflow for Feature Development and Merging

## Development Phase

1. **Make Changes**: Modify your files as needed.

2. **Check Status**:
   ```bash
   git status
   ```

3. **Stage Changes**:
   ```bash
   git add .
   ```

4. **Check Status Again** (optional):
   ```bash
   git status
   ```

5. **Commit Changes**:
   ```bash
   git commit -m "commit message"
   ```

6. **Push to Remote**:
   ```bash
   git push origin your-feature-branch
   ```

7. **Create a Merge Request**: 
   - Go to your remote repository (GitHub, GitLab, etc.) and create a merge request (or pull request).

8. **Merge Request Gets Accepted**: 
   - Wait for the merge request to be reviewed and accepted.

---

## After Merge Request Acceptance

9. **Switch to Main Branch**:
   ```bash
   git checkout main
   ```

10. **Fetch Latest Changes from Remote**:
    ```bash
    git fetch origin
    ```

11. **Merge Changes from the Remote Main Branch**:
    ```bash
    git merge origin/main
    ```

12. **(Optional) Check Logs of the Merged Branch**:
    ```bash
    git log origin/your-feature-branch
    ```

13. **Delete the Feature Branch (Optional)**:
    - To delete the branch locally:
    ```bash
    git branch -d your-feature-branch
    ```
    - To delete it from the remote if no longer needed:
    ```bash
    git push origin --delete your-feature-branch
    ```

14. **Continue Development on the Same Branch** (if applicable):
    - If you want to continue development on the same feature branch:
    ```bash
    git checkout your-feature-branch
    ```
    - Make further changes and repeat the commit and push process:
    ```bash
    git add .
    git commit -m "Further changes"
    git push origin your-feature-branch
    ```

---

### Summary

This workflow outlines the steps for developing features, creating a merge request, and managing branches effectively in Git. Keep this guide handy for reference during your development process!
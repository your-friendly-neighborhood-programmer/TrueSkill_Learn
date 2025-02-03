# Adding Collaborators, Branching, and Restricting Merges to Main Branch

## Adding Collaborators to a GitHub Repository
Collaborators can contribute directly to a private or public repository on GitHub. Follow these steps to add collaborators:

1. **Go to Your Repository**
   - Navigate to your GitHub account and open the repository where you want to add collaborators.

2. **Open the Settings Tab**
   - Click on the **Settings** tab at the top of the repository page.

3. **Manage Access**
   - In the left sidebar, click on **Collaborators and teams** (or **Manage access** in newer versions of GitHub).
   
4. **Add Collaborators**
   - Click **Invite a collaborator** and enter their GitHub username or email.
   - Click **Add** to send an invitation.
   - The invited user will receive an email and must accept the invitation to gain access.

## Collaborating with Branching
Branching allows multiple contributors to work on different features without affecting the main codebase.

### Creating a New Branch
1. Open your repository in GitHub or a local Git client.
2. Use the following command to create and switch to a new branch:
   ```sh
   git checkout -b feature-branch
   ```
3. Make changes and commit them:
   ```sh
   git add .
   git commit -m "Added new feature"
   ```
4. Push the branch to GitHub:
   ```sh
   git push origin feature-branch
   ```

### Collaborating on a Branch
- Other team members can check out the branch using:
  ```sh
  git checkout feature-branch
  ```
- They can make changes, commit, and push updates to the branch.
- Use `git pull` to get the latest updates from the branch before making changes.

### Merging a Branch via Pull Request
1. Go to your repository on GitHub.
2. Click on the **Pull Requests** tab.
3. Click **New Pull Request** and select the feature branch to merge into `main`.
4. Request a review from team members.
5. Once approved, click **Merge Pull Request**.

## Restricting Merges to the Main Branch
To ensure only approved changes get merged into the main branch, you can enable branch protection rules.

### Steps to Restrict Merges:
1. **Go to Repository Settings**
   - Open your GitHub repository and click **Settings**.
   
2. **Access Branch Protection Rules**
   - In the left sidebar, click on **Branches**.
   - Under **Branch protection rules**, click **Add branch protection rule**.
   
3. **Set Up Protection for `main`**
   - In the **Branch name pattern**, type `main` to target the main branch.
   - Check **Require a pull request before merging** to prevent direct commits to main.
   - Check **Require approvals** to ensure reviews before merging.
   - Optionally, enable **Require status checks to pass before merging** to enforce automated testing.
   
4. **Save Changes**
   - Click **Save changes** to enforce the rules.

## Summary
- **Adding collaborators** allows multiple users to contribute to your repository.
- **Branching** enables working on separate features without affecting the main codebase.
- **Pull requests** facilitate code review before merging.
- **Restricting merges to `main`** ensures quality control and collaboration best practices.
- These steps help maintain a secure, structured, and efficient GitHub workflow.

- [Main](./README.md)
# Adding Collaborators, Forking, and Restricting Merges to Main Branch

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

## Collaborating with Forking
Forking allows contributors to make changes to a project without directly modifying the original repository. This is useful for open-source projects where contributors don’t have direct write access.

### Creating a Fork
1. Go to the repository you want to contribute to.
2. Click the **Fork** button at the top right corner.
3. This creates a copy of the repository under your GitHub account.

### Making Changes in the Forked Repository
1. Clone the forked repository to your local machine:
   ```sh
   git clone https://github.com/your-username/repository-name.git
   ```
2. Navigate into the repository directory:
   ```sh
   cd repository-name
   ```
3. Create a new branch for your changes:
   ```sh
   git checkout -b feature-branch
   ```
4. Make changes and commit them:
   ```sh
   git add .
   git commit -m "Added new feature"
   ```
5. Push changes to your fork:
   ```sh
   git push origin feature-branch
   ```

### Submitting a Pull Request (PR) from a Fork
1. Go to the original repository on GitHub.
2. Click on the **Pull Requests** tab.
3. Click **New Pull Request**.
4. Select your forked repository and the branch you worked on.
5. Provide a description of your changes and click **Create Pull Request**.
6. Request a review from the repository maintainers.
7. Once approved, the maintainers will merge your changes into the original repository.

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
- **Forking** enables contributors to make changes without modifying the original repository.
- **Pull requests** facilitate code review before merging.
- **Restricting merges to `main`** ensures quality control and collaboration best practices.
- These steps help maintain a secure, structured, and efficient GitHub workflow.


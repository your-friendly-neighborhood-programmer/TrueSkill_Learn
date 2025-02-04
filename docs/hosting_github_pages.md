
![GE](https://github.com/user-attachments/assets/a15436c4-5c13-4676-940b-0832c3bbb925)
- [Visit TrueSkill.dev](https://trueskill.dev)
- [<< Back to Main](../README.md)

# Hosting Static Sites with GitHub Pages

GitHub Pages is a static site hosting service that takes HTML, CSS, and JavaScript files straight from a repository on GitHub, optionally runs the files through a build process, and publishes a website.

<details>
<summary>Enabling GitHub Pages</summary>
Steps to enable GitHub Pages for your repository.
1. **Go to Repository Settings**
   - Navigate to your repository on GitHub and click on the **Settings** tab.
2. **Access GitHub Pages Settings**
   - Scroll down to the **GitHub Pages** section.
3. **Select Source**
   - Under **Source**, select the branch you want to use for GitHub Pages (usually `main` or `gh-pages`).
   - Click **Save**.
4. **Configure Custom Domain (Optional)**
   - If you have a custom domain, you can configure it in the **Custom domain** section.
</details>

<details>
<summary>Creating Your Static Site</summary>
Steps to create and publish your static site.
1. **Add Your Site Files**
   - Add your HTML, CSS, and JavaScript files to the selected branch.
2. **Commit and Push Changes**
   - Commit and push your changes to the repository.
3. **Access Your Site**
   - Your site will be published at `https://<username>.github.io/<repository-name>/`.
</details>

<details>
<summary>Using Jekyll for Static Site Generation</summary>
Steps to use Jekyll for generating a static site.
1. **Create a Jekyll Site**
   - Follow the [Jekyll documentation](https://jekyllrb.com/docs/) to create a new Jekyll site.
2. **Add Jekyll Files to Repository**
   - Add the generated Jekyll files to your repository.
3. **Configure `_config.yml`**
   - Configure the `_config.yml` file as needed for your site.
4. **Commit and Push Changes**
   - Commit and push your changes to the repository.
5. **Access Your Site**
   - Your Jekyll site will be published at `https://<username>.github.io/<repository-name>/`.
</details>

<< [Main](../README.md)  <<

# Instructions for Setting Up the Jupyter Template

## Template Setup & Usage

- Click the `Use Template` button to initialize your project.
  - `fork` is also appropriate. The advantage is that you can easily merge my upcoming updates by click `fetch-upstream` button, the disadvantage is that you can not set a forked public repository to private.
  - `main` branch contains following files
  - To modify:
    - `index.html`, settings, **must modify, at least modify those commented with `!!!`**.
    - `README.md`, homepage of your site, **change it to yours**.
    - `_navbar.md, _sidebar.md, _footer.md`, **change it to yours**. Remove any if you don't like.
    - `favicon.svg`, the icon your site, **change it to yours**. To use other format, edit `index.html`.
  - To remove:
    - Folder `a-great-subfoloder`, just for demo, **remove it and its contents**.
    - `NOTEBOOK.ipynb`, just for demo, **remove it**.
  - Do not change:
    - `.nojekyll`. The `.nojekyll` file is crucial for ensuring that GitHub Pages does not ignore files or folders that start with an underscore (`_`). Without this file, GitHub Pages may treat such files as special Jekyll files and exclude them from the published site. This is especially important for projects that do not use Jekyll but still rely on files with underscores.
- Go to repository settings, set `github pages` **work on `gh-pages` branch**.
  - If there is no `gh-pages` branch, push to this repository once to trigger the workflow, it will create `gh-pages` branch.
- Done!

## Repository Setup

1. **Clone the Repository**  
   Clone the repository to your local machine using the following command:

   ```bash
   git clone https://github.com/Aaravshah2907/Aarav-Jupyter-Site-Template.git
   ```

## Workflow Setup

The workflows are located in the `.github/workflows` folder. Follow these steps to set up and customize them:

### **Workflow Setup**

- File: `.github/workflows/jupyter-site-template-deploy.yml`
- **Purpose**: Automates tasks such as testing, linting, and deployment for the project.
- **Setup**:

  1. Ensure the repository has a `.github/workflows/jupyter-site-template-deploy.yml` and `verify-and-redeploy.yml` files.
  2. Modify the `python-version` or other configurations in the workflow files to match your project requirements.
  3. Push changes to trigger the workflow:
     ```bash
        git add .
        git commit -m "Set up main workflow"
        git push origin main
     ```

- **Customizing the Workflow**:
  - Modify the `jupyter-site-template-deploy.yml` file to suit your project's needs.
  - Refer to [GitHub Actions Documentation](https://docs.github.com/en/actions) for advanced configurations.

## Additional Notes

- `README.md` of each folder level would serve as homepage of this level, like this one you are reading.
  - So don't hesitate to change this `README.md` to create your own homepage!
- The sidebar serve as a document navigator as well as `table of contents` of current document.
  - The sidebar item starts with an `-` belongs to `table of contents` of current document.
  - Other sidebar items are defined in `_sidebar.md`.
- To disable features, comment its plugin `<script>` tag inside `index.html`.
- Ensure you have the necessary permissions to run workflows in your repository.
- For titles in Markdown files, use the `[]` syntax in the `_sidebar.md`.
- For troubleshooting, check the Actions tab in your GitHub repository.

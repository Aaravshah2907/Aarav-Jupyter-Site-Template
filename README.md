# Homepage

Set up your jupyter-markdown hybrid site in one minute, powered by [Docsify](https://docsify.js.org/).

My Demo is here: [Aarav's Jupter Site Template](https://aaravshah2907.github.io/Aarav-Jupyter-Site-Template/#/)

Original Creator's Demo is here: [Maxlinn's Jupyter Site Template Demo](https://maxlinn.github.io/linn-jupyter-site-template).

## Differences from [Maxlinn/linn-docsify-template](https://github.com/Maxlinn/linn-docsify-template)

- It adds script of Github Actions to convert `.ipynb` to `.md`, and publish site to `gh-pages` branch.
  - [Maxlinn/linn-docsify-template](https://github.com/Maxlinn/linn-docsify-template) doesn't use Github Actions, and publish on `main` branch.

## Usage

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
  - Nevermind:
    - `.nojekyll`, nevermind.
- Go to repository settings, set `github pages` **work on `gh-pages` branch**.
  - If there is no `gh-pages` branch, push to this repository once to trigger the workflow, it will create `gh-pages` branch.
- Done!

## Reminder

- `README.md` of each folder level would serve as homepage of this level, like this one you are reading.
  - So don't hesitate to change this `README.md` to create your own homepage!
- The sidebar serve as a document navigator as well as `table of contents` of current document.
  - The sidebar item starts with an `-` belongs to `table of contents` of current document.
  - Other sidebar items are defined in `_sidebar.md`.
- To disable features, comment its plugin `<script>` tag inside `index.html`.

## Features

See [Maxlinn/linn-docsify-template](https://github.com/Maxlinn/linn-docsify-template).

## Note

This is my personal template (modified) of the original one.

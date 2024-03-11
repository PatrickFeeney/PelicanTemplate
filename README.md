# PelicanTemplate
Blank template for a Pelican GitHub Pages site.

## How to Replicate

1. Create GitHub repo with default Python `.gitignore` and a `README.md`.
If you want this to be your GitHub Pages user site (`username.github.io` without `/reponame/` after), the repo must be named `username.github.io`.
1. Clone the repo and launch shell in that directory.
1. Run `pipenv install pelican[markdown] ghp-import` to create a Pipenv environment for Pelican and its GitHub Pages package.
1. Run `pipenv shell` to run subsequent commands in the Pipenv environment.
1. Run `pelican-quickstart` and choose the following non-default answers: URL prefix to `https://username.github.io/reponame/`, yes to GitHub Pages.
This will default to a GitHub project page (`https://username.github.io/reponame/`), but Pelican quickstart will give you the option to make a GitHub user site (must use URL prefix `https://username.github.io`).
1. Run `make html` to convert content to static site output.
1. Run `make serve` to serve the site at http://localhost:8000 for local viewing.
1. Run `make github` to push that content to GitHub and automatically update GitHub Pages.

Optional themes:
1. In repo directory run `mkdir submodules; cd submodules`.
1. Run `git submodule add REPO_URL`, with most themes available at `https://github.com/getpelican/pelican-themes.git`.
1. Follow the install instructions for whichever theme you want to use.
pelican-bootstrap3 is used in this repo.
1. Convert content to static site output, view locally, and push content to GitHub.

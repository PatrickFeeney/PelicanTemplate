# PelicanTemplate
Blank template for a Pelican GitHub Pages site.

## How to Replicate

1. Create GitHub repo with default Python `.gitignore` and a `README.md`.
1. Clone the repo and launch shell in that directory.
1. Run `pipenv install pelican[markdown] ghp-import` to create a Pipenv environment for Pelican and its GitHub Pages package.
1. Run `pipenv shell` to run subsequent commands in the Pipenv environment.
1. Run `pelican-quickstart` and choose the following non-default answers: URL prefix to `username.github.io/reponame/`, yes to GitHub Pages.
This will default to a GitHub project page (`username.github.io/reponame/`), but Pelican quickstart will give you the option to make a user site (`username.github.io` without `/reponame/` after; must change URL prefix to match).
1. Run `make html` to convert content to static site output.
1. Run `make serve` to serve the site at http://localhost:8000 for local viewing.
1. Run `make github` to push that content to GitHub and automatically update GitHub Pages.

Optional themes:
1. In repo directory run `mkdir submodules; cd submodules`.
1. Run `git submodule add REPO_URL`, with most themes available at `https://github.com/getpelican/pelican-themes.git`.
1. Follow the install instructions for whichever theme you want to use.
pelican-bootstrap3 is used in this repo.

# PelicanTemplate
Blank template for a Pelican GitHub Pages site.

## How to Replicate

1. Create GitHub repo with default Python `.gitignore` and a `README.md`.
1. Clone the repo and launch shell in that directory.
1. Run `pipenv install pelican[markdown] ghp-import` to create a Pipenv environment for Pelican and its GitHub Pages package.
1. Run `pipenv shell` to run subsequent commands in the Pipenv environment.
1. Run `pelican-quickstart` and choose the following non-default answers: no to URL prefix, yes to GitHub Pages.
This will default to a GitHub project page (`username.github.io/reponame/`), but Pelican quickstart will give you the option to make a user site (`username.github.io` without `/reponame/` after).
1. Run `make html` to convert content to static site output.
1. Run `make github` to push that content to GitHub and automatically update GitHub Pages.

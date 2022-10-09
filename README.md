# Latex and GitHub actions introduction

This repo shows a minimal Latex example and implements a GitHub action that automatically builds an artifact containing the compiled PDF Latex document.

After every push on the `main` branch a GitHub action is triggered. The action compiles a latex document and publishes it as an artifact.

## Latex installation

You need to install a Tex distribution, and then you can use the editor of your choice to work with Latex.

- You can get a Tex distribution from the [Latex-project website](https://www.latex-project.org/get/).

- A good editor choice available for Windows, Linux, and MacOS is [TexStudio](https://www.texstudio.org/).

Once you installed the two components mentioned above, you can use your editor and open the file in `latex-example/latex_example.tex`.


## Github Actions

GitHub actions automatize the CI/CD process and can be used for a variety of things. For instance, we can use them to validate the code inside a PR.

Most of the times you don't have to write actions yourself but you can search for them in the [actions marketplace](https://github.com/marketplace?type=actions).

In this repo, we implement [latex-action@v2](https://github.com/marketplace/actions/github-action-for-latex) by writing a `.yml` file in `.github/workflows/main.yml`. 
We trigger the action everytime someone pushes on main or opens a PR on main.

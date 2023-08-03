# quarto-scaffold

Base a new repo off this public template to get started with a reproducible analysis or graphic quickly. The template comes with a [dev container](https://code.visualstudio.com/docs/remote/containers) in order to get working with 360's data science stack quickly.

## 🛠 Get started

To start working with a preconfigured, reproducible environment:

- Make sure you have [VSCode](https://code.visualstudio.com) and [Docker](https://www.docker.com/) installed
- Clone this repository
- Open it in VSCode
- Open the command palette (Cmd/Ctrl+Shift+P) and run **"Remote-Containers: Reopen in Container"**
- The project will now be open in a container that includes [Quarto](https://quarto.org), [R](https://r-project.org) and the packages needed to reproduce the analysis
- To customise the container, edit the `.devcontainer/devcontainer.json` file. You can:
  - Add or change the R packages installed using the `r-packages` feature;
  - Add external dependencies from APT using the `apt-packages` feature; or
  - Add major external dependencies or features, like Node, by adding other dev container features (although for the widest compatibility, you should check to ensure they run on both x64 and ARM64).

## ➕ Adding stories

This repo just keeps the dev environment scaffolding; templates for individual analyses and graphics are kept in the [`quarto-templates`](https://github.com/360-info/quarto-templates) repo. To bring one of them into your project with [Quarto](https://quarto.org), run (for example):

```shell
quarto use extension 360-info/quarto-templates/360-embed
```

## ✅ Publication checklist

- [ ] Replace this README with [`README-template.md`](README-template.md), adding:
  * [ ] `[report_title]`
  * [ ] `[report_share_url]`
  * [ ] `[report_summary]`
  * [ ] `[report_graphic_and_link]`
  * [ ] `[report_datasources_links]` (plus any exceptions to [CC BY 4.0](https://creativecommons.org/licenses/by/4.0) licensing)
  * [ ] `[report_codespaces_id]`
  * [ ] `[report repo name]` under Help
  * [ ] Any changes that need to be made to manual reproduction instructions
- [ ] Fill in [`data/README.md`](data/README.md) with the data dictionary, links or other notes needed to understand and re-use the dataset
- [ ] Make sure any additional R packages used in the analysis are installed at the bottom of [`.devcontainer/Dockerfile`](.devcontainer/Dockerfile)

### Codespaces ID

Lookup the repo ID in the address bar once you select it [in the Codespaces launcher](https://github.com/codespaces/new)).

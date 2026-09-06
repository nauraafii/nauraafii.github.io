# Naufal Abrar Afifi

Personal portfolio for Naufal Abrar Afifi, a Computer Engineering student at PENS.

The site is available in [Bahasa Indonesia](https://nauraafii.github.io/) and [English](https://nauraafii.github.io/en/).

## Stack

- [Hugo](https://gohugo.io/)
- [Blowfish](https://blowfish.page/) theme
- GitHub Pages and GitHub Actions

## Run locally

Install Git and Hugo Extended **0.155.3**, the version used by the [deployment workflow](.github/workflows/hugo.yaml). Check your installation with `hugo version`.

1. Clone this repository with its submodule:

   ```powershell
   git clone --recurse-submodules https://github.com/nauraafii/nauraafii.github.io.git
   cd nauraafii.github.io
   ```

2. Run the local server from the repository directory:

   ```powershell
   hugo server
   ```

Open the local address shown by Hugo. Changes pushed to `main` are deployed through GitHub Actions.

If you already cloned without the theme, run `git submodule update --init --recursive` from the repository directory.

## Where to edit

| File or directory | Purpose |
| --- | --- |
| [`layouts/partials/home/custom.html`](layouts/partials/home/custom.html) | Homepage layout and project descriptions in both languages. |
| [`static/css/home.css`](static/css/home.css) | Custom homepage styling and responsive layout. |
| [`content/`](content/) | Homepage titles and descriptions for each language. |
| [`config/_default/`](config/_default/) | Site settings, author details, menus, and language settings. |
| [`i18n/`](i18n/) | Translation overrides for theme labels. |
| [`themes/`](themes/) | Blowfish theme submodule. Put site customizations in this repository's layouts and CSS. |

When updating a project description, update both language versions in `custom.html`. Keep the author details and page descriptions consistent with the visible content.

## Check before publishing

- Preview `/` and `/en/` with `hugo server`.
- Check navigation, links, theme switching, and accessibility controls on a narrow and wide screen.
- Run `hugo --minify`, matching the build command used for deployment.

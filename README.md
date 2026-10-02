# Personal website

Built with [Hugo](https://gohugo.io) and the [hugo-coder](https://github.com/luizdepra/hugo-coder) theme,
deployed to GitHub Pages by `.github/workflows/hugo.yaml` on every push to `main`.

## Local preview

    git clone --recurse-submodules <repo-url>   # the theme is a git submodule
    hugo server                                 # http://localhost:1313

## Editing

- Landing page (name, tagline, social links): `hugo.toml`
- About page: `content/about.md`
- Projects: one Markdown file per entry in `content/projects/`.
  Create one with `hugo new projects/my-project.md`, then set `draft = false`.
  Set `externalLink` to make the entry point to an external URL instead of its own page.
- Avatar: put a picture in `static/images/avatar.jpg` and uncomment `avatarURL` in `hugo.toml`.

## Updating the theme

    git submodule update --remote themes/hugo-coder

# /xerographic

An experimental* theme for the [Hugo](https://gohugo.io/) static site generator. See [heracl.es](https://heracl.es) for a live preview, and the theme’s Git respority [/xerographic](https://github.com/Arty2/xerographic) for more details.

* Major breaking changes may occur between versions, both in functionality and design approach. Using versioned releases is more than encouraged.

## Installation

The following instructions assume that you already have your site’s content in a Git repository. The official [Hugo documentation for themes](https://gohugo.io/getting-started/quick-start/#step-3-add-a-theme) suggest to install as a *submodule*, but installing as a *subtree* has [several advantages](https://training.github.com/downloads/submodule-vs-subtree-cheat-sheet/).

```
git remote add xerographic https://github.com/Arty2/xerographic.git
git subtree add --prefix=themes/xerographic xerographic master --squash
```

To update the theme to the most current version:

```
git subtree pull --prefix=themes/xerographic xerographic master --squash
```

## Features

- Plug & Play; should work with zero configuration.
- Multilingual ready.
- Fully responsive. Two fluid breakpoints.
- Themable. Automatic light and dark themes respective to user settings.
- Sidenotes (marginalia) inspired by [Tufte CSS](https://edwardtufte.github.io/tufte-css/). Collapsible on mobile.
- Inline comments and external links preview when `title=""` is provided.
- Detailed & extensible page and post metadata. Automatic Table of Contents for lengthy posts.
- Page and post types: normal; preformatted.

## Built-in Shortcodes

- articles-list
- articles-filter
- gallery
- img
- marginalia
- menu-social
- section


## Customisation

### Favicon

Add a `/static/favicon.png` file.

### CSS Variables

...

### Custom CSS

This theme supports per page custom styles via `custom.css` in the page’s bundle or folder. Global styles may be customized by creating a `/static/styles/custom.css` file.

### Custom JavaScript

`./script.js` ...

### Site configuration

See `config.default.yml`

```yaml
...
```


## Post and page frontmatter options

Automatic featured images, by name `*__featured.ext`

```yaml
title
summary
tags
draft
featured_image
show_comments
show_meta
license
rating
dateread
datecreated
crosspost
publication.title
```



***

## Bundled / Credits

- jQuery
- [fancybox](http://fancyapps.com/fancybox/3/)
- Alegreya font
- Fantasque Sans Mono font


***

© 2018-2020 [Heracles Papatheodorou](http://heracl.es) a.k.a [@Arty2](https://www.twitter.com/Arty2), [MIT Licence](LICENCE.txt)

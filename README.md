# Foundation for Public Code Jekyll Theme

[![Build Status](https://travis-ci.org/publiccodenet/jekyll-theme.svg?branch=master)](https://travis-ci.org/publiccodenet/jekyll-theme)

A jekyll theme for the set up of quick generic static sites and for use with GitHub pages.

## Building locally

This theme is built to run predictably on GitHub pages, therefore the [`github-pages`](https://github.com/github/pages-gem) gem is required. Run `bundle install` before building with Jekyll.

To serve locally with Jekyll, use `bundle exec jekyll serve`.

## Customising

### Table of contents

#### For your whole site

You can turn on the display of Table of Contents ('On this page' section) for any page by adding `toc: true` to the `_config.yml` 

#### For just a specific page

Or adding `toc: true` to the front matter of any page where you want the Table of Contents to display.

### Breadcrumbs

You can add a breadcrumbs object to a page's front-matter with the name and path of the items that need to be in the breadcrumbs, the home page and the current page will be automatically added.

```yaml
breadcrumbs:
  - name: 'Important guidance'
    path: '/x/'
  - name: 'For everyone'
    path: '/x/index.html'
```

Will result in breadcrumbs like

> Site title > Important guidance > For everyone > Page title

These can also be added as Jekyll default variables for every or specific pages.

### Navigation

⚠️ This feature is experimental and might be removed.

You can turn on the navigation by adding `show_navigation: true` to the `_config.yml`. The position of items can be set on  the `order` property in the front-matter or in the `_config.yml`, and whether a page displays can be set by setting `hidden: true`.

## Licence

© Foundation for Public Code 2018

The code in this repository is licensed under [EUPL 1.2](LICENSE.md).

Logos, brands and trademarks of the Foundation for Public Code are licensed differently, check out https://brand.publiccode.net/ for more information.

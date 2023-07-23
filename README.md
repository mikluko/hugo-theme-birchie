# Birchie - Hugo theme

Birchie is a minimal and clean theme for hugo with a markdown-ish UI.

Forked from [Archie Theme](https://github.com/athul/archie)

## Features

- Google Analytics Script
- Callouts
- Tags
- Auto Dark Mode(based on system theme)
- Dark/Light Mode toggle
- tl:dr; frontamatter
- Cache busting for CSS files
- Disqus Comments

## Installation

1. [Init modules in your hugo site](https://gohugo.io/hugo-modules/use-modules/) if you haven't already.
2. Add this theme as a module in your site's config file

    ```toml
    [module]
    [[module.imports]]
    path = "github.com/mikluko/birchie"
    ```

3. Make sure legacy `theme` field is not set in site config file.

## Writing Posts

Create a new `.md` file in the *content/posts* folder

```yml
---
date: 2023-07-23
title: Title of the post
description: Description of the post
tldr: (optional)
draft: true/false (optional)
tags: [ tag names ] (optional)
---
```

## Running example site

```bash
hugo -s ./example server
``` 

----

## Config Options

### Custom CSS

Custom CSS files can be included though the `customcss` config parameter.

Note: CSS files should be placed under the `assets` directory e.g. `assets/css/first.css`.

```toml
[params]
customcss = ["css/first.css", "css/second.css"]
```

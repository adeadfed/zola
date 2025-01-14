
+++
title = "anemone"
description = "Nearly no-Javascript, efficient, minimal theme."
template = "theme.html"
date = 2023-07-10T22:28:41+01:00

[extra]
created = 2023-07-10T22:28:41+01:00
updated = 2023-07-10T22:28:41+01:00
repository = "https://github.com/Speyll/anemone"
homepage = "https://github.com/Speyll/anemone"
minimum_version = "0.4.0"
license = "MIT"
demo = "https://anemone.pages.dev"

[extra.author]
name = "Lyes 'Speyll'"
homepage = "https://speyllsite.pages.dev/"
+++        

# anemone

Nearly no-Javascript, efficient, minimal [Zola](https://www.getzola.org) theme.
I use it on my own [website](https://speyllsite.pages.dev/)

## Light and dark theme
![screenshotLight](screenshot.png)

## Installation
First download this theme to your `themes` directory:

```bash
cd themes
git clone https://github.com/Speyll/anemone
```

and then enable it in your `config.toml`:

```toml
theme = "anemone"
```

## Options

### Default taxonomies
To use tags, in a page metadata add

```toml
[taxonomies]
tags = [ 'tag1', 'tag2' ]
```

### Pages list in homepage
To enable listing of pages in homepage add the following in `config.toml`

```toml
[extra]
list_pages = true
```

### Header and footer nav links
Also in the `extra` section in `config.toml`

```toml
[extra]

header_nav = [
  { name = "/home/", url = "/" },
  { name = "/about/", url = "/about" },
  { name = "/journal/", url = "/journal" },
  { name = "/blog/", url = "/blog" },
]

footer_nav = [
  { name = "< previous", url = "#" },
  { name = "webring", url = "#" },
  { name = "next >", url = "#" },
]
```

### Add TOC to pages

In a page frontmatter, set `extra.toc` to `true`

```toml
[extra]
toc = true
```

### Extra data

- `author` can be set in both main config and in pages metadata
- `image` variable can be used in pages to add an image to HTML `<meta>` tags
- Same for `favicon` in main config, except this one is also used as the site icon

### Disable Twitter card

Twitter metatags are generated by default, to disable them set `extra.twitter_card` to `false` in in your `config.toml`

```toml
[extra]
twitter_card = true
```

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

        
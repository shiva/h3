# H3

H3 renders gallery posts with thumbnails using photoswipe. 

H3 = fork\([fork][2]\([Hemingway][1])) + [Hugo Easy Gallery][3] \(using [Photoswipe][4]\)

## Getting Started

Clone this repository to your hugo theme directory.

```
mkdir themes
cd themes
git clone https://github.com/tanksuzuki/hemingway.git
```

## Configuration

Take a look in the [exampleSite](https://github.com/tanksuzuki/hemingway/tree/master/exampleSite) folder.

This directory contains an example config file and the content for the demo.
It serves as an example setup for your documentation.

Copy the `config.toml` in the root directory of your website. Overwrite the existing config file if necessary.

__[config.toml](https://github.com/tanksuzuki/hemingway/blob/master/exampleSite/config.toml)__:

```toml
baseurl = "https://example.com"
languageCode = "en"
title = "Hemingway"
theme = "hemingway"
copyright = "&copy; <a href=\"https://github.com/tanksuzuki\">Asuka Suzuki</a> 2016"
disqusShortname = "shortname"
googleAnalytics = ""

[params]

[params.highlight]
style = "github"
languages = ["go", "dockerfile"]

[[params.social]]
url = "https://github.com/tanksuzuki"
fa_icon = "fa-github"

[[params.social]]
url = "https://twitter.com/tanksuzuki"
fa_icon = "fa-twitter"

[[params.social]]
url = "/index.xml"
fa_icon = "fa-rss"
```

## Creating posts

For normal posts, follow instructions on how to create Hugo posts.

To make H3 render posts as gallery, the type of the post should be set to "gallery".

```
title: <some title>
*type: gallery*
```

## Build

```
hugo server
```

You can go to localhost:1313 and this theme should be visible.

## License

H3 is licensed under the [MIT License](LICENSE.md).

## Authors

H3 - [Shiva](http://github.com/shiva)
Hemingway fork - [Lars Cromley](https://github.com/callmeradical)
Hemingway for Hugo - [Asuka Suzuki](https://github.com/tanksuzuki)
Hugo Easy Gallery - [Li-Wen Yip](https://github.com/liwenyip)
Photoswipe - [Dmitry Semenov](https://github.com/dimsemenov)

[1]: https://github.com/tanksuzuki/hemingway
[2]: https://github.com/callmeradical/hemingway
[3]: https://github.com/liwenyip/hugo-easy-gallery
[4]: https://github.com/dimsemenov/PhotoSwipe

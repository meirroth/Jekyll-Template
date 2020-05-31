# <img src="assets/img/jekyll-template-logo.svg" alt="Jekyll-Template" title="Jekyll-Template" width="260">


Quick and easy template to get your Jekyll site up and running.

See a live demo [here](https://meirroth.github.io/Jekyll-Template/).

### Features
  - Navigation
  - Autoprefixer
  - Easy adding of SEO terms, favicon and google analytics token.
  - linking/embedding JavaScript files stored locally or from a CDN

### Installation
Dev
```
bundle exec jekyll serve -l -o
```
Deploy
```
bundle clean
bundle exec jekyll build
```
### Site Settings

customize your site in ``_config.yml``

```yaml
lang: en
title: Your awesome title
description: >-
  Write an awesome description for your new site here.
keywords: ""
author: "Jane Doe"
url:  # the base hostname & protocol for your site, e.g. http://example.com
baseurl:  # the subpath of your site, e.g. /blog
permalink: pretty
environment: development

google-tracking-id: # Google Tracking ID and property number

# theme and favicons (https://favicon.io/)
theme-color: 

# seo meta tags
seo: 
  og:
    type: # The type of the website. default is 'website'
    image:  # An image URL which should represent your website.
  twitter:
    username:  # creator twitter username
    card: # default is 'summary'

```
### Page Settings

customize page specific settings by adding them on top of the page, delimited by ---.

```yaml
---
layout: default
title: Awesome Page Title
permalink: /

# add class/id to body tag
bodyId:  ""
bodyClass:  ""

# Add custom scripts to page
js:
  - jquery: yes     # defaults to false
  - link: ''        # inline: _includes/js/" ".js  self: assets/js/" "  ex: "fullpath"
    type: ''        # inline, self, ex (first two letters of the word enough. If not set it will check if link contains '//' it will be set to external or if does not contain. js ending it will be set to inline. default is self.)
    integrity: ''   # optinal (will add crossorigin="anonymous")
  - link: ''
    
css_link:     # link to external stylesheet files. for example "https://use.fontawesome.com/releases/v5.13.0/css/all.css"
---
```

### Todos
 - Documentation
 - And more...

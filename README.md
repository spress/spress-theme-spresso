## Spresso theme

Spresso is a simple theme for **[Spress 2.0](http://spress.yosymfony.com)** 
based on Bootstrap 3. The content is organized in one central column.
Spresso is the basic theme for Spress.

See a [demo](http://yosymfony.github.io/Spress-example/).

**This theme requires Spress >= 2.0**. If you are using Spress 1.x, go to [1.1.1](https://github.com/yosymfony/Spress-theme-spresso/releases/tag/v1.1.1) version of the theme.

### Features:

* Responsive design: Support to mobile and tablets.
* Disqus comments on your posts.
* Support to [Twitter Cards](https://dev.twitter.com/docs/cards) and [Facebook Open Graph](https://developers.facebook.com/docs/opengraph/).
* Top and bottom menu.
* Social networks link at the footer.
* Support to Google and Bing site validation.
* Code snippets highlight.
* Iconic font by [Fort Awesome](http://fortawesome.github.io/Font-Awesome).
* Sitemap and RSS feed.

### How to install?

This theme is included with Spress.

### How to use?

**Create a new site**:

`$ spress new:site /your-site-dir spresso`

#### Menus

Spresso support top and bottom menus. To configure, you can edit
`top_menu` and `bottom_menu` options from the `config.yml`:

```yaml
top_menu:
    - { name: Home, url: / }
    - { name: About, url: /about }

    # To generate a absolute URL using site.url value:
    - { name: Docs, url: /docs, site_url: true}
    
bottom_menu:
    - { name: Your link, url: https://your-url }
```

#### Comments

Comments are powered by [Disqus](disqus.com) and it need your 
**disqus shortname**. To get it, you need create a account at this service.
It's free.

##### Disable comments

By default, Disqus comments are enabled. If you want a post without comments, set
the `comments` variable to `false` at the Front-matter of the post:

```yaml
---
comments: false
---
```
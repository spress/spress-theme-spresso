## Spresso theme

Spresso is a simple theme for [Spress](https://github.com/yosymfony/Spress) 
based on Bootstrap 3. The content is organized in one central column.
Spresso is the basic theme for Spress.

See a [demo](http://yosymfony.github.io/Spress-example/).

### Featured:

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

Go to your Spress installation folder and add the following to your `composer.json`
and run `composer update`:

```
"require": {
    "yosymfony/spress-theme-spresso": "1.1.*@dev"
}
```

### How to use?

**Create a new site**:

`$ spress new:site /your-site-dir spresso`

#### Menus

Spresso support top and bottom menus. To configure, you can edit
`top_menu` and `bottom_menu` options from the `config.yml`:

```
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
```
---
comments: false
---
```
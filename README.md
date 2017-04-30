## Spresso theme

Spresso is a simple theme for **[Spress](http://spress.yosymfony.com)**
based on Bootstrap 3. The content is organized in one central column.

See a [demo](http://yosymfony.github.io/Spress-example/).

![Spresso theme preview](/screenshot.png)

## Installation
You can create a [site based on Spresso](#creating-a-new-site-based-on-this-theme-creating-site)
or install this one as a theme of a [pre-existing site](#install-as-a-theme-of-pre-existing-site-pre-existing).

**Requirements:**
* Spress >= 2.2.0

### Creating a new site based on this theme

Performs the following command and Spresso theme will be
installed in `mysite` folder:

```bash
$ spress new:site mysite spress/spress-theme-spresso
```

### Install as a theme of an pre-existing site

Go to your site folder and performs the following command:

```bash
$ spress add:plugin spress/spress-theme-spresso
```
And add this line to the `config.yml` file of your site:

```yaml
themes:
    name: spress/spress-theme-spresso
```

### How to update?

You can get the latest version of Spresso theme with just run the following command:

```bash
$ spress update:plugin
```

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

### How to use?

This theme has support for [Spress themes](http://spress.yosymfony.com/docs/themes/).
This feature is new in version 2.2.0

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

Comments are powered by [Disqus](disqus.com). This feature needs a
**disqus shortname**. To get it, you need create a account at this service.
It's free. You can find out more about Disqus' shortnames
[here](https://help.disqus.com/customer/portal/articles/466208).

To enable it, set to `true` the option `enabled` and set your disqus shortname
in the `config.yml` of your site:

```yaml
# Comments in posts
comments:
    enabled: false
    disqus_shortname: ""
```

##### Disable comments in a post

If you want to publish a post without comments, set the `comments` variable to
`false` at the Front-matter of the post:

```yaml
---
comments: false
---
The content of my post.
```

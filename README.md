## Spresso theme

Spresso is a simple theme for **[Spress](http://spress.yosymfony.com)**
based on Bootstrap 3. The content is organized in one central column.

![Spresso theme preview](/screenshot.png)

### Features:

* Responsive design: Supports mobile and tablets.
* Disqus comments on your posts.
* Support for [Twitter Cards](https://dev.twitter.com/docs/cards) and [Facebook Open Graph](https://developers.facebook.com/docs/opengraph/).
* Top and bottom menu.
* Social network links in the footer.
* Support for Google and Bing site validation.
* Code snippet highlighting with [Highlight.js](http://highlightjs.org/)
* Iconic font by [Fort Awesome](http://fortawesome.github.io/Font-Awesome).
* Sitemap and RSS feed.

## Installation
You can create a [site based on Spresso](#creating-a-new-site-based-on-this-theme-creating-site)
or install this one as a theme of a [pre-existing site](#install-as-a-theme-of-pre-existing-site-pre-existing).

**Requirements:**
* Spress >= 2.2.0

### Creating a new site based on this theme

Perform the following command and the Spresso theme will be installed in `mysite` folder:

```bash
$ spress new:site mysite spress/spress-theme-spresso
```

### Install as a theme of an pre-existing site

Go to your site folder and input the following command:

```bash
$ spress add:plugin spress/spress-theme-spresso
```
Then, add the following line to the `config.yml` file of your site:

```yaml
themes:
    name: spress/spress-theme-spresso
```

### Updating the theme

You can get the latest version of the Spresso theme by running the following command:

```bash
$ spress update:plugin
```

### Using the theme

This theme has support for [Spress themes](http://spress.yosymfony.com/docs/themes/).
This feature is new in version 2.2.0

#### Menus

The Spresso theme supports both top and bottom menus. To configure, you can edit the
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
**disqus shortname**. To get it, you need to create a account at this service.
It's free. You can find out more about Disqus' shortnames
[here](https://help.disqus.com/customer/portal/articles/466208).


To enable comments, edit the `config.yml` of your site. 
Set the `enabled` option to `true`  and set your disqus shortname.


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

## License

The theme is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

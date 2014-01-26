## Spresso theme

Spresso is the basic theme for [Spress](https://github.com/yosymfony/Spress).

See a [demo](http://yosymfony.github.io/Spress-example/).

### Featured:

* Responsive design: Support to mobile and tablets.
* Disqus comments on your posts.
* Support to [Twitter Cards](https://dev.twitter.com/docs/cards) and [Facebook Open Graph](https://developers.facebook.com/docs/opengraph/).
* Top and bottom menu.
* Social networks link at the footer.
* Support to Google and Bing site validation.
* Code snippets highlight.
* Sitemap and RSS feed.

### How to install?

Go to your Spress installation folder and add the following to your `composer.json`
and run `composer update`:

```
"require": {
    "yosymfony/spress-theme-spresso": ">=1.0,<2.0-dev",
}
```

### How to use?

**Create a new site**:

`$ spress site:new /your-site-dir spresso`
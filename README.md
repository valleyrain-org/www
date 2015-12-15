# WWW for valleyrain.org

[![Join the chat at https://gitter.im/valleyrain-org/www](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/valleyrain-org/www?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

This project is for [http://www.valleyrain.org](http://www.valleyrain.org) website. Right now it is based on [Jekyll Static Site Generator](http://jekyllrb.com/) using [Clean Blog](http://startbootstrap.com/template-overviews/clean-blog/) theme.

The website is hosted as [GitHub Project Pages](https://pages.github.com), and content is on "gh-pages" branch.

## Before You Begin

In the _config.yml file, the base URL is set to /startbootstrap-clean-blog-jekyll which is this themes gh-pages preview. It's recommended that you remove the base URL before working with this theme locally!

It should look like this:
`baseurl: ""`

## What's Included

A full Jekyll environment is included with this theme. If you have Jekyll installed, simply run `jekyll serve` in your command line and preview the build in your browser. You can use `jekyll serve --watch` to watch for changes in the source files as well.

To install Jekyll (on Mac Mavericks):
```
sudo ARCHFLAGS=-Wno-error=unused-command-line-argument-hard-error-in-future gem install jekyll
sudo gem install jekyll-sitemap jekyll-redirect-from
```

A Grunt environment is also included. There are a number of tasks it performs like minification of the JavaScript, compiling of the LESS files, adding banners to keep the Apache 2.0 license intact, and watching for changes. Run the grunt default task by entering `grunt` into your command line which will build the files. You can use `grunt watch` if you are working on the JavaScript or the LESS.

You can run `jekyll serve --watch` and `grunt watch` at the same time to watch for changes and then build them all at once.

## Support

Please open github project [issues](https://github.com/valleyrain-org/www/issues/new) or [send pull requests](https://help.github.com/articles/using-pull-requests/) if any problems are found.

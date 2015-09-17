%YAML 1.1
---
title: handroll - A website generator for software artisans
template: base.j2
---
<div class='hero'>handroll</div>

### A website generator for software artisans

handroll is a website generator designed to be simple and fast.
The concept is easy:
you make content in your favorite format
and handroll makes a website out of it.

Want to make a blog using [Markdown][md]? No problem. How about a personal
website in [reStructuredText][rst]? Sure thing. Maybe [Textile][text] is more
your style. You're good.

[md]: http://daringfireball.net/projects/markdown/
[rst]: http://docutils.sourceforge.net/rst.html
[text]: http://en.wikipedia.org/wiki/Textile_%28markup_language%29

Who is this for?
----------------

handroll is for people who want to use plain text editors to make websites.
That group could include programmers, students, scientists, writers, poets,
and more.

handroll is a command line tool. In almost all cases, you will only ever need
to type `handroll`, but a basic comfort level with a command line terminal is
beneficial.

What can it do?
---------------

* Generate HTML from [Markdown][md], [reStructuredText][rst], or
  [Textile][text].
* Generate CSS from [Sass][sass].
* Track blog entries and [generate a feed][blog].
* Run a [development server][devserver] to update as you work.
* Translated into
  Arabic,
  Dutch,
  English,
  French,
  German,
  Greek,
  Italian,
  Portuguese,
  and Spanish.

You can find a full list of features in the
[developer documentation][devfeatures].

[devfeatures]: http://handroll.readthedocs.org/en/latest/#features
[sass]: http://sass-lang.com/
[blog]: http://handroll.readthedocs.org/en/latest/extensions.html#blog-extension
[devserver]: http://handroll.readthedocs.org/en/latest/server.html#devserver

How much?
---------

handroll is free and open source software. That means no cost to you. The tool
is made available under the [BSD license][bsd]. In layman's terms, the
developers aren't liable for anything.

[bsd]: https://github.com/handroll/handroll/blob/master/LICENSE

Getting started
---------------

The first thing to do is to install handroll from a terminal.

```bash
$ pip install handroll
```

After installing, make a directory for your project. Add a [template][template]
or [configuration file][conf] to show handroll that your new directory is a
handroll project.
Then you are free to add whatever content you want.

You can generate your site by running `handroll`,
or let handroll watch your work
and update as you go by using `handroll --watch`
(see [Development Server][devserver]).

[template]: http://handroll.readthedocs.org/en/latest/templates.html
[conf]: http://handroll.readthedocs.org/en/latest/configuration.html
[devserver]: http://handroll.readthedocs.org/en/latest/server.html

Contributing
------------

There are many ways to contribute to handroll.

 * [Start a discussion about a feature][groups].
 * [Report a problem you're experiencing][issues].
 * [Translate for a new language or fix a broken one][i18n].
 * [Submit some code you wrote][pr].
 * [Write a plugin for your favorite tool][composer].
 * [Extend handroll in some new way][extension].

The contributions of others will always be appreciated. Contributors of code
or translations are [recorded in the source code][authors].

[groups]: https://groups.google.com/forum/#!forum/handroll
[issues]: https://github.com/handroll/handroll/issues
[i18n]: http://handroll.readthedocs.org/en/latest/i18n.html
[pr]: https://github.com/handroll/handroll/pulls?q=is%3Aopen+is%3Apr
[composer]: http://handroll.readthedocs.org/en/latest/composers.html
[extension]: http://handroll.readthedocs.org/en/latest/extensions.html
[authors]: https://github.com/handroll/handroll/blob/master/AUTHORS

More information
----------------

Any other information can be found at the various sites used by the handroll
project.

* [GitHub project for source code and issues][github]
* [PyPI for package hosting][pypi]
* [Read the Docs for developer documentation][rtd]
* [Google Group for announcements and discussion][groups]
* [Transifex project for language translation][transifex]
* [Travis project for Continuous Integration][travis]
* [Coveralls for source coverage measurement][coveralls]
* [GitHub project for this website][website]

[github]: https://github.com/handroll/handroll
[pypi]: https://pypi.python.org/pypi/handroll
[rtd]: http://handroll.readthedocs.org/en/latest/
[website]: https://github.com/handroll/handroll.github.io
[transifex]: https://www.transifex.com/projects/p/handroll/
[travis]: https://travis-ci.org/handroll/handroll
[coveralls]: https://coveralls.io/r/handroll/handroll

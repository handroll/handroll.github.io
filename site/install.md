%YAML 1.1
---
title: handroll - How to install
template: base.j2
---
If you already know the `pip` tool,
here's how you can install:

```console
$ pip install handroll
```

The rest of this documentation explains Python's installation tools
and how to deal with some common issues.

## Detailed instructions

handroll is written in the [Python][python] programming language.
The tool uses Python's standard packaging
and is uploaded to the primary Python repository,
the [Python Package Index (PyPI)][pypi].

[python]: https://www.python.org/
[pypi]: https://pypi.python.org/pypi

PyPI uses a standard installation tool
called `pip`.
A recent version of Python *should* include `pip`
as part of the installation,
but there are a few reasons why it may not be installed.

If you run `pip`
and get results like:

```console
$ pip
pip: command not found
```

then you need to install the tool
before proceeding.

Your operating system may have `pip`
as an available package.
On Ubuntu,
`sudo apt-get install python-pip`
would install `pip`.
The [`pip` documentation][pip] includes alternative instructions
for how to get it installed.

[pip]: http://pip.readthedocs.org/en/stable/installing/

Once `pip` is installed, run:

```console
$ pip install handroll
```

## Troubleshooting

Sometimes things go wrong
and `pip` may not give you helpful feedback.
A common problem is administrative permissions.
If you see something like:

```console
$ pip install handroll
Downloading/unpacking handroll
  Downloading handroll-2.0-py2.py3-none-any.whl (80kB): 80kB downloaded
  ... snip ...
Installing collected packages: handroll, mock, blinker, textile, Pygments, werkzeug, docutils, watchdog, Markdown, argh, pathtools
Cleaning up...
Exception:
Traceback (most recent call last):
  File "/usr/lib/python2.7/dist-packages/pip/basecommand.py", line 122, in main
    status = self.run(options, args)
  ... snip ...
OSError: [Errno 13] Permission denied: '/usr/local/lib/python2.7/dist-packages/handroll'
```

then that means you are not installing
with the required permissions.

There are a few options to fixing this problem:

1.  Install with administrative permissions (i.e., a system installation).
2.  Install to a user account.
3.  Install in a directory with a virtual environment.

### System installation

The easiest option is
to run the command with elevated permissions.
On a Linux operating system,
this is commonly done with `sudo`.

```console
$ sudo pip install handroll
```

This should install handroll
at the system level
and put the `handroll` command
in the system's `bin` directory
(i.e., a location where your terminal can find the command).

### User installation

`pip` can install into a user's home directory
where permissions shouldn't be an issue.

```console
$ pip install handroll --user
```

With this option,
handroll will install in a user's home directory
(most likely `$HOME/.local`).
If this is the first time using a user installation,
you may need to add to your `PATH`
so your terminal can find the `handroll` command.

```bash
$ export PATH="$PATH:$HOME/.local/bin"
```

### Virtual environment installation

Virtual environments are special directories
where Python code can be stored
and isolated from other code.
These environments are popular
because they consolidate all code
to a single place.
A detailed explanation is a little out of scope
for this guide;
you can look at the [virtual environment documentation][venv]
for a thorough walk-through.

[venv]: https://virtualenv.pypa.io/en/latest/userguide.html

To use a virtual environment:

```console
$ virtualenv venv
$ source venv/bin/activate
(venv)$ pip install handroll
```

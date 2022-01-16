# Getting started

- Adjust `setup.cfg` and `LICENSE`. Things to do include but are not limited to:
  - Set author and maintainer info
  - Find and replace `examplepackage` by another package name
  - Exchange the `LICENSE` file and license metadata as appropriate (see https://choosealicense.com)
  - Adjust, remove, and add other settings as necessary
- Read `CONTRIBUTING.md` for more details on how to install in dev mode, add or remove dependencies, etc.

# Explanations of some choices

## Python version

Well, choose whichever you like. In my world, Python 3.6 is the minimum worth considering for new projects. For now I'm putting Python 3.7 (released June 2018) as a default because
- `dataclasses` (PEP 557)
- Delayed evaluation of type annotations (PEP 563)
- `importlib.resources`

## `.gitattributes`

tl;dr: `*	text=auto` because Windows

Slightly longer explanation: We don't want to depend on each contributor having the right settings in their git config. `.gitattributes` can be used to define what to do about line endings on repository level.

More advanced settings may be useful to add depending on your needs: https://git-scm.com/docs/gitattributes

# TODO

- Docs using Sphinx
- Formatting using Black
- Hynek Schlawack https://www.youtube.com/watch?v=9G2s1TN9QQY
  - pyflakes
  - isort
  - check-manifest?
  - make sure tox and/or pre-commit-config automate all these things; write docs on how to set it up
  - probably check `attrs` repo
- For release, make a detailed check list and/or automate
- Automated version bumps?
- Automated releases / CI?

# Credits and references

## Tools

- Setuptools <https://setuptools.pypa.io>
- pip-tools <https://github.com/jazzband/pip-tools>
- tox <https://tox.wiki>
- pytest <https://docs.pytest.org>
- Click <https://click.palletsprojects.com>

# Guides and inspiration
- <https://packaging.python.org/tutorials/packaging-projects/>
- <https://setuptools.pypa.io/en/latest/userguide/quickstart.html>
- <https://blog.ionelmc.ro/2014/05/25/python-packaging/#the-structure>
- <https://tox.wiki/en/latest/example/package.html>
- <https://github.com/pallets> (many details heavily inspired by Click and Jinja2 repositories

# How to

- Adjust `setup.cfg`. Things to do include but are not limited to:
  - Set author and maintainer info
  - Find and replace `examplepackage` by another package name
  - Exchange the `LICENSE.txt` file and license metadata if you wish
  - Adjust, remove, and add other settings as necessary

# Python version

Well, choose whichever you like. In my world, Python 3.6 is the minimum worth considering for new projects. For now I'm putting Python 3.7 (released June 2018) as a default because
- `dataclasses` (PEP 557)
- Delayed evaluation of type annotations (PEP 563)
- `importlib.resources`

# `.gitattributes`

tl;dr: `*	text=auto` because Windows

Slightly longer explanation: We don't want to depend on each contributor having the right settings in their git config. `.gitattributes` can be used to define what to do about line endings on repository level.

More advanced settings may be useful to add depending on your needs: https://git-scm.com/docs/gitattributes

# TODO

- MANIFEST.in
- Testing using tox
- Docs using Sphinx
- Formatting using Black
- Automated version bumps?
- Automated releases

# Credits and references

- https://packaging.python.org/tutorials/packaging-projects/
- https://setuptools.pypa.io/en/latest/userguide/quickstart.html
- https://blog.ionelmc.ro/2014/05/25/python-packaging/#the-structure

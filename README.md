# quickrelease
Highly configurable interface for quickly packaging builds with a single command.

## Notes
- YAML config (.quickrelease.yml)
  - build version number
  - files/folders to include (search patterns like gitignore)
  - pre/post build hooks (python scripts, like cookiecutter?)
  - output name
  - output path
  - disable releasing on certain branches?
- written in Python 3, runnable on PATH (how to install? what about Windows?)
- override anything in YAML config with command line options
  - if not specified then default value
- automatically tag git repo
- automatically upload release to GitHub/Lab/whatever
- if git repo then parse previous commits on branch for changelog
  - otherwise use txt file for changelog

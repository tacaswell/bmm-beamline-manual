# BMM Beamline Manual

Compiled document at
https://nsls2.github.io/bmm-beamline-manual/

The *docs/* folder contains the sphinx source of the manual. 

This repository is instrumented to use Github Actions to compile the
sphinx text to HTML automatically when pushed.  So the manual should
always be as up to date as possible.

This documentation project uses the lovely
[{book}theme](https://sphinx-book-theme.readthedocs.io/en/latest/index.html)
from the [The Executable Book Project](https://ebp.jupyterbook.org/).


## Dependencies

To compile this manual, you will need to install the following using
pip or some other method:

1. [sphinx-math-dollar](https://github.com/sympy/sphinx-math-dollar/)
2. [sphinx-subfigure](https://github.com/sphinx-extensions2/sphinx-subfigure)
3. [spinx-book-theme](https://github.com/executablebooks/sphinx-book-theme)

## Hints

To compile the manual on a machine with an externally managed python
environment, you may need to use a python virtual environment.  After
installing the dependencies into the venv, try something like this:

     make SPHINXBUILD=./my-venv/bin/sphinx-build html


## A note about copyright

This document and the BlueSky data collection profile it covers was
developed primarily by a NIST employee. Pursuant to title 17 United
States Code Section 105, works of NIST employees are not subject to
copyright protection in the United States. Thus this repository may
not be licensed under the same terms as Bluesky itself or its
documentation.

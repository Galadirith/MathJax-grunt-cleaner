# MathJax-grunt-cleaner

A `gruntfile` to reduce the footprint of a MathJax installation. The default
task in this branch is configured to reduce
[MathJax `2.4.0`](https://github.com/mathjax/MathJax/releases/tag/2.4.0) to a
packed distribution with support for only TeX input and HTML-CSS output. Further
all fonts and formats are removed except for the
[MathJax TeX](http://docs.mathjax.org/en/latest/font-support.html#mathjax-font-support)
font in the `.woff` and `.otf` formats.

The motivation for these choices was to provide a minimal distribution for use
in [Atom](https://github.com/atom/atom) packages that provides the best single
output MathJax can produce (HTML-CSS) while removing all files purely supporting
legacy browsers.

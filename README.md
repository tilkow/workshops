PostgreSQL Workshops
===============================================================================

[![Build
Status](https://travis-ci.org/dalibo/workshops.svg?branch=master)](https://travis-ci.org/dalibo/workshops)

This project contains various PostgreSQL workshops including slides, handouts or
exercises. This was initially produced by [dalibo](https://dalibo.com) and it's 
now available to everyone under the [PostgreSQL License](LICENSE.md). 

The content is written in markdown using a specific set of [SYNTAX](SYNTAX.md) rules. 

We use [pandoc](http://pandoc.org/) to export this content in various format. 
For now the following formats are supported : reveal slides (HTML), PDF, EPUB, doc.

The workshops are available in 2 languages:

* [French Workshops](fr/README.md) are in the `fr` directory 
* [English workshops](en/README.md) are in the `en` directory 

Any other translation is welcome !

Install                                                                          
------------------------------------------------------------------------------- 

We built a [dedicated docker image](https://hub.docker.com/r/dalibo/pandocker/) 
to compile this content. See the [QUICKSTART](QUICKSTART.md) guide for more details.

Alternavely you can also [INSTALL](INSTALL.md) the entire debian/pandoc/latex
toolchain.

Compile
-------------------------------------------------------------------------------

Each workshop is contained in a single markdown file (for instance
[fr/100-postgresql_10.md](fr/100-postgresql_10.md) )

You can export the content using `make` by specifying the file extension you want

```
make fr/100-postgresql_10.html
make fr/100-postgresql_10.epub
make fr/100-postgresql_10.pdf
etc.
```

You can also build all workshops in all formats with:

```
make all
```

Contribute
------------------------------------------------------------------------------- 

This is an open project. You can [CONTRIBUTE](CONTRIBUTING.md) in many ways: 

* declare a bug
* fix a typo
* translate
* submit a brand new workshop
* etc.




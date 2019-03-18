# Introduction

A [Giter8](http://www.foundweekends.org/giter8/) template for generating a document based on [Tufte-LaTeX](https://tufte-latex.github.io/tufte-latex/), a Tufte-inspired LaTeX class for producing books.

Projects generated from _tufte-latex-book.g8_ come with starter text from the original Tufte-LaTeX distribution that demonstrates the document style, including graphics, table of contents, bibliography and index generation, etc. The default document serves as a reference to the format.

# Prerequisites

You need:

 * [Giter8](http://www.foundweekends.org/giter8/)
 * GNU Make (or reasonably compatible version of make; exotic features aren't used)
 * [TeX Live](https://www.tug.org/texlive/)
 * Optionally a PDF viewer of your choice (the Makefile assumes Mac OS X Preview.app)

# Creating a Project

To create a new working project invoke giter8 using the giter8 template:
```console
foo@bar:~$ g8 jerrykuch/tufte-latex-book.g8
```
Enter a name for the project when prompted. A canonicalized version of it with all letters lower-cased and spaces replaced by hyphens, will be used for the name of the directory created and as the base name of the '.tex' and '.bib' file created therein.

# Project Structure

If you entered "My First Project" when instantiating the Giter8 template, you'll end up with a directory of the following form:
```
my-first-project/
├── History.txt
├── Makefile
├── Manifest.txt
├── README.txt
├── graphics
│   ├── be-contents.pdf
│   ├── be-title.pdf
│   ├── ei-contents.pdf
│   ├── ei-title.pdf
│   ├── helix.asy
│   ├── helix.pdf
│   ├── hilbertcurves.pdf
│   ├── nasa_vision_sm.png
│   ├── satir_graph.png
│   ├── sine.asy
│   ├── sine.pdf
│   ├── vdqi-contents.pdf
│   ├── vdqi-title.pdf
│   ├── ve-contents.pdf
│   └── ve-title.pdf
├── my-first-project.bib
├── my-first-project.tex
├── tufte-book.cls
├── tufte-common.def
└── tufte-handout.cls
```

# Usage

# Licenses

## License for the Template

To the extent possible under law, the author(s) have dedicated all copyright and related and neighboring rights to this template to the public domain worldwide.  This template is distributed without any warranty. See <http://creativecommons.org/publicdomain/zero/1.0/>.

## License for Tufte-LaTeX

Copyright 2007–2015 by Kevin Godby, Bil Kleb, and Bill Wood.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.


# Software Factory
PELUX Software Factory documentation

Software Factory is maintained at https://github.com/Pelagicore/software-factory

Maintainer: Joakim Gross <joakim.gross@pelagicore.com>


## Dependencies
* cmake
* Sphinx
* plantuml
* sphinxcontrib-seqdiag
* sphinxcontrib-blockdiag
* sphinxcontrib-plantuml
* sphinxcontrib-actdiag
* sphinxcontrib-manpage
* sphinx\_rtd\_theme
* texlive-latex-base (when building PDF)
* texlive-latex-extra (when building PDF)
* texlive-latex-recommended (when building PDF)

###  Install build dependencies on Debian

``` bash
sudo apt-get install cmake python-pip plantuml
sudo pip install sphinxcontrib-seqdiag sphinxcontrib-blockdiag \
    sphinxcontrib-actdiag sphinxcontrib-manpage sphinxcontrib-plantuml \
    sphinx_rtd_theme
```


## Building
The project uses cmake to configure the build. Supported options are:

* `ENABLE_PDF` - Enables building the docs in PDF format. Set to OFF by default

Check out the swf-blueprint submodule like so:
``` bash
    git submodule update --init
```

Configure and build from the git top dir like so:
``` bash
    cmake -H. -Bbuild
    cd build
    make
```

After a successfull build you can find the documentation in `build/docs/html/`
if you open the `index.html` in your browser you will see the entry point.

# License and Copyright
Copyright (C) Pelagicore AB 2017

This work is licensed under the Creative Commons
Attribution-ShareAlike 4.0 International License. To view a copy of
this license, visit http://creativecommons.org/licenses/by-sa/4.0/ or
send a letter to Creative Commons, PO Box 1866, Mountain View, CA
94042, USA.

Code and scripts are licensed under LGPL 2.1

SPDX-License-Identifier: CC-BY-SA-4.0

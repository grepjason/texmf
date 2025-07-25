# brahmic-maps

## ISO 15919 TECkit mappings for Indic scripts in XeTeX

This package implements a set of [TECkit](https://software.sil.org/teckit/) mappings based on ISO 15919 *Transliteration of Devanāgarī and related Indic scripts into Latin characters* for reverse transliteration of Latin-based characters into various Indic scripts in the Brahmic family.

Full documentation including some examples is in [brahmic.pdf](/doc/fonts/misc/brahmic-maps/brahmic.pdf).

`sanskrit.sty` and `vedic-example.tex` contain some rudimentary examples of how to use the maps.

To regenerate the `.map` files and rebuild the `.tec` files, connect to the build directory and type:

    make

If you don't have `make`, try this:

    xetex brahmic.ins

and then

    teckit_compile deva.map -o deva.tec

etc., for each `.map` file.

## License

Copyright 2015, 2025 David M. Jones (<dmjones@alum.mit.edu>).

This work may be distributed and/or modified under the conditions of the LaTeX Project Public License, either version 1.3c of this license or (at your option) any later version. The latest version of this license is in <https://www.latex-project.org/lppl.txt> and version 1.3c or later is part of all distributions of LaTeX version 2005/12/01 or later.

This work has the LPPL maintenance status `maintained`.

The Current Maintainer of this work is David M. Jones.



# Description

Latex package to create pulse sequence diagrams in magnetic resonance imaging.


# Installation


## Project by project

Just copy the file `mrseqdia.sty` next to the tex file you want to compile.


## Add mrseqdia to your global latex installation

1.  Find out your latex distributions folder for custom packages
    
        kpsewhich -var-value=TEXMFHOME
2.  under this folder, copy `mrseqdia.sty` to [&#x2026;]/tex/latex/mrseqdia/mrseqdia.sty


# Usage

    % FID acquisition
    \begin{tikzpicture}
      \init;
      \startline{1}{RF};
      \pulse{1}{1}{$\alpha$};
      \xline{0.5};
      \acq{3}{0.5}{Acquire};
      \xline{1};
    \end{tikzpicture}


# Examples

[test\_mrseqdia.tex](./test_mrseqdia.tex)


# Contributing

Things I plan to do:

-   write documentation
-   add more examples
-   implement new sequence elements
-   rewrite commands to pass options to tikz elements
-   include functionality for configuration model


# Acknowledgement

This repository is a translation of [GitHub - dangom/mr-sequence-diagrams: Draw MR Sequence Diagrams for LaTeX / M&#x2026;](https://github.com/dangom/mr-sequence-diagrams) from metapost to TikZ/LaTeX. The initial metapost repository was originally created by Mark J White for his PhD Thesis. A snapshot is available in the Internet Archive [here](http://web.archive.org/web/20160629144038/http://www.celos.net/comp/pulses/). Two of the macros &#x2014; the ones for the trapez gradient wave forms &#x2014;  were written by T. A. Wilkinson and can be found in his blog [here](https://tinkertailorsoldiersponge.wordpress.com/category/tinker/latex/).


# License

mrseqdia
Copyright (C) 2018  maxdiefenbach

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License


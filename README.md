# dockercontainers
Build of various docker containers.

 - latexbasic:
   - Minimum for running LaTeX & TeX, including Beamer, transfig, make (for building) &  perl (for dependencies processing).
   - Package list:
     - make
     - perl
     - latex-beamer
     - texlive-latex-recommended
     - texlive-bibtex-extra
     - texlive-fonts-extra
     - transfig
     - ghostscript
     - git
 - latex2:
   - Same as latexbasic + gnuplot.
 - latexXls:
   - Same as latex2 + xlispstat.
 - latexOctave:
   - Same as latexXls + octave + octave eps output support (poppler-utils + epstool).

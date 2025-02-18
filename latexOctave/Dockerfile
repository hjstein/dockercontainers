FROM ubuntu:24.04

MAINTAINER Harvey Stein <hjstein@gmail.com>

RUN \
   apt-get update -y && \
   apt-get install software-properties-common -y && \
   apt-get update -y && \
   apt-get install \
      make \
      perl \
      texlive-latex-recommended \
      texlive-bibtex-extra \
      texlive-fonts-extra \
      texlive-font-utils \
      transfig \
      ghostscript \
      git \
      gnuplot \
      octave \
      octave-io \
      octave-statistics \
      octave-financial \
      poppler-utils \
      epstool \
      tar gcc automake -y && \
   git clone https://github.com/jhbadger/xlispstat.git && \
   cd xlispstat && \
   ./configure && make && make install &&\
   cd .. && rm -rf xlispstat-3-52-20 && \
   apt-get autoremove -y && \
   apt-get clean -y && \
   apt-get autoclean -y

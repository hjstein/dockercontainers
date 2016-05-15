FROM ubuntu:16.04

MAINTAINER Harvey Stein <hjstein@gmail.com>

RUN \
   apt-get update -y && \
   apt-get install \
      make \
      perl \
      latex-beamer \
      texlive-latex-recommended \
      texlive-bibtex-extra \
      texlive-fonts-extra \
      transfig \
      ghostscript \
      git \
      gnuplot \
      curl tar gcc automake -y && \
   curl http://ftp.uni-bayreuth.de/math/statlib/xlispstat/Src/3-52/xlispstat-3-52-20.tar.gz >xlispstat-3-52-20.tar.gz && \
   tar xzvf xlispstat-3-52-20.tar.gz && \
   cd xlispstat-3-52-20 && \
   ./configure && make && make install &&\
   cd .. && rm -rf xlispstat-3-52-20 && \
   apt-get purge curl tar gcc configure -y && \
   apt-get autoremove -y && \
   apt-get clean -y && \
   apt-get autoclean -y

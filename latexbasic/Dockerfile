FROM ubuntu:24.04

MAINTAINER Harvey Stein <hjstein@gmail.com>

RUN \
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
   git -y && \
   apt-get autoremove -y && \
   apt-get clean -y && \
   apt-get autoclean -y

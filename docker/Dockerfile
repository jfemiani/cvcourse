FROM continuumio/anaconda:5.1.0

RUN conda update conda
RUN conda config --append channels conda-forge
RUN conda install -y \
      jupyter \
      scipy matplotlib \
      munch \
      tqdm \
      autopep8 \
      flake8 \
      pylint \
      jupyter_contrib_nbextensions

RUN apt-get update && \
    apt-get install -y vim && \
    rm -rf /var/lib/apt/lists/*

RUN apt-get update && \
    apt-get install -y vim-addon-manager && \
    rm -rf /var/lib/apt/lists/*


WORKDIR /course

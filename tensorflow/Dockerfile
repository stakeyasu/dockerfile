FROM nvidia/cuda:9.0-cudnn7-devel-ubuntu16.04
LABEL maintainer s.takeyasu@ff.tmc

WORKDIR /home

# install python3 enviroment
ADD Miniconda3-latest-Linux-x86_64.sh miniconda.sh
RUN bash miniconda.sh -b -p  /opt/conda
ENV PATH /opt/conda/bin:$PATH

#install tensorflow
RUN pip install tensorflow-gpu==1.5
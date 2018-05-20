FROM nvidia/cuda:8.0-cudnn6-devel-ubuntu16.04
LABEL maintainer s.takeyasu@ff.tmc

WORKDIR /home

# ENV LD_LIBRARY_PATH /usr/local/cuda/lib64:/usr/local/cuda/extras/CUPTI/lib64:${LD_LIBRARY_PATH}
# ENV CUDA_HOME /usr/local/cuda:${CUDA_HOME}

# install python3 enviroment
ADD Miniconda3-latest-Linux-x86_64.sh miniconda.sh
RUN bash miniconda.sh -b -p  /opt/conda
ENV PATH /opt/conda/bin:${PATH}

#install tensorflow
RUN pip install tensorflow-gpu==1.3

#install python tools
RUN pip install sklearn keras


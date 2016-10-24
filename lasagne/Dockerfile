FROM nvidia/cuda:8.0-cudnn5-devel
RUN apt-get update && apt-get install -y python3 python3-pip liblapack-dev \
libopenblas-dev python3-dev gfortran
RUN pip3 install numpy scipy
RUN pip3 install -r https://raw.githubusercontent.com/Lasagne/Lasagne/master/requirements.txt
RUN pip3 install https://github.com/Lasagne/Lasagne/archive/master.zip

FROM nvidia/cuda:8.0-cudnn5-devel
RUN apt-get update && apt-get install -y python3 python3-pip liblapack-dev \
libopenblas-dev python3-dev gfortran libpng-dev libjpeg8-dev libfreetype6-dev
RUn pip3 install --upgrade pip
RUN pip3 install numpy scipy matplotlib
RUN pip3 install -r https://raw.githubusercontent.com/Lasagne/Lasagne/master/requirements.txt
RUN pip3 install https://github.com/Lasagne/Lasagne/archive/master.zip

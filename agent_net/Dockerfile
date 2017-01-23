FROM penguin138/lasagne
RUN apt-get install -y git cmake zlib1g-dev
RUN pip3 install --upgrade pip
RUN pip3 install cython
RUN pip3 install --upgrade https://github.com/yandexdataschool/AgentNet/archive/master.zip
RUN mkdir ~/gym && cd ~/gym && git clone https://github.com/openai/gym.git && cd gym && pip3 install -e .[atari]
RUN pip3 install jupyter
COPY run_jupyter.sh /
COPY jupyter_config.py /root/.jupyter/
RUN mkdir /dqn
WORKDIR dqn
CMD /run_jupyter.sh

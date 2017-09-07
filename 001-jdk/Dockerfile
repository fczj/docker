#JDK 1.7

#build cmd
# sudo docker build -t ubuntu:jdk-1.8 .

#run 
#sudo docker run --name jdk -v /opt/:/opt -d ubuntu:jdk-1.8 /bin/sh -c "while true; do sleep 100000; done"

#attach
#sudo docker exec -it jdk /bin/bash


FROM ubuntu:14.04

ADD ./jdk-8u72-linux-x64.tar.gz /usr/software


ENV JAVA_HOME /usr/software/jdk
ENV PATH=$PATH:$JAVA_HOME/bin
ENV LANG=C.UTF-8
RUN \
    ln -sv /usr/software/jdk1.8.0_72/ /usr/software/jdk && \
    export JAVA_HOME && \
    export PATH && \
    export LANG

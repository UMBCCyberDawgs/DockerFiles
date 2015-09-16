FROM ubuntu:trusty
RUN apt-get update && apt-get upgrade -y

RUN apt-get install git -y
RUN git clone https://github.com/isislab/CTFd.git /opt/ctfd && cd /opt/ctfd && ./prepare.sh


ENTRYPOINT ["/usr/bin/python", "/opt/ctfd/serve.py"]

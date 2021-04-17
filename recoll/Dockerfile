FROM debian:latest
MAINTAINER sn0b4ll

RUN apt -y update
RUN apt -y install python3 python3-pip recoll x11vnc unzip xsltproc unrtf untex libimage-exiftool-perl antiword poppler-utils git wv

RUN python3 -m pip install waitress

RUN git clone https://framagit.org/medoc92/recollwebui.git recoll-webui-master

RUN mkdir /homes && mkdir /root/.recoll

EXPOSE 8080

RUN recollindex -m
CMD ["/usr/bin/python3", "/recoll-webui-master/webui-standalone.py", "-a", "0.0.0.0"]

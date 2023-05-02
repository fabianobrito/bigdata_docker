FROM ubuntu:20.04
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && apt-get upgrade -y
RUN apt-get install python3 -y
RUN apt-get install python3-pip -y
RUN pip install schedule
RUN apt update && apt install -y tcl
RUN apt-cache policy docker-ce
RUN apt-get install docker -y
COPY src/main.py /
CMD [ "python3", "main.py"]
FROM matthewfeickert/docker-python3-ubuntu
RUN pip install schedule
RUN apt update && apt install -y tcl
RUN apt-cache policy docker-ce
RUN apt-get install docker -y
COPY src/main.py .
CMD [ "python3", "main.py"]

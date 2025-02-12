FROM ubuntu:latest
RUN apt-get update 
RUN apt-get install -y python3
RUN apt-get install -y python3-pip
COPY . /
RUN pip3 install --break-system-packages  -r requirements.txt
VOLUME /tmp/
EXPOSE 5000
ENTRYPOINT [ "python3", "webapp.py" ] 


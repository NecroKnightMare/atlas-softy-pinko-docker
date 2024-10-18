FROM ubuntu:latest
# update apt 
RUN apt-get update && apt-get upgrade -y
# install python3 and python-pip
RUN apt-get python3 install -y python3 python3-pip
# running before installing pip to avoid error
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED
# install flask
RUN pip3 install flask
# install cors
RUN pip3 install flask-cors
# be in app dir
WORKDIR /app
# copy file to dir
COPY ./api.py /app/api.py
# run the file
CMD ["python3", "api.py"]
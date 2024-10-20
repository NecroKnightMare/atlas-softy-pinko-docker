FROM docker.io/library/ubuntu:latest@sha256:ac58ff7fe25edc58bdf0067ca99df00014dbd032e2246d30a722fa348fd799a5
# running before installing pip to avoid error
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED || true
# update apt 
RUN apt-get update && apt-get upgrade -y
# install python3 and python-pip
RUN apt-get install -y python3 python3-pip
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
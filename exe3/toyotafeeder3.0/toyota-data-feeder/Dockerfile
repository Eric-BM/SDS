FROM python:3.9
# build an image starting with python 3.9

ADD feeder.py .
# add feeder.py to the working directory

COPY toyota_data.csv toyota_data.csv
# copy metadata to the image

COPY requirements.txt requirements.txt
# copy requirements to the image

COPY /certs /certs
# copy ca.crt to the image


RUN pip3 install -r requirements.txt
# tell Docker to use pip3 to install 

CMD ["python3", "./feeder.py"]
# tell Docker what command we want to run when our image is executed inside a container

FROM python:3.9

ADD feeder.py .

COPY requirements.txt requirements.txt

COPY ca.crt ca.crt

COPY toyota_data.csv toyota_data.csv

RUN pip3 install -r requirements.txt

CMD ["python3", "./feeder.py"]

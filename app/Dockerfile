FROM ubuntu

RUN apt-get update -y
RUN apt-get install -y python
RUN apt-get install -y python3-pip
RUN pip install flask

COPY app.py /opt/app.py

ENTRYPOINT FLASK_APP=/opt/app.py flask run --host=0.0.0.0

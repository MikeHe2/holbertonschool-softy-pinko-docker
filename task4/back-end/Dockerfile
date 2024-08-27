FROM ubuntu

RUN apt-get update

RUN apt-get upgrade -y

RUN apt-get install python3 -y python3 pip

RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

WORKDIR /app

COPY ./api.py /app/api.py

RUN pip install flask

RUN pip install flask-cors

CMD python3 /app/api.py
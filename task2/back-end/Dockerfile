FROM ubuntu

RUN apt-get update

RUN apt-get upgrade -y

RUN apt-get install python3 -y python3 pip

RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

WORKDIR /app                                                                0.0s

COPY ./api.py /app/api.py

RUN pip install flask

CMD python3 /app/api.py
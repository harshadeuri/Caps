FROM python:3.7.3

ADD . /var/www/dofile

WORKDIR /var/www/dofile

RUN pip3 install -r requirements.txt

EXPOSE 8002

RUN ./manage.py makemigrations

RUN ./manage.py migrate

CMD ./manage.py runserver 0.0.0.0:8002

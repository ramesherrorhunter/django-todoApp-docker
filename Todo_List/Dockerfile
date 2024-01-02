FROM python:latest
WORKDIR /todo
COPY . /todo
RUN apt-get install libcairo2-dev
RUN pip install -r requirements.txt
RUN python3 manage.py makemigrations
RUN python3 manage.py migrate
CMD ["python3","manage.py","runserver","0.0.0.0:9001"]

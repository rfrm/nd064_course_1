FROM python:2.7
LABEL maintainer="Robinson Rodriguez"

WORKDIR /app
COPY ./project/techtrends .
RUN pip install -r requirements.txt

EXPOSE 3111
RUN [ "python", "init_db.py" ]

# command to run on container start
CMD [ "python", "app.py" ]

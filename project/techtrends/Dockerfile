FROM python:2.7
LABEL maintainer="Manu"

COPY ./project/techtrends /app
WORKDIR /app
RUN python -m pip install --upgrade pip &&\
     pip install -r requirements.txt

RUN python init_db.py

EXPOSE 3111

# command to run on container start
CMD [ "python", "app.py" ]



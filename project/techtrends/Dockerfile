FROM python:3.8
#LABEL maintainer="yu"

COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt

EXPOSE 3111

# command to run on container start
RUN python init_db.py
CMD [ "python", "app.py" ]

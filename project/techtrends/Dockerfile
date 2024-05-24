FROM python:3.8
#LABEL maintainer="yu"

COPY . /app
WORKDIR /app
RUN pip install -r /app/project/techtrends/requirements.txt

EXPOSE 3111

# command to run on container start
RUN python /app/project/techtrends/init_db.py
CMD [ "python", "/app/project/techtrends/app.py" ]

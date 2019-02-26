FROM python:3.6.0-alpine

WORKDIR /app
ADD . /app

RUN apk add --no-cache bash && pip install -r /app/requirements.txt

ENV POST_DATABASE_HOST post_db
ENV POST_DATABASE posts

CMD ["python3", "/app/post_app.py"]

# Dockerfile for development

FROM ubuntu

WORKDIR /app

COPY . .

RUN rm .env

RUN mv .env.docker .env

RUN apt update

RUN apt install -y python3 python3-pip gcc libmysqlclient-dev python3-dev build-essential pkg-config

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 8000

CMD ["uvicorn", "main:app", "--reload"]
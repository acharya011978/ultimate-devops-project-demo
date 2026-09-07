FROM python:3.12.14-slim-trixie AS base
WORKDIR /usr/src/app
COPY requirements.txt ./

RUN pip install --upgrade pip --no-cache-dir 

RUN pip install -r requirements.txt --no-cache-dir 

COPY . .

ENTRYPOINT ["python", "recommendation_server.py"]




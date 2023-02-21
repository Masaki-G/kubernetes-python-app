FROM python:3.7

WORKDIR /app

COPY ./ ./
RUN pip install --upgrade pip
RUN apt-get update && \
    apt-get -y install gcc libmariadb-dev
RUN pip install --no-cache-dir --upgrade -r requirements.txt

EXPOSE 5000
CMD ["python", "/app/app/main.py"]


# Airflow

This repository is for testing and experimentations. The implementations do not reflect how I code for production.

## Setup Environment

```text
python3.8 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

## Run Airflow for Development

```text
airflow db init
airflow users create -u admin -p admin -f FIRST_NAME -l LAST_NAME -r Admin -e admin@example.org
airflow webserver
airflow scheduler
airflow celery flower
airflow celery worker
redis-server /usr/local/etc/redis.conf
```

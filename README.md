# Airflow

## Setup Environment

```text
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
```

## Run Airflow for Development

```text
airflow db init
airflow webserver -D
airflow scheduler -D
airflow users create -u admin -p admin -f FIRST_NAME -l LAST_NAME -r Admin -e admin@example.org
```

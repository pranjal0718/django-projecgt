# Sample Django Project

## Prerequisites
- Python 3.10+
- pip, virtualenv

## Setup
```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\\Scripts\\activate
pip install -r requirements.txt
```

## Run migrations & start server
```bash
python manage.py makemigrations core
python manage.py migrate
python manage.py runserver
```
Visit: http://127.0.0.1:8000/

## Run tests
```bash
python manage.py test -v2 --keepdb
```

## Build (Docker)
```bash
docker build -t sample-django-app .
docker run -p 8000:8000 sample-django-app
```

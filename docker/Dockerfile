FROM python:3.9-slim

WORKDIR /app

COPY ../flask-sample-app/requirements.txt .

RUN pip install -r requirements.txt

COPY ../flask-sample-app .

EXPOSE 8000

CMD ["gunicorn", "run:app", "-b", "0.0.0.0:8000"]
FROM python:3.8.18-bullseye

EXPOSE 3111

WORKDIR /app

COPY techtrends/ /app

RUN pip install -r /app/requirements.txt

RUN python3 /app/init_db.py

CMD ["python3", "/app/app.py"]

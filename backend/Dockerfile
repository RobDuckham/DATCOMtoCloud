FROM python:3.9

WORKDIR /backend

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 8000

CMD ["gunicorn","--bind=0.0.0.0","--timeout","600","main:app"]

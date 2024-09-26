# Dockerfile for booking_catalog microservice
FROM python:3.11-slim

WORKDIR /app

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

ENV DATABASE_URL = "postgresql://sit722part5_user:9sSwL4aBp8Q97OMx3CDNqnJsyD87wmCU@dpg-crqj1g2j1k6c738hh6l0-a.oregon-postgres.render.com/sit722part5"

EXPOSE 8000

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]
# Your Solution
# Dockerfile for book_catalog microservice

# Use an official Python runtime as a parent image
FROM python:3.9-slim

# Root Directory
WORKDIR /book_catalog

# Copies the source code for this microservice into the image
COPY ./* .

# Set Environment Variable
ENV DATABASE_URL=postgresql://s223828778_sit722_db_b74o_user:jprulNUiNVrz1Qc53yOc6YIUSknb1xeB@dpg-crh8fs5svqrc7389ei7g-a.oregon-postgres.render.com/s223828778_sit722_db_b74o

# Build Command
RUN pip install -r requirements.txt

# Start command
CMD uvicorn main:app --host 0.0.0.0 --port $PORT
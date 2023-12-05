# syntax=docker/dockerfile:1
FROM python:3.10
ENV PYTHONUNBUFFERED=1
WORKDIR /code
COPY requirements.txt /code/requirements.txt
COPY final_project /code/final_project
RUN pip install --no-cache-dir -r requirements.txt
COPY . /code/
CMD ["python", "final_project/manage.py", "runserver", "0.0.0.0:8000"]

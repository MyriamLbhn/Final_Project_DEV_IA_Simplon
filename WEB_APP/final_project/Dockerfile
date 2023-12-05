# syntax=docker/dockerfile:1
FROM python:3.10

ENV PYTHONUNBUFFERED=1

WORKDIR /code

COPY ./requirements.txt /code

RUN pip install --no-cache-dir -r requirements.txt

COPY . /code

EXPOSE 8000

CMD ["gunicorn", "--bind", ":8000", "final_project.wsgi:application"]

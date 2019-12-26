FROM python:3.8-alpine

RUN mkdir /code
WORKDIR /code

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt


COPY . .
CMD ["python3", "./manage.py", "runserver"]
EXPOSE 8000
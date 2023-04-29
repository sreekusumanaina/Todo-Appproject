FROM python:3.9
WORKDIR /usr/src/app
COPY ./requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
ENV PYTHONDONTWRITEBYCODE 1
ENV PYTHONUNBUFFERED 1
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

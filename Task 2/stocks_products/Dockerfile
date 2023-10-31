FROM python:latest

WORKDIR /stocks_products

COPY . /stocks_products/

RUN pip install -r /stocks_products/requirements.txt

RUN python manage.py migrate

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
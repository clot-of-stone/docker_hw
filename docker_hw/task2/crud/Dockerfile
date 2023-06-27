FROM python:3.10

COPY . /src

COPY ./requirements.txt /src/requirements.txt
RUN pip3 install --no-cache-dir --upgrade -r /src/requirements.txt

EXPOSE 7707
WORKDIR /src

RUN python manage.py migrate
RUN python manage.py collectstatic --noinput

CMD ["gunicorn", "--bind", "0.0.0.0:7707", "stocks_products.wsgi:application"]

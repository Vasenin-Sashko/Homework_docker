FROM python:3.10
ENV PYTHONUNBUFFERED 1
COPY ./stocks_products /stocks_products
RUN pip install -U pip
RUN pip install -Ur /stocks_products/requirements.txt
RUN python3 /stocks_products/manage.py migrate
CMD ["python3", "/stocks_products/manage.py", "runserver", "0.0.0.0:6060"]
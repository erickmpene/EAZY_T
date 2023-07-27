FROM python:3.6-alpine
LABEL EMAIL="erickmpene@gmail.com"

ENV ODOO_URL https://odoo.comm
ENV PGADMIN_URL: https://pgadmin.org

WORKDIR /opt

COPY . ./

RUN pip install flask==1.1.2

EXPOSE 8080

ENTRYPOINT [ "python", "app.py" ]

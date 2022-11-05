FROM python:3.10.8
#ENV PYTHONCLEAN 1
RUN bash -c "mkdir /api"
WORKDIR /api
COPY requirements.txt /api
RUN pip install -r requirements.txt
COPY . /api
EXPOSE 8000
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]


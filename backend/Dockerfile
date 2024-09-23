FROM python:3.9
WORKDIR /backend
RUN pip install gunicorn==20.1.0
COPY . .
RUN pip install --upgrade pip && pip install -r requirements.txt
CMD ["gunicorn", "--bind", "0.0.0.0:8000", "kittygram_backend.wsgi"]
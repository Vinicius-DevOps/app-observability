FROM python:3.11-slim
WORKDIR /app
COPY requirements.txt .
RUN pip install --upgrade setuptools==78.1.1
RUN pip install --no-cache-dir -r requirements.txt
COPY app ./app
EXPOSE 8000
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]

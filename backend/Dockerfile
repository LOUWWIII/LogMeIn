FROM python:3.11-slim

WORKDIR /backend

RUN pip install --upgrade pip
RUN apt update && apt upgrade -y
COPY /requirements.txt .
RUN pip install -r requirements.txt
COPY . .

EXPOSE 5000

CMD ["python", "app.py"]

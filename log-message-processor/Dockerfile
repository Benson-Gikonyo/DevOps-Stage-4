FROM python:3.10

WORKDIR /app

COPY requirements.txt .

RUN apt-get update && apt-get install -y gcc python3-dev

RUN pip install --upgrade pip setuptools wheel

RUN pip install -r requirements.txt

COPY . .

CMD ["python", "main.py"]
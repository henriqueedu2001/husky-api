FROM python:3

RUN apt update
RUN apt install python3 -y

WORKDIR /usr/app/src

COPY . .

RUN pip install fastapi[standard]

RUN pip install -r requirements.txt

EXPOSE 8000

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]


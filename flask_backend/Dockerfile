FROM python

WORKDIR /app

COPY requirements.txt requirements.txt

RUN apt-get update && apt-get install ffmpeg libsm6 libxext6  -y

RUN pip install -r requirements.txt


COPY . .

CMD ["python", "app.py"]
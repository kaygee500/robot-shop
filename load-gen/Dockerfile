FROM python:3.13.0b4-slim

# Some default values
ENV HOST="http://localhost:8080/" \
    SILENT=0 \
    NUM_CLIENTS=1 \
    ERROR=0 \
    RUN_TIME=0
    

WORKDIR /load

COPY requirements.txt /load/

RUN pip install -r requirements.txt

COPY entrypoint.sh /load/
COPY robot-shop.py /load/

CMD ["./entrypoint.sh"]


FROM ubuntu:latest

WORKDIR /app

RUN apt-get update && apt-get upgrade -y && \
    apt-get install -y python3 python3-pip && \
    rm /usr/lib/python*/EXTERNALLY-MANAGED && \
    pip3 install flask

COPY api.py /app

EXPOSE 5252

CMD ["python3", "api.py"]
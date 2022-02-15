FROM ubuntu:18.04
LABEL maintainer="alexey.chasovnikov@gmail.com"
EXPOSE 8008
COPY . /app
RUN apt update \
    && apt install -y \
    python3 \
    python3-pip \
    && git clone https://github.com/anfederico/Flaskex\
    && pip3 install -r ./Flaskex/requirements.txt
CMD python ./Flaskex/app.py

FROM ubuntu

WORKDIR /opt/

RUN apt-get update && apt-get install -yq build-essential make libsqlite3-dev sqlite3 git

RUN git clone https://github.com/schoolofdevops/facebooc.git

RUN cd /opt/facebooc/ && make all

EXPOSE 16000

CMD "/opt/facebooc/bin/facebooc"

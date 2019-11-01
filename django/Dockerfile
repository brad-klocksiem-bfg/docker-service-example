FROM python:3.7-alpine

ENV TZ=America/Los_Angeles

RUN apk update
RUN apk add --no-cache \
    alpine-sdk \
    bash \
    build-base \
    linux-headers \
    mysql-dev \
    openldap-dev \
    python3 \
    python3-dev \
    py3-pip \
    pcre \
    pcre-dev

ENV INSTALL_PATH /django
RUN mkdir -p ${INSTALL_PATH}
WORKDIR ${INSTALL_PATH}

COPY requirements.txt ${INSTALL_PATH}
RUN python -m pip install --no-cache-dir --upgrade pip
RUN python -m pip install --no-cache-dir -r ./requirements.txt

COPY . ${INSTALL_PATH}

ENTRYPOINT ["bash", "init.sh"]
CMD ["portmapper", "2", "9000"]

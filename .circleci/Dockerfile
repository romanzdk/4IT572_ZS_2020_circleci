FROM node:10.23.0-alpine3.9
ENV PYTHONUNBUFFERED=1
RUN apk add --update --no-cache python3 && ln -sf python3 /usr/bin/python
RUN python3 -m ensurepip
RUN pip3 install --no-cache --upgrade pip setuptools
RUN apk add --update ansible
RUN apk add openssh-client
RUN pip3 install boto boto3
ENTRYPOINT [ "/bin/sh" ]
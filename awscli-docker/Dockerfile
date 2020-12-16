FROM docker:dind
LABEL maintainer="Gabriel Poleze Ferreira" email="gabriel.poleze@gmail.com"

# Installing Python
RUN apk add --update --no-cache python3 && ln -sf python3 /usr/bin/python
RUN python3 -m ensurepip
RUN pip3 install --no-cache --upgrade \
    pip \
    setuptools

# Intalling AWS CLI
RUN pip3 install --no-cache --upgrade awscli

ENTRYPOINT ["/bin/sh"]

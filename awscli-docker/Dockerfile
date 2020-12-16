FROM amazon/aws-cli
LABEL maintainer="Gabriel Poleze Ferreira" email="gabriel.poleze@gmail.com"

RUN yum update \
    && amazon-linux-extras install docker

ENTRYPOINT ["/bin/bash"]

FROM bitnami/aws-cli:latest

RUN apt-get update -y &&
    apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg-agent \
    software-properties-common

RUN curl -fsSL https://download.docker.com/linux/debian/gpg | sudo apt-key add -
RUN add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/debian \
   $(lsb_release -cs) \
   stable"

RUN apt-get update -y &&
    apt-get install docker-ce docker-ce-cli containerd.io
    
ENTRYPOINT ["/bin/bash"]

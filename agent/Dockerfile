FROM alpine:3.7

RUN apk add --update git curl bash openssl

# Install `kubectl`
RUN curl -sLO https://storage.googleapis.com/kubernetes-release/release/v1.9.3/bin/linux/amd64/kubectl &&\
  chmod +x kubectl &&\
  mv kubectl /usr/local/bin

# Install `helm`
RUN curl -sLO https://storage.googleapis.com/kubernetes-helm/helm-v2.8.2-linux-amd64.tar.gz &&\
  tar -xf helm-v2.8.2-linux-amd64.tar.gz &&\
  chmod +x linux-amd64/helm &&\
  mv linux-amd64/helm /usr/local/bin &&\
  rm helm-v2.8.2-linux-amd64.tar.gz

# Install `ankh`
RUN curl -sLO https://github.com/appnexus/ankh/releases/download/v1.0.0-beta.3/ankh-linux-amd64.tar.gz &&\
  tar -xf ankh-linux-amd64.tar.gz &&\
  mv ankh /usr/local/bin &&\
  rm ankh-linux-amd64.tar.gz

# Install `gitwatch`
RUN curl -sLO https://github.com/jondlm/gitwatch/releases/download/0.7.0/gitwatch_linux_amd64 &&\
  chmod +x gitwatch_linux_amd64 &&\
  mv gitwatch_linux_amd64 /usr/local/bin/gitwatch


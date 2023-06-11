FROM mcr.microsoft.com/devcontainers/base:alpine

# RUN apk add --no-cache \
#     bash \
#     curl \
#     git \
#     jq \
#     openssh-client \
#     python3 \
#     python3-dev \
#     py3-pip \
#     py3-setuptools \
#     py3-wheel \
#     rsync \
#     sudo \
#     unzip \
#     wget \
#     zip \
#     zsh

RUN apk update && apk add --no-cache \
  neovim

CMD [ "bash" ]

FROM mcr.microsoft.com/devcontainers/base:alpine

# Install neovim
RUN apk add --no-cache neovim

# Install next dependencies
RUN apk add --no-cache \
    openssh \
    git \
    curl \
    jq \
    make \
    nodejs \
    npm \
    cargo \
    python3 \
    py3-pip \
    ripgrep \
    neovim

RUN LV_BRANCH='release-1.3/neovim-0.9' bash <(curl -s https://raw.githubusercontent.com/LunarVim/LunarVim/release-1.3/neovim-0.9/utils/installer/install.sh) -y --overwrite

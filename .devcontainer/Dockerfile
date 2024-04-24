# FROM mcr.microsoft.com/devcontainers/base:alpine
FROM mcr.microsoft.com/devcontainers/base:debian

# Install neovim
# RUN apk add --no-cache neovim

# # Install next dependencies
# RUN apk add --no-cache \
#     openssh \
#     git \
#     curl \
#     jq \
#     make \
#     nodejs \
#     npm \
#     cargo \
#     python3 \
#     py3-pip \
#     ripgrep \
#     neovim

# Same as above but for debian
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
    neovim \
    git \
    curl \
    jq \
    make \
    nodejs \
    npm \
    # cargo \
    python3 \
    python3-pip \
    ripgrep

# Install LunarVim
RUN LV_BRANCH='release-1.2/neovim-0.8' bash <(curl -s https://raw.githubusercontent.com/LunarVim/LunarVim/release-1.3/neovim-0.9/utils/installer/install.sh) --no-install-dependencies -y

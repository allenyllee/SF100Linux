# Use an Ubuntu-based image as the base
FROM mcr.microsoft.com/devcontainers/base:jammy

# Install dependencies
RUN apt-get update && \
    apt-get install -y libusb-1.0-0-dev pkg-config

# install lsusb
RUN apt-get install -y usbutils

# Add vscode user to the root group
RUN usermod -aG root vscode

# Set default user to vscode
USER vscode

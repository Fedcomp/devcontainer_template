FROM ubuntu:22.04

RUN apt-get update

# This snippet makes sure your
# vscode in container will create/edit
# files with same permissions as your host user
ARG UID
ARG GID
RUN groupadd -g $GID vscode
RUN useradd vscode -u $UID -g $GID -m
USER vscode

WORKDIR /home/vscode/workspace
CMD ["sleep", "infinity"]

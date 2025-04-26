FROM ubuntu:24.04

RUN apt-get update

ARG UID
ARG GID
RUN userdel ubuntu
RUN groupadd -g $GID vscode
RUN useradd vscode -u $UID -g $GID -m
USER vscode

WORKDIR /home/vscode/workspace
CMD ["sleep", "infinity"]

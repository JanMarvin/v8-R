FROM archlinux:latest

ENV target v8-r

RUN pacman -Syu && pacman -S python2 python3 git icu rlwrap

RUN git clone https://github.com/JanMarvin/v8-r

WORKDIR /v8-r

RUN makepkg
